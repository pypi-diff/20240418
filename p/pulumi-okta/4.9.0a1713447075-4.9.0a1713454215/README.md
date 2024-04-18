# Comparing `tmp/pulumi_okta-4.9.0a1713447075.tar.gz` & `tmp/pulumi_okta-4.9.0a1713454215.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_okta-4.9.0a1713447075.tar", last modified: Thu Apr 18 13:34:13 2024, max compression
+gzip compressed data, was "pulumi_okta-4.9.0a1713454215.tar", last modified: Thu Apr 18 15:33:09 2024, max compression
```

## Comparing `pulumi_okta-4.9.0a1713447075.tar` & `pulumi_okta-4.9.0a1713454215.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.303452 pulumi_okta-4.9.0a1713447075/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-18 13:34:13.303452 pulumi_okta-4.9.0a1713447075/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.279452 pulumi_okta-4.9.0a1713447075/pulumi_okta/
--rw-r--r--   0 runner    (1001) docker     (127)    21302 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/admin_role_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/admin_role_custom_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/admin_role_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.283452 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/access_policy_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    64105 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/auto_login.py
--rw-r--r--   0 runner    (1001) docker     (127)    37151 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    40464 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    32406 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/group_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)   147044 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/o_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/o_auth_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/oauth_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   138292 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    72919 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/secure_password_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    59554 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/swa.py
--rw-r--r--   0 runner    (1001) docker     (127)    67402 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/three_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_oauth_api_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_saml_app_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    66199 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_shared_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    91388 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_signon_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    23715 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    51605 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/app_user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.287452 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/get_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/get_server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/get_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23581 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    17696 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    47955 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_policy_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    47597 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    22572 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    20134 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth_server_claim_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/auth_server_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    47596 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24178 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)    30565 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/brand.py
--rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/captcha_org_wide_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.287452 pulumi_okta-4.9.0a1713447075/pulumi_okta/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    14270 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/domain_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    39467 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/email_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/email_sender_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/event_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/event_hook_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.287452 pulumi_okta-4.9.0a1713447075/pulumi_okta/factor/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/factor/factor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/factor_totp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_app_user_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_auth_server_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_auth_server_claims.py
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_brands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_email_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_email_customizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_network_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_themes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_trusted_origins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/get_user_security_questions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.291452 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/get_everyone_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/get_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    15299 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    24255 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    20949 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    47368 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/group_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.291452 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    18055 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_social.py
--rw-r--r--   0 runner    (1001) docker     (127)    87493 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    83512 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/saml_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    72978 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/social.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.295452 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50207 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18671 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/customized_signin_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/email_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/email_domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_default_signin_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_org_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    43669 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18545 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/index/preview_signin_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.295452 pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19244 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/link_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/link_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.295452 pulumi_okta-4.9.0a1713447075/pulumi_okta/network/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26479 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/network/zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    36906 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/org_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/org_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    37606 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.299452 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16040 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22470 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_android.py
--rw-r--r--   0 runner    (1001) docker     (127)    46102 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_chromeos.py
--rw-r--r--   0 runner    (1001) docker     (127)    17701 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_ios.py
--rw-r--r--   0 runner    (1001) docker     (127)    56229 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_macos.py
--rw-r--r--   0 runner    (1001) docker     (127)    71621 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/get_default_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    69300 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    79741 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/password.py
--rw-r--r--   0 runner    (1001) docker     (127)    51815 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_idp_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    34098 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_password.py
--rw-r--r--   0 runner    (1001) docker     (127)    69730 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_signon.py
--rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/signon.py
--rw-r--r--   0 runner    (1001) docker     (127)    65473 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_mfa_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    71555 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_password_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_profile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_profile_enrollment_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    35011 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_rule_profile_enrollment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.299452 pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23956 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/rate_limiting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/resource_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    21342 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    21992 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/security_notification_emails.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/template_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    42952 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/theme.py
--rw-r--r--   0 runner    (1001) docker     (127)    14948 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/threat_insight_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.299452 pulumi_okta-4.9.0a1713447075/pulumi_okta/trustedorigin/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/trustedorigin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/trustedorigin/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.303452 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25722 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_user_profile_mapping_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   100207 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user/user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user_admin_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    23075 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user_factor_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user_group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    51854 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta/user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:13.303452 pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-18 13:34:13.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-18 13:34:13.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:34:13.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 13:34:13.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 13:34:13.000000 pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-18 13:34:06.000000 pulumi_okta-4.9.0a1713447075/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:34:13.303452 pulumi_okta-4.9.0a1713447075/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.777334 pulumi_okta-4.9.0a1713454215/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-18 15:33:09.777334 pulumi_okta-4.9.0a1713454215/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.757334 pulumi_okta-4.9.0a1713454215/pulumi_okta/
+-rw-r--r--   0 runner    (1001) docker     (127)    21302 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/admin_role_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/admin_role_custom_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/admin_role_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.761334 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/access_policy_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64105 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/auto_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37151 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40464 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/get_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32406 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/group_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)   147044 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/o_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/o_auth_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/oauth_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138292 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72919 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/secure_password_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59554 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/swa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67402 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/three_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app_oauth_api_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app_saml_app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66199 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app_shared_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91388 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app_signon_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23715 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app_user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51605 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/app_user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.765334 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/get_server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/get_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23581 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17696 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47955 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/server_policy_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47597 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/server_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22572 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20134 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth_server_claim_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/auth_server_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47596 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24178 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30565 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/captcha_org_wide_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.765334 pulumi_okta-4.9.0a1713454215/pulumi_okta/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14270 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/domain_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39467 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/email_sender_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/event_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/event_hook_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.765334 pulumi_okta-4.9.0a1713454215/pulumi_okta/factor/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/factor/factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/factor_totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_app_user_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_auth_server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_auth_server_claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_brands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_email_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_network_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_themes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_trusted_origins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/get_user_security_questions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.765334 pulumi_okta-4.9.0a1713454215/pulumi_okta/group/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/group/get_everyone_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/group/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/group/get_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15299 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24255 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/group/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20949 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/group/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47368 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/group_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.769334 pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/get_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18055 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/get_social.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87493 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83512 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/saml_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72978 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/social.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.769334 pulumi_okta-4.9.0a1713454215/pulumi_okta/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50207 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/index/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/index/customized_signin_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/index/email_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/index/email_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/index/get_default_signin_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/index/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/index/get_log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/index/get_org_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/index/log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43669 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/index/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18617 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/index/preview_signin_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.773334 pulumi_okta-4.9.0a1713454215/pulumi_okta/inline/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/inline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19244 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/inline/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/inline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/link_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/link_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.773334 pulumi_okta-4.9.0a1713454215/pulumi_okta/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26479 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/network/zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36906 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/org_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/org_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37606 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.777334 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16040 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22720 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/device_assurance_android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48316 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/device_assurance_chromeos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/device_assurance_ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56471 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/device_assurance_macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71871 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/device_assurance_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/get_default_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69300 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79741 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51815 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/rule_idp_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34098 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/rule_mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/rule_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69730 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/rule_signon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/signon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65473 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy_mfa_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71555 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy_password_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy_profile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy_profile_enrollment_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35011 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/policy_rule_profile_enrollment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.777334 pulumi_okta-4.9.0a1713454215/pulumi_okta/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/profile/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23956 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/profile/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/profile/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/rate_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/resource_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21342 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21992 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/security_notification_emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/template_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42952 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14948 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/threat_insight_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.777334 pulumi_okta-4.9.0a1713454215/pulumi_okta/trustedorigin/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/trustedorigin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/trustedorigin/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.777334 pulumi_okta-4.9.0a1713454215/pulumi_okta/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25722 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user/get_user_profile_mapping_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user/get_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100207 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user_admin_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23075 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user_factor_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user_group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51854 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta/user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:33:09.777334 pulumi_okta-4.9.0a1713454215/pulumi_okta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-18 15:33:09.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-18 15:33:09.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:33:09.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 15:33:09.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 15:33:09.000000 pulumi_okta-4.9.0a1713454215/pulumi_okta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-18 15:33:03.000000 pulumi_okta-4.9.0a1713454215/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:33:09.777334 pulumi_okta-4.9.0a1713454215/setup.cfg
```

### Comparing `pulumi_okta-4.9.0a1713447075/PKG-INFO` & `pulumi_okta-4.9.0a1713454215/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.9.0a1713447075
+Version: 4.9.0a1713454215
 Summary: A Pulumi package for creating and managing okta resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi,okta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_okta-4.9.0a1713447075/README.md` & `pulumi_okta-4.9.0a1713454215/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/__init__.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/_inputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/_utilities.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/admin_role_custom.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/admin_role_custom.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/admin_role_custom_assignments.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/admin_role_custom_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/admin_role_targets.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/admin_role_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/__init__.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/_inputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/access_policy_assignment.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/access_policy_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/auto_login.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/auto_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/basic_auth.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/bookmark.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/bookmark.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_app.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_metadata_saml.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_oauth.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/get_oauth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/get_saml.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/group_assignment.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/group_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/o_auth.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/o_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/o_auth_post_logout_redirect_uri.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/o_auth_post_logout_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/o_auth_redirect_uri.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/o_auth_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/oauth_role_assignment.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/oauth_role_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/outputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/saml.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/secure_password_store.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/secure_password_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/swa.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/swa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/three_field.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/three_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app/user.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_group_assignments.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_oauth_api_scope.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app_oauth_api_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_saml_app_settings.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app_saml_app_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_shared_credentials.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app_shared_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_signon_policy.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_signon_policy_rule.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app_signon_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_user_base_schema_property.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app_user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/app_user_schema_property.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/app_user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/__init__.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/get_server.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/get_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/get_server_policy.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/get_server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/get_server_scopes.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/get_server_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/outputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_claim.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_policy.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_policy_claim.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/server_policy_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_policy_rule.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/server_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth/server_scope.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/auth/server_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth_server_claim_default.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/auth_server_claim_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/auth_server_default.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/auth_server_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/authenticator.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/behaviour.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/brand.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/captcha.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/captcha.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/captcha_org_wide_settings.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/captcha_org_wide_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/config/__init__.pyi` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/config/vars.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/domain.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/domain_certificate.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/domain_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/domain_verification.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/email_customization.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/email_sender.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/email_sender.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/email_sender_verification.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/email_sender_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/event_hook.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/event_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/event_hook_verification.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/event_hook_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/factor/factor.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/factor/factor.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/factor_totp.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/factor_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_app_group_assignments.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_app_signon_policy.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_app_user_assignments.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_app_user_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_auth_server_claim.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_auth_server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_auth_server_claims.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_auth_server_claims.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_authenticator.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_behaviour.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_behaviours.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_behaviours.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_brand.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_brands.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_brands.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_email_customization.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_email_customizations.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_email_customizations.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_groups.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_network_zone.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_network_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_role_subscription.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_template.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_templates.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_theme.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_themes.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_themes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_trusted_origins.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_trusted_origins.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/get_user_security_questions.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/get_user_security_questions.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/group/get_everyone_group.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/group/get_everyone_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/group/get_group.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/group/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/group/get_rule.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/group/get_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/group/group.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/group/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/group/role.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/group/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/group/rule.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/group/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/group_memberships.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/group_schema_property.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/group_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_metadata_saml.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_oidc.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/get_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_saml.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/get_social.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/get_social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/oidc.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/saml.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/saml_key.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/saml_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/idp/social.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/idp/social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/__init__.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/index/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/_inputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/index/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/customized_signin_page.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/index/customized_signin_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,19 +21,20 @@
                  widget_version: pulumi.Input[str],
                  content_security_policy_setting: Optional[pulumi.Input['CustomizedSigninPageContentSecurityPolicySettingArgs']] = None,
                  widget_customizations: Optional[pulumi.Input['CustomizedSigninPageWidgetCustomizationsArgs']] = None):
         """
         The set of arguments for constructing a CustomizedSigninPage resource.
         :param pulumi.Input[str] brand_id: brand id of the preview signin page
         :param pulumi.Input[str] page_content: page content of the preview signin page
-        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-               1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-               2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-               5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-               6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported
+               		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+               		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+               		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+               		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+               		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         pulumi.set(__self__, "brand_id", brand_id)
         pulumi.set(__self__, "page_content", page_content)
         pulumi.set(__self__, "widget_version", widget_version)
         if content_security_policy_setting is not None:
             pulumi.set(__self__, "content_security_policy_setting", content_security_policy_setting)
         if widget_customizations is not None:
@@ -63,19 +64,20 @@
     def page_content(self, value: pulumi.Input[str]):
         pulumi.set(self, "page_content", value)
 
     @property
     @pulumi.getter(name="widgetVersion")
     def widget_version(self) -> pulumi.Input[str]:
         """
-        widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-        1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-        2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-        5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-        6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        widget version specified as a Semver. The following are currently supported
+        		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+        		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+        		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+        		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+        		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         return pulumi.get(self, "widget_version")
 
     @widget_version.setter
     def widget_version(self, value: pulumi.Input[str]):
         pulumi.set(self, "widget_version", value)
 
@@ -106,19 +108,20 @@
                  page_content: Optional[pulumi.Input[str]] = None,
                  widget_customizations: Optional[pulumi.Input['CustomizedSigninPageWidgetCustomizationsArgs']] = None,
                  widget_version: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering CustomizedSigninPage resources.
         :param pulumi.Input[str] brand_id: brand id of the preview signin page
         :param pulumi.Input[str] page_content: page content of the preview signin page
-        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-               1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-               2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-               5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-               6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported
+               		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+               		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+               		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+               		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+               		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         if brand_id is not None:
             pulumi.set(__self__, "brand_id", brand_id)
         if content_security_policy_setting is not None:
             pulumi.set(__self__, "content_security_policy_setting", content_security_policy_setting)
         if page_content is not None:
             pulumi.set(__self__, "page_content", page_content)
@@ -169,19 +172,20 @@
     def widget_customizations(self, value: Optional[pulumi.Input['CustomizedSigninPageWidgetCustomizationsArgs']]):
         pulumi.set(self, "widget_customizations", value)
 
     @property
     @pulumi.getter(name="widgetVersion")
     def widget_version(self) -> Optional[pulumi.Input[str]]:
         """
-        widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-        1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-        2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-        5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-        6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        widget version specified as a Semver. The following are currently supported
+        		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+        		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+        		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+        		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+        		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         return pulumi.get(self, "widget_version")
 
     @widget_version.setter
     def widget_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "widget_version", value)
 
@@ -194,33 +198,48 @@
                  brand_id: Optional[pulumi.Input[str]] = None,
                  content_security_policy_setting: Optional[pulumi.Input[pulumi.InputType['CustomizedSigninPageContentSecurityPolicySettingArgs']]] = None,
                  page_content: Optional[pulumi.Input[str]] = None,
                  widget_customizations: Optional[pulumi.Input[pulumi.InputType['CustomizedSigninPageWidgetCustomizationsArgs']]] = None,
                  widget_version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a CustomizedSigninPage resource with the given unique name, props, and options.
+        Manage the customized signin page of a brand
+
+        ## Import
+
+        ```sh
+        $ pulumi import okta:Index/customizedSigninPage:CustomizedSigninPage example &#60;customized_signin_page_id&#62;
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] brand_id: brand id of the preview signin page
         :param pulumi.Input[str] page_content: page content of the preview signin page
-        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-               1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-               2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-               5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-               6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported
+               		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+               		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+               		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+               		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+               		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: CustomizedSigninPageArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a CustomizedSigninPage resource with the given unique name, props, and options.
+        Manage the customized signin page of a brand
+
+        ## Import
+
+        ```sh
+        $ pulumi import okta:Index/customizedSigninPage:CustomizedSigninPage example &#60;customized_signin_page_id&#62;
+        ```
+
         :param str resource_name: The name of the resource.
         :param CustomizedSigninPageArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(CustomizedSigninPageArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -277,19 +296,20 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] brand_id: brand id of the preview signin page
         :param pulumi.Input[str] page_content: page content of the preview signin page
-        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-               1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-               2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-               5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-               6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported
+               		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+               		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+               		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+               		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+               		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _CustomizedSigninPageState.__new__(_CustomizedSigninPageState)
 
         __props__.__dict__["brand_id"] = brand_id
         __props__.__dict__["content_security_policy_setting"] = content_security_policy_setting
@@ -324,15 +344,16 @@
     def widget_customizations(self) -> pulumi.Output[Optional['outputs.CustomizedSigninPageWidgetCustomizations']]:
         return pulumi.get(self, "widget_customizations")
 
     @property
     @pulumi.getter(name="widgetVersion")
     def widget_version(self) -> pulumi.Output[str]:
         """
-        widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-        1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-        2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-        5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-        6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        widget version specified as a Semver. The following are currently supported
+        		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+        		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+        		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+        		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+        		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         return pulumi.get(self, "widget_version")
```

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/email_domain.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/index/email_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/email_domain_verification.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/index/email_domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_default_signin_page.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/index/get_default_signin_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,39 +42,51 @@
         if widget_version and not isinstance(widget_version, str):
             raise TypeError("Expected argument 'widget_version' to be a str")
         pulumi.set(__self__, "widget_version", widget_version)
 
     @property
     @pulumi.getter(name="brandId")
     def brand_id(self) -> str:
+        """
+        brand id of the preview signin page
+        """
         return pulumi.get(self, "brand_id")
 
     @property
     @pulumi.getter(name="contentSecurityPolicySetting")
     def content_security_policy_setting(self) -> Optional['outputs.GetDefaultSigninPageContentSecurityPolicySettingResult']:
         return pulumi.get(self, "content_security_policy_setting")
 
     @property
     @pulumi.getter
     def id(self) -> str:
+        """
+        placeholder id
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="pageContent")
     def page_content(self) -> str:
+        """
+        page content of the preview signin page
+        """
         return pulumi.get(self, "page_content")
 
     @property
     @pulumi.getter(name="widgetCustomizations")
     def widget_customizations(self) -> Optional['outputs.GetDefaultSigninPageWidgetCustomizationsResult']:
         return pulumi.get(self, "widget_customizations")
 
     @property
     @pulumi.getter(name="widgetVersion")
     def widget_version(self) -> str:
+        """
+        widget version specified as a Semver
+        """
         return pulumi.get(self, "widget_version")
 
 
 class AwaitableGetDefaultSigninPageResult(GetDefaultSigninPageResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -89,15 +101,18 @@
 
 
 def get_default_signin_page(brand_id: Optional[str] = None,
                             content_security_policy_setting: Optional[pulumi.InputType['GetDefaultSigninPageContentSecurityPolicySettingArgs']] = None,
                             widget_customizations: Optional[pulumi.InputType['GetDefaultSigninPageWidgetCustomizationsArgs']] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDefaultSigninPageResult:
     """
-    Use this data source to access information about an existing resource.
+    Retrieve the default signin page of a brand
+
+
+    :param str brand_id: brand id of the preview signin page
     """
     __args__ = dict()
     __args__['brandId'] = brand_id
     __args__['contentSecurityPolicySetting'] = content_security_policy_setting
     __args__['widgetCustomizations'] = widget_customizations
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:Index/getDefaultSigninPage:getDefaultSigninPage', __args__, opts=opts, typ=GetDefaultSigninPageResult).value
@@ -113,10 +128,13 @@
 
 @_utilities.lift_output_func(get_default_signin_page)
 def get_default_signin_page_output(brand_id: Optional[pulumi.Input[str]] = None,
                                    content_security_policy_setting: Optional[pulumi.Input[Optional[pulumi.InputType['GetDefaultSigninPageContentSecurityPolicySettingArgs']]]] = None,
                                    widget_customizations: Optional[pulumi.Input[Optional[pulumi.InputType['GetDefaultSigninPageWidgetCustomizationsArgs']]]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDefaultSigninPageResult]:
     """
-    Use this data source to access information about an existing resource.
+    Retrieve the default signin page of a brand
+
+
+    :param str brand_id: brand id of the preview signin page
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_domain.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/index/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_log_stream.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/index/get_log_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/get_org_metadata.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/index/get_org_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/log_stream.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/index/log_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/outputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/index/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/index/preview_signin_page.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/index/preview_signin_page.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,20 @@
                  widget_version: pulumi.Input[str],
                  content_security_policy_setting: Optional[pulumi.Input['PreviewSigninPageContentSecurityPolicySettingArgs']] = None,
                  widget_customizations: Optional[pulumi.Input['PreviewSigninPageWidgetCustomizationsArgs']] = None):
         """
         The set of arguments for constructing a PreviewSigninPage resource.
         :param pulumi.Input[str] brand_id: brand id of the preview signin page
         :param pulumi.Input[str] page_content: page content of the preview signin page
-        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-               1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-               2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-               5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-               6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported
+               		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+               		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+               		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+               		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+               		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         pulumi.set(__self__, "brand_id", brand_id)
         pulumi.set(__self__, "page_content", page_content)
         pulumi.set(__self__, "widget_version", widget_version)
         if content_security_policy_setting is not None:
             pulumi.set(__self__, "content_security_policy_setting", content_security_policy_setting)
         if widget_customizations is not None:
@@ -63,19 +64,20 @@
     def page_content(self, value: pulumi.Input[str]):
         pulumi.set(self, "page_content", value)
 
     @property
     @pulumi.getter(name="widgetVersion")
     def widget_version(self) -> pulumi.Input[str]:
         """
-        widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-        1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-        2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-        5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-        6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        widget version specified as a Semver. The following are currently supported
+        		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+        		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+        		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+        		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+        		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         return pulumi.get(self, "widget_version")
 
     @widget_version.setter
     def widget_version(self, value: pulumi.Input[str]):
         pulumi.set(self, "widget_version", value)
 
@@ -106,19 +108,20 @@
                  page_content: Optional[pulumi.Input[str]] = None,
                  widget_customizations: Optional[pulumi.Input['PreviewSigninPageWidgetCustomizationsArgs']] = None,
                  widget_version: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering PreviewSigninPage resources.
         :param pulumi.Input[str] brand_id: brand id of the preview signin page
         :param pulumi.Input[str] page_content: page content of the preview signin page
-        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-               1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-               2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-               5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-               6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported
+               		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+               		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+               		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+               		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+               		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         if brand_id is not None:
             pulumi.set(__self__, "brand_id", brand_id)
         if content_security_policy_setting is not None:
             pulumi.set(__self__, "content_security_policy_setting", content_security_policy_setting)
         if page_content is not None:
             pulumi.set(__self__, "page_content", page_content)
@@ -169,19 +172,20 @@
     def widget_customizations(self, value: Optional[pulumi.Input['PreviewSigninPageWidgetCustomizationsArgs']]):
         pulumi.set(self, "widget_customizations", value)
 
     @property
     @pulumi.getter(name="widgetVersion")
     def widget_version(self) -> Optional[pulumi.Input[str]]:
         """
-        widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-        1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-        2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-        5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-        6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        widget version specified as a Semver. The following are currently supported
+        		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+        		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+        		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+        		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+        		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         return pulumi.get(self, "widget_version")
 
     @widget_version.setter
     def widget_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "widget_version", value)
 
@@ -194,33 +198,36 @@
                  brand_id: Optional[pulumi.Input[str]] = None,
                  content_security_policy_setting: Optional[pulumi.Input[pulumi.InputType['PreviewSigninPageContentSecurityPolicySettingArgs']]] = None,
                  page_content: Optional[pulumi.Input[str]] = None,
                  widget_customizations: Optional[pulumi.Input[pulumi.InputType['PreviewSigninPageWidgetCustomizationsArgs']]] = None,
                  widget_version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a PreviewSigninPage resource with the given unique name, props, and options.
+        Manage the preview signin page of a brand
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] brand_id: brand id of the preview signin page
         :param pulumi.Input[str] page_content: page content of the preview signin page
-        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-               1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-               2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-               5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-               6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported
+               		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+               		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+               		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+               		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+               		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: PreviewSigninPageArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a PreviewSigninPage resource with the given unique name, props, and options.
+        Manage the preview signin page of a brand
+
         :param str resource_name: The name of the resource.
         :param PreviewSigninPageArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(PreviewSigninPageArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -277,19 +284,20 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] brand_id: brand id of the preview signin page
         :param pulumi.Input[str] page_content: page content of the preview signin page
-        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-               1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-               2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-               5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-               6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        :param pulumi.Input[str] widget_version: widget version specified as a Semver. The following are currently supported
+               		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+               		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+               		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+               		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+               		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PreviewSigninPageState.__new__(_PreviewSigninPageState)
 
         __props__.__dict__["brand_id"] = brand_id
         __props__.__dict__["content_security_policy_setting"] = content_security_policy_setting
@@ -324,15 +332,16 @@
     def widget_customizations(self) -> pulumi.Output[Optional['outputs.PreviewSigninPageWidgetCustomizations']]:
         return pulumi.get(self, "widget_customizations")
 
     @property
     @pulumi.getter(name="widgetVersion")
     def widget_version(self) -> pulumi.Output[str]:
         """
-        widget version specified as a Semver. The following are currently supported *, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7,
-        1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16,
-        2.17, 2.18, 2.19, 2.20, 2.21, 3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1,
-        5.2, 5.3, 5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5, 6.6,
-        6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
+        widget version specified as a Semver. The following are currently supported
+        		*, ^1, ^2, ^3, ^4, ^5, ^6, ^7, 1.6, 1.7, 1.8, 1.9, 1.10, 1.11, 1.12, 1.13, 2.1, 2.2, 2.3, 2.4,
+        		2.5, 2.6, 2.7, 2.8, 2.9, 2.10, 2.11, 2.12, 2.13, 2.14, 2.15, 2.16, 2.17, 2.18, 2.19, 2.20, 2.21,
+        		3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 4.0, 4.1, 4.2, 4.3, 4.4, 4.5, 5.0, 5.1, 5.2, 5.3,
+        		5.4, 5.5, 5.6, 5.7, 5.8, 5.9, 5.10, 5.11, 5.12, 5.13, 5.14, 5.15, 5.16, 6.0, 6.1, 6.2, 6.3, 6.4, 6.5,
+        		6.6, 6.7, 6.8, 6.9, 7.0, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6, 7.7, 7.8, 7.9, 7.10, 7.11, 7.12, 7.13.
         """
         return pulumi.get(self, "widget_version")
```

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/_inputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/inline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/hook.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/inline/hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/inline/outputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/inline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/link_definition.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/link_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/link_value.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/link_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/network/zone.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/network/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/org_configuration.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/org_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/org_support.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/org_support.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/outputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/__init__.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/_inputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_android.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/device_assurance_android.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,15 +308,22 @@
                  jailbreak: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  os_version: Optional[pulumi.Input[str]] = None,
                  screenlock_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  secure_hardware_present: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        Create a DeviceAssuranceAndroid resource with the given unique name, props, and options.
+        Manages a device assurance policy for android.
+
+        ## Import
+
+        ```sh
+        $ pulumi import okta:policy/deviceAssuranceAndroid:DeviceAssuranceAndroid example &#60;device assurance id&#62;
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `FULL`, `USER`
         :param pulumi.Input[bool] jailbreak: Is the device jailbroken in the device assurance policy.
         :param pulumi.Input[str] name: Policy device assurance name
         :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
@@ -325,15 +332,22 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[DeviceAssuranceAndroidArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a DeviceAssuranceAndroid resource with the given unique name, props, and options.
+        Manages a device assurance policy for android.
+
+        ## Import
+
+        ```sh
+        $ pulumi import okta:policy/deviceAssuranceAndroid:DeviceAssuranceAndroid example &#60;device assurance id&#62;
+        ```
+
         :param str resource_name: The name of the resource.
         :param DeviceAssuranceAndroidArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(DeviceAssuranceAndroidArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_chromeos.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/device_assurance_chromeos.py`

 * *Files 2% similar despite different names*

```diff
@@ -605,15 +605,47 @@
                  tpsp_password_proctection_warning_trigger: Optional[pulumi.Input[str]] = None,
                  tpsp_realtime_url_check_mode: Optional[pulumi.Input[bool]] = None,
                  tpsp_safe_browsing_protection_level: Optional[pulumi.Input[str]] = None,
                  tpsp_screen_lock_secured: Optional[pulumi.Input[bool]] = None,
                  tpsp_site_isolation_enabled: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        Create a DeviceAssuranceChromeos resource with the given unique name, props, and options.
+        Manages a device assurance policy for chromeos.
+
+        ## Example Usage
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_okta as okta
+
+        example = okta.policy.DeviceAssuranceChromeos("example",
+            tpsp_allow_screen_lock=True,
+            tpsp_browser_version="15393.27.0",
+            tpsp_builtin_dns_client_enabled=True,
+            tpsp_chrome_remote_desktop_app_blocked=True,
+            tpsp_device_enrollment_domain="exampleDomain",
+            tpsp_disk_encrypted=True,
+            tpsp_key_trust_level="CHROME_OS_VERIFIED_MODE",
+            tpsp_os_firewall=True,
+            tpsp_os_version="10.0.19041.1110",
+            tpsp_password_proctection_warning_trigger="PASSWORD_PROTECTION_OFF",
+            tpsp_realtime_url_check_mode=True,
+            tpsp_safe_browsing_protection_level="ENHANCED_PROTECTION",
+            tpsp_screen_lock_secured=True,
+            tpsp_site_isolation_enabled=True)
+        ```
+        <!--End PulumiCodeChooser -->
+
+        ## Import
+
+        ```sh
+        $ pulumi import okta:policy/deviceAssuranceChromeos:DeviceAssuranceChromeos example &#60;device assurance id&#62;
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: Name of the device assurance policy.
         :param pulumi.Input[bool] tpsp_allow_screen_lock: Third party signal provider allow screen lock
         :param pulumi.Input[str] tpsp_browser_version: Third party signal provider minimum browser version
         :param pulumi.Input[bool] tpsp_builtin_dns_client_enabled: Third party signal provider builtin dns client enabled
         :param pulumi.Input[bool] tpsp_chrome_remote_desktop_app_blocked: Third party signal provider chrome remote desktop app blocked
@@ -631,15 +663,47 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[DeviceAssuranceChromeosArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a DeviceAssuranceChromeos resource with the given unique name, props, and options.
+        Manages a device assurance policy for chromeos.
+
+        ## Example Usage
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_okta as okta
+
+        example = okta.policy.DeviceAssuranceChromeos("example",
+            tpsp_allow_screen_lock=True,
+            tpsp_browser_version="15393.27.0",
+            tpsp_builtin_dns_client_enabled=True,
+            tpsp_chrome_remote_desktop_app_blocked=True,
+            tpsp_device_enrollment_domain="exampleDomain",
+            tpsp_disk_encrypted=True,
+            tpsp_key_trust_level="CHROME_OS_VERIFIED_MODE",
+            tpsp_os_firewall=True,
+            tpsp_os_version="10.0.19041.1110",
+            tpsp_password_proctection_warning_trigger="PASSWORD_PROTECTION_OFF",
+            tpsp_realtime_url_check_mode=True,
+            tpsp_safe_browsing_protection_level="ENHANCED_PROTECTION",
+            tpsp_screen_lock_secured=True,
+            tpsp_site_isolation_enabled=True)
+        ```
+        <!--End PulumiCodeChooser -->
+
+        ## Import
+
+        ```sh
+        $ pulumi import okta:policy/deviceAssuranceChromeos:DeviceAssuranceChromeos example &#60;device assurance id&#62;
+        ```
+
         :param str resource_name: The name of the resource.
         :param DeviceAssuranceChromeosArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(DeviceAssuranceChromeosArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_ios.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/device_assurance_ios.py`

 * *Files 5% similar despite different names*

```diff
@@ -242,30 +242,44 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  jailbreak: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  os_version: Optional[pulumi.Input[str]] = None,
                  screenlock_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
-        Create a DeviceAssuranceIos resource with the given unique name, props, and options.
+        Manages a device assurance policy for ios.
+
+        ## Import
+
+        ```sh
+        $ pulumi import okta:policy/deviceAssuranceIos:DeviceAssuranceIos example &#60;device assurance id&#62;
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] jailbreak: Is the device jailbroken in the device assurance policy.
         :param pulumi.Input[str] name: Name of the device assurance policy.
         :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[DeviceAssuranceIosArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a DeviceAssuranceIos resource with the given unique name, props, and options.
+        Manages a device assurance policy for ios.
+
+        ## Import
+
+        ```sh
+        $ pulumi import okta:policy/deviceAssuranceIos:DeviceAssuranceIos example &#60;device assurance id&#62;
+        ```
+
         :param str resource_name: The name of the resource.
         :param DeviceAssuranceIosArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(DeviceAssuranceIosArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_macos.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/device_assurance_macos.py`

 * *Files 0% similar despite different names*

```diff
@@ -737,15 +737,22 @@
                  tpsp_password_proctection_warning_trigger: Optional[pulumi.Input[str]] = None,
                  tpsp_realtime_url_check_mode: Optional[pulumi.Input[bool]] = None,
                  tpsp_safe_browsing_protection_level: Optional[pulumi.Input[str]] = None,
                  tpsp_screen_lock_secured: Optional[pulumi.Input[bool]] = None,
                  tpsp_site_isolation_enabled: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        Create a DeviceAssuranceMacos resource with the given unique name, props, and options.
+        Manages a device assurance policy for macos.
+
+        ## Import
+
+        ```sh
+        $ pulumi import okta:policy/deviceAssuranceMacos:DeviceAssuranceMacos example &#60;device assurance id&#62;
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
         :param pulumi.Input[str] name: Name of the device assurance policy.
         :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         :param pulumi.Input[bool] secure_hardware_present: Is the device secure with hardware in the device assurance policy.
@@ -767,15 +774,22 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[DeviceAssuranceMacosArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a DeviceAssuranceMacos resource with the given unique name, props, and options.
+        Manages a device assurance policy for macos.
+
+        ## Import
+
+        ```sh
+        $ pulumi import okta:policy/deviceAssuranceMacos:DeviceAssuranceMacos example &#60;device assurance id&#62;
+        ```
+
         :param str resource_name: The name of the resource.
         :param DeviceAssuranceMacosArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(DeviceAssuranceMacosArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/device_assurance_windows.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/device_assurance_windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -935,15 +935,22 @@
                  tpsp_secure_boot_enabled: Optional[pulumi.Input[bool]] = None,
                  tpsp_site_isolation_enabled: Optional[pulumi.Input[bool]] = None,
                  tpsp_third_party_blocking_enabled: Optional[pulumi.Input[bool]] = None,
                  tpsp_windows_machine_domain: Optional[pulumi.Input[str]] = None,
                  tpsp_windows_user_domain: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a DeviceAssuranceWindows resource with the given unique name, props, and options.
+        Manages a device assurance policy for windows.
+
+        ## Import
+
+        ```sh
+        $ pulumi import okta:policy/deviceAssuranceWindows:DeviceAssuranceWindows example &#60;device assurance id&#62;
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] disk_encryption_types: List of disk encryption type, can be `ALL_INTERNAL_VOLUMES`
         :param pulumi.Input[str] name: Name of the device assurance policy.
         :param pulumi.Input[str] os_version: Minimum os version of the device in the device assurance policy.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] screenlock_types: List of screenlock type, can be `BIOMETRIC` or `BIOMETRIC, PASSCODE`
         :param pulumi.Input[bool] secure_hardware_present: Is the device secure with hardware in the device assurance policy.
@@ -971,15 +978,22 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[DeviceAssuranceWindowsArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a DeviceAssuranceWindows resource with the given unique name, props, and options.
+        Manages a device assurance policy for windows.
+
+        ## Import
+
+        ```sh
+        $ pulumi import okta:policy/deviceAssuranceWindows:DeviceAssuranceWindows example &#60;device assurance id&#62;
+        ```
+
         :param str resource_name: The name of the resource.
         :param DeviceAssuranceWindowsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(DeviceAssuranceWindowsArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/get_default_policy.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/get_default_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/get_policy.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/get_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/mfa.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/outputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/password.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_idp_discovery.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/rule_idp_discovery.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_mfa.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/rule_mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_password.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/rule_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/rule_signon.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/rule_signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy/signon.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy/signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_mfa_default.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy_mfa_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_password_default.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy_password_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_profile_enrollment.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_profile_enrollment_apps.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy_profile_enrollment_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/policy_rule_profile_enrollment.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/policy_rule_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/_inputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/profile/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/mapping.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/profile/mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/profile/outputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/profile/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/provider.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/rate_limiting.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/resource_set.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/resource_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/role_subscription.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/security_notification_emails.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/security_notification_emails.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/template_sms.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/template_sms.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/theme.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/threat_insight_settings.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/threat_insight_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/trustedorigin/origin.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/trustedorigin/origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/_inputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/user/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_user.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/user/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_user_profile_mapping_source.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/user/get_user_profile_mapping_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_user_type.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/user/get_user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/get_users.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/user/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/outputs.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/user/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/user.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/user/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/user/user_type.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/user/user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/user_admin_roles.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/user_admin_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/user_base_schema_property.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/user_factor_question.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/user_factor_question.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/user_group_memberships.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/user_group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta/user_schema_property.py` & `pulumi_okta-4.9.0a1713454215/pulumi_okta/user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/PKG-INFO` & `pulumi_okta-4.9.0a1713454215/pulumi_okta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.9.0a1713447075
+Version: 4.9.0a1713454215
 Summary: A Pulumi package for creating and managing okta resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi,okta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_okta-4.9.0a1713447075/pulumi_okta.egg-info/SOURCES.txt` & `pulumi_okta-4.9.0a1713454215/pulumi_okta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713447075/pyproject.toml` & `pulumi_okta-4.9.0a1713454215/pyproject.toml`

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
-  version = "4.9.0a1713447075"
+  version = "4.9.0a1713454215"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-okta"
 
 [build-system]
```

