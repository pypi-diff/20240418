# Comparing `tmp/pulumi_okta-4.9.0a1713445751.tar.gz` & `tmp/pulumi_okta-4.9.0a1713447075.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_okta-4.9.0a1713445751.tar", last modified: Thu Apr 18 13:12:24 2024, max compression
+gzip compressed data, was "pulumi_okta-4.9.0a1713447075.tar", last modified: Thu Apr 18 13:34:13 2024, max compression
```

## Comparing `pulumi_okta-4.9.0a1713445751.tar` & `pulumi_okta-4.9.0a1713447075.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.384225 pulumi_okta-4.9.0a1713445751/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-18 13:12:24.380225 pulumi_okta-4.9.0a1713445751/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.360225 pulumi_okta-4.9.0a1713445751/pulumi_okta/
--rw-r--r--   0 runner    (1001) docker     (127)    21302 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/admin_role_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/admin_role_custom_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/admin_role_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.368224 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/access_policy_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    64105 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/auto_login.py
--rw-r--r--   0 runner    (1001) docker     (127)    37151 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    40464 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/get_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/get_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    32406 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/group_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)   147044 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/o_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/o_auth_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/oauth_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   138292 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    72919 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/secure_password_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    59554 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/swa.py
--rw-r--r--   0 runner    (1001) docker     (127)    67010 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/three_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app_oauth_api_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app_saml_app_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    66199 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app_shared_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    91388 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app_signon_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    23715 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app_user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    51059 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/app_user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.368224 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/get_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/get_server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/get_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23581 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/server_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    17696 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    47955 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/server_policy_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    47597 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/server_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    22572 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/server_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    20134 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth_server_claim_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/auth_server_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    47596 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24178 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)    30565 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/brand.py
--rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/captcha_org_wide_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.368224 pulumi_okta-4.9.0a1713445751/pulumi_okta/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    14270 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/domain_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    39467 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/email_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/email_sender_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    18126 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/event_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/event_hook_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.368224 pulumi_okta-4.9.0a1713445751/pulumi_okta/factor/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/factor/factor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/factor_totp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_app_user_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_auth_server_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_auth_server_claims.py
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_brands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_email_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_email_customizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_network_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_themes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_trusted_origins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/get_user_security_questions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.372225 pulumi_okta-4.9.0a1713445751/pulumi_okta/group/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/group/get_everyone_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/group/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/group/get_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    15299 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/group/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    24129 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/group/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    20949 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/group/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    47368 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/group_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.372225 pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/get_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    18055 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/get_social.py
--rw-r--r--   0 runner    (1001) docker     (127)    90649 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    83512 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/saml_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    72978 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/social.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.372225 pulumi_okta-4.9.0a1713445751/pulumi_okta/index/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50207 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/index/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18671 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/index/customized_signin_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/index/email_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/index/email_domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/index/get_default_signin_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/index/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/index/get_log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/index/get_org_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/index/log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    43669 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/index/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18545 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/index/preview_signin_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.376225 pulumi_okta-4.9.0a1713445751/pulumi_okta/inline/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/inline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/inline/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/inline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/link_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/link_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.376225 pulumi_okta-4.9.0a1713445751/pulumi_okta/network/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26479 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/network/zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    35541 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/org_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/org_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    37606 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.380225 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16040 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22169 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/device_assurance_android.py
--rw-r--r--   0 runner    (1001) docker     (127)    46046 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/device_assurance_chromeos.py
--rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/device_assurance_ios.py
--rw-r--r--   0 runner    (1001) docker     (127)    55879 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/device_assurance_macos.py
--rw-r--r--   0 runner    (1001) docker     (127)    71271 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/device_assurance_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/get_default_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    69300 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    79741 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/password.py
--rw-r--r--   0 runner    (1001) docker     (127)    49297 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/rule_idp_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    30920 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/rule_mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/rule_password.py
--rw-r--r--   0 runner    (1001) docker     (127)    66504 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/rule_signon.py
--rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/signon.py
--rw-r--r--   0 runner    (1001) docker     (127)    65473 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy_mfa_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    71555 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy_password_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy_profile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy_profile_enrollment_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    35011 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/policy_rule_profile_enrollment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.380225 pulumi_okta-4.9.0a1713445751/pulumi_okta/profile/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/profile/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23956 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/profile/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/profile/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/rate_limiting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/resource_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    21992 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/security_notification_emails.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/template_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    42952 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/theme.py
--rw-r--r--   0 runner    (1001) docker     (127)    14948 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/threat_insight_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.380225 pulumi_okta-4.9.0a1713445751/pulumi_okta/trustedorigin/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/trustedorigin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/trustedorigin/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.380225 pulumi_okta-4.9.0a1713445751/pulumi_okta/user/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25722 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user/get_user_profile_mapping_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user/get_user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    99171 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user/user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user_admin_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    23075 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user_factor_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user_group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    51854 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta/user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:12:24.380225 pulumi_okta-4.9.0a1713445751/pulumi_okta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-18 13:12:24.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-18 13:12:24.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:12:24.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 13:12:24.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 13:12:24.000000 pulumi_okta-4.9.0a1713445751/pulumi_okta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-18 13:12:18.000000 pulumi_okta-4.9.0a1713445751/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:12:24.384225 pulumi_okta-4.9.0a1713445751/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.303452 pulumi_okta-4.9.0a1713447075/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-18 13:34:13.303452 pulumi_okta-4.9.0a1713447075/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.279452 pulumi_okta-4.9.0a1713447075/pulumi_okta/
+-rw-r--r--   0 runner    (1001) docker     (127)    21302 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/admin_role_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/admin_role_custom_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/admin_role_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.283452 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/access_policy_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64105 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/auto_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37151 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40464 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32406 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/group_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)   147044 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/o_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/o_auth_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/oauth_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138292 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72919 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/secure_password_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59554 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/swa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67402 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/three_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_oauth_api_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_saml_app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66199 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_shared_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91388 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_signon_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23715 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51605 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.287452 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/get_server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/get_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23581 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17696 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47955 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_policy_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47597 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22572 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20134 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth_server_claim_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth_server_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47596 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24178 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30565 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/captcha_org_wide_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.287452 pulumi_okta-4.9.0a1713447075/pulumi_okta/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14270 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/domain_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39467 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/email_sender_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/event_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/event_hook_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.287452 pulumi_okta-4.9.0a1713447075/pulumi_okta/factor/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/factor/factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/factor_totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_app_user_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_auth_server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_auth_server_claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_brands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_email_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_network_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_themes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_trusted_origins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_user_security_questions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.291452 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/get_everyone_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/get_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15299 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24255 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20949 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47368 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.291452 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18055 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_social.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87493 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83512 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/saml_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72978 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/social.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.295452 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50207 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18671 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/customized_signin_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/email_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/email_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_default_signin_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_org_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43669 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18545 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/preview_signin_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.295452 pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19244 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/link_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/link_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.295452 pulumi_okta-4.9.0a1713447075/pulumi_okta/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26479 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/network/zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36906 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/org_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/org_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37606 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.299452 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16040 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22470 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46102 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_chromeos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17701 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56229 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71621 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/get_default_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69300 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79741 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51815 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_idp_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34098 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69730 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_signon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/signon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65473 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_mfa_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71555 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_password_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_profile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_profile_enrollment_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35011 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_rule_profile_enrollment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.299452 pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23956 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/rate_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/resource_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21342 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21992 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/security_notification_emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/template_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42952 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14948 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/threat_insight_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.299452 pulumi_okta-4.9.0a1713447075/pulumi_okta/trustedorigin/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/trustedorigin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/trustedorigin/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.303452 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25722 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_user_profile_mapping_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100207 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user_admin_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23075 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user_factor_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user_group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51854 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.303452 pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-18 13:34:13.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-18 13:34:13.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:34:13.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 13:34:13.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 13:34:13.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:34:13.303452 pulumi_okta-4.9.0a1713447075/setup.cfg
```

### Comparing `pulumi_okta-4.9.0a1713445751/PKG-INFO` & `pulumi_okta-4.9.0a1713447075/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.9.0a1713445751
+Version: 4.9.0a1713447075
 Summary: A Pulumi package for creating and managing okta resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi,okta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_okta-4.9.0a1713445751/README.md` & `pulumi_okta-4.9.0a1713447075/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/__init__.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/_inputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/_utilities.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/admin_role_custom.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/admin_role_custom.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/admin_role_custom_assignments.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/admin_role_custom_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/admin_role_targets.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/admin_role_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/__init__.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/_inputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/access_policy_assignment.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/access_policy_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/auto_login.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/auto_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/basic_auth.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/bookmark.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/bookmark.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/get_app.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/get_metadata_saml.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/get_oauth.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_oauth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/get_saml.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_saml.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,15 @@
         """
         return pulumi.get(self, "saml_signed_request_enabled")
 
     @property
     @pulumi.getter(name="signatureAlgorithm")
     def signature_algorithm(self) -> str:
         """
-        Signature algorithm used ot digitally sign the assertion and response.
+        Signature algorithm used to digitally sign the assertion and response.
         """
         return pulumi.get(self, "signature_algorithm")
 
     @property
     @pulumi.getter(name="singleLogoutCertificate")
     def single_logout_certificate(self) -> str:
         """
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/group_assignment.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/group_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/o_auth.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/o_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/o_auth_post_logout_redirect_uri.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/o_auth_post_logout_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/o_auth_redirect_uri.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/o_auth_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/oauth_role_assignment.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/oauth_role_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/outputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/saml.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/saml.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         :param pulumi.Input[str] logo: Local file path to the logo. The file must be in PNG, JPG, or GIF format, and less than 1 MB in size.
         :param pulumi.Input[str] preconfigured_app: name of application from the Okta Integration Network, if not included a custom app will be created.  If not provided the following arguments are required:
         :param pulumi.Input[str] recipient: The location where the app may present the SAML assertion.
         :param pulumi.Input[bool] request_compressed: Denotes whether the request is compressed or not.
         :param pulumi.Input[bool] response_signed: Determines whether the SAML auth response message is digitally signed.
         :param pulumi.Input[bool] saml_signed_request_enabled: SAML Signed Request enabled
         :param pulumi.Input[str] saml_version: SAML version for the app's sign-on mode. Valid values are: `"2.0"` or `"1.1"`. Default is `"2.0"`.
-        :param pulumi.Input[str] signature_algorithm: Signature algorithm used ot digitally sign the assertion and response.
+        :param pulumi.Input[str] signature_algorithm: Signature algorithm used to digitally sign the assertion and response.
         :param pulumi.Input[str] single_logout_certificate: x509 encoded certificate that the Service Provider uses to sign Single Logout requests.  Note: should be provided without `-----BEGIN CERTIFICATE-----` and `-----END CERTIFICATE-----`, see [official documentation](https://developer.okta.com/docs/reference/api/apps/#service-provider-certificate).
         :param pulumi.Input[str] single_logout_issuer: The issuer of the Service Provider that generates the Single Logout request.
         :param pulumi.Input[str] single_logout_url: The location where the logout response is sent.
         :param pulumi.Input[str] sp_issuer: SAML service provider issuer.
         :param pulumi.Input[str] sso_url: Single Sign-on Url.
         :param pulumi.Input[str] status: status of application.
         :param pulumi.Input[str] subject_name_id_format: Identifies the SAML processing rules.
@@ -599,15 +599,15 @@
     def saml_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "saml_version", value)
 
     @property
     @pulumi.getter(name="signatureAlgorithm")
     def signature_algorithm(self) -> Optional[pulumi.Input[str]]:
         """
-        Signature algorithm used ot digitally sign the assertion and response.
+        Signature algorithm used to digitally sign the assertion and response.
         """
         return pulumi.get(self, "signature_algorithm")
 
     @signature_algorithm.setter
     def signature_algorithm(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "signature_algorithm", value)
 
@@ -864,15 +864,15 @@
         :param pulumi.Input[str] preconfigured_app: name of application from the Okta Integration Network, if not included a custom app will be created.  If not provided the following arguments are required:
         :param pulumi.Input[str] recipient: The location where the app may present the SAML assertion.
         :param pulumi.Input[bool] request_compressed: Denotes whether the request is compressed or not.
         :param pulumi.Input[bool] response_signed: Determines whether the SAML auth response message is digitally signed.
         :param pulumi.Input[bool] saml_signed_request_enabled: SAML Signed Request enabled
         :param pulumi.Input[str] saml_version: SAML version for the app's sign-on mode. Valid values are: `"2.0"` or `"1.1"`. Default is `"2.0"`.
         :param pulumi.Input[str] sign_on_mode: Sign-on mode of application.
-        :param pulumi.Input[str] signature_algorithm: Signature algorithm used ot digitally sign the assertion and response.
+        :param pulumi.Input[str] signature_algorithm: Signature algorithm used to digitally sign the assertion and response.
         :param pulumi.Input[str] single_logout_certificate: x509 encoded certificate that the Service Provider uses to sign Single Logout requests.  Note: should be provided without `-----BEGIN CERTIFICATE-----` and `-----END CERTIFICATE-----`, see [official documentation](https://developer.okta.com/docs/reference/api/apps/#service-provider-certificate).
         :param pulumi.Input[str] single_logout_issuer: The issuer of the Service Provider that generates the Single Logout request.
         :param pulumi.Input[str] single_logout_url: The location where the logout response is sent.
         :param pulumi.Input[str] sp_issuer: SAML service provider issuer.
         :param pulumi.Input[str] sso_url: Single Sign-on Url.
         :param pulumi.Input[str] status: status of application.
         :param pulumi.Input[str] subject_name_id_format: Identifies the SAML processing rules.
@@ -1567,15 +1567,15 @@
     def sign_on_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "sign_on_mode", value)
 
     @property
     @pulumi.getter(name="signatureAlgorithm")
     def signature_algorithm(self) -> Optional[pulumi.Input[str]]:
         """
-        Signature algorithm used ot digitally sign the assertion and response.
+        Signature algorithm used to digitally sign the assertion and response.
         """
         return pulumi.get(self, "signature_algorithm")
 
     @signature_algorithm.setter
     def signature_algorithm(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "signature_algorithm", value)
 
@@ -1973,15 +1973,15 @@
         :param pulumi.Input[str] logo: Local file path to the logo. The file must be in PNG, JPG, or GIF format, and less than 1 MB in size.
         :param pulumi.Input[str] preconfigured_app: name of application from the Okta Integration Network, if not included a custom app will be created.  If not provided the following arguments are required:
         :param pulumi.Input[str] recipient: The location where the app may present the SAML assertion.
         :param pulumi.Input[bool] request_compressed: Denotes whether the request is compressed or not.
         :param pulumi.Input[bool] response_signed: Determines whether the SAML auth response message is digitally signed.
         :param pulumi.Input[bool] saml_signed_request_enabled: SAML Signed Request enabled
         :param pulumi.Input[str] saml_version: SAML version for the app's sign-on mode. Valid values are: `"2.0"` or `"1.1"`. Default is `"2.0"`.
-        :param pulumi.Input[str] signature_algorithm: Signature algorithm used ot digitally sign the assertion and response.
+        :param pulumi.Input[str] signature_algorithm: Signature algorithm used to digitally sign the assertion and response.
         :param pulumi.Input[str] single_logout_certificate: x509 encoded certificate that the Service Provider uses to sign Single Logout requests.  Note: should be provided without `-----BEGIN CERTIFICATE-----` and `-----END CERTIFICATE-----`, see [official documentation](https://developer.okta.com/docs/reference/api/apps/#service-provider-certificate).
         :param pulumi.Input[str] single_logout_issuer: The issuer of the Service Provider that generates the Single Logout request.
         :param pulumi.Input[str] single_logout_url: The location where the logout response is sent.
         :param pulumi.Input[str] sp_issuer: SAML service provider issuer.
         :param pulumi.Input[str] sso_url: Single Sign-on Url.
         :param pulumi.Input[str] status: status of application.
         :param pulumi.Input[str] subject_name_id_format: Identifies the SAML processing rules.
@@ -2415,15 +2415,15 @@
         :param pulumi.Input[str] preconfigured_app: name of application from the Okta Integration Network, if not included a custom app will be created.  If not provided the following arguments are required:
         :param pulumi.Input[str] recipient: The location where the app may present the SAML assertion.
         :param pulumi.Input[bool] request_compressed: Denotes whether the request is compressed or not.
         :param pulumi.Input[bool] response_signed: Determines whether the SAML auth response message is digitally signed.
         :param pulumi.Input[bool] saml_signed_request_enabled: SAML Signed Request enabled
         :param pulumi.Input[str] saml_version: SAML version for the app's sign-on mode. Valid values are: `"2.0"` or `"1.1"`. Default is `"2.0"`.
         :param pulumi.Input[str] sign_on_mode: Sign-on mode of application.
-        :param pulumi.Input[str] signature_algorithm: Signature algorithm used ot digitally sign the assertion and response.
+        :param pulumi.Input[str] signature_algorithm: Signature algorithm used to digitally sign the assertion and response.
         :param pulumi.Input[str] single_logout_certificate: x509 encoded certificate that the Service Provider uses to sign Single Logout requests.  Note: should be provided without `-----BEGIN CERTIFICATE-----` and `-----END CERTIFICATE-----`, see [official documentation](https://developer.okta.com/docs/reference/api/apps/#service-provider-certificate).
         :param pulumi.Input[str] single_logout_issuer: The issuer of the Service Provider that generates the Single Logout request.
         :param pulumi.Input[str] single_logout_url: The location where the logout response is sent.
         :param pulumi.Input[str] sp_issuer: SAML service provider issuer.
         :param pulumi.Input[str] sso_url: Single Sign-on Url.
         :param pulumi.Input[str] status: status of application.
         :param pulumi.Input[str] subject_name_id_format: Identifies the SAML processing rules.
@@ -2875,15 +2875,15 @@
         """
         return pulumi.get(self, "sign_on_mode")
 
     @property
     @pulumi.getter(name="signatureAlgorithm")
     def signature_algorithm(self) -> pulumi.Output[Optional[str]]:
         """
-        Signature algorithm used ot digitally sign the assertion and response.
+        Signature algorithm used to digitally sign the assertion and response.
         """
         return pulumi.get(self, "signature_algorithm")
 
     @property
     @pulumi.getter(name="singleLogoutCertificate")
     def single_logout_certificate(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/secure_password_store.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/secure_password_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/swa.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/swa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/three_field.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/three_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         :param pulumi.Input[str] password_selector: Login password field CSS selector.
         :param pulumi.Input[str] url: Login URL.
         :param pulumi.Input[str] username_selector: Login username field CSS selector.
         :param pulumi.Input[str] accessibility_error_redirect_url: Custom error page URL.
         :param pulumi.Input[str] accessibility_login_redirect_url: Custom login page for this application.
         :param pulumi.Input[bool] accessibility_self_service: Enable self-service. By default, it is `false`.
         :param pulumi.Input[str] admin_note: Application notes for admins.
-        :param pulumi.Input[str] app_links_json: Displays specific appLinks for the app
+        :param pulumi.Input[str] app_links_json: Displays specific appLinks for the app. The value for each application link should be boolean.
         :param pulumi.Input[bool] auto_submit_toolbar: Display auto submit toolbar.
         :param pulumi.Input[str] credentials_scheme: Application credentials scheme. Can be set to `"EDIT_USERNAME_AND_PASSWORD"`, `"ADMIN_SETS_CREDENTIALS"`, `"EDIT_PASSWORD_ONLY"`, `"EXTERNAL_PASSWORD_SYNC"`, or `"SHARED_USERNAME_AND_PASSWORD"`.
         :param pulumi.Input[str] enduser_note: Application notes for end users.
         :param pulumi.Input[bool] hide_ios: Do not display application icon on mobile app.
         :param pulumi.Input[bool] hide_web: Do not display application icon to users.
         :param pulumi.Input[str] logo: Local file path to the logo. The file must be in PNG, JPG, or GIF format, and less than 1 MB in size.
         :param pulumi.Input[bool] reveal_password: Allow user to reveal password. It can not be set to `true` if `credentials_scheme` is `"ADMIN_SETS_CREDENTIALS"`, `"SHARED_USERNAME_AND_PASSWORD"` or `"EXTERNAL_PASSWORD_SYNC"`.
@@ -251,15 +251,15 @@
     def admin_note(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "admin_note", value)
 
     @property
     @pulumi.getter(name="appLinksJson")
     def app_links_json(self) -> Optional[pulumi.Input[str]]:
         """
-        Displays specific appLinks for the app
+        Displays specific appLinks for the app. The value for each application link should be boolean.
         """
         return pulumi.get(self, "app_links_json")
 
     @app_links_json.setter
     def app_links_json(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "app_links_json", value)
 
@@ -479,15 +479,15 @@
                  username_selector: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ThreeField resources.
         :param pulumi.Input[str] accessibility_error_redirect_url: Custom error page URL.
         :param pulumi.Input[str] accessibility_login_redirect_url: Custom login page for this application.
         :param pulumi.Input[bool] accessibility_self_service: Enable self-service. By default, it is `false`.
         :param pulumi.Input[str] admin_note: Application notes for admins.
-        :param pulumi.Input[str] app_links_json: Displays specific appLinks for the app
+        :param pulumi.Input[str] app_links_json: Displays specific appLinks for the app. The value for each application link should be boolean.
         :param pulumi.Input[bool] auto_submit_toolbar: Display auto submit toolbar.
         :param pulumi.Input[str] button_selector: Login button field CSS selector.
         :param pulumi.Input[str] credentials_scheme: Application credentials scheme. Can be set to `"EDIT_USERNAME_AND_PASSWORD"`, `"ADMIN_SETS_CREDENTIALS"`, `"EDIT_PASSWORD_ONLY"`, `"EXTERNAL_PASSWORD_SYNC"`, or `"SHARED_USERNAME_AND_PASSWORD"`.
         :param pulumi.Input[str] enduser_note: Application notes for end users.
         :param pulumi.Input[str] extra_field_selector: Extra field CSS selector.
         :param pulumi.Input[str] extra_field_value: Value for extra form field.
         :param pulumi.Input[bool] hide_ios: Do not display application icon on mobile app.
@@ -619,15 +619,15 @@
     def admin_note(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "admin_note", value)
 
     @property
     @pulumi.getter(name="appLinksJson")
     def app_links_json(self) -> Optional[pulumi.Input[str]]:
         """
-        Displays specific appLinks for the app
+        Displays specific appLinks for the app. The value for each application link should be boolean.
         """
         return pulumi.get(self, "app_links_json")
 
     @app_links_json.setter
     def app_links_json(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "app_links_json", value)
 
@@ -982,15 +982,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] accessibility_error_redirect_url: Custom error page URL.
         :param pulumi.Input[str] accessibility_login_redirect_url: Custom login page for this application.
         :param pulumi.Input[bool] accessibility_self_service: Enable self-service. By default, it is `false`.
         :param pulumi.Input[str] admin_note: Application notes for admins.
-        :param pulumi.Input[str] app_links_json: Displays specific appLinks for the app
+        :param pulumi.Input[str] app_links_json: Displays specific appLinks for the app. The value for each application link should be boolean.
         :param pulumi.Input[bool] auto_submit_toolbar: Display auto submit toolbar.
         :param pulumi.Input[str] button_selector: Login button field CSS selector.
         :param pulumi.Input[str] credentials_scheme: Application credentials scheme. Can be set to `"EDIT_USERNAME_AND_PASSWORD"`, `"ADMIN_SETS_CREDENTIALS"`, `"EDIT_PASSWORD_ONLY"`, `"EXTERNAL_PASSWORD_SYNC"`, or `"SHARED_USERNAME_AND_PASSWORD"`.
         :param pulumi.Input[str] enduser_note: Application notes for end users.
         :param pulumi.Input[str] extra_field_selector: Extra field CSS selector.
         :param pulumi.Input[str] extra_field_value: Value for extra form field.
         :param pulumi.Input[bool] hide_ios: Do not display application icon on mobile app.
@@ -1173,15 +1173,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] accessibility_error_redirect_url: Custom error page URL.
         :param pulumi.Input[str] accessibility_login_redirect_url: Custom login page for this application.
         :param pulumi.Input[bool] accessibility_self_service: Enable self-service. By default, it is `false`.
         :param pulumi.Input[str] admin_note: Application notes for admins.
-        :param pulumi.Input[str] app_links_json: Displays specific appLinks for the app
+        :param pulumi.Input[str] app_links_json: Displays specific appLinks for the app. The value for each application link should be boolean.
         :param pulumi.Input[bool] auto_submit_toolbar: Display auto submit toolbar.
         :param pulumi.Input[str] button_selector: Login button field CSS selector.
         :param pulumi.Input[str] credentials_scheme: Application credentials scheme. Can be set to `"EDIT_USERNAME_AND_PASSWORD"`, `"ADMIN_SETS_CREDENTIALS"`, `"EDIT_PASSWORD_ONLY"`, `"EXTERNAL_PASSWORD_SYNC"`, or `"SHARED_USERNAME_AND_PASSWORD"`.
         :param pulumi.Input[str] enduser_note: Application notes for end users.
         :param pulumi.Input[str] extra_field_selector: Extra field CSS selector.
         :param pulumi.Input[str] extra_field_value: Value for extra form field.
         :param pulumi.Input[bool] hide_ios: Do not display application icon on mobile app.
@@ -1272,15 +1272,15 @@
         """
         return pulumi.get(self, "admin_note")
 
     @property
     @pulumi.getter(name="appLinksJson")
     def app_links_json(self) -> pulumi.Output[Optional[str]]:
         """
-        Displays specific appLinks for the app
+        Displays specific appLinks for the app. The value for each application link should be boolean.
         """
         return pulumi.get(self, "app_links_json")
 
     @property
     @pulumi.getter(name="autoSubmitToolbar")
     def auto_submit_toolbar(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app/user.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app_group_assignments.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app_oauth_api_scope.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_oauth_api_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app_saml_app_settings.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_saml_app_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app_shared_credentials.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_shared_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app_signon_policy.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app_signon_policy_rule.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_signon_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app_user_base_schema_property.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/app_user_schema_property.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_user_schema_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         :param pulumi.Input[int] max_length: The maximum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[int] min_length: The minimum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[Sequence[pulumi.Input['AppUserSchemaPropertyOneOfArgs']]] one_ofs: Array of maps containing a mapping for display name to enum value.
         :param pulumi.Input[str] permissions: Access control permissions for the property. It can be set to `"READ_WRITE"`, `"READ_ONLY"`, `"HIDE"`.
         :param pulumi.Input[bool] required: Whether the property is required for this application's users.
         :param pulumi.Input[str] scope: determines whether an app user attribute can be set at the Personal `"SELF"` or Group `"NONE"` level. Default value is `"NONE"`.
         :param pulumi.Input[bool] union: If `type` is set to `"array"`, used to set whether attribute value is determined by group priority `false`, or combine values across groups `true`. Can not be set to `true` if `scope` is set to `"SELF"`.
-        :param pulumi.Input[str] unique: Subschema unique restriction
-        :param pulumi.Input[str] user_type: Custom subschema user type
+        :param pulumi.Input[str] unique: Whether the property should be unique. It can be set to `UNIQUE_VALIDATED` or `NOT_UNIQUE`.
+        :param pulumi.Input[str] user_type: User type ID. By default, it is `default`
         """
         pulumi.set(__self__, "app_id", app_id)
         pulumi.set(__self__, "index", index)
         pulumi.set(__self__, "title", title)
         pulumi.set(__self__, "type", type)
         if array_enums is not None:
             pulumi.set(__self__, "array_enums", array_enums)
@@ -328,27 +328,27 @@
     def union(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "union", value)
 
     @property
     @pulumi.getter
     def unique(self) -> Optional[pulumi.Input[str]]:
         """
-        Subschema unique restriction
+        Whether the property should be unique. It can be set to `UNIQUE_VALIDATED` or `NOT_UNIQUE`.
         """
         return pulumi.get(self, "unique")
 
     @unique.setter
     def unique(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "unique", value)
 
     @property
     @pulumi.getter(name="userType")
     def user_type(self) -> Optional[pulumi.Input[str]]:
         """
-        Custom subschema user type
+        User type ID. By default, it is `default`
         """
         return pulumi.get(self, "user_type")
 
     @user_type.setter
     def user_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_type", value)
 
@@ -394,16 +394,16 @@
         :param pulumi.Input[Sequence[pulumi.Input['AppUserSchemaPropertyOneOfArgs']]] one_ofs: Array of maps containing a mapping for display name to enum value.
         :param pulumi.Input[str] permissions: Access control permissions for the property. It can be set to `"READ_WRITE"`, `"READ_ONLY"`, `"HIDE"`.
         :param pulumi.Input[bool] required: Whether the property is required for this application's users.
         :param pulumi.Input[str] scope: determines whether an app user attribute can be set at the Personal `"SELF"` or Group `"NONE"` level. Default value is `"NONE"`.
         :param pulumi.Input[str] title: display name for the enum value.
         :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[bool] union: If `type` is set to `"array"`, used to set whether attribute value is determined by group priority `false`, or combine values across groups `true`. Can not be set to `true` if `scope` is set to `"SELF"`.
-        :param pulumi.Input[str] unique: Subschema unique restriction
-        :param pulumi.Input[str] user_type: Custom subschema user type
+        :param pulumi.Input[str] unique: Whether the property should be unique. It can be set to `UNIQUE_VALIDATED` or `NOT_UNIQUE`.
+        :param pulumi.Input[str] user_type: User type ID. By default, it is `default`
         """
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if array_enums is not None:
             pulumi.set(__self__, "array_enums", array_enums)
         if array_one_ofs is not None:
             pulumi.set(__self__, "array_one_ofs", array_one_ofs)
@@ -672,27 +672,27 @@
     def union(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "union", value)
 
     @property
     @pulumi.getter
     def unique(self) -> Optional[pulumi.Input[str]]:
         """
-        Subschema unique restriction
+        Whether the property should be unique. It can be set to `UNIQUE_VALIDATED` or `NOT_UNIQUE`.
         """
         return pulumi.get(self, "unique")
 
     @unique.setter
     def unique(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "unique", value)
 
     @property
     @pulumi.getter(name="userType")
     def user_type(self) -> Optional[pulumi.Input[str]]:
         """
-        Custom subschema user type
+        User type ID. By default, it is `default`
         """
         return pulumi.get(self, "user_type")
 
     @user_type.setter
     def user_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_type", value)
 
@@ -768,16 +768,16 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AppUserSchemaPropertyOneOfArgs']]]] one_ofs: Array of maps containing a mapping for display name to enum value.
         :param pulumi.Input[str] permissions: Access control permissions for the property. It can be set to `"READ_WRITE"`, `"READ_ONLY"`, `"HIDE"`.
         :param pulumi.Input[bool] required: Whether the property is required for this application's users.
         :param pulumi.Input[str] scope: determines whether an app user attribute can be set at the Personal `"SELF"` or Group `"NONE"` level. Default value is `"NONE"`.
         :param pulumi.Input[str] title: display name for the enum value.
         :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[bool] union: If `type` is set to `"array"`, used to set whether attribute value is determined by group priority `false`, or combine values across groups `true`. Can not be set to `true` if `scope` is set to `"SELF"`.
-        :param pulumi.Input[str] unique: Subschema unique restriction
-        :param pulumi.Input[str] user_type: Custom subschema user type
+        :param pulumi.Input[str] unique: Whether the property should be unique. It can be set to `UNIQUE_VALIDATED` or `NOT_UNIQUE`.
+        :param pulumi.Input[str] user_type: User type ID. By default, it is `default`
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: AppUserSchemaPropertyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -935,16 +935,16 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AppUserSchemaPropertyOneOfArgs']]]] one_ofs: Array of maps containing a mapping for display name to enum value.
         :param pulumi.Input[str] permissions: Access control permissions for the property. It can be set to `"READ_WRITE"`, `"READ_ONLY"`, `"HIDE"`.
         :param pulumi.Input[bool] required: Whether the property is required for this application's users.
         :param pulumi.Input[str] scope: determines whether an app user attribute can be set at the Personal `"SELF"` or Group `"NONE"` level. Default value is `"NONE"`.
         :param pulumi.Input[str] title: display name for the enum value.
         :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[bool] union: If `type` is set to `"array"`, used to set whether attribute value is determined by group priority `false`, or combine values across groups `true`. Can not be set to `true` if `scope` is set to `"SELF"`.
-        :param pulumi.Input[str] unique: Subschema unique restriction
-        :param pulumi.Input[str] user_type: Custom subschema user type
+        :param pulumi.Input[str] unique: Whether the property should be unique. It can be set to `UNIQUE_VALIDATED` or `NOT_UNIQUE`.
+        :param pulumi.Input[str] user_type: User type ID. By default, it is `default`
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _AppUserSchemaPropertyState.__new__(_AppUserSchemaPropertyState)
 
         __props__.__dict__["app_id"] = app_id
         __props__.__dict__["array_enums"] = array_enums
@@ -1121,19 +1121,19 @@
         """
         return pulumi.get(self, "union")
 
     @property
     @pulumi.getter
     def unique(self) -> pulumi.Output[Optional[str]]:
         """
-        Subschema unique restriction
+        Whether the property should be unique. It can be set to `UNIQUE_VALIDATED` or `NOT_UNIQUE`.
         """
         return pulumi.get(self, "unique")
 
     @property
     @pulumi.getter(name="userType")
     def user_type(self) -> pulumi.Output[Optional[str]]:
         """
-        Custom subschema user type
+        User type ID. By default, it is `default`
         """
         return pulumi.get(self, "user_type")
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/__init__.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/get_server.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/get_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/get_server_policy.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/get_server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/get_server_scopes.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/get_server_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/outputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/server.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/server_claim.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/server_policy.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/server_policy_claim.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_policy_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/server_policy_rule.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/auth/server_scope.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/auth_server_claim_default.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth_server_claim_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/auth_server_default.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth_server_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/authenticator.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/behaviour.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/brand.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/captcha.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/captcha.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/captcha_org_wide_settings.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/captcha_org_wide_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/config/__init__.pyi` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/config/vars.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/domain.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/domain_certificate.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/domain_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/domain_verification.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/email_customization.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/email_sender.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/email_sender.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/email_sender_verification.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/email_sender_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/event_hook.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/event_hook.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         """
         The set of arguments for constructing a EventHook resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] channel: Details of the endpoint the event hook will hit.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: The events that will be delivered to this hook. [See here for a list of supported events](https://developer.okta.com/docs/reference/api/event-types/?q=event-hook-eligible).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] auth: Authentication required for event hook request.
         :param pulumi.Input[Sequence[pulumi.Input['EventHookHeaderArgs']]] headers: Map of headers to send along in event hook request.
         :param pulumi.Input[str] name: The event hook display name.
+        :param pulumi.Input[str] status: Default to `ACTIVE`
         """
         pulumi.set(__self__, "channel", channel)
         pulumi.set(__self__, "events", events)
         if auth is not None:
             pulumi.set(__self__, "auth", auth)
         if headers is not None:
             pulumi.set(__self__, "headers", headers)
@@ -100,14 +101,17 @@
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
+        """
+        Default to `ACTIVE`
+        """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
 
@@ -123,14 +127,15 @@
         """
         Input properties used for looking up and filtering EventHook resources.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] auth: Authentication required for event hook request.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] channel: Details of the endpoint the event hook will hit.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: The events that will be delivered to this hook. [See here for a list of supported events](https://developer.okta.com/docs/reference/api/event-types/?q=event-hook-eligible).
         :param pulumi.Input[Sequence[pulumi.Input['EventHookHeaderArgs']]] headers: Map of headers to send along in event hook request.
         :param pulumi.Input[str] name: The event hook display name.
+        :param pulumi.Input[str] status: Default to `ACTIVE`
         """
         if auth is not None:
             pulumi.set(__self__, "auth", auth)
         if channel is not None:
             pulumi.set(__self__, "channel", channel)
         if events is not None:
             pulumi.set(__self__, "events", events)
@@ -200,14 +205,17 @@
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
+        """
+        Default to `ACTIVE`
+        """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
 
@@ -264,14 +272,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] auth: Authentication required for event hook request.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] channel: Details of the endpoint the event hook will hit.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: The events that will be delivered to this hook. [See here for a list of supported events](https://developer.okta.com/docs/reference/api/event-types/?q=event-hook-eligible).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EventHookHeaderArgs']]]] headers: Map of headers to send along in event hook request.
         :param pulumi.Input[str] name: The event hook display name.
+        :param pulumi.Input[str] status: Default to `ACTIVE`
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: EventHookArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -377,14 +386,15 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] auth: Authentication required for event hook request.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] channel: Details of the endpoint the event hook will hit.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: The events that will be delivered to this hook. [See here for a list of supported events](https://developer.okta.com/docs/reference/api/event-types/?q=event-hook-eligible).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EventHookHeaderArgs']]]] headers: Map of headers to send along in event hook request.
         :param pulumi.Input[str] name: The event hook display name.
+        :param pulumi.Input[str] status: Default to `ACTIVE`
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _EventHookState.__new__(_EventHookState)
 
         __props__.__dict__["auth"] = auth
         __props__.__dict__["channel"] = channel
@@ -433,9 +443,12 @@
         The event hook display name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Output[Optional[str]]:
+        """
+        Default to `ACTIVE`
+        """
         return pulumi.get(self, "status")
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/event_hook_verification.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/event_hook_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/factor/factor.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/factor/factor.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/factor_totp.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/factor_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_app_group_assignments.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_app_signon_policy.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_app_user_assignments.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_app_user_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_auth_server_claim.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_auth_server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_auth_server_claims.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_auth_server_claims.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_authenticator.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_behaviour.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_behaviours.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_behaviours.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_brand.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_brands.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_brands.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_email_customization.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_email_customizations.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_email_customizations.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_groups.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_network_zone.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_network_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_role_subscription.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_role_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     <!--End PulumiCodeChooser -->
 
 
     :param str notification_type: Type of the notification. Valid values: `"CONNECTOR_AGENT"`, `"USER_LOCKED_OUT"`, 
            `"APP_IMPORT"`, `"LDAP_AGENT"`, `"AD_AGENT"`, `"OKTA_ANNOUNCEMENT"`, `"OKTA_ISSUE"`, `"OKTA_UPDATE"`, `"IWA_AGENT"`,
            `"USER_DEPROVISION"`, `"REPORT_SUSPICIOUS_ACTIVITY"`, `"RATELIMIT_NOTIFICATION"`.
     :param str role_type: Type of the role. Valid values:
-           `"API_ADMIN"`,
+           `"API_ACCESS_MANAGEMENT_ADMIN"`,
            `"APP_ADMIN"`,
            `"CUSTOM"`,
            `"GROUP_MEMBERSHIP_ADMIN"`,
            `"HELP_DESK_ADMIN"`,
            `"MOBILE_ADMIN"`,
            `"ORG_ADMIN"`,
            `"READ_ONLY_ADMIN"`,
@@ -143,15 +143,15 @@
     <!--End PulumiCodeChooser -->
 
 
     :param str notification_type: Type of the notification. Valid values: `"CONNECTOR_AGENT"`, `"USER_LOCKED_OUT"`, 
            `"APP_IMPORT"`, `"LDAP_AGENT"`, `"AD_AGENT"`, `"OKTA_ANNOUNCEMENT"`, `"OKTA_ISSUE"`, `"OKTA_UPDATE"`, `"IWA_AGENT"`,
            `"USER_DEPROVISION"`, `"REPORT_SUSPICIOUS_ACTIVITY"`, `"RATELIMIT_NOTIFICATION"`.
     :param str role_type: Type of the role. Valid values:
-           `"API_ADMIN"`,
+           `"API_ACCESS_MANAGEMENT_ADMIN"`,
            `"APP_ADMIN"`,
            `"CUSTOM"`,
            `"GROUP_MEMBERSHIP_ADMIN"`,
            `"HELP_DESK_ADMIN"`,
            `"MOBILE_ADMIN"`,
            `"ORG_ADMIN"`,
            `"READ_ONLY_ADMIN"`,
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_template.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_templates.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_theme.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_themes.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_themes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_trusted_origins.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_trusted_origins.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/get_user_security_questions.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_user_security_questions.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/group/get_everyone_group.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/group/get_everyone_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/group/get_group.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/group/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/group/get_rule.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/group/get_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/group/group.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/group/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/group/role.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/group/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                  disable_notifications: Optional[pulumi.Input[bool]] = None,
                  target_app_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  target_group_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a Role resource.
         :param pulumi.Input[str] group_id: The ID of group to attach admin roles to.
         :param pulumi.Input[str] role_type: Admin role assigned to the group. It can be any one of the following values:
-               `"API_ADMIN"`,
+               `"API_ACCESS_MANAGEMENT_ADMIN"`,
                `"APP_ADMIN"`,
                `"CUSTOM"`,
                `"GROUP_MEMBERSHIP_ADMIN"`,
                `"HELP_DESK_ADMIN"`,
                `"MOBILE_ADMIN"`,
                `"ORG_ADMIN"`,
                `"READ_ONLY_ADMIN"`,
@@ -69,15 +69,15 @@
         pulumi.set(self, "group_id", value)
 
     @property
     @pulumi.getter(name="roleType")
     def role_type(self) -> pulumi.Input[str]:
         """
         Admin role assigned to the group. It can be any one of the following values:
-        `"API_ADMIN"`,
+        `"API_ACCESS_MANAGEMENT_ADMIN"`,
         `"APP_ADMIN"`,
         `"CUSTOM"`,
         `"GROUP_MEMBERSHIP_ADMIN"`,
         `"HELP_DESK_ADMIN"`,
         `"MOBILE_ADMIN"`,
         `"ORG_ADMIN"`,
         `"READ_ONLY_ADMIN"`,
@@ -147,15 +147,15 @@
                  target_group_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering Role resources.
         :param pulumi.Input[bool] disable_notifications: When this setting is enabled, the admins won't receive any of the default Okta
                administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
         :param pulumi.Input[str] group_id: The ID of group to attach admin roles to.
         :param pulumi.Input[str] role_type: Admin role assigned to the group. It can be any one of the following values:
-               `"API_ADMIN"`,
+               `"API_ACCESS_MANAGEMENT_ADMIN"`,
                `"APP_ADMIN"`,
                `"CUSTOM"`,
                `"GROUP_MEMBERSHIP_ADMIN"`,
                `"HELP_DESK_ADMIN"`,
                `"MOBILE_ADMIN"`,
                `"ORG_ADMIN"`,
                `"READ_ONLY_ADMIN"`,
@@ -210,15 +210,15 @@
         pulumi.set(self, "group_id", value)
 
     @property
     @pulumi.getter(name="roleType")
     def role_type(self) -> Optional[pulumi.Input[str]]:
         """
         Admin role assigned to the group. It can be any one of the following values:
-        `"API_ADMIN"`,
+        `"API_ACCESS_MANAGEMENT_ADMIN"`,
         `"APP_ADMIN"`,
         `"CUSTOM"`,
         `"GROUP_MEMBERSHIP_ADMIN"`,
         `"HELP_DESK_ADMIN"`,
         `"MOBILE_ADMIN"`,
         `"ORG_ADMIN"`,
         `"READ_ONLY_ADMIN"`,
@@ -305,15 +305,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] disable_notifications: When this setting is enabled, the admins won't receive any of the default Okta
                administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
         :param pulumi.Input[str] group_id: The ID of group to attach admin roles to.
         :param pulumi.Input[str] role_type: Admin role assigned to the group. It can be any one of the following values:
-               `"API_ADMIN"`,
+               `"API_ACCESS_MANAGEMENT_ADMIN"`,
                `"APP_ADMIN"`,
                `"CUSTOM"`,
                `"GROUP_MEMBERSHIP_ADMIN"`,
                `"HELP_DESK_ADMIN"`,
                `"MOBILE_ADMIN"`,
                `"ORG_ADMIN"`,
                `"READ_ONLY_ADMIN"`,
@@ -424,15 +424,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] disable_notifications: When this setting is enabled, the admins won't receive any of the default Okta
                administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
         :param pulumi.Input[str] group_id: The ID of group to attach admin roles to.
         :param pulumi.Input[str] role_type: Admin role assigned to the group. It can be any one of the following values:
-               `"API_ADMIN"`,
+               `"API_ACCESS_MANAGEMENT_ADMIN"`,
                `"APP_ADMIN"`,
                `"CUSTOM"`,
                `"GROUP_MEMBERSHIP_ADMIN"`,
                `"HELP_DESK_ADMIN"`,
                `"MOBILE_ADMIN"`,
                `"ORG_ADMIN"`,
                `"READ_ONLY_ADMIN"`,
@@ -479,15 +479,15 @@
         return pulumi.get(self, "group_id")
 
     @property
     @pulumi.getter(name="roleType")
     def role_type(self) -> pulumi.Output[str]:
         """
         Admin role assigned to the group. It can be any one of the following values:
-        `"API_ADMIN"`,
+        `"API_ACCESS_MANAGEMENT_ADMIN"`,
         `"APP_ADMIN"`,
         `"CUSTOM"`,
         `"GROUP_MEMBERSHIP_ADMIN"`,
         `"HELP_DESK_ADMIN"`,
         `"MOBILE_ADMIN"`,
         `"ORG_ADMIN"`,
         `"READ_ONLY_ADMIN"`,
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/group/rule.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/group/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/group_memberships.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/group_schema_property.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/group_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/get_metadata_saml.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/get_oidc.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/get_saml.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/get_social.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/oidc.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/oidc.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
                  groups_action: Optional[pulumi.Input[str]] = None,
                  groups_assignments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  groups_attribute: Optional[pulumi.Input[str]] = None,
                  groups_filters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  issuer_mode: Optional[pulumi.Input[str]] = None,
                  max_clock_skew: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 pkce_required: Optional[pulumi.Input[bool]] = None,
                  profile_master: Optional[pulumi.Input[bool]] = None,
                  protocol_type: Optional[pulumi.Input[str]] = None,
                  provisioning_action: Optional[pulumi.Input[str]] = None,
                  request_signature_algorithm: Optional[pulumi.Input[str]] = None,
                  request_signature_scope: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  subject_match_attribute: Optional[pulumi.Input[str]] = None,
@@ -65,16 +64,14 @@
         :param pulumi.Input[str] groups_action: Provisioning action for IdP user's group memberships. It can be `"NONE"`, `"SYNC"`, `"APPEND"`, or `"ASSIGN"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_assignments: List of Okta Group IDs to add an IdP user as a member with the `"ASSIGN"` `groups_action`.
         :param pulumi.Input[str] groups_attribute: IdP user profile attribute name (case-insensitive) for an array value that contains group memberships.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_filters: Whitelist of Okta Group identifiers that are allowed for the `"APPEND"` or `"SYNC"` `groups_action`.
         :param pulumi.Input[str] issuer_mode: Indicates whether Okta uses the original Okta org domain URL, a custom domain URL, or dynamic. It can be `"ORG_URL"`, `"CUSTOM_URL"`, or `"DYNAMIC"`.
         :param pulumi.Input[int] max_clock_skew: Maximum allowable clock-skew when processing messages from the IdP.
         :param pulumi.Input[str] name: The Application's display name.
-        :param pulumi.Input[bool] pkce_required: Require Proof Key for Code Exchange (PKCE) for additional verification key rotation mode. See:
-               https://developer.okta.com/docs/reference/api/idps/#oauth-2-0-and-openid-connect-client-object
         :param pulumi.Input[bool] profile_master: Determines if the IdP should act as a source of truth for user profile attributes.
         :param pulumi.Input[str] protocol_type: The type of protocol to use. It can be `"OIDC"` or `"OAUTH2"`.
         :param pulumi.Input[str] provisioning_action: Provisioning action for an IdP user during authentication.
         :param pulumi.Input[str] request_signature_algorithm: The HMAC Signature Algorithm used when signing an authorization request. Defaults to `"HS256"`. It can be `"HS256"`, `"HS384"`, `"HS512"`, `"SHA-256"`. `"RS256"`, `"RS384"`, or `"RS512"`. NOTE: `"SHA-256"` an undocumented legacy value and not continue to be valid. See API docs https://developer.okta.com/docs/reference/api/idps/#oidc-request-signature-algorithm-object
         :param pulumi.Input[str] request_signature_scope: Specifies whether to digitally sign an AuthnRequest messages to the IdP. Defaults to `"REQUEST"`. It can be `"REQUEST"` or `"NONE"`.
         :param pulumi.Input[str] status: Status of the IdP.
         :param pulumi.Input[str] subject_match_attribute: Okta user profile attribute for matching transformed IdP username. Only for matchType `"CUSTOM_ATTRIBUTE"`.
@@ -109,16 +106,14 @@
             pulumi.set(__self__, "groups_filters", groups_filters)
         if issuer_mode is not None:
             pulumi.set(__self__, "issuer_mode", issuer_mode)
         if max_clock_skew is not None:
             pulumi.set(__self__, "max_clock_skew", max_clock_skew)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if pkce_required is not None:
-            pulumi.set(__self__, "pkce_required", pkce_required)
         if profile_master is not None:
             pulumi.set(__self__, "profile_master", profile_master)
         if protocol_type is not None:
             pulumi.set(__self__, "protocol_type", protocol_type)
         if provisioning_action is not None:
             pulumi.set(__self__, "provisioning_action", provisioning_action)
         if request_signature_algorithm is not None:
@@ -377,27 +372,14 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="pkceRequired")
-    def pkce_required(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Require Proof Key for Code Exchange (PKCE) for additional verification key rotation mode. See:
-        https://developer.okta.com/docs/reference/api/idps/#oauth-2-0-and-openid-connect-client-object
-        """
-        return pulumi.get(self, "pkce_required")
-
-    @pkce_required.setter
-    def pkce_required(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "pkce_required", value)
-
-    @property
     @pulumi.getter(name="profileMaster")
     def profile_master(self) -> Optional[pulumi.Input[bool]]:
         """
         Determines if the IdP should act as a source of truth for user profile attributes.
         """
         return pulumi.get(self, "profile_master")
 
@@ -551,15 +533,14 @@
                  groups_filters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  issuer_mode: Optional[pulumi.Input[str]] = None,
                  issuer_url: Optional[pulumi.Input[str]] = None,
                  jwks_binding: Optional[pulumi.Input[str]] = None,
                  jwks_url: Optional[pulumi.Input[str]] = None,
                  max_clock_skew: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 pkce_required: Optional[pulumi.Input[bool]] = None,
                  profile_master: Optional[pulumi.Input[bool]] = None,
                  protocol_type: Optional[pulumi.Input[str]] = None,
                  provisioning_action: Optional[pulumi.Input[str]] = None,
                  request_signature_algorithm: Optional[pulumi.Input[str]] = None,
                  request_signature_scope: Optional[pulumi.Input[str]] = None,
                  scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  status: Optional[pulumi.Input[str]] = None,
@@ -588,16 +569,14 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_filters: Whitelist of Okta Group identifiers that are allowed for the `"APPEND"` or `"SYNC"` `groups_action`.
         :param pulumi.Input[str] issuer_mode: Indicates whether Okta uses the original Okta org domain URL, a custom domain URL, or dynamic. It can be `"ORG_URL"`, `"CUSTOM_URL"`, or `"DYNAMIC"`.
         :param pulumi.Input[str] issuer_url: URI that identifies the issuer.
         :param pulumi.Input[str] jwks_binding: The method of making a request for the OIDC JWKS. It can be set to `"HTTP-POST"` or `"HTTP-REDIRECT"`.
         :param pulumi.Input[str] jwks_url: Endpoint where the keys signer publishes its keys in a JWK Set.
         :param pulumi.Input[int] max_clock_skew: Maximum allowable clock-skew when processing messages from the IdP.
         :param pulumi.Input[str] name: The Application's display name.
-        :param pulumi.Input[bool] pkce_required: Require Proof Key for Code Exchange (PKCE) for additional verification key rotation mode. See:
-               https://developer.okta.com/docs/reference/api/idps/#oauth-2-0-and-openid-connect-client-object
         :param pulumi.Input[bool] profile_master: Determines if the IdP should act as a source of truth for user profile attributes.
         :param pulumi.Input[str] protocol_type: The type of protocol to use. It can be `"OIDC"` or `"OAUTH2"`.
         :param pulumi.Input[str] provisioning_action: Provisioning action for an IdP user during authentication.
         :param pulumi.Input[str] request_signature_algorithm: The HMAC Signature Algorithm used when signing an authorization request. Defaults to `"HS256"`. It can be `"HS256"`, `"HS384"`, `"HS512"`, `"SHA-256"`. `"RS256"`, `"RS384"`, or `"RS512"`. NOTE: `"SHA-256"` an undocumented legacy value and not continue to be valid. See API docs https://developer.okta.com/docs/reference/api/idps/#oidc-request-signature-algorithm-object
         :param pulumi.Input[str] request_signature_scope: Specifies whether to digitally sign an AuthnRequest messages to the IdP. Defaults to `"REQUEST"`. It can be `"REQUEST"` or `"NONE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scopes of the IdP.
         :param pulumi.Input[str] status: Status of the IdP.
@@ -641,16 +620,14 @@
             pulumi.set(__self__, "jwks_binding", jwks_binding)
         if jwks_url is not None:
             pulumi.set(__self__, "jwks_url", jwks_url)
         if max_clock_skew is not None:
             pulumi.set(__self__, "max_clock_skew", max_clock_skew)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if pkce_required is not None:
-            pulumi.set(__self__, "pkce_required", pkce_required)
         if profile_master is not None:
             pulumi.set(__self__, "profile_master", profile_master)
         if protocol_type is not None:
             pulumi.set(__self__, "protocol_type", protocol_type)
         if provisioning_action is not None:
             pulumi.set(__self__, "provisioning_action", provisioning_action)
         if request_signature_algorithm is not None:
@@ -883,27 +860,14 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="pkceRequired")
-    def pkce_required(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Require Proof Key for Code Exchange (PKCE) for additional verification key rotation mode. See:
-        https://developer.okta.com/docs/reference/api/idps/#oauth-2-0-and-openid-connect-client-object
-        """
-        return pulumi.get(self, "pkce_required")
-
-    @pkce_required.setter
-    def pkce_required(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "pkce_required", value)
-
-    @property
     @pulumi.getter(name="profileMaster")
     def profile_master(self) -> Optional[pulumi.Input[bool]]:
         """
         Determines if the IdP should act as a source of truth for user profile attributes.
         """
         return pulumi.get(self, "profile_master")
 
@@ -1119,15 +1083,14 @@
                  groups_filters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  issuer_mode: Optional[pulumi.Input[str]] = None,
                  issuer_url: Optional[pulumi.Input[str]] = None,
                  jwks_binding: Optional[pulumi.Input[str]] = None,
                  jwks_url: Optional[pulumi.Input[str]] = None,
                  max_clock_skew: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 pkce_required: Optional[pulumi.Input[bool]] = None,
                  profile_master: Optional[pulumi.Input[bool]] = None,
                  protocol_type: Optional[pulumi.Input[str]] = None,
                  provisioning_action: Optional[pulumi.Input[str]] = None,
                  request_signature_algorithm: Optional[pulumi.Input[str]] = None,
                  request_signature_scope: Optional[pulumi.Input[str]] = None,
                  scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  status: Optional[pulumi.Input[str]] = None,
@@ -1192,16 +1155,14 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_filters: Whitelist of Okta Group identifiers that are allowed for the `"APPEND"` or `"SYNC"` `groups_action`.
         :param pulumi.Input[str] issuer_mode: Indicates whether Okta uses the original Okta org domain URL, a custom domain URL, or dynamic. It can be `"ORG_URL"`, `"CUSTOM_URL"`, or `"DYNAMIC"`.
         :param pulumi.Input[str] issuer_url: URI that identifies the issuer.
         :param pulumi.Input[str] jwks_binding: The method of making a request for the OIDC JWKS. It can be set to `"HTTP-POST"` or `"HTTP-REDIRECT"`.
         :param pulumi.Input[str] jwks_url: Endpoint where the keys signer publishes its keys in a JWK Set.
         :param pulumi.Input[int] max_clock_skew: Maximum allowable clock-skew when processing messages from the IdP.
         :param pulumi.Input[str] name: The Application's display name.
-        :param pulumi.Input[bool] pkce_required: Require Proof Key for Code Exchange (PKCE) for additional verification key rotation mode. See:
-               https://developer.okta.com/docs/reference/api/idps/#oauth-2-0-and-openid-connect-client-object
         :param pulumi.Input[bool] profile_master: Determines if the IdP should act as a source of truth for user profile attributes.
         :param pulumi.Input[str] protocol_type: The type of protocol to use. It can be `"OIDC"` or `"OAUTH2"`.
         :param pulumi.Input[str] provisioning_action: Provisioning action for an IdP user during authentication.
         :param pulumi.Input[str] request_signature_algorithm: The HMAC Signature Algorithm used when signing an authorization request. Defaults to `"HS256"`. It can be `"HS256"`, `"HS384"`, `"HS512"`, `"SHA-256"`. `"RS256"`, `"RS384"`, or `"RS512"`. NOTE: `"SHA-256"` an undocumented legacy value and not continue to be valid. See API docs https://developer.okta.com/docs/reference/api/idps/#oidc-request-signature-algorithm-object
         :param pulumi.Input[str] request_signature_scope: Specifies whether to digitally sign an AuthnRequest messages to the IdP. Defaults to `"REQUEST"`. It can be `"REQUEST"` or `"NONE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scopes of the IdP.
         :param pulumi.Input[str] status: Status of the IdP.
@@ -1284,15 +1245,14 @@
                  groups_filters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  issuer_mode: Optional[pulumi.Input[str]] = None,
                  issuer_url: Optional[pulumi.Input[str]] = None,
                  jwks_binding: Optional[pulumi.Input[str]] = None,
                  jwks_url: Optional[pulumi.Input[str]] = None,
                  max_clock_skew: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 pkce_required: Optional[pulumi.Input[bool]] = None,
                  profile_master: Optional[pulumi.Input[bool]] = None,
                  protocol_type: Optional[pulumi.Input[str]] = None,
                  provisioning_action: Optional[pulumi.Input[str]] = None,
                  request_signature_algorithm: Optional[pulumi.Input[str]] = None,
                  request_signature_scope: Optional[pulumi.Input[str]] = None,
                  scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  status: Optional[pulumi.Input[str]] = None,
@@ -1340,15 +1300,14 @@
                 raise TypeError("Missing required property 'jwks_binding'")
             __props__.__dict__["jwks_binding"] = jwks_binding
             if jwks_url is None and not opts.urn:
                 raise TypeError("Missing required property 'jwks_url'")
             __props__.__dict__["jwks_url"] = jwks_url
             __props__.__dict__["max_clock_skew"] = max_clock_skew
             __props__.__dict__["name"] = name
-            __props__.__dict__["pkce_required"] = pkce_required
             __props__.__dict__["profile_master"] = profile_master
             __props__.__dict__["protocol_type"] = protocol_type
             __props__.__dict__["provisioning_action"] = provisioning_action
             __props__.__dict__["request_signature_algorithm"] = request_signature_algorithm
             __props__.__dict__["request_signature_scope"] = request_signature_scope
             if scopes is None and not opts.urn:
                 raise TypeError("Missing required property 'scopes'")
@@ -1393,15 +1352,14 @@
             groups_filters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             issuer_mode: Optional[pulumi.Input[str]] = None,
             issuer_url: Optional[pulumi.Input[str]] = None,
             jwks_binding: Optional[pulumi.Input[str]] = None,
             jwks_url: Optional[pulumi.Input[str]] = None,
             max_clock_skew: Optional[pulumi.Input[int]] = None,
             name: Optional[pulumi.Input[str]] = None,
-            pkce_required: Optional[pulumi.Input[bool]] = None,
             profile_master: Optional[pulumi.Input[bool]] = None,
             protocol_type: Optional[pulumi.Input[str]] = None,
             provisioning_action: Optional[pulumi.Input[str]] = None,
             request_signature_algorithm: Optional[pulumi.Input[str]] = None,
             request_signature_scope: Optional[pulumi.Input[str]] = None,
             scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             status: Optional[pulumi.Input[str]] = None,
@@ -1435,16 +1393,14 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_filters: Whitelist of Okta Group identifiers that are allowed for the `"APPEND"` or `"SYNC"` `groups_action`.
         :param pulumi.Input[str] issuer_mode: Indicates whether Okta uses the original Okta org domain URL, a custom domain URL, or dynamic. It can be `"ORG_URL"`, `"CUSTOM_URL"`, or `"DYNAMIC"`.
         :param pulumi.Input[str] issuer_url: URI that identifies the issuer.
         :param pulumi.Input[str] jwks_binding: The method of making a request for the OIDC JWKS. It can be set to `"HTTP-POST"` or `"HTTP-REDIRECT"`.
         :param pulumi.Input[str] jwks_url: Endpoint where the keys signer publishes its keys in a JWK Set.
         :param pulumi.Input[int] max_clock_skew: Maximum allowable clock-skew when processing messages from the IdP.
         :param pulumi.Input[str] name: The Application's display name.
-        :param pulumi.Input[bool] pkce_required: Require Proof Key for Code Exchange (PKCE) for additional verification key rotation mode. See:
-               https://developer.okta.com/docs/reference/api/idps/#oauth-2-0-and-openid-connect-client-object
         :param pulumi.Input[bool] profile_master: Determines if the IdP should act as a source of truth for user profile attributes.
         :param pulumi.Input[str] protocol_type: The type of protocol to use. It can be `"OIDC"` or `"OAUTH2"`.
         :param pulumi.Input[str] provisioning_action: Provisioning action for an IdP user during authentication.
         :param pulumi.Input[str] request_signature_algorithm: The HMAC Signature Algorithm used when signing an authorization request. Defaults to `"HS256"`. It can be `"HS256"`, `"HS384"`, `"HS512"`, `"SHA-256"`. `"RS256"`, `"RS384"`, or `"RS512"`. NOTE: `"SHA-256"` an undocumented legacy value and not continue to be valid. See API docs https://developer.okta.com/docs/reference/api/idps/#oidc-request-signature-algorithm-object
         :param pulumi.Input[str] request_signature_scope: Specifies whether to digitally sign an AuthnRequest messages to the IdP. Defaults to `"REQUEST"`. It can be `"REQUEST"` or `"NONE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scopes of the IdP.
         :param pulumi.Input[str] status: Status of the IdP.
@@ -1475,15 +1431,14 @@
         __props__.__dict__["groups_filters"] = groups_filters
         __props__.__dict__["issuer_mode"] = issuer_mode
         __props__.__dict__["issuer_url"] = issuer_url
         __props__.__dict__["jwks_binding"] = jwks_binding
         __props__.__dict__["jwks_url"] = jwks_url
         __props__.__dict__["max_clock_skew"] = max_clock_skew
         __props__.__dict__["name"] = name
-        __props__.__dict__["pkce_required"] = pkce_required
         __props__.__dict__["profile_master"] = profile_master
         __props__.__dict__["protocol_type"] = protocol_type
         __props__.__dict__["provisioning_action"] = provisioning_action
         __props__.__dict__["request_signature_algorithm"] = request_signature_algorithm
         __props__.__dict__["request_signature_scope"] = request_signature_scope
         __props__.__dict__["scopes"] = scopes
         __props__.__dict__["status"] = status
@@ -1632,23 +1587,14 @@
     def name(self) -> pulumi.Output[str]:
         """
         The Application's display name.
         """
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="pkceRequired")
-    def pkce_required(self) -> pulumi.Output[Optional[bool]]:
-        """
-        Require Proof Key for Code Exchange (PKCE) for additional verification key rotation mode. See:
-        https://developer.okta.com/docs/reference/api/idps/#oauth-2-0-and-openid-connect-client-object
-        """
-        return pulumi.get(self, "pkce_required")
-
-    @property
     @pulumi.getter(name="profileMaster")
     def profile_master(self) -> pulumi.Output[Optional[bool]]:
         """
         Determines if the IdP should act as a source of truth for user profile attributes.
         """
         return pulumi.get(self, "profile_master")
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/saml.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/saml_key.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/saml_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/idp/social.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/index/__init__.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/index/_inputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/index/customized_signin_page.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/customized_signin_page.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/index/email_domain.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/email_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/index/email_domain_verification.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/email_domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/index/get_default_signin_page.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_default_signin_page.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/index/get_domain.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/index/get_log_stream.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_log_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/index/get_org_metadata.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_org_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/index/log_stream.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/log_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/index/outputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/index/preview_signin_page.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/preview_signin_page.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/inline/_inputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/inline/hook.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         The set of arguments for constructing a Hook resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] channel: Details of the endpoint the inline hook will hit.
         :param pulumi.Input[str] type: The type of hook to trigger. Currently, the only supported type is `"HTTP"`.
         :param pulumi.Input[str] version: Version of the channel. The currently-supported version is `"1.0.0"`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] auth: Authentication required for inline hook request.
         :param pulumi.Input[Sequence[pulumi.Input['HookHeaderArgs']]] headers: Map of headers to send along in inline hook request.
         :param pulumi.Input[str] name: The inline hook display name.
+        :param pulumi.Input[str] status: Default to `ACTIVE`
         """
         pulumi.set(__self__, "channel", channel)
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "version", version)
         if auth is not None:
             pulumi.set(__self__, "auth", auth)
         if headers is not None:
@@ -115,14 +116,17 @@
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
+        """
+        Default to `ACTIVE`
+        """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
 
@@ -138,14 +142,15 @@
                  version: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Hook resources.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] auth: Authentication required for inline hook request.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] channel: Details of the endpoint the inline hook will hit.
         :param pulumi.Input[Sequence[pulumi.Input['HookHeaderArgs']]] headers: Map of headers to send along in inline hook request.
         :param pulumi.Input[str] name: The inline hook display name.
+        :param pulumi.Input[str] status: Default to `ACTIVE`
         :param pulumi.Input[str] type: The type of hook to trigger. Currently, the only supported type is `"HTTP"`.
         :param pulumi.Input[str] version: Version of the channel. The currently-supported version is `"1.0.0"`.
         """
         if auth is not None:
             pulumi.set(__self__, "auth", auth)
         if channel is not None:
             pulumi.set(__self__, "channel", channel)
@@ -207,14 +212,17 @@
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
+        """
+        Default to `ACTIVE`
+        """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
     @property
@@ -293,14 +301,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] auth: Authentication required for inline hook request.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] channel: Details of the endpoint the inline hook will hit.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['HookHeaderArgs']]]] headers: Map of headers to send along in inline hook request.
         :param pulumi.Input[str] name: The inline hook display name.
+        :param pulumi.Input[str] status: Default to `ACTIVE`
         :param pulumi.Input[str] type: The type of hook to trigger. Currently, the only supported type is `"HTTP"`.
         :param pulumi.Input[str] version: Version of the channel. The currently-supported version is `"1.0.0"`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -410,14 +419,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] auth: Authentication required for inline hook request.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] channel: Details of the endpoint the inline hook will hit.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['HookHeaderArgs']]]] headers: Map of headers to send along in inline hook request.
         :param pulumi.Input[str] name: The inline hook display name.
+        :param pulumi.Input[str] status: Default to `ACTIVE`
         :param pulumi.Input[str] type: The type of hook to trigger. Currently, the only supported type is `"HTTP"`.
         :param pulumi.Input[str] version: Version of the channel. The currently-supported version is `"1.0.0"`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _HookState.__new__(_HookState)
 
@@ -461,14 +471,17 @@
         The inline hook display name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Output[Optional[str]]:
+        """
+        Default to `ACTIVE`
+        """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
         The type of hook to trigger. Currently, the only supported type is `"HTTP"`.
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/inline/outputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/link_definition.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/link_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/link_value.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/link_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/network/zone.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/network/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/org_configuration.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/org_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         :param pulumi.Input[str] company_name: Name of org
         :param pulumi.Input[str] address1: Primary address of org
         :param pulumi.Input[str] address2: Secondary address of org
         :param pulumi.Input[str] billing_contact_user: User ID representing the billing contact
         :param pulumi.Input[str] city: City of org
         :param pulumi.Input[str] country: Country of org
         :param pulumi.Input[str] end_user_support_help_url: Support link of org
-        :param pulumi.Input[str] logo: Local path to logo of the org.
+        :param pulumi.Input[str] logo: Logo of org. The file must be in PNG, JPG, or GIF format and less than 1 MB in size. For best results use landscape
+               orientation, a transparent background, and a minimum size of 420px by 120px to prevent upscaling.
         :param pulumi.Input[bool] opt_out_communication_emails: Indicates whether the org's users receive Okta Communication emails
         :param pulumi.Input[str] phone_number: Support help phone of org
         :param pulumi.Input[str] postal_code: Postal code of org
         :param pulumi.Input[str] state: State of org
         :param pulumi.Input[str] support_phone_number: Support help phone of org
         :param pulumi.Input[str] technical_contact_user: User ID representing the technical contact
         :param pulumi.Input[str] website: The org's website
@@ -161,15 +162,16 @@
     def end_user_support_help_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "end_user_support_help_url", value)
 
     @property
     @pulumi.getter
     def logo(self) -> Optional[pulumi.Input[str]]:
         """
-        Local path to logo of the org.
+        Logo of org. The file must be in PNG, JPG, or GIF format and less than 1 MB in size. For best results use landscape
+        orientation, a transparent background, and a minimum size of 420px by 120px to prevent upscaling.
         """
         return pulumi.get(self, "logo")
 
     @logo.setter
     def logo(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "logo", value)
 
@@ -284,15 +286,16 @@
         :param pulumi.Input[str] address2: Secondary address of org
         :param pulumi.Input[str] billing_contact_user: User ID representing the billing contact
         :param pulumi.Input[str] city: City of org
         :param pulumi.Input[str] company_name: Name of org
         :param pulumi.Input[str] country: Country of org
         :param pulumi.Input[str] end_user_support_help_url: Support link of org
         :param pulumi.Input[str] expires_at: Expiration of org
-        :param pulumi.Input[str] logo: Local path to logo of the org.
+        :param pulumi.Input[str] logo: Logo of org. The file must be in PNG, JPG, or GIF format and less than 1 MB in size. For best results use landscape
+               orientation, a transparent background, and a minimum size of 420px by 120px to prevent upscaling.
         :param pulumi.Input[bool] opt_out_communication_emails: Indicates whether the org's users receive Okta Communication emails
         :param pulumi.Input[str] phone_number: Support help phone of org
         :param pulumi.Input[str] postal_code: Postal code of org
         :param pulumi.Input[str] state: State of org
         :param pulumi.Input[str] subdomain: Subdomain of org
         :param pulumi.Input[str] support_phone_number: Support help phone of org
         :param pulumi.Input[str] technical_contact_user: User ID representing the technical contact
@@ -429,15 +432,16 @@
     def expires_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "expires_at", value)
 
     @property
     @pulumi.getter
     def logo(self) -> Optional[pulumi.Input[str]]:
         """
-        Local path to logo of the org.
+        Logo of org. The file must be in PNG, JPG, or GIF format and less than 1 MB in size. For best results use landscape
+        orientation, a transparent background, and a minimum size of 420px by 120px to prevent upscaling.
         """
         return pulumi.get(self, "logo")
 
     @logo.setter
     def logo(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "logo", value)
 
@@ -590,15 +594,16 @@
         :param pulumi.Input[str] address1: Primary address of org
         :param pulumi.Input[str] address2: Secondary address of org
         :param pulumi.Input[str] billing_contact_user: User ID representing the billing contact
         :param pulumi.Input[str] city: City of org
         :param pulumi.Input[str] company_name: Name of org
         :param pulumi.Input[str] country: Country of org
         :param pulumi.Input[str] end_user_support_help_url: Support link of org
-        :param pulumi.Input[str] logo: Local path to logo of the org.
+        :param pulumi.Input[str] logo: Logo of org. The file must be in PNG, JPG, or GIF format and less than 1 MB in size. For best results use landscape
+               orientation, a transparent background, and a minimum size of 420px by 120px to prevent upscaling.
         :param pulumi.Input[bool] opt_out_communication_emails: Indicates whether the org's users receive Okta Communication emails
         :param pulumi.Input[str] phone_number: Support help phone of org
         :param pulumi.Input[str] postal_code: Postal code of org
         :param pulumi.Input[str] state: State of org
         :param pulumi.Input[str] support_phone_number: Support help phone of org
         :param pulumi.Input[str] technical_contact_user: User ID representing the technical contact
         :param pulumi.Input[str] website: The org's website
@@ -731,15 +736,16 @@
         :param pulumi.Input[str] address2: Secondary address of org
         :param pulumi.Input[str] billing_contact_user: User ID representing the billing contact
         :param pulumi.Input[str] city: City of org
         :param pulumi.Input[str] company_name: Name of org
         :param pulumi.Input[str] country: Country of org
         :param pulumi.Input[str] end_user_support_help_url: Support link of org
         :param pulumi.Input[str] expires_at: Expiration of org
-        :param pulumi.Input[str] logo: Local path to logo of the org.
+        :param pulumi.Input[str] logo: Logo of org. The file must be in PNG, JPG, or GIF format and less than 1 MB in size. For best results use landscape
+               orientation, a transparent background, and a minimum size of 420px by 120px to prevent upscaling.
         :param pulumi.Input[bool] opt_out_communication_emails: Indicates whether the org's users receive Okta Communication emails
         :param pulumi.Input[str] phone_number: Support help phone of org
         :param pulumi.Input[str] postal_code: Postal code of org
         :param pulumi.Input[str] state: State of org
         :param pulumi.Input[str] subdomain: Subdomain of org
         :param pulumi.Input[str] support_phone_number: Support help phone of org
         :param pulumi.Input[str] technical_contact_user: User ID representing the technical contact
@@ -832,15 +838,16 @@
         """
         return pulumi.get(self, "expires_at")
 
     @property
     @pulumi.getter
     def logo(self) -> pulumi.Output[Optional[str]]:
         """
-        Local path to logo of the org.
+        Logo of org. The file must be in PNG, JPG, or GIF format and less than 1 MB in size. For best results use landscape
+        orientation, a transparent background, and a minimum size of 420px by 120px to prevent upscaling.
         """
         return pulumi.get(self, "logo")
 
     @property
     @pulumi.getter(name="optOutCommunicationEmails")
     def opt_out_communication_emails(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/org_support.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/org_support.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/outputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/__init__.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/_inputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/device_assurance_android.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_android.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,20 @@
                  jailbreak: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  os_version: Optional[pulumi.Input[str]] = None,
                  screenlock_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  secure_hardware_present: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a DeviceAssuranceAndroid resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be FULL, USER
-        :param pulumi.Input[bool] jailbreak: The device jailbreak. Only for android and iOS platform
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `FULL`, `USER`
+        :param pulumi.Input[bool] jailbreak: Is the device jailbroken in the device assurance policy.
         :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
-        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device constains a secure hardware functionality
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
+        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device contains a secure hardware functionality
         """
         if disk_encryption_types is not None:
             pulumi.set(__self__, "disk_encryption_types", disk_encryption_types)
         if jailbreak is not None:
             pulumi.set(__self__, "jailbreak", jailbreak)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -42,27 +42,27 @@
         if secure_hardware_present is not None:
             pulumi.set(__self__, "secure_hardware_present", secure_hardware_present)
 
     @property
     @pulumi.getter(name="diskEncryptionTypes")
     def disk_encryption_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of disk encryption type, can be FULL, USER
+        List of disk encryption type, can be `FULL`, `USER`
         """
         return pulumi.get(self, "disk_encryption_types")
 
     @disk_encryption_types.setter
     def disk_encryption_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "disk_encryption_types", value)
 
     @property
     @pulumi.getter
     def jailbreak(self) -> Optional[pulumi.Input[bool]]:
         """
-        The device jailbreak. Only for android and iOS platform
+        Is the device jailbroken in the device assurance policy.
         """
         return pulumi.get(self, "jailbreak")
 
     @jailbreak.setter
     def jailbreak(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "jailbreak", value)
 
@@ -78,39 +78,39 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="osVersion")
     def os_version(self) -> Optional[pulumi.Input[str]]:
         """
-        The device os minimum version
+        Minimum os version of the device in the device assurance policy.
         """
         return pulumi.get(self, "os_version")
 
     @os_version.setter
     def os_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "os_version", value)
 
     @property
     @pulumi.getter(name="screenlockTypes")
     def screenlock_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         return pulumi.get(self, "screenlock_types")
 
     @screenlock_types.setter
     def screenlock_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "screenlock_types", value)
 
     @property
     @pulumi.getter(name="secureHardwarePresent")
     def secure_hardware_present(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates if the device constains a secure hardware functionality
+        Indicates if the device contains a secure hardware functionality
         """
         return pulumi.get(self, "secure_hardware_present")
 
     @secure_hardware_present.setter
     def secure_hardware_present(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "secure_hardware_present", value)
 
@@ -129,23 +129,23 @@
                  platform: Optional[pulumi.Input[str]] = None,
                  screenlock_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  secure_hardware_present: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering DeviceAssuranceAndroid resources.
         :param pulumi.Input[str] created_by: Created by
         :param pulumi.Input[str] created_date: Created date
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be FULL, USER
-        :param pulumi.Input[bool] jailbreak: The device jailbreak. Only for android and iOS platform
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `FULL`, `USER`
+        :param pulumi.Input[bool] jailbreak: Is the device jailbroken in the device assurance policy.
         :param pulumi.Input[str] last_update: Last update
         :param pulumi.Input[str] last_updated_by: Last updated by
         :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
         :param pulumi.Input[str] platform: Policy device assurance platform
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
-        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device constains a secure hardware functionality
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
+        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device contains a secure hardware functionality
         """
         if created_by is not None:
             pulumi.set(__self__, "created_by", created_by)
         if created_date is not None:
             pulumi.set(__self__, "created_date", created_date)
         if disk_encryption_types is not None:
             pulumi.set(__self__, "disk_encryption_types", disk_encryption_types)
@@ -190,27 +190,27 @@
     def created_date(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_date", value)
 
     @property
     @pulumi.getter(name="diskEncryptionTypes")
     def disk_encryption_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of disk encryption type, can be FULL, USER
+        List of disk encryption type, can be `FULL`, `USER`
         """
         return pulumi.get(self, "disk_encryption_types")
 
     @disk_encryption_types.setter
     def disk_encryption_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "disk_encryption_types", value)
 
     @property
     @pulumi.getter
     def jailbreak(self) -> Optional[pulumi.Input[bool]]:
         """
-        The device jailbreak. Only for android and iOS platform
+        Is the device jailbroken in the device assurance policy.
         """
         return pulumi.get(self, "jailbreak")
 
     @jailbreak.setter
     def jailbreak(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "jailbreak", value)
 
@@ -250,15 +250,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="osVersion")
     def os_version(self) -> Optional[pulumi.Input[str]]:
         """
-        The device os minimum version
+        Minimum os version of the device in the device assurance policy.
         """
         return pulumi.get(self, "os_version")
 
     @os_version.setter
     def os_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "os_version", value)
 
@@ -274,27 +274,27 @@
     def platform(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "platform", value)
 
     @property
     @pulumi.getter(name="screenlockTypes")
     def screenlock_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         return pulumi.get(self, "screenlock_types")
 
     @screenlock_types.setter
     def screenlock_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "screenlock_types", value)
 
     @property
     @pulumi.getter(name="secureHardwarePresent")
     def secure_hardware_present(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates if the device constains a secure hardware functionality
+        Indicates if the device contains a secure hardware functionality
         """
         return pulumi.get(self, "secure_hardware_present")
 
     @secure_hardware_present.setter
     def secure_hardware_present(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "secure_hardware_present", value)
 
@@ -311,20 +311,20 @@
                  screenlock_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  secure_hardware_present: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Create a DeviceAssuranceAndroid resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be FULL, USER
-        :param pulumi.Input[bool] jailbreak: The device jailbreak. Only for android and iOS platform
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `FULL`, `USER`
+        :param pulumi.Input[bool] jailbreak: Is the device jailbroken in the device assurance policy.
         :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
-        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device constains a secure hardware functionality
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
+        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device contains a secure hardware functionality
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[DeviceAssuranceAndroidArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -397,23 +397,23 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_by: Created by
         :param pulumi.Input[str] created_date: Created date
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be FULL, USER
-        :param pulumi.Input[bool] jailbreak: The device jailbreak. Only for android and iOS platform
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `FULL`, `USER`
+        :param pulumi.Input[bool] jailbreak: Is the device jailbroken in the device assurance policy.
         :param pulumi.Input[str] last_update: Last update
         :param pulumi.Input[str] last_updated_by: Last updated by
         :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
         :param pulumi.Input[str] platform: Policy device assurance platform
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
-        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device constains a secure hardware functionality
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
+        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device contains a secure hardware functionality
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DeviceAssuranceAndroidState.__new__(_DeviceAssuranceAndroidState)
 
         __props__.__dict__["created_by"] = created_by
         __props__.__dict__["created_date"] = created_date
@@ -444,23 +444,23 @@
         """
         return pulumi.get(self, "created_date")
 
     @property
     @pulumi.getter(name="diskEncryptionTypes")
     def disk_encryption_types(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of disk encryption type, can be FULL, USER
+        List of disk encryption type, can be `FULL`, `USER`
         """
         return pulumi.get(self, "disk_encryption_types")
 
     @property
     @pulumi.getter
     def jailbreak(self) -> pulumi.Output[Optional[bool]]:
         """
-        The device jailbreak. Only for android and iOS platform
+        Is the device jailbroken in the device assurance policy.
         """
         return pulumi.get(self, "jailbreak")
 
     @property
     @pulumi.getter(name="lastUpdate")
     def last_update(self) -> pulumi.Output[str]:
         """
@@ -484,15 +484,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="osVersion")
     def os_version(self) -> pulumi.Output[Optional[str]]:
         """
-        The device os minimum version
+        Minimum os version of the device in the device assurance policy.
         """
         return pulumi.get(self, "os_version")
 
     @property
     @pulumi.getter
     def platform(self) -> pulumi.Output[str]:
         """
@@ -500,19 +500,19 @@
         """
         return pulumi.get(self, "platform")
 
     @property
     @pulumi.getter(name="screenlockTypes")
     def screenlock_types(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         return pulumi.get(self, "screenlock_types")
 
     @property
     @pulumi.getter(name="secureHardwarePresent")
     def secure_hardware_present(self) -> pulumi.Output[Optional[bool]]:
         """
-        Indicates if the device constains a secure hardware functionality
+        Indicates if the device contains a secure hardware functionality
         """
         return pulumi.get(self, "secure_hardware_present")
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/device_assurance_chromeos.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_chromeos.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                  tpsp_password_proctection_warning_trigger: Optional[pulumi.Input[str]] = None,
                  tpsp_realtime_url_check_mode: Optional[pulumi.Input[bool]] = None,
                  tpsp_safe_browsing_protection_level: Optional[pulumi.Input[str]] = None,
                  tpsp_screen_lock_secured: Optional[pulumi.Input[bool]] = None,
                  tpsp_site_isolation_enabled: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a DeviceAssuranceChromeos resource.
-        :param pulumi.Input[str] name: Policy device assurance name
+        :param pulumi.Input[str] name: Name of the device assurance policy.
         :param pulumi.Input[bool] tpsp_allow_screen_lock: Third party signal provider allow screen lock
         :param pulumi.Input[str] tpsp_browser_version: Third party signal provider minimum browser version
         :param pulumi.Input[bool] tpsp_builtin_dns_client_enabled: Third party signal provider builtin dns client enabled
         :param pulumi.Input[bool] tpsp_chrome_remote_desktop_app_blocked: Third party signal provider chrome remote desktop app blocked
         :param pulumi.Input[str] tpsp_device_enrollment_domain: Third party signal provider device enrollment domain
         :param pulumi.Input[bool] tpsp_disk_encrypted: Third party signal provider disk encrypted
         :param pulumi.Input[str] tpsp_key_trust_level: Third party signal provider key trust level
@@ -78,15 +78,15 @@
         if tpsp_site_isolation_enabled is not None:
             pulumi.set(__self__, "tpsp_site_isolation_enabled", tpsp_site_isolation_enabled)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy device assurance name
+        Name of the device assurance policy.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -284,15 +284,15 @@
                  tpsp_site_isolation_enabled: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering DeviceAssuranceChromeos resources.
         :param pulumi.Input[str] created_by: Created by
         :param pulumi.Input[str] created_date: Created date
         :param pulumi.Input[str] last_update: Last update
         :param pulumi.Input[str] last_updated_by: Last updated by
-        :param pulumi.Input[str] name: Policy device assurance name
+        :param pulumi.Input[str] name: Name of the device assurance policy.
         :param pulumi.Input[str] platform: Policy device assurance platform
         :param pulumi.Input[bool] tpsp_allow_screen_lock: Third party signal provider allow screen lock
         :param pulumi.Input[str] tpsp_browser_version: Third party signal provider minimum browser version
         :param pulumi.Input[bool] tpsp_builtin_dns_client_enabled: Third party signal provider builtin dns client enabled
         :param pulumi.Input[bool] tpsp_chrome_remote_desktop_app_blocked: Third party signal provider chrome remote desktop app blocked
         :param pulumi.Input[str] tpsp_device_enrollment_domain: Third party signal provider device enrollment domain
         :param pulumi.Input[bool] tpsp_disk_encrypted: Third party signal provider disk encrypted
@@ -394,15 +394,15 @@
     def last_updated_by(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "last_updated_by", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy device assurance name
+        Name of the device assurance policy.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -608,15 +608,15 @@
                  tpsp_screen_lock_secured: Optional[pulumi.Input[bool]] = None,
                  tpsp_site_isolation_enabled: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Create a DeviceAssuranceChromeos resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: Policy device assurance name
+        :param pulumi.Input[str] name: Name of the device assurance policy.
         :param pulumi.Input[bool] tpsp_allow_screen_lock: Third party signal provider allow screen lock
         :param pulumi.Input[str] tpsp_browser_version: Third party signal provider minimum browser version
         :param pulumi.Input[bool] tpsp_builtin_dns_client_enabled: Third party signal provider builtin dns client enabled
         :param pulumi.Input[bool] tpsp_chrome_remote_desktop_app_blocked: Third party signal provider chrome remote desktop app blocked
         :param pulumi.Input[str] tpsp_device_enrollment_domain: Third party signal provider device enrollment domain
         :param pulumi.Input[bool] tpsp_disk_encrypted: Third party signal provider disk encrypted
         :param pulumi.Input[str] tpsp_key_trust_level: Third party signal provider key trust level
@@ -732,15 +732,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_by: Created by
         :param pulumi.Input[str] created_date: Created date
         :param pulumi.Input[str] last_update: Last update
         :param pulumi.Input[str] last_updated_by: Last updated by
-        :param pulumi.Input[str] name: Policy device assurance name
+        :param pulumi.Input[str] name: Name of the device assurance policy.
         :param pulumi.Input[str] platform: Policy device assurance platform
         :param pulumi.Input[bool] tpsp_allow_screen_lock: Third party signal provider allow screen lock
         :param pulumi.Input[str] tpsp_browser_version: Third party signal provider minimum browser version
         :param pulumi.Input[bool] tpsp_builtin_dns_client_enabled: Third party signal provider builtin dns client enabled
         :param pulumi.Input[bool] tpsp_chrome_remote_desktop_app_blocked: Third party signal provider chrome remote desktop app blocked
         :param pulumi.Input[str] tpsp_device_enrollment_domain: Third party signal provider device enrollment domain
         :param pulumi.Input[bool] tpsp_disk_encrypted: Third party signal provider disk encrypted
@@ -811,15 +811,15 @@
         """
         return pulumi.get(self, "last_updated_by")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Policy device assurance name
+        Name of the device assurance policy.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def platform(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/device_assurance_ios.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_ios.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,69 +16,69 @@
     def __init__(__self__, *,
                  jailbreak: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  os_version: Optional[pulumi.Input[str]] = None,
                  screenlock_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a DeviceAssuranceIos resource.
-        :param pulumi.Input[bool] jailbreak: The device jailbreak. Only for android and iOS platform
-        :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        :param pulumi.Input[bool] jailbreak: Is the device jailbroken in the device assurance policy.
+        :param pulumi.Input[str] name: Name of the device assurance policy.
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         if jailbreak is not None:
             pulumi.set(__self__, "jailbreak", jailbreak)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if os_version is not None:
             pulumi.set(__self__, "os_version", os_version)
         if screenlock_types is not None:
             pulumi.set(__self__, "screenlock_types", screenlock_types)
 
     @property
     @pulumi.getter
     def jailbreak(self) -> Optional[pulumi.Input[bool]]:
         """
-        The device jailbreak. Only for android and iOS platform
+        Is the device jailbroken in the device assurance policy.
         """
         return pulumi.get(self, "jailbreak")
 
     @jailbreak.setter
     def jailbreak(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "jailbreak", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy device assurance name
+        Name of the device assurance policy.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="osVersion")
     def os_version(self) -> Optional[pulumi.Input[str]]:
         """
-        The device os minimum version
+        Minimum os version of the device in the device assurance policy.
         """
         return pulumi.get(self, "os_version")
 
     @os_version.setter
     def os_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "os_version", value)
 
     @property
     @pulumi.getter(name="screenlockTypes")
     def screenlock_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         return pulumi.get(self, "screenlock_types")
 
     @screenlock_types.setter
     def screenlock_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "screenlock_types", value)
 
@@ -93,23 +93,23 @@
                  last_updated_by: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  os_version: Optional[pulumi.Input[str]] = None,
                  platform: Optional[pulumi.Input[str]] = None,
                  screenlock_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering DeviceAssuranceIos resources.
-        :param pulumi.Input[str] created_by: Created by
-        :param pulumi.Input[str] created_date: Created date
-        :param pulumi.Input[bool] jailbreak: The device jailbreak. Only for android and iOS platform
-        :param pulumi.Input[str] last_update: Last update
-        :param pulumi.Input[str] last_updated_by: Last updated by
-        :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
+        :param pulumi.Input[str] created_by: Created by of the device assurance polic
+        :param pulumi.Input[str] created_date: Created date of the device assurance polic
+        :param pulumi.Input[bool] jailbreak: Is the device jailbroken in the device assurance policy.
+        :param pulumi.Input[str] last_update: Last update of the device assurance polic
+        :param pulumi.Input[str] last_updated_by: Last updated by of the device assurance polic
+        :param pulumi.Input[str] name: Name of the device assurance policy.
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
         :param pulumi.Input[str] platform: Policy device assurance platform
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         if created_by is not None:
             pulumi.set(__self__, "created_by", created_by)
         if created_date is not None:
             pulumi.set(__self__, "created_date", created_date)
         if jailbreak is not None:
             pulumi.set(__self__, "jailbreak", jailbreak)
@@ -126,87 +126,87 @@
         if screenlock_types is not None:
             pulumi.set(__self__, "screenlock_types", screenlock_types)
 
     @property
     @pulumi.getter(name="createdBy")
     def created_by(self) -> Optional[pulumi.Input[str]]:
         """
-        Created by
+        Created by of the device assurance polic
         """
         return pulumi.get(self, "created_by")
 
     @created_by.setter
     def created_by(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_by", value)
 
     @property
     @pulumi.getter(name="createdDate")
     def created_date(self) -> Optional[pulumi.Input[str]]:
         """
-        Created date
+        Created date of the device assurance polic
         """
         return pulumi.get(self, "created_date")
 
     @created_date.setter
     def created_date(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_date", value)
 
     @property
     @pulumi.getter
     def jailbreak(self) -> Optional[pulumi.Input[bool]]:
         """
-        The device jailbreak. Only for android and iOS platform
+        Is the device jailbroken in the device assurance policy.
         """
         return pulumi.get(self, "jailbreak")
 
     @jailbreak.setter
     def jailbreak(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "jailbreak", value)
 
     @property
     @pulumi.getter(name="lastUpdate")
     def last_update(self) -> Optional[pulumi.Input[str]]:
         """
-        Last update
+        Last update of the device assurance polic
         """
         return pulumi.get(self, "last_update")
 
     @last_update.setter
     def last_update(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "last_update", value)
 
     @property
     @pulumi.getter(name="lastUpdatedBy")
     def last_updated_by(self) -> Optional[pulumi.Input[str]]:
         """
-        Last updated by
+        Last updated by of the device assurance polic
         """
         return pulumi.get(self, "last_updated_by")
 
     @last_updated_by.setter
     def last_updated_by(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "last_updated_by", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy device assurance name
+        Name of the device assurance policy.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="osVersion")
     def os_version(self) -> Optional[pulumi.Input[str]]:
         """
-        The device os minimum version
+        Minimum os version of the device in the device assurance policy.
         """
         return pulumi.get(self, "os_version")
 
     @os_version.setter
     def os_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "os_version", value)
 
@@ -222,15 +222,15 @@
     def platform(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "platform", value)
 
     @property
     @pulumi.getter(name="screenlockTypes")
     def screenlock_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         return pulumi.get(self, "screenlock_types")
 
     @screenlock_types.setter
     def screenlock_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "screenlock_types", value)
 
@@ -245,18 +245,18 @@
                  os_version: Optional[pulumi.Input[str]] = None,
                  screenlock_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Create a DeviceAssuranceIos resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] jailbreak: The device jailbreak. Only for android and iOS platform
-        :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        :param pulumi.Input[bool] jailbreak: Is the device jailbroken in the device assurance policy.
+        :param pulumi.Input[str] name: Name of the device assurance policy.
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[DeviceAssuranceIosArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -321,23 +321,23 @@
         """
         Get an existing DeviceAssuranceIos resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] created_by: Created by
-        :param pulumi.Input[str] created_date: Created date
-        :param pulumi.Input[bool] jailbreak: The device jailbreak. Only for android and iOS platform
-        :param pulumi.Input[str] last_update: Last update
-        :param pulumi.Input[str] last_updated_by: Last updated by
-        :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
+        :param pulumi.Input[str] created_by: Created by of the device assurance polic
+        :param pulumi.Input[str] created_date: Created date of the device assurance polic
+        :param pulumi.Input[bool] jailbreak: Is the device jailbroken in the device assurance policy.
+        :param pulumi.Input[str] last_update: Last update of the device assurance polic
+        :param pulumi.Input[str] last_updated_by: Last updated by of the device assurance polic
+        :param pulumi.Input[str] name: Name of the device assurance policy.
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
         :param pulumi.Input[str] platform: Policy device assurance platform
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DeviceAssuranceIosState.__new__(_DeviceAssuranceIosState)
 
         __props__.__dict__["created_by"] = created_by
         __props__.__dict__["created_date"] = created_date
@@ -350,63 +350,63 @@
         __props__.__dict__["screenlock_types"] = screenlock_types
         return DeviceAssuranceIos(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="createdBy")
     def created_by(self) -> pulumi.Output[str]:
         """
-        Created by
+        Created by of the device assurance polic
         """
         return pulumi.get(self, "created_by")
 
     @property
     @pulumi.getter(name="createdDate")
     def created_date(self) -> pulumi.Output[str]:
         """
-        Created date
+        Created date of the device assurance polic
         """
         return pulumi.get(self, "created_date")
 
     @property
     @pulumi.getter
     def jailbreak(self) -> pulumi.Output[Optional[bool]]:
         """
-        The device jailbreak. Only for android and iOS platform
+        Is the device jailbroken in the device assurance policy.
         """
         return pulumi.get(self, "jailbreak")
 
     @property
     @pulumi.getter(name="lastUpdate")
     def last_update(self) -> pulumi.Output[str]:
         """
-        Last update
+        Last update of the device assurance polic
         """
         return pulumi.get(self, "last_update")
 
     @property
     @pulumi.getter(name="lastUpdatedBy")
     def last_updated_by(self) -> pulumi.Output[str]:
         """
-        Last updated by
+        Last updated by of the device assurance polic
         """
         return pulumi.get(self, "last_updated_by")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Policy device assurance name
+        Name of the device assurance policy.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="osVersion")
     def os_version(self) -> pulumi.Output[Optional[str]]:
         """
-        The device os minimum version
+        Minimum os version of the device in the device assurance policy.
         """
         return pulumi.get(self, "os_version")
 
     @property
     @pulumi.getter
     def platform(self) -> pulumi.Output[str]:
         """
@@ -414,11 +414,11 @@
         """
         return pulumi.get(self, "platform")
 
     @property
     @pulumi.getter(name="screenlockTypes")
     def screenlock_types(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         return pulumi.get(self, "screenlock_types")
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/device_assurance_macos.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_macos.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
                  tpsp_password_proctection_warning_trigger: Optional[pulumi.Input[str]] = None,
                  tpsp_realtime_url_check_mode: Optional[pulumi.Input[bool]] = None,
                  tpsp_safe_browsing_protection_level: Optional[pulumi.Input[str]] = None,
                  tpsp_screen_lock_secured: Optional[pulumi.Input[bool]] = None,
                  tpsp_site_isolation_enabled: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a DeviceAssuranceMacos resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be ALL_INTERNAL_VOLUMES
-        :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
-        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device constains a secure hardware functionality
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
+        :param pulumi.Input[str] name: Name of the device assurance policy.
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
+        :param pulumi.Input[bool] secure_hardware_present: Is the device secure with hardware in the device assurance policy.
         :param pulumi.Input[bool] third_party_signal_providers: Check to include third party signal provider
         :param pulumi.Input[str] tpsp_browser_version: Third party signal provider minimum browser version
         :param pulumi.Input[bool] tpsp_builtin_dns_client_enabled: Third party signal provider builtin dns client enable
         :param pulumi.Input[bool] tpsp_chrome_remote_desktop_app_blocked: Third party signal provider chrome remote desktop app blocked
         :param pulumi.Input[str] tpsp_device_enrollment_domain: Third party signal provider device enrollment domain
         :param pulumi.Input[bool] tpsp_disk_encrypted: Third party signal provider disk encrypted
         :param pulumi.Input[str] tpsp_key_trust_level: Third party signal provider key trust level
@@ -94,63 +94,63 @@
         if tpsp_site_isolation_enabled is not None:
             pulumi.set(__self__, "tpsp_site_isolation_enabled", tpsp_site_isolation_enabled)
 
     @property
     @pulumi.getter(name="diskEncryptionTypes")
     def disk_encryption_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of disk encryption type, can be ALL_INTERNAL_VOLUMES
+        List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
         """
         return pulumi.get(self, "disk_encryption_types")
 
     @disk_encryption_types.setter
     def disk_encryption_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "disk_encryption_types", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy device assurance name
+        Name of the device assurance policy.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="osVersion")
     def os_version(self) -> Optional[pulumi.Input[str]]:
         """
-        The device os minimum version
+        Minimum os version of the device in the device assurance policy.
         """
         return pulumi.get(self, "os_version")
 
     @os_version.setter
     def os_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "os_version", value)
 
     @property
     @pulumi.getter(name="screenlockTypes")
     def screenlock_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         return pulumi.get(self, "screenlock_types")
 
     @screenlock_types.setter
     def screenlock_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "screenlock_types", value)
 
     @property
     @pulumi.getter(name="secureHardwarePresent")
     def secure_hardware_present(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates if the device constains a secure hardware functionality
+        Is the device secure with hardware in the device assurance policy.
         """
         return pulumi.get(self, "secure_hardware_present")
 
     @secure_hardware_present.setter
     def secure_hardware_present(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "secure_hardware_present", value)
 
@@ -350,22 +350,22 @@
                  tpsp_safe_browsing_protection_level: Optional[pulumi.Input[str]] = None,
                  tpsp_screen_lock_secured: Optional[pulumi.Input[bool]] = None,
                  tpsp_site_isolation_enabled: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering DeviceAssuranceMacos resources.
         :param pulumi.Input[str] created_by: Created by
         :param pulumi.Input[str] created_date: Created date
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be ALL_INTERNAL_VOLUMES
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
         :param pulumi.Input[str] last_update: Last update
         :param pulumi.Input[str] last_updated_by: Last updated by
-        :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
+        :param pulumi.Input[str] name: Name of the device assurance policy.
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
         :param pulumi.Input[str] platform: Policy device assurance platform
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
-        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device constains a secure hardware functionality
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
+        :param pulumi.Input[bool] secure_hardware_present: Is the device secure with hardware in the device assurance policy.
         :param pulumi.Input[bool] third_party_signal_providers: Check to include third party signal provider
         :param pulumi.Input[str] tpsp_browser_version: Third party signal provider minimum browser version
         :param pulumi.Input[bool] tpsp_builtin_dns_client_enabled: Third party signal provider builtin dns client enable
         :param pulumi.Input[bool] tpsp_chrome_remote_desktop_app_blocked: Third party signal provider chrome remote desktop app blocked
         :param pulumi.Input[str] tpsp_device_enrollment_domain: Third party signal provider device enrollment domain
         :param pulumi.Input[bool] tpsp_disk_encrypted: Third party signal provider disk encrypted
         :param pulumi.Input[str] tpsp_key_trust_level: Third party signal provider key trust level
@@ -450,15 +450,15 @@
     def created_date(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_date", value)
 
     @property
     @pulumi.getter(name="diskEncryptionTypes")
     def disk_encryption_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of disk encryption type, can be ALL_INTERNAL_VOLUMES
+        List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
         """
         return pulumi.get(self, "disk_encryption_types")
 
     @disk_encryption_types.setter
     def disk_encryption_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "disk_encryption_types", value)
 
@@ -486,27 +486,27 @@
     def last_updated_by(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "last_updated_by", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy device assurance name
+        Name of the device assurance policy.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="osVersion")
     def os_version(self) -> Optional[pulumi.Input[str]]:
         """
-        The device os minimum version
+        Minimum os version of the device in the device assurance policy.
         """
         return pulumi.get(self, "os_version")
 
     @os_version.setter
     def os_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "os_version", value)
 
@@ -522,27 +522,27 @@
     def platform(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "platform", value)
 
     @property
     @pulumi.getter(name="screenlockTypes")
     def screenlock_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         return pulumi.get(self, "screenlock_types")
 
     @screenlock_types.setter
     def screenlock_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "screenlock_types", value)
 
     @property
     @pulumi.getter(name="secureHardwarePresent")
     def secure_hardware_present(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates if the device constains a secure hardware functionality
+        Is the device secure with hardware in the device assurance policy.
         """
         return pulumi.get(self, "secure_hardware_present")
 
     @secure_hardware_present.setter
     def secure_hardware_present(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "secure_hardware_present", value)
 
@@ -740,19 +740,19 @@
                  tpsp_screen_lock_secured: Optional[pulumi.Input[bool]] = None,
                  tpsp_site_isolation_enabled: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Create a DeviceAssuranceMacos resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be ALL_INTERNAL_VOLUMES
-        :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
-        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device constains a secure hardware functionality
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
+        :param pulumi.Input[str] name: Name of the device assurance policy.
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
+        :param pulumi.Input[bool] secure_hardware_present: Is the device secure with hardware in the device assurance policy.
         :param pulumi.Input[bool] third_party_signal_providers: Check to include third party signal provider
         :param pulumi.Input[str] tpsp_browser_version: Third party signal provider minimum browser version
         :param pulumi.Input[bool] tpsp_builtin_dns_client_enabled: Third party signal provider builtin dns client enable
         :param pulumi.Input[bool] tpsp_chrome_remote_desktop_app_blocked: Third party signal provider chrome remote desktop app blocked
         :param pulumi.Input[str] tpsp_device_enrollment_domain: Third party signal provider device enrollment domain
         :param pulumi.Input[bool] tpsp_disk_encrypted: Third party signal provider disk encrypted
         :param pulumi.Input[str] tpsp_key_trust_level: Third party signal provider key trust level
@@ -878,22 +878,22 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_by: Created by
         :param pulumi.Input[str] created_date: Created date
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be ALL_INTERNAL_VOLUMES
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
         :param pulumi.Input[str] last_update: Last update
         :param pulumi.Input[str] last_updated_by: Last updated by
-        :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
+        :param pulumi.Input[str] name: Name of the device assurance policy.
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
         :param pulumi.Input[str] platform: Policy device assurance platform
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
-        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device constains a secure hardware functionality
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
+        :param pulumi.Input[bool] secure_hardware_present: Is the device secure with hardware in the device assurance policy.
         :param pulumi.Input[bool] third_party_signal_providers: Check to include third party signal provider
         :param pulumi.Input[str] tpsp_browser_version: Third party signal provider minimum browser version
         :param pulumi.Input[bool] tpsp_builtin_dns_client_enabled: Third party signal provider builtin dns client enable
         :param pulumi.Input[bool] tpsp_chrome_remote_desktop_app_blocked: Third party signal provider chrome remote desktop app blocked
         :param pulumi.Input[str] tpsp_device_enrollment_domain: Third party signal provider device enrollment domain
         :param pulumi.Input[bool] tpsp_disk_encrypted: Third party signal provider disk encrypted
         :param pulumi.Input[str] tpsp_key_trust_level: Third party signal provider key trust level
@@ -951,15 +951,15 @@
         """
         return pulumi.get(self, "created_date")
 
     @property
     @pulumi.getter(name="diskEncryptionTypes")
     def disk_encryption_types(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of disk encryption type, can be ALL_INTERNAL_VOLUMES
+        List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
         """
         return pulumi.get(self, "disk_encryption_types")
 
     @property
     @pulumi.getter(name="lastUpdate")
     def last_update(self) -> pulumi.Output[str]:
         """
@@ -975,23 +975,23 @@
         """
         return pulumi.get(self, "last_updated_by")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Policy device assurance name
+        Name of the device assurance policy.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="osVersion")
     def os_version(self) -> pulumi.Output[Optional[str]]:
         """
-        The device os minimum version
+        Minimum os version of the device in the device assurance policy.
         """
         return pulumi.get(self, "os_version")
 
     @property
     @pulumi.getter
     def platform(self) -> pulumi.Output[str]:
         """
@@ -999,23 +999,23 @@
         """
         return pulumi.get(self, "platform")
 
     @property
     @pulumi.getter(name="screenlockTypes")
     def screenlock_types(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         return pulumi.get(self, "screenlock_types")
 
     @property
     @pulumi.getter(name="secureHardwarePresent")
     def secure_hardware_present(self) -> pulumi.Output[Optional[bool]]:
         """
-        Indicates if the device constains a secure hardware functionality
+        Is the device secure with hardware in the device assurance policy.
         """
         return pulumi.get(self, "secure_hardware_present")
 
     @property
     @pulumi.getter(name="thirdPartySignalProviders")
     def third_party_signal_providers(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/device_assurance_windows.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,19 @@
                  tpsp_secure_boot_enabled: Optional[pulumi.Input[bool]] = None,
                  tpsp_site_isolation_enabled: Optional[pulumi.Input[bool]] = None,
                  tpsp_third_party_blocking_enabled: Optional[pulumi.Input[bool]] = None,
                  tpsp_windows_machine_domain: Optional[pulumi.Input[str]] = None,
                  tpsp_windows_user_domain: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a DeviceAssuranceWindows resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be ALL_INTERNAL_VOLUMES
-        :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
-        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device constains a secure hardware functionality
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
+        :param pulumi.Input[str] name: Name of the device assurance policy.
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
+        :param pulumi.Input[bool] secure_hardware_present: Is the device secure with hardware in the device assurance policy.
         :param pulumi.Input[bool] third_party_signal_providers: Check to include third party signal provider
         :param pulumi.Input[str] tpsp_browser_version: Third party signal provider minimum browser version
         :param pulumi.Input[bool] tpsp_builtin_dns_client_enabled: Third party signal provider builtin dns client enable
         :param pulumi.Input[bool] tpsp_chrome_remote_desktop_app_blocked: Third party signal provider chrome remote desktop app blocked
         :param pulumi.Input[str] tpsp_crowd_strike_agent_id: Third party signal provider crowdstrike agent id
         :param pulumi.Input[str] tpsp_crowd_strike_customer_id: Third party signal provider crowdstrike user id
         :param pulumi.Input[str] tpsp_device_enrollment_domain: Third party signal provider device enrollment domain
@@ -118,63 +118,63 @@
         if tpsp_windows_user_domain is not None:
             pulumi.set(__self__, "tpsp_windows_user_domain", tpsp_windows_user_domain)
 
     @property
     @pulumi.getter(name="diskEncryptionTypes")
     def disk_encryption_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of disk encryption type, can be ALL_INTERNAL_VOLUMES
+        List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
         """
         return pulumi.get(self, "disk_encryption_types")
 
     @disk_encryption_types.setter
     def disk_encryption_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "disk_encryption_types", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy device assurance name
+        Name of the device assurance policy.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="osVersion")
     def os_version(self) -> Optional[pulumi.Input[str]]:
         """
-        The device os minimum version
+        Minimum os version of the device in the device assurance policy.
         """
         return pulumi.get(self, "os_version")
 
     @os_version.setter
     def os_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "os_version", value)
 
     @property
     @pulumi.getter(name="screenlockTypes")
     def screenlock_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         return pulumi.get(self, "screenlock_types")
 
     @screenlock_types.setter
     def screenlock_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "screenlock_types", value)
 
     @property
     @pulumi.getter(name="secureHardwarePresent")
     def secure_hardware_present(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates if the device constains a secure hardware functionality
+        Is the device secure with hardware in the device assurance policy.
         """
         return pulumi.get(self, "secure_hardware_present")
 
     @secure_hardware_present.setter
     def secure_hardware_present(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "secure_hardware_present", value)
 
@@ -452,22 +452,22 @@
                  tpsp_third_party_blocking_enabled: Optional[pulumi.Input[bool]] = None,
                  tpsp_windows_machine_domain: Optional[pulumi.Input[str]] = None,
                  tpsp_windows_user_domain: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering DeviceAssuranceWindows resources.
         :param pulumi.Input[str] created_by: Created by
         :param pulumi.Input[str] created_date: Created date
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be ALL_INTERNAL_VOLUMES
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
         :param pulumi.Input[str] last_update: Last update
         :param pulumi.Input[str] last_updated_by: Last updated by
-        :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
+        :param pulumi.Input[str] name: Name of the device assurance policy.
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
         :param pulumi.Input[str] platform: Policy device assurance platform
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
-        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device constains a secure hardware functionality
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
+        :param pulumi.Input[bool] secure_hardware_present: Is the device secure with hardware in the device assurance policy.
         :param pulumi.Input[bool] third_party_signal_providers: Check to include third party signal provider
         :param pulumi.Input[str] tpsp_browser_version: Third party signal provider minimum browser version
         :param pulumi.Input[bool] tpsp_builtin_dns_client_enabled: Third party signal provider builtin dns client enable
         :param pulumi.Input[bool] tpsp_chrome_remote_desktop_app_blocked: Third party signal provider chrome remote desktop app blocked
         :param pulumi.Input[str] tpsp_crowd_strike_agent_id: Third party signal provider crowdstrike agent id
         :param pulumi.Input[str] tpsp_crowd_strike_customer_id: Third party signal provider crowdstrike user id
         :param pulumi.Input[str] tpsp_device_enrollment_domain: Third party signal provider device enrollment domain
@@ -570,15 +570,15 @@
     def created_date(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_date", value)
 
     @property
     @pulumi.getter(name="diskEncryptionTypes")
     def disk_encryption_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of disk encryption type, can be ALL_INTERNAL_VOLUMES
+        List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
         """
         return pulumi.get(self, "disk_encryption_types")
 
     @disk_encryption_types.setter
     def disk_encryption_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "disk_encryption_types", value)
 
@@ -606,27 +606,27 @@
     def last_updated_by(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "last_updated_by", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy device assurance name
+        Name of the device assurance policy.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="osVersion")
     def os_version(self) -> Optional[pulumi.Input[str]]:
         """
-        The device os minimum version
+        Minimum os version of the device in the device assurance policy.
         """
         return pulumi.get(self, "os_version")
 
     @os_version.setter
     def os_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "os_version", value)
 
@@ -642,27 +642,27 @@
     def platform(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "platform", value)
 
     @property
     @pulumi.getter(name="screenlockTypes")
     def screenlock_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         return pulumi.get(self, "screenlock_types")
 
     @screenlock_types.setter
     def screenlock_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "screenlock_types", value)
 
     @property
     @pulumi.getter(name="secureHardwarePresent")
     def secure_hardware_present(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates if the device constains a secure hardware functionality
+        Is the device secure with hardware in the device assurance policy.
         """
         return pulumi.get(self, "secure_hardware_present")
 
     @secure_hardware_present.setter
     def secure_hardware_present(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "secure_hardware_present", value)
 
@@ -938,19 +938,19 @@
                  tpsp_windows_machine_domain: Optional[pulumi.Input[str]] = None,
                  tpsp_windows_user_domain: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a DeviceAssuranceWindows resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be ALL_INTERNAL_VOLUMES
-        :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
-        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device constains a secure hardware functionality
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
+        :param pulumi.Input[str] name: Name of the device assurance policy.
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
+        :param pulumi.Input[bool] secure_hardware_present: Is the device secure with hardware in the device assurance policy.
         :param pulumi.Input[bool] third_party_signal_providers: Check to include third party signal provider
         :param pulumi.Input[str] tpsp_browser_version: Third party signal provider minimum browser version
         :param pulumi.Input[bool] tpsp_builtin_dns_client_enabled: Third party signal provider builtin dns client enable
         :param pulumi.Input[bool] tpsp_chrome_remote_desktop_app_blocked: Third party signal provider chrome remote desktop app blocked
         :param pulumi.Input[str] tpsp_crowd_strike_agent_id: Third party signal provider crowdstrike agent id
         :param pulumi.Input[str] tpsp_crowd_strike_customer_id: Third party signal provider crowdstrike user id
         :param pulumi.Input[str] tpsp_device_enrollment_domain: Third party signal provider device enrollment domain
@@ -1100,22 +1100,22 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_by: Created by
         :param pulumi.Input[str] created_date: Created date
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be ALL_INTERNAL_VOLUMES
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
         :param pulumi.Input[str] last_update: Last update
         :param pulumi.Input[str] last_updated_by: Last updated by
-        :param pulumi.Input[str] name: Policy device assurance name
-        :param pulumi.Input[str] os_version: The device os minimum version
+        :param pulumi.Input[str] name: Name of the device assurance policy.
+        :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
         :param pulumi.Input[str] platform: Policy device assurance platform
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
-        :param pulumi.Input[bool] secure_hardware_present: Indicates if the device constains a secure hardware functionality
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
+        :param pulumi.Input[bool] secure_hardware_present: Is the device secure with hardware in the device assurance policy.
         :param pulumi.Input[bool] third_party_signal_providers: Check to include third party signal provider
         :param pulumi.Input[str] tpsp_browser_version: Third party signal provider minimum browser version
         :param pulumi.Input[bool] tpsp_builtin_dns_client_enabled: Third party signal provider builtin dns client enable
         :param pulumi.Input[bool] tpsp_chrome_remote_desktop_app_blocked: Third party signal provider chrome remote desktop app blocked
         :param pulumi.Input[str] tpsp_crowd_strike_agent_id: Third party signal provider crowdstrike agent id
         :param pulumi.Input[str] tpsp_crowd_strike_customer_id: Third party signal provider crowdstrike user id
         :param pulumi.Input[str] tpsp_device_enrollment_domain: Third party signal provider device enrollment domain
@@ -1185,15 +1185,15 @@
         """
         return pulumi.get(self, "created_date")
 
     @property
     @pulumi.getter(name="diskEncryptionTypes")
     def disk_encryption_types(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of disk encryption type, can be ALL_INTERNAL_VOLUMES
+        List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
         """
         return pulumi.get(self, "disk_encryption_types")
 
     @property
     @pulumi.getter(name="lastUpdate")
     def last_update(self) -> pulumi.Output[str]:
         """
@@ -1209,23 +1209,23 @@
         """
         return pulumi.get(self, "last_updated_by")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Policy device assurance name
+        Name of the device assurance policy.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="osVersion")
     def os_version(self) -> pulumi.Output[Optional[str]]:
         """
-        The device os minimum version
+        Minimum os version of the device in the device assurance policy.
         """
         return pulumi.get(self, "os_version")
 
     @property
     @pulumi.getter
     def platform(self) -> pulumi.Output[str]:
         """
@@ -1233,23 +1233,23 @@
         """
         return pulumi.get(self, "platform")
 
     @property
     @pulumi.getter(name="screenlockTypes")
     def screenlock_types(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of screenlock type, can be BIOMETRIC or BIOMETRIC, PASSCODE
+        List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         return pulumi.get(self, "screenlock_types")
 
     @property
     @pulumi.getter(name="secureHardwarePresent")
     def secure_hardware_present(self) -> pulumi.Output[Optional[bool]]:
         """
-        Indicates if the device constains a secure hardware functionality
+        Is the device secure with hardware in the device assurance policy.
         """
         return pulumi.get(self, "secure_hardware_present")
 
     @property
     @pulumi.getter(name="thirdPartySignalProviders")
     def third_party_signal_providers(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/get_default_policy.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/get_default_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/get_policy.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/get_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/mfa.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/outputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/password.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/rule_idp_discovery.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_idp_discovery.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,17 @@
         :param pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryAppIncludeArgs']]] app_includes: Applications to include in discovery rule.
         :param pulumi.Input[str] idp_id: The identifier for the Idp the rule should route to if all conditions are met.
         :param pulumi.Input[str] idp_type: Type of Idp. One of: `"SAML2"`, `"IWA"`, `"AgentlessDSSO"`, `"X509"`, `"FACEBOOK"`, `"GOOGLE"`, `"LINKEDIN"`, `"MICROSOFT"`, `"OIDC"`
         :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         :param pulumi.Input[str] network_connection: The network selection mode. One of `"ANYWEHRE"` or `"ZONE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to exclude.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to include.
+        :param pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryPlatformIncludeArgs']]] platform_includes: Platform to include in discovery rule. - 'type' - (Optional) One of: 'ANY', 'MOBILE', 'DESKTOP' - 'os_expression -
+               (Optional) Only available when using os_type = 'OTHER' - 'os_type' - (Optional) One of: 'ANY', 'IOS', 'WINDOWS',
+               'ANDROID', 'OTHER', 'OSX'
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[int] priority: Idp rule priority. This attribute can be set to a valid priority. To avoid an endless diff situation an error is thrown if an invalid property is provided. The Okta API defaults to the last (lowest) if not provided.
         :param pulumi.Input[str] status: Idp rule status: `"ACTIVE"` or `"INACTIVE"`. By default, it is `"ACTIVE"`.
         :param pulumi.Input[str] user_identifier_attribute: Profile attribute matching can only have a single value that describes the type indicated in `user_identifier_type`. This is the attribute or identifier that the `user_identifier_patterns` are checked against.
         :param pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryUserIdentifierPatternArgs']]] user_identifier_patterns: Specifies a User Identifier pattern condition to match against. If `match_type` of `"EXPRESSION"` is used, only a *single* element can be set, otherwise multiple elements of matching patterns may be provided.
         :param pulumi.Input[str] user_identifier_type: One of: `"IDENTIFIER"`, `"ATTRIBUTE"`
         """
@@ -186,14 +189,19 @@
     @network_includes.setter
     def network_includes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "network_includes", value)
 
     @property
     @pulumi.getter(name="platformIncludes")
     def platform_includes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryPlatformIncludeArgs']]]]:
+        """
+        Platform to include in discovery rule. - 'type' - (Optional) One of: 'ANY', 'MOBILE', 'DESKTOP' - 'os_expression -
+        (Optional) Only available when using os_type = 'OTHER' - 'os_type' - (Optional) One of: 'ANY', 'IOS', 'WINDOWS',
+        'ANDROID', 'OTHER', 'OSX'
+        """
         return pulumi.get(self, "platform_includes")
 
     @platform_includes.setter
     def platform_includes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryPlatformIncludeArgs']]]]):
         pulumi.set(self, "platform_includes", value)
 
     @property
@@ -299,14 +307,17 @@
         :param pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryAppIncludeArgs']]] app_includes: Applications to include in discovery rule.
         :param pulumi.Input[str] idp_id: The identifier for the Idp the rule should route to if all conditions are met.
         :param pulumi.Input[str] idp_type: Type of Idp. One of: `"SAML2"`, `"IWA"`, `"AgentlessDSSO"`, `"X509"`, `"FACEBOOK"`, `"GOOGLE"`, `"LINKEDIN"`, `"MICROSOFT"`, `"OIDC"`
         :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         :param pulumi.Input[str] network_connection: The network selection mode. One of `"ANYWEHRE"` or `"ZONE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to exclude.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to include.
+        :param pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryPlatformIncludeArgs']]] platform_includes: Platform to include in discovery rule. - 'type' - (Optional) One of: 'ANY', 'MOBILE', 'DESKTOP' - 'os_expression -
+               (Optional) Only available when using os_type = 'OTHER' - 'os_type' - (Optional) One of: 'ANY', 'IOS', 'WINDOWS',
+               'ANDROID', 'OTHER', 'OSX'
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[int] priority: Idp rule priority. This attribute can be set to a valid priority. To avoid an endless diff situation an error is thrown if an invalid property is provided. The Okta API defaults to the last (lowest) if not provided.
         :param pulumi.Input[str] status: Idp rule status: `"ACTIVE"` or `"INACTIVE"`. By default, it is `"ACTIVE"`.
         :param pulumi.Input[str] user_identifier_attribute: Profile attribute matching can only have a single value that describes the type indicated in `user_identifier_type`. This is the attribute or identifier that the `user_identifier_patterns` are checked against.
         :param pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryUserIdentifierPatternArgs']]] user_identifier_patterns: Specifies a User Identifier pattern condition to match against. If `match_type` of `"EXPRESSION"` is used, only a *single* element can be set, otherwise multiple elements of matching patterns may be provided.
         :param pulumi.Input[str] user_identifier_type: One of: `"IDENTIFIER"`, `"ATTRIBUTE"`
         """
@@ -442,14 +453,19 @@
     @network_includes.setter
     def network_includes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "network_includes", value)
 
     @property
     @pulumi.getter(name="platformIncludes")
     def platform_includes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryPlatformIncludeArgs']]]]:
+        """
+        Platform to include in discovery rule. - 'type' - (Optional) One of: 'ANY', 'MOBILE', 'DESKTOP' - 'os_expression -
+        (Optional) Only available when using os_type = 'OTHER' - 'os_type' - (Optional) One of: 'ANY', 'IOS', 'WINDOWS',
+        'ANDROID', 'OTHER', 'OSX'
+        """
         return pulumi.get(self, "platform_includes")
 
     @platform_includes.setter
     def platform_includes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryPlatformIncludeArgs']]]]):
         pulumi.set(self, "platform_includes", value)
 
     @property
@@ -622,14 +638,17 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleIdpDiscoveryAppIncludeArgs']]]] app_includes: Applications to include in discovery rule.
         :param pulumi.Input[str] idp_id: The identifier for the Idp the rule should route to if all conditions are met.
         :param pulumi.Input[str] idp_type: Type of Idp. One of: `"SAML2"`, `"IWA"`, `"AgentlessDSSO"`, `"X509"`, `"FACEBOOK"`, `"GOOGLE"`, `"LINKEDIN"`, `"MICROSOFT"`, `"OIDC"`
         :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         :param pulumi.Input[str] network_connection: The network selection mode. One of `"ANYWEHRE"` or `"ZONE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to exclude.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to include.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleIdpDiscoveryPlatformIncludeArgs']]]] platform_includes: Platform to include in discovery rule. - 'type' - (Optional) One of: 'ANY', 'MOBILE', 'DESKTOP' - 'os_expression -
+               (Optional) Only available when using os_type = 'OTHER' - 'os_type' - (Optional) One of: 'ANY', 'IOS', 'WINDOWS',
+               'ANDROID', 'OTHER', 'OSX'
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[int] priority: Idp rule priority. This attribute can be set to a valid priority. To avoid an endless diff situation an error is thrown if an invalid property is provided. The Okta API defaults to the last (lowest) if not provided.
         :param pulumi.Input[str] status: Idp rule status: `"ACTIVE"` or `"INACTIVE"`. By default, it is `"ACTIVE"`.
         :param pulumi.Input[str] user_identifier_attribute: Profile attribute matching can only have a single value that describes the type indicated in `user_identifier_type`. This is the attribute or identifier that the `user_identifier_patterns` are checked against.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleIdpDiscoveryUserIdentifierPatternArgs']]]] user_identifier_patterns: Specifies a User Identifier pattern condition to match against. If `match_type` of `"EXPRESSION"` is used, only a *single* element can be set, otherwise multiple elements of matching patterns may be provided.
         :param pulumi.Input[str] user_identifier_type: One of: `"IDENTIFIER"`, `"ATTRIBUTE"`
         """
@@ -799,14 +818,17 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleIdpDiscoveryAppIncludeArgs']]]] app_includes: Applications to include in discovery rule.
         :param pulumi.Input[str] idp_id: The identifier for the Idp the rule should route to if all conditions are met.
         :param pulumi.Input[str] idp_type: Type of Idp. One of: `"SAML2"`, `"IWA"`, `"AgentlessDSSO"`, `"X509"`, `"FACEBOOK"`, `"GOOGLE"`, `"LINKEDIN"`, `"MICROSOFT"`, `"OIDC"`
         :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         :param pulumi.Input[str] network_connection: The network selection mode. One of `"ANYWEHRE"` or `"ZONE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to exclude.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to include.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleIdpDiscoveryPlatformIncludeArgs']]]] platform_includes: Platform to include in discovery rule. - 'type' - (Optional) One of: 'ANY', 'MOBILE', 'DESKTOP' - 'os_expression -
+               (Optional) Only available when using os_type = 'OTHER' - 'os_type' - (Optional) One of: 'ANY', 'IOS', 'WINDOWS',
+               'ANDROID', 'OTHER', 'OSX'
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[int] priority: Idp rule priority. This attribute can be set to a valid priority. To avoid an endless diff situation an error is thrown if an invalid property is provided. The Okta API defaults to the last (lowest) if not provided.
         :param pulumi.Input[str] status: Idp rule status: `"ACTIVE"` or `"INACTIVE"`. By default, it is `"ACTIVE"`.
         :param pulumi.Input[str] user_identifier_attribute: Profile attribute matching can only have a single value that describes the type indicated in `user_identifier_type`. This is the attribute or identifier that the `user_identifier_patterns` are checked against.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleIdpDiscoveryUserIdentifierPatternArgs']]]] user_identifier_patterns: Specifies a User Identifier pattern condition to match against. If `match_type` of `"EXPRESSION"` is used, only a *single* element can be set, otherwise multiple elements of matching patterns may be provided.
         :param pulumi.Input[str] user_identifier_type: One of: `"IDENTIFIER"`, `"ATTRIBUTE"`
         """
@@ -900,14 +922,19 @@
         Required if `network_connection` = `"ZONE"`. Indicates the network zones to include.
         """
         return pulumi.get(self, "network_includes")
 
     @property
     @pulumi.getter(name="platformIncludes")
     def platform_includes(self) -> pulumi.Output[Optional[Sequence['outputs.RuleIdpDiscoveryPlatformInclude']]]:
+        """
+        Platform to include in discovery rule. - 'type' - (Optional) One of: 'ANY', 'MOBILE', 'DESKTOP' - 'os_expression -
+        (Optional) Only available when using os_type = 'OTHER' - 'os_type' - (Optional) One of: 'ANY', 'IOS', 'WINDOWS',
+        'ANDROID', 'OTHER', 'OSX'
+        """
         return pulumi.get(self, "platform_includes")
 
     @property
     @pulumi.getter(name="policyId")
     def policy_id(self) -> pulumi.Output[Optional[str]]:
         """
         Policy ID.
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/rule_mfa.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_mfa.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,18 @@
                  network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[int]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a RuleMfa resource.
-        :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]] app_excludes: Applications to exclude
+        :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+               - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+               is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+               of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
         :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
         :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
         :param pulumi.Input[str] policy_id: Policy ID.
@@ -64,15 +67,18 @@
         if users_excludeds is not None:
             pulumi.set(__self__, "users_excludeds", users_excludeds)
 
     @property
     @pulumi.getter(name="appExcludes")
     def app_excludes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]]:
         """
-        Applications to exclude
+        Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+        - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+        is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+        of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         """
         return pulumi.get(self, "app_excludes")
 
     @app_excludes.setter
     def app_excludes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]]):
         pulumi.set(self, "app_excludes", value)
 
@@ -209,15 +215,18 @@
                  network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[int]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering RuleMfa resources.
-        :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]] app_excludes: Applications to exclude
+        :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+               - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+               is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+               of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
         :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
         :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
         :param pulumi.Input[str] policy_id: Policy ID.
@@ -248,15 +257,18 @@
         if users_excludeds is not None:
             pulumi.set(__self__, "users_excludeds", users_excludeds)
 
     @property
     @pulumi.getter(name="appExcludes")
     def app_excludes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]]:
         """
-        Applications to exclude
+        Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+        - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+        is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+        of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         """
         return pulumi.get(self, "app_excludes")
 
     @app_excludes.setter
     def app_excludes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]]]):
         pulumi.set(self, "app_excludes", value)
 
@@ -407,15 +419,18 @@
 
         ```sh
         $ pulumi import okta:policy/ruleMfa:RuleMfa example &#60;policy id&#62;/&#60;rule id&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]] app_excludes: Applications to exclude
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+               - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+               is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+               of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
         :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
         :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
         :param pulumi.Input[str] policy_id: Policy ID.
@@ -510,15 +525,18 @@
         """
         Get an existing RuleMfa resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]] app_excludes: Applications to exclude
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+               - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+               is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+               of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
         :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
         :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
         :param pulumi.Input[str] policy_id: Policy ID.
@@ -543,15 +561,18 @@
         __props__.__dict__["users_excludeds"] = users_excludeds
         return RuleMfa(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="appExcludes")
     def app_excludes(self) -> pulumi.Output[Optional[Sequence['outputs.RuleMfaAppExclude']]]:
         """
-        Applications to exclude
+        Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
+        - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
+        is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
+        of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         """
         return pulumi.get(self, "app_excludes")
 
     @property
     @pulumi.getter(name="appIncludes")
     def app_includes(self) -> pulumi.Output[Optional[Sequence['outputs.RuleMfaAppInclude']]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/rule_password.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/rule_signon.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_signon.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
                  network_connection: Optional[pulumi.Input[str]] = None,
                  network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  primary_factor: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[int]] = None,
                  risc_level: Optional[pulumi.Input[str]] = None,
+                 risk_level: Optional[pulumi.Input[str]] = None,
                  session_idle: Optional[pulumi.Input[int]] = None,
                  session_lifetime: Optional[pulumi.Input[int]] = None,
                  session_persistent: Optional[pulumi.Input[bool]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a RuleSignon resource.
@@ -59,14 +60,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[str] primary_factor: Rule's primary factor. **WARNING** Ony works as a part of the Identity Engine. Valid values: 
                `"PASSWORD_IDP_ANY_FACTOR"`, `"PASSWORD_IDP"`.
         :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
         :param pulumi.Input[str] risc_level: Risc level: `"ANY"`, `"LOW"`, `"MEDIUM"` or `"HIGH"`. Default is `"ANY"`. It can be also 
                set to an empty string in case `RISC_SCORING` org feature flag is disabled.
+        :param pulumi.Input[str] risk_level: Risk level: ANY, LOW, MEDIUM or HIGH. Default: `ANY`
         :param pulumi.Input[int] session_idle: Max minutes a session can be idle.,
         :param pulumi.Input[int] session_lifetime: Max minutes a session is active: Disable = 0.
         :param pulumi.Input[bool] session_persistent: Whether session cookies will last across browser sessions. Okta Administrators can never have persistent session cookies.
         :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: The list of user IDs that would be excluded when rules are processed.
         """
         if access is not None:
@@ -100,15 +102,20 @@
         if policy_id is not None:
             pulumi.set(__self__, "policy_id", policy_id)
         if primary_factor is not None:
             pulumi.set(__self__, "primary_factor", primary_factor)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
         if risc_level is not None:
+            warnings.warn("""Attribute typo, switch to risk_level instead. Default: `ANY`""", DeprecationWarning)
+            pulumi.log.warn("""risc_level is deprecated: Attribute typo, switch to risk_level instead. Default: `ANY`""")
+        if risc_level is not None:
             pulumi.set(__self__, "risc_level", risc_level)
+        if risk_level is not None:
+            pulumi.set(__self__, "risk_level", risk_level)
         if session_idle is not None:
             pulumi.set(__self__, "session_idle", session_idle)
         if session_lifetime is not None:
             pulumi.set(__self__, "session_lifetime", session_lifetime)
         if session_persistent is not None:
             pulumi.set(__self__, "session_persistent", session_persistent)
         if status is not None:
@@ -326,21 +333,36 @@
     @property
     @pulumi.getter(name="riscLevel")
     def risc_level(self) -> Optional[pulumi.Input[str]]:
         """
         Risc level: `"ANY"`, `"LOW"`, `"MEDIUM"` or `"HIGH"`. Default is `"ANY"`. It can be also 
         set to an empty string in case `RISC_SCORING` org feature flag is disabled.
         """
+        warnings.warn("""Attribute typo, switch to risk_level instead. Default: `ANY`""", DeprecationWarning)
+        pulumi.log.warn("""risc_level is deprecated: Attribute typo, switch to risk_level instead. Default: `ANY`""")
+
         return pulumi.get(self, "risc_level")
 
     @risc_level.setter
     def risc_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "risc_level", value)
 
     @property
+    @pulumi.getter(name="riskLevel")
+    def risk_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        Risk level: ANY, LOW, MEDIUM or HIGH. Default: `ANY`
+        """
+        return pulumi.get(self, "risk_level")
+
+    @risk_level.setter
+    def risk_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "risk_level", value)
+
+    @property
     @pulumi.getter(name="sessionIdle")
     def session_idle(self) -> Optional[pulumi.Input[int]]:
         """
         Max minutes a session can be idle.,
         """
         return pulumi.get(self, "session_idle")
 
@@ -414,14 +436,15 @@
                  network_connection: Optional[pulumi.Input[str]] = None,
                  network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  primary_factor: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[int]] = None,
                  risc_level: Optional[pulumi.Input[str]] = None,
+                 risk_level: Optional[pulumi.Input[str]] = None,
                  session_idle: Optional[pulumi.Input[int]] = None,
                  session_lifetime: Optional[pulumi.Input[int]] = None,
                  session_persistent: Optional[pulumi.Input[bool]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering RuleSignon resources.
@@ -443,14 +466,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[str] primary_factor: Rule's primary factor. **WARNING** Ony works as a part of the Identity Engine. Valid values: 
                `"PASSWORD_IDP_ANY_FACTOR"`, `"PASSWORD_IDP"`.
         :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
         :param pulumi.Input[str] risc_level: Risc level: `"ANY"`, `"LOW"`, `"MEDIUM"` or `"HIGH"`. Default is `"ANY"`. It can be also 
                set to an empty string in case `RISC_SCORING` org feature flag is disabled.
+        :param pulumi.Input[str] risk_level: Risk level: ANY, LOW, MEDIUM or HIGH. Default: `ANY`
         :param pulumi.Input[int] session_idle: Max minutes a session can be idle.,
         :param pulumi.Input[int] session_lifetime: Max minutes a session is active: Disable = 0.
         :param pulumi.Input[bool] session_persistent: Whether session cookies will last across browser sessions. Okta Administrators can never have persistent session cookies.
         :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: The list of user IDs that would be excluded when rules are processed.
         """
         if access is not None:
@@ -484,15 +508,20 @@
         if policy_id is not None:
             pulumi.set(__self__, "policy_id", policy_id)
         if primary_factor is not None:
             pulumi.set(__self__, "primary_factor", primary_factor)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
         if risc_level is not None:
+            warnings.warn("""Attribute typo, switch to risk_level instead. Default: `ANY`""", DeprecationWarning)
+            pulumi.log.warn("""risc_level is deprecated: Attribute typo, switch to risk_level instead. Default: `ANY`""")
+        if risc_level is not None:
             pulumi.set(__self__, "risc_level", risc_level)
+        if risk_level is not None:
+            pulumi.set(__self__, "risk_level", risk_level)
         if session_idle is not None:
             pulumi.set(__self__, "session_idle", session_idle)
         if session_lifetime is not None:
             pulumi.set(__self__, "session_lifetime", session_lifetime)
         if session_persistent is not None:
             pulumi.set(__self__, "session_persistent", session_persistent)
         if status is not None:
@@ -710,21 +739,36 @@
     @property
     @pulumi.getter(name="riscLevel")
     def risc_level(self) -> Optional[pulumi.Input[str]]:
         """
         Risc level: `"ANY"`, `"LOW"`, `"MEDIUM"` or `"HIGH"`. Default is `"ANY"`. It can be also 
         set to an empty string in case `RISC_SCORING` org feature flag is disabled.
         """
+        warnings.warn("""Attribute typo, switch to risk_level instead. Default: `ANY`""", DeprecationWarning)
+        pulumi.log.warn("""risc_level is deprecated: Attribute typo, switch to risk_level instead. Default: `ANY`""")
+
         return pulumi.get(self, "risc_level")
 
     @risc_level.setter
     def risc_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "risc_level", value)
 
     @property
+    @pulumi.getter(name="riskLevel")
+    def risk_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        Risk level: ANY, LOW, MEDIUM or HIGH. Default: `ANY`
+        """
+        return pulumi.get(self, "risk_level")
+
+    @risk_level.setter
+    def risk_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "risk_level", value)
+
+    @property
     @pulumi.getter(name="sessionIdle")
     def session_idle(self) -> Optional[pulumi.Input[int]]:
         """
         Max minutes a session can be idle.,
         """
         return pulumi.get(self, "session_idle")
 
@@ -800,14 +844,15 @@
                  network_connection: Optional[pulumi.Input[str]] = None,
                  network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  primary_factor: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[int]] = None,
                  risc_level: Optional[pulumi.Input[str]] = None,
+                 risk_level: Optional[pulumi.Input[str]] = None,
                  session_idle: Optional[pulumi.Input[int]] = None,
                  session_lifetime: Optional[pulumi.Input[int]] = None,
                  session_persistent: Optional[pulumi.Input[bool]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
@@ -920,14 +965,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[str] primary_factor: Rule's primary factor. **WARNING** Ony works as a part of the Identity Engine. Valid values: 
                `"PASSWORD_IDP_ANY_FACTOR"`, `"PASSWORD_IDP"`.
         :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
         :param pulumi.Input[str] risc_level: Risc level: `"ANY"`, `"LOW"`, `"MEDIUM"` or `"HIGH"`. Default is `"ANY"`. It can be also 
                set to an empty string in case `RISC_SCORING` org feature flag is disabled.
+        :param pulumi.Input[str] risk_level: Risk level: ANY, LOW, MEDIUM or HIGH. Default: `ANY`
         :param pulumi.Input[int] session_idle: Max minutes a session can be idle.,
         :param pulumi.Input[int] session_lifetime: Max minutes a session is active: Disable = 0.
         :param pulumi.Input[bool] session_persistent: Whether session cookies will last across browser sessions. Okta Administrators can never have persistent session cookies.
         :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: The list of user IDs that would be excluded when rules are processed.
         """
         ...
@@ -1055,14 +1101,15 @@
                  network_connection: Optional[pulumi.Input[str]] = None,
                  network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  primary_factor: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[int]] = None,
                  risc_level: Optional[pulumi.Input[str]] = None,
+                 risk_level: Optional[pulumi.Input[str]] = None,
                  session_idle: Optional[pulumi.Input[int]] = None,
                  session_lifetime: Optional[pulumi.Input[int]] = None,
                  session_persistent: Optional[pulumi.Input[bool]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
@@ -1087,14 +1134,15 @@
             __props__.__dict__["network_connection"] = network_connection
             __props__.__dict__["network_excludes"] = network_excludes
             __props__.__dict__["network_includes"] = network_includes
             __props__.__dict__["policy_id"] = policy_id
             __props__.__dict__["primary_factor"] = primary_factor
             __props__.__dict__["priority"] = priority
             __props__.__dict__["risc_level"] = risc_level
+            __props__.__dict__["risk_level"] = risk_level
             __props__.__dict__["session_idle"] = session_idle
             __props__.__dict__["session_lifetime"] = session_lifetime
             __props__.__dict__["session_persistent"] = session_persistent
             __props__.__dict__["status"] = status
             __props__.__dict__["users_excludeds"] = users_excludeds
         super(RuleSignon, __self__).__init__(
             'okta:policy/ruleSignon:RuleSignon',
@@ -1120,14 +1168,15 @@
             network_connection: Optional[pulumi.Input[str]] = None,
             network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             network_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             policy_id: Optional[pulumi.Input[str]] = None,
             primary_factor: Optional[pulumi.Input[str]] = None,
             priority: Optional[pulumi.Input[int]] = None,
             risc_level: Optional[pulumi.Input[str]] = None,
+            risk_level: Optional[pulumi.Input[str]] = None,
             session_idle: Optional[pulumi.Input[int]] = None,
             session_lifetime: Optional[pulumi.Input[int]] = None,
             session_persistent: Optional[pulumi.Input[bool]] = None,
             status: Optional[pulumi.Input[str]] = None,
             users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'RuleSignon':
         """
         Get an existing RuleSignon resource's state with the given name, id, and optional extra
@@ -1154,14 +1203,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[str] primary_factor: Rule's primary factor. **WARNING** Ony works as a part of the Identity Engine. Valid values: 
                `"PASSWORD_IDP_ANY_FACTOR"`, `"PASSWORD_IDP"`.
         :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
         :param pulumi.Input[str] risc_level: Risc level: `"ANY"`, `"LOW"`, `"MEDIUM"` or `"HIGH"`. Default is `"ANY"`. It can be also 
                set to an empty string in case `RISC_SCORING` org feature flag is disabled.
+        :param pulumi.Input[str] risk_level: Risk level: ANY, LOW, MEDIUM or HIGH. Default: `ANY`
         :param pulumi.Input[int] session_idle: Max minutes a session can be idle.,
         :param pulumi.Input[int] session_lifetime: Max minutes a session is active: Disable = 0.
         :param pulumi.Input[bool] session_persistent: Whether session cookies will last across browser sessions. Okta Administrators can never have persistent session cookies.
         :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: The list of user IDs that would be excluded when rules are processed.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -1182,14 +1232,15 @@
         __props__.__dict__["network_connection"] = network_connection
         __props__.__dict__["network_excludes"] = network_excludes
         __props__.__dict__["network_includes"] = network_includes
         __props__.__dict__["policy_id"] = policy_id
         __props__.__dict__["primary_factor"] = primary_factor
         __props__.__dict__["priority"] = priority
         __props__.__dict__["risc_level"] = risc_level
+        __props__.__dict__["risk_level"] = risk_level
         __props__.__dict__["session_idle"] = session_idle
         __props__.__dict__["session_lifetime"] = session_lifetime
         __props__.__dict__["session_persistent"] = session_persistent
         __props__.__dict__["status"] = status
         __props__.__dict__["users_excludeds"] = users_excludeds
         return RuleSignon(resource_name, opts=opts, __props__=__props__)
 
@@ -1335,17 +1386,28 @@
     @property
     @pulumi.getter(name="riscLevel")
     def risc_level(self) -> pulumi.Output[Optional[str]]:
         """
         Risc level: `"ANY"`, `"LOW"`, `"MEDIUM"` or `"HIGH"`. Default is `"ANY"`. It can be also 
         set to an empty string in case `RISC_SCORING` org feature flag is disabled.
         """
+        warnings.warn("""Attribute typo, switch to risk_level instead. Default: `ANY`""", DeprecationWarning)
+        pulumi.log.warn("""risc_level is deprecated: Attribute typo, switch to risk_level instead. Default: `ANY`""")
+
         return pulumi.get(self, "risc_level")
 
     @property
+    @pulumi.getter(name="riskLevel")
+    def risk_level(self) -> pulumi.Output[Optional[str]]:
+        """
+        Risk level: ANY, LOW, MEDIUM or HIGH. Default: `ANY`
+        """
+        return pulumi.get(self, "risk_level")
+
+    @property
     @pulumi.getter(name="sessionIdle")
     def session_idle(self) -> pulumi.Output[Optional[int]]:
         """
         Max minutes a session can be idle.,
         """
         return pulumi.get(self, "session_idle")
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy/signon.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy_mfa_default.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_mfa_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy_password_default.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_password_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy_profile_enrollment.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy_profile_enrollment_apps.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_profile_enrollment_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/policy_rule_profile_enrollment.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_rule_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/profile/_inputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/profile/mapping.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/profile/outputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/provider.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/rate_limiting.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/resource_set.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/resource_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/role_subscription.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/role_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                - `"OKTA_UPDATE"` - Scheduled system updates.
                - `"IWA_AGENT"` - Disconnects and reconnects: IWA agent.
                - `"USER_DEPROVISION"` - User deprovisions.
                - `"REPORT_SUSPICIOUS_ACTIVITY"` - User reporting of suspicious activity.
                - `"RATELIMIT_NOTIFICATION"` - Rate limit warning and violation.
                - `"AGENT_AUTO_UPDATE_NOTIFICATION"` - Agent auto-update notifications: AD Agent.
         :param pulumi.Input[str] role_type: Type of the role. Valid values:
-               `"API_ADMIN"`,
+               `"API_ACCESS_MANAGEMENT_ADMIN"`,
                `"APP_ADMIN"`,
                `"CUSTOM"`,
                `"GROUP_MEMBERSHIP_ADMIN"`,
                `"HELP_DESK_ADMIN"`,
                `"MOBILE_ADMIN"`,
                `"ORG_ADMIN"`,
                `"READ_ONLY_ADMIN"`,
@@ -79,15 +79,15 @@
         pulumi.set(self, "notification_type", value)
 
     @property
     @pulumi.getter(name="roleType")
     def role_type(self) -> pulumi.Input[str]:
         """
         Type of the role. Valid values:
-        `"API_ADMIN"`,
+        `"API_ACCESS_MANAGEMENT_ADMIN"`,
         `"APP_ADMIN"`,
         `"CUSTOM"`,
         `"GROUP_MEMBERSHIP_ADMIN"`,
         `"HELP_DESK_ADMIN"`,
         `"MOBILE_ADMIN"`,
         `"ORG_ADMIN"`,
         `"READ_ONLY_ADMIN"`,
@@ -134,15 +134,15 @@
                - `"OKTA_UPDATE"` - Scheduled system updates.
                - `"IWA_AGENT"` - Disconnects and reconnects: IWA agent.
                - `"USER_DEPROVISION"` - User deprovisions.
                - `"REPORT_SUSPICIOUS_ACTIVITY"` - User reporting of suspicious activity.
                - `"RATELIMIT_NOTIFICATION"` - Rate limit warning and violation.
                - `"AGENT_AUTO_UPDATE_NOTIFICATION"` - Agent auto-update notifications: AD Agent.
         :param pulumi.Input[str] role_type: Type of the role. Valid values:
-               `"API_ADMIN"`,
+               `"API_ACCESS_MANAGEMENT_ADMIN"`,
                `"APP_ADMIN"`,
                `"CUSTOM"`,
                `"GROUP_MEMBERSHIP_ADMIN"`,
                `"HELP_DESK_ADMIN"`,
                `"MOBILE_ADMIN"`,
                `"ORG_ADMIN"`,
                `"READ_ONLY_ADMIN"`,
@@ -185,15 +185,15 @@
         pulumi.set(self, "notification_type", value)
 
     @property
     @pulumi.getter(name="roleType")
     def role_type(self) -> Optional[pulumi.Input[str]]:
         """
         Type of the role. Valid values:
-        `"API_ADMIN"`,
+        `"API_ACCESS_MANAGEMENT_ADMIN"`,
         `"APP_ADMIN"`,
         `"CUSTOM"`,
         `"GROUP_MEMBERSHIP_ADMIN"`,
         `"HELP_DESK_ADMIN"`,
         `"MOBILE_ADMIN"`,
         `"ORG_ADMIN"`,
         `"READ_ONLY_ADMIN"`,
@@ -270,15 +270,15 @@
                - `"OKTA_UPDATE"` - Scheduled system updates.
                - `"IWA_AGENT"` - Disconnects and reconnects: IWA agent.
                - `"USER_DEPROVISION"` - User deprovisions.
                - `"REPORT_SUSPICIOUS_ACTIVITY"` - User reporting of suspicious activity.
                - `"RATELIMIT_NOTIFICATION"` - Rate limit warning and violation.
                - `"AGENT_AUTO_UPDATE_NOTIFICATION"` - Agent auto-update notifications: AD Agent.
         :param pulumi.Input[str] role_type: Type of the role. Valid values:
-               `"API_ADMIN"`,
+               `"API_ACCESS_MANAGEMENT_ADMIN"`,
                `"APP_ADMIN"`,
                `"CUSTOM"`,
                `"GROUP_MEMBERSHIP_ADMIN"`,
                `"HELP_DESK_ADMIN"`,
                `"MOBILE_ADMIN"`,
                `"ORG_ADMIN"`,
                `"READ_ONLY_ADMIN"`,
@@ -386,15 +386,15 @@
                - `"OKTA_UPDATE"` - Scheduled system updates.
                - `"IWA_AGENT"` - Disconnects and reconnects: IWA agent.
                - `"USER_DEPROVISION"` - User deprovisions.
                - `"REPORT_SUSPICIOUS_ACTIVITY"` - User reporting of suspicious activity.
                - `"RATELIMIT_NOTIFICATION"` - Rate limit warning and violation.
                - `"AGENT_AUTO_UPDATE_NOTIFICATION"` - Agent auto-update notifications: AD Agent.
         :param pulumi.Input[str] role_type: Type of the role. Valid values:
-               `"API_ADMIN"`,
+               `"API_ACCESS_MANAGEMENT_ADMIN"`,
                `"APP_ADMIN"`,
                `"CUSTOM"`,
                `"GROUP_MEMBERSHIP_ADMIN"`,
                `"HELP_DESK_ADMIN"`,
                `"MOBILE_ADMIN"`,
                `"ORG_ADMIN"`,
                `"READ_ONLY_ADMIN"`,
@@ -435,15 +435,15 @@
         return pulumi.get(self, "notification_type")
 
     @property
     @pulumi.getter(name="roleType")
     def role_type(self) -> pulumi.Output[str]:
         """
         Type of the role. Valid values:
-        `"API_ADMIN"`,
+        `"API_ACCESS_MANAGEMENT_ADMIN"`,
         `"APP_ADMIN"`,
         `"CUSTOM"`,
         `"GROUP_MEMBERSHIP_ADMIN"`,
         `"HELP_DESK_ADMIN"`,
         `"MOBILE_ADMIN"`,
         `"ORG_ADMIN"`,
         `"READ_ONLY_ADMIN"`,
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/security_notification_emails.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/security_notification_emails.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/template_sms.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/template_sms.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/theme.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/threat_insight_settings.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/threat_insight_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/trustedorigin/origin.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/trustedorigin/origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/user/_inputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/user/get_user.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/user/get_user_profile_mapping_source.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_user_profile_mapping_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/user/get_user_type.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/user/get_users.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/user/outputs.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/user/user.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,16 @@
         :param pulumi.Input[str] first_name: User's First Name, required by default.
         :param pulumi.Input[str] last_name: User's Last Name, required by default.
         :param pulumi.Input[str] login: User profile property.
         :param pulumi.Input[str] city: User profile property.
         :param pulumi.Input[str] cost_center: User profile property.
         :param pulumi.Input[str] country_code: User profile property.
         :param pulumi.Input[str] custom_profile_attributes: raw JSON containing all custom profile attributes.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_profile_attributes_to_ignores: List of custom_profile_attribute keys that should be excluded from being managed by Terraform.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_profile_attributes_to_ignores: List of custom_profile_attribute keys that should be excluded from being managed by Terraform. This is useful in
+               situations where specific custom fields may contain sensitive information and should be managed outside of Terraform.
         :param pulumi.Input[str] department: User profile property.
         :param pulumi.Input[str] display_name: User profile property.
         :param pulumi.Input[str] division: User profile property.
         :param pulumi.Input[str] employee_number: User profile property.
         :param pulumi.Input[bool] expire_password_on_create: If set to `true`, the user will have to change the password at the next login. This property will be used
                when user is being created and works only when `password` field is set. Default is `false`.
         :param pulumi.Input[str] honorific_prefix: User profile property.
@@ -292,15 +293,16 @@
     def custom_profile_attributes(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_profile_attributes", value)
 
     @property
     @pulumi.getter(name="customProfileAttributesToIgnores")
     def custom_profile_attributes_to_ignores(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of custom_profile_attribute keys that should be excluded from being managed by Terraform.
+        List of custom_profile_attribute keys that should be excluded from being managed by Terraform. This is useful in
+        situations where specific custom fields may contain sensitive information and should be managed outside of Terraform.
         """
         return pulumi.get(self, "custom_profile_attributes_to_ignores")
 
     @custom_profile_attributes_to_ignores.setter
     def custom_profile_attributes_to_ignores(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "custom_profile_attributes_to_ignores", value)
 
@@ -761,15 +763,16 @@
                  zip_code: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering User resources.
         :param pulumi.Input[str] city: User profile property.
         :param pulumi.Input[str] cost_center: User profile property.
         :param pulumi.Input[str] country_code: User profile property.
         :param pulumi.Input[str] custom_profile_attributes: raw JSON containing all custom profile attributes.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_profile_attributes_to_ignores: List of custom_profile_attribute keys that should be excluded from being managed by Terraform.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_profile_attributes_to_ignores: List of custom_profile_attribute keys that should be excluded from being managed by Terraform. This is useful in
+               situations where specific custom fields may contain sensitive information and should be managed outside of Terraform.
         :param pulumi.Input[str] department: User profile property.
         :param pulumi.Input[str] display_name: User profile property.
         :param pulumi.Input[str] division: User profile property.
         :param pulumi.Input[str] email: User profile property.
         :param pulumi.Input[str] employee_number: User profile property.
         :param pulumi.Input[bool] expire_password_on_create: If set to `true`, the user will have to change the password at the next login. This property will be used
                when user is being created and works only when `password` field is set. Default is `false`.
@@ -952,15 +955,16 @@
     def custom_profile_attributes(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_profile_attributes", value)
 
     @property
     @pulumi.getter(name="customProfileAttributesToIgnores")
     def custom_profile_attributes_to_ignores(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of custom_profile_attribute keys that should be excluded from being managed by Terraform.
+        List of custom_profile_attribute keys that should be excluded from being managed by Terraform. This is useful in
+        situations where specific custom fields may contain sensitive information and should be managed outside of Terraform.
         """
         return pulumi.get(self, "custom_profile_attributes_to_ignores")
 
     @custom_profile_attributes_to_ignores.setter
     def custom_profile_attributes_to_ignores(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "custom_profile_attributes_to_ignores", value)
 
@@ -1556,15 +1560,16 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] city: User profile property.
         :param pulumi.Input[str] cost_center: User profile property.
         :param pulumi.Input[str] country_code: User profile property.
         :param pulumi.Input[str] custom_profile_attributes: raw JSON containing all custom profile attributes.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_profile_attributes_to_ignores: List of custom_profile_attribute keys that should be excluded from being managed by Terraform.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_profile_attributes_to_ignores: List of custom_profile_attribute keys that should be excluded from being managed by Terraform. This is useful in
+               situations where specific custom fields may contain sensitive information and should be managed outside of Terraform.
         :param pulumi.Input[str] department: User profile property.
         :param pulumi.Input[str] display_name: User profile property.
         :param pulumi.Input[str] division: User profile property.
         :param pulumi.Input[str] email: User profile property.
         :param pulumi.Input[str] employee_number: User profile property.
         :param pulumi.Input[bool] expire_password_on_create: If set to `true`, the user will have to change the password at the next login. This property will be used
                when user is being created and works only when `password` field is set. Default is `false`.
@@ -1866,15 +1871,16 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] city: User profile property.
         :param pulumi.Input[str] cost_center: User profile property.
         :param pulumi.Input[str] country_code: User profile property.
         :param pulumi.Input[str] custom_profile_attributes: raw JSON containing all custom profile attributes.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_profile_attributes_to_ignores: List of custom_profile_attribute keys that should be excluded from being managed by Terraform.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_profile_attributes_to_ignores: List of custom_profile_attribute keys that should be excluded from being managed by Terraform. This is useful in
+               situations where specific custom fields may contain sensitive information and should be managed outside of Terraform.
         :param pulumi.Input[str] department: User profile property.
         :param pulumi.Input[str] display_name: User profile property.
         :param pulumi.Input[str] division: User profile property.
         :param pulumi.Input[str] email: User profile property.
         :param pulumi.Input[str] employee_number: User profile property.
         :param pulumi.Input[bool] expire_password_on_create: If set to `true`, the user will have to change the password at the next login. This property will be used
                when user is being created and works only when `password` field is set. Default is `false`.
@@ -2000,15 +2006,16 @@
         """
         return pulumi.get(self, "custom_profile_attributes")
 
     @property
     @pulumi.getter(name="customProfileAttributesToIgnores")
     def custom_profile_attributes_to_ignores(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of custom_profile_attribute keys that should be excluded from being managed by Terraform.
+        List of custom_profile_attribute keys that should be excluded from being managed by Terraform. This is useful in
+        situations where specific custom fields may contain sensitive information and should be managed outside of Terraform.
         """
         return pulumi.get(self, "custom_profile_attributes_to_ignores")
 
     @property
     @pulumi.getter
     def department(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/user/user_type.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/user_admin_roles.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/user_admin_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/user_base_schema_property.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/user_factor_question.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/user_factor_question.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/user_group_memberships.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/user_group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta/user_schema_property.py` & `pulumi_okta-4.9.0a1713447075/pulumi_okta/user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta.egg-info/PKG-INFO` & `pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.9.0a1713445751
+Version: 4.9.0a1713447075
 Summary: A Pulumi package for creating and managing okta resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi,okta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_okta-4.9.0a1713445751/pulumi_okta.egg-info/SOURCES.txt` & `pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713445751/pyproject.toml` & `pulumi_okta-4.9.0a1713447075/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_okta"
   description = "A Pulumi package for creating and managing okta resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "okta"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "4.9.0a1713445751"
+  version = "4.9.0a1713447075"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-okta"
 
 [build-system]
```

