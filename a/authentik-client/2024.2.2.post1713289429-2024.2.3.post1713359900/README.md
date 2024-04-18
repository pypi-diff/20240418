# Comparing `tmp/authentik_client-2024.2.2.post1713289429.tar.gz` & `tmp/authentik_client-2024.2.3.post1713359900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authentik_client-2024.2.2.post1713289429.tar", max compression
+gzip compressed data, was "authentik_client-2024.2.3.post1713359900.tar", max compression
```

## Comparing `authentik_client-2024.2.2.post1713289429.tar` & `authentik_client-2024.2.3.post1713359900.tar`

### file list

```diff
@@ -1,594 +1,594 @@
--rw-r--r--   0        0        0   143895 2024-04-16 17:44:03.282151 authentik_client-2024.2.2.post1713289429/README.md
--rw-r--r--   0        0        0    48410 2024-04-16 17:44:03.294151 authentik_client-2024.2.2.post1713289429/authentik_client/__init__.py
--rw-r--r--   0        0        0     1170 2024-04-16 17:44:03.298151 authentik_client-2024.2.2.post1713289429/authentik_client/api/__init__.py
--rw-r--r--   0        0        0    97518 2024-04-16 17:44:02.938151 authentik_client-2024.2.2.post1713289429/authentik_client/api/admin_api.py
--rw-r--r--   0        0        0   700271 2024-04-16 17:44:02.958151 authentik_client-2024.2.2.post1713289429/authentik_client/api/authenticators_api.py
--rw-r--r--   0        0        0   701197 2024-04-16 17:44:02.982151 authentik_client-2024.2.2.post1713289429/authentik_client/api/core_api.py
--rw-r--r--   0        0        0   116805 2024-04-16 17:44:02.994151 authentik_client-2024.2.2.post1713289429/authentik_client/api/crypto_api.py
--rw-r--r--   0        0        0   107946 2024-04-16 17:44:03.002151 authentik_client-2024.2.2.post1713289429/authentik_client/api/enterprise_api.py
--rw-r--r--   0        0        0   408008 2024-04-16 17:44:03.014151 authentik_client-2024.2.2.post1713289429/authentik_client/api/events_api.py
--rw-r--r--   0        0        0   280806 2024-04-16 17:44:03.030151 authentik_client-2024.2.2.post1713289429/authentik_client/api/flows_api.py
--rw-r--r--   0        0        0   101134 2024-04-16 17:44:03.038151 authentik_client-2024.2.2.post1713289429/authentik_client/api/managed_api.py
--rw-r--r--   0        0        0   135649 2024-04-16 17:44:03.046151 authentik_client-2024.2.2.post1713289429/authentik_client/api/oauth2_api.py
--rw-r--r--   0        0        0   413301 2024-04-16 17:44:03.058151 authentik_client-2024.2.2.post1713289429/authentik_client/api/outposts_api.py
--rw-r--r--   0        0        0   725201 2024-04-16 17:44:03.078151 authentik_client-2024.2.2.post1713289429/authentik_client/api/policies_api.py
--rw-r--r--   0        0        0   552586 2024-04-16 17:44:03.102151 authentik_client-2024.2.2.post1713289429/authentik_client/api/propertymappings_api.py
--rw-r--r--   0        0        0   718066 2024-04-16 17:44:03.126151 authentik_client-2024.2.2.post1713289429/authentik_client/api/providers_api.py
--rw-r--r--   0        0        0   150485 2024-04-16 17:44:03.138152 authentik_client-2024.2.2.post1713289429/authentik_client/api/rac_api.py
--rw-r--r--   0        0        0   207550 2024-04-16 17:44:03.150151 authentik_client-2024.2.2.post1713289429/authentik_client/api/rbac_api.py
--rw-r--r--   0        0        0    10391 2024-04-16 17:44:03.166151 authentik_client-2024.2.2.post1713289429/authentik_client/api/root_api.py
--rw-r--r--   0        0        0    11845 2024-04-16 17:44:03.170151 authentik_client-2024.2.2.post1713289429/authentik_client/api/schema_api.py
--rw-r--r--   0        0        0  1037225 2024-04-16 17:44:03.198151 authentik_client-2024.2.2.post1713289429/authentik_client/api/sources_api.py
--rw-r--r--   0        0        0  1945986 2024-04-16 17:44:03.250151 authentik_client-2024.2.2.post1713289429/authentik_client/api/stages_api.py
--rw-r--r--   0        0        0   157909 2024-04-16 17:44:03.270151 authentik_client-2024.2.2.post1713289429/authentik_client/api/tenants_api.py
--rw-r--r--   0        0        0    25779 2024-04-16 17:44:03.298151 authentik_client-2024.2.2.post1713289429/authentik_client/api_client.py
--rw-r--r--   0        0        0      652 2024-04-16 17:44:03.298151 authentik_client-2024.2.2.post1713289429/authentik_client/api_response.py
--rw-r--r--   0        0        0    14724 2024-04-16 17:44:03.294151 authentik_client-2024.2.2.post1713289429/authentik_client/configuration.py
--rw-r--r--   0        0        0     5934 2024-04-16 17:44:03.298151 authentik_client-2024.2.2.post1713289429/authentik_client/exceptions.py
--rw-r--r--   0        0        0    46712 2024-04-16 17:44:03.298151 authentik_client-2024.2.2.post1713289429/authentik_client/models/__init__.py
--rw-r--r--   0        0        0     4513 2024-04-16 17:44:00.006152 authentik_client-2024.2.2.post1713289429/authentik_client/models/access_denied_challenge.py
--rw-r--r--   0        0        0     2482 2024-04-16 17:44:00.022152 authentik_client-2024.2.2.post1713289429/authentik_client/models/app.py
--rw-r--r--   0        0        0     4230 2024-04-16 17:44:00.030152 authentik_client-2024.2.2.post1713289429/authentik_client/models/app_enum.py
--rw-r--r--   0        0        0     2702 2024-04-16 17:44:00.042152 authentik_client-2024.2.2.post1713289429/authentik_client/models/apple_challenge_response_request.py
--rw-r--r--   0        0        0     4508 2024-04-16 17:44:00.050152 authentik_client-2024.2.2.post1713289429/authentik_client/models/apple_login_challenge.py
--rw-r--r--   0        0        0     6686 2024-04-16 17:44:00.062152 authentik_client-2024.2.2.post1713289429/authentik_client/models/application.py
--rw-r--r--   0        0        0     4473 2024-04-16 17:44:00.070152 authentik_client-2024.2.2.post1713289429/authentik_client/models/application_request.py
--rw-r--r--   0        0        0      711 2024-04-16 17:44:00.074152 authentik_client-2024.2.2.post1713289429/authentik_client/models/auth_mode_enum.py
--rw-r--r--   0        0        0      709 2024-04-16 17:44:00.078152 authentik_client-2024.2.2.post1713289429/authentik_client/models/auth_type_enum.py
--rw-r--r--   0        0        0     5195 2024-04-16 17:44:00.082152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session.py
--rw-r--r--   0        0        0     3064 2024-04-16 17:44:00.090152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_asn.py
--rw-r--r--   0        0        0     2826 2024-04-16 17:44:00.094152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_geo_ip.py
--rw-r--r--   0        0        0     3865 2024-04-16 17:44:00.118152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent.py
--rw-r--r--   0        0        0     2646 2024-04-16 17:44:00.122152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent_device.py
--rw-r--r--   0        0        0     2792 2024-04-16 17:44:00.130152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent_os.py
--rw-r--r--   0        0        0     2725 2024-04-16 17:44:00.134152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent_user_agent.py
--rw-r--r--   0        0        0      895 2024-04-16 17:44:00.138152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authentication_enum.py
--rw-r--r--   0        0        0      782 2024-04-16 17:44:00.142152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_attachment_enum.py
--rw-r--r--   0        0        0     4686 2024-04-16 17:44:00.146152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_challenge.py
--rw-r--r--   0        0        0     2743 2024-04-16 17:44:00.154152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_challenge_response_request.py
--rw-r--r--   0        0        0     5327 2024-04-16 17:44:00.158152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage.py
--rw-r--r--   0        0        0     2768 2024-04-16 17:44:00.166152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage_device_import_response.py
--rw-r--r--   0        0        0     2785 2024-04-16 17:44:00.170152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
--rw-r--r--   0        0        0     4744 2024-04-16 17:44:00.178152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-16 17:44:00.182152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_challenge.py
--rw-r--r--   0        0        0     3022 2024-04-16 17:44:00.190152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_challenge_response_request.py
--rw-r--r--   0        0        0     6409 2024-04-16 17:44:00.194152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_stage.py
--rw-r--r--   0        0        0     5595 2024-04-16 17:44:00.202152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4474 2024-04-16 17:44:00.210152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_challenge.py
--rw-r--r--   0        0        0     2761 2024-04-16 17:44:00.214152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_challenge_response_request.py
--rw-r--r--   0        0        0     5363 2024-04-16 17:44:00.222152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_stage.py
--rw-r--r--   0        0        0     4392 2024-04-16 17:44:00.226152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4468 2024-04-16 17:44:00.230152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_challenge.py
--rw-r--r--   0        0        0     2858 2024-04-16 17:44:00.234152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_challenge_response_request.py
--rw-r--r--   0        0        0     5132 2024-04-16 17:44:00.242152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_stage.py
--rw-r--r--   0        0        0     4201 2024-04-16 17:44:00.246152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     6722 2024-04-16 17:44:00.254152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validate_stage.py
--rw-r--r--   0        0        0     4893 2024-04-16 17:44:00.258152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5717 2024-04-16 17:44:00.266152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validation_challenge.py
--rw-r--r--   0        0        0     3805 2024-04-16 17:44:00.270152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validation_challenge_response_request.py
--rw-r--r--   0        0        0     4499 2024-04-16 17:44:00.274152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_challenge.py
--rw-r--r--   0        0        0     2852 2024-04-16 17:44:00.282152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_challenge_response_request.py
--rw-r--r--   0        0        0     7081 2024-04-16 17:44:00.286152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_stage.py
--rw-r--r--   0        0        0     5302 2024-04-16 17:44:00.290152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     2718 2024-04-16 17:44:00.298152 authentik_client-2024.2.2.post1713289429/authentik_client/models/auto_submit_challenge_response_request.py
--rw-r--r--   0        0        0     4388 2024-04-16 17:44:00.302152 authentik_client-2024.2.2.post1713289429/authentik_client/models/autosubmit_challenge.py
--rw-r--r--   0        0        0      950 2024-04-16 17:44:00.306152 authentik_client-2024.2.2.post1713289429/authentik_client/models/backends_enum.py
--rw-r--r--   0        0        0      748 2024-04-16 17:44:00.310152 authentik_client-2024.2.2.post1713289429/authentik_client/models/binding_type_enum.py
--rw-r--r--   0        0        0     2995 2024-04-16 17:44:00.314152 authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_file.py
--rw-r--r--   0        0        0     4453 2024-04-16 17:44:00.318152 authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_instance.py
--rw-r--r--   0        0        0     3208 2024-04-16 17:44:00.322152 authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_instance_request.py
--rw-r--r--   0        0        0      836 2024-04-16 17:44:00.322152 authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_instance_status_enum.py
--rw-r--r--   0        0        0     6255 2024-04-16 17:44:00.326152 authentik_client-2024.2.2.post1713289429/authentik_client/models/brand.py
--rw-r--r--   0        0        0     6307 2024-04-16 17:44:00.330152 authentik_client-2024.2.2.post1713289429/authentik_client/models/brand_request.py
--rw-r--r--   0        0        0     2501 2024-04-16 17:44:00.334152 authentik_client-2024.2.2.post1713289429/authentik_client/models/cache.py
--rw-r--r--   0        0        0      875 2024-04-16 17:44:00.338152 authentik_client-2024.2.2.post1713289429/authentik_client/models/capabilities_enum.py
--rw-r--r--   0        0        0     4476 2024-04-16 17:44:00.342152 authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_challenge.py
--rw-r--r--   0        0        0     2797 2024-04-16 17:44:00.346152 authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_challenge_response_request.py
--rw-r--r--   0        0        0     4438 2024-04-16 17:44:00.350152 authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_stage.py
--rw-r--r--   0        0        0     3774 2024-04-16 17:44:00.354152 authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_stage_request.py
--rw-r--r--   0        0        0     2522 2024-04-16 17:44:00.358152 authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_data.py
--rw-r--r--   0        0        0     2861 2024-04-16 17:44:00.362152 authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_generation_request.py
--rw-r--r--   0        0        0     6655 2024-04-16 17:44:00.366152 authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_key_pair.py
--rw-r--r--   0        0        0     2989 2024-04-16 17:44:00.374152 authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_key_pair_request.py
--rw-r--r--   0        0        0      747 2024-04-16 17:44:00.378152 authentik_client-2024.2.2.post1713289429/authentik_client/models/challenge_choices.py
--rw-r--r--   0        0        0    24236 2024-04-16 17:44:00.386152 authentik_client-2024.2.2.post1713289429/authentik_client/models/challenge_types.py
--rw-r--r--   0        0        0      729 2024-04-16 17:44:00.390152 authentik_client-2024.2.2.post1713289429/authentik_client/models/client_type_enum.py
--rw-r--r--   0        0        0     3539 2024-04-16 17:44:00.394152 authentik_client-2024.2.2.post1713289429/authentik_client/models/config.py
--rw-r--r--   0        0        0     4021 2024-04-16 17:44:00.398152 authentik_client-2024.2.2.post1713289429/authentik_client/models/connection_token.py
--rw-r--r--   0        0        0     2662 2024-04-16 17:44:00.402152 authentik_client-2024.2.2.post1713289429/authentik_client/models/connection_token_request.py
--rw-r--r--   0        0        0     5736 2024-04-16 17:44:00.410152 authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_challenge.py
--rw-r--r--   0        0        0     2838 2024-04-16 17:44:00.414152 authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_challenge_response_request.py
--rw-r--r--   0        0        0     2513 2024-04-16 17:44:00.418152 authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_permission.py
--rw-r--r--   0        0        0     4511 2024-04-16 17:44:00.422152 authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_stage.py
--rw-r--r--   0        0        0      783 2024-04-16 17:44:00.426152 authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_stage_mode_enum.py
--rw-r--r--   0        0        0     3569 2024-04-16 17:44:00.430152 authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_stage_request.py
--rw-r--r--   0        0        0     2891 2024-04-16 17:44:00.434152 authentik_client-2024.2.2.post1713289429/authentik_client/models/contextual_flow_info.py
--rw-r--r--   0        0        0      879 2024-04-16 17:44:00.438152 authentik_client-2024.2.2.post1713289429/authentik_client/models/contextual_flow_info_layout_enum.py
--rw-r--r--   0        0        0     2657 2024-04-16 17:44:00.442152 authentik_client-2024.2.2.post1713289429/authentik_client/models/coordinate.py
--rw-r--r--   0        0        0     4704 2024-04-16 17:44:00.446152 authentik_client-2024.2.2.post1713289429/authentik_client/models/current_brand.py
--rw-r--r--   0        0        0      771 2024-04-16 17:44:00.450152 authentik_client-2024.2.2.post1713289429/authentik_client/models/denied_action_enum.py
--rw-r--r--   0        0        0     4200 2024-04-16 17:44:00.454152 authentik_client-2024.2.2.post1713289429/authentik_client/models/deny_stage.py
--rw-r--r--   0        0        0     3230 2024-04-16 17:44:00.458152 authentik_client-2024.2.2.post1713289429/authentik_client/models/deny_stage_request.py
--rw-r--r--   0        0        0     3522 2024-04-16 17:44:00.462152 authentik_client-2024.2.2.post1713289429/authentik_client/models/device.py
--rw-r--r--   0        0        0     2657 2024-04-16 17:44:00.470152 authentik_client-2024.2.2.post1713289429/authentik_client/models/device_challenge.py
--rw-r--r--   0        0        0     2792 2024-04-16 17:44:00.474152 authentik_client-2024.2.2.post1713289429/authentik_client/models/device_challenge_request.py
--rw-r--r--   0        0        0      780 2024-04-16 17:44:00.478152 authentik_client-2024.2.2.post1713289429/authentik_client/models/device_classes_enum.py
--rw-r--r--   0        0        0     1244 2024-04-16 17:44:00.482152 authentik_client-2024.2.2.post1713289429/authentik_client/models/digest_algorithm_enum.py
--rw-r--r--   0        0        0      695 2024-04-16 17:44:00.482152 authentik_client-2024.2.2.post1713289429/authentik_client/models/digits_enum.py
--rw-r--r--   0        0        0     4969 2024-04-16 17:44:00.486152 authentik_client-2024.2.2.post1713289429/authentik_client/models/docker_service_connection.py
--rw-r--r--   0        0        0     4087 2024-04-16 17:44:00.490152 authentik_client-2024.2.2.post1713289429/authentik_client/models/docker_service_connection_request.py
--rw-r--r--   0        0        0     2847 2024-04-16 17:44:00.494152 authentik_client-2024.2.2.post1713289429/authentik_client/models/domain.py
--rw-r--r--   0        0        0     2746 2024-04-16 17:44:00.498152 authentik_client-2024.2.2.post1713289429/authentik_client/models/domain_request.py
--rw-r--r--   0        0        0     4155 2024-04-16 17:44:00.506152 authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_challenge.py
--rw-r--r--   0        0        0     2681 2024-04-16 17:44:00.510152 authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_challenge_response_request.py
--rw-r--r--   0        0        0     4515 2024-04-16 17:44:00.514152 authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_policy.py
--rw-r--r--   0        0        0     3237 2024-04-16 17:44:00.518152 authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_policy_request.py
--rw-r--r--   0        0        0     4213 2024-04-16 17:44:00.522152 authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_stage.py
--rw-r--r--   0        0        0     3232 2024-04-16 17:44:00.526152 authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_stage_request.py
--rw-r--r--   0        0        0     2720 2024-04-16 17:44:00.530152 authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_device.py
--rw-r--r--   0        0        0     2575 2024-04-16 17:44:00.534152 authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_device_enrollment_status.py
--rw-r--r--   0        0        0     2619 2024-04-16 17:44:00.538152 authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_device_request.py
--rw-r--r--   0        0        0      748 2024-04-16 17:44:00.542152 authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_response_enum.py
--rw-r--r--   0        0        0     4090 2024-04-16 17:44:00.546152 authentik_client-2024.2.2.post1713289429/authentik_client/models/email_challenge.py
--rw-r--r--   0        0        0     2770 2024-04-16 17:44:00.554152 authentik_client-2024.2.2.post1713289429/authentik_client/models/email_challenge_response_request.py
--rw-r--r--   0        0        0     5902 2024-04-16 17:44:00.558152 authentik_client-2024.2.2.post1713289429/authentik_client/models/email_stage.py
--rw-r--r--   0        0        0     5121 2024-04-16 17:44:00.562152 authentik_client-2024.2.2.post1713289429/authentik_client/models/email_stage_request.py
--rw-r--r--   0        0        0     4707 2024-04-16 17:44:00.566152 authentik_client-2024.2.2.post1713289429/authentik_client/models/endpoint.py
--rw-r--r--   0        0        0     3678 2024-04-16 17:44:00.574152 authentik_client-2024.2.2.post1713289429/authentik_client/models/endpoint_request.py
--rw-r--r--   0        0        0     2530 2024-04-16 17:44:00.578152 authentik_client-2024.2.2.post1713289429/authentik_client/models/error_detail.py
--rw-r--r--   0        0        0     3309 2024-04-16 17:44:00.582152 authentik_client-2024.2.2.post1713289429/authentik_client/models/error_reporting_config.py
--rw-r--r--   0        0        0     4129 2024-04-16 17:44:00.586152 authentik_client-2024.2.2.post1713289429/authentik_client/models/event.py
--rw-r--r--   0        0        0     1730 2024-04-16 17:44:00.590152 authentik_client-2024.2.2.post1713289429/authentik_client/models/event_actions.py
--rw-r--r--   0        0        0     6006 2024-04-16 17:44:00.594152 authentik_client-2024.2.2.post1713289429/authentik_client/models/event_matcher_policy.py
--rw-r--r--   0        0        0     4807 2024-04-16 17:44:00.598152 authentik_client-2024.2.2.post1713289429/authentik_client/models/event_matcher_policy_request.py
--rw-r--r--   0        0        0     3990 2024-04-16 17:44:00.602152 authentik_client-2024.2.2.post1713289429/authentik_client/models/event_request.py
--rw-r--r--   0        0        0     2697 2024-04-16 17:44:00.606152 authentik_client-2024.2.2.post1713289429/authentik_client/models/event_top_per_user.py
--rw-r--r--   0        0        0     3926 2024-04-16 17:44:00.610152 authentik_client-2024.2.2.post1713289429/authentik_client/models/expiring_base_grant_model.py
--rw-r--r--   0        0        0     4191 2024-04-16 17:44:00.614152 authentik_client-2024.2.2.post1713289429/authentik_client/models/expression_policy.py
--rw-r--r--   0        0        0     2992 2024-04-16 17:44:00.618152 authentik_client-2024.2.2.post1713289429/authentik_client/models/expression_policy_request.py
--rw-r--r--   0        0        0     4524 2024-04-16 17:44:00.622152 authentik_client-2024.2.2.post1713289429/authentik_client/models/extra_role_object_permission.py
--rw-r--r--   0        0        0     4524 2024-04-16 17:44:00.626152 authentik_client-2024.2.2.post1713289429/authentik_client/models/extra_user_object_permission.py
--rw-r--r--   0        0        0     2519 2024-04-16 17:44:00.630152 authentik_client-2024.2.2.post1713289429/authentik_client/models/file_path_request.py
--rw-r--r--   0        0        0     6047 2024-04-16 17:44:00.638152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow.py
--rw-r--r--   0        0        0    25850 2024-04-16 17:44:00.646152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_challenge_response_request.py
--rw-r--r--   0        0        0      934 2024-04-16 17:44:00.650152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_designation_enum.py
--rw-r--r--   0        0        0     2533 2024-04-16 17:44:00.654152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_diagram.py
--rw-r--r--   0        0        0     4505 2024-04-16 17:44:00.662152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_error_challenge.py
--rw-r--r--   0        0        0     3111 2024-04-16 17:44:00.670152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_import_result.py
--rw-r--r--   0        0        0     3418 2024-04-16 17:44:00.678152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_inspection.py
--rw-r--r--   0        0        0     3875 2024-04-16 17:44:00.686152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_inspector_plan.py
--rw-r--r--   0        0        0      837 2024-04-16 17:44:00.686152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_layout_enum.py
--rw-r--r--   0        0        0     4741 2024-04-16 17:44:00.694152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_request.py
--rw-r--r--   0        0        0     5223 2024-04-16 17:44:00.702152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_set.py
--rw-r--r--   0        0        0     4459 2024-04-16 17:44:00.710152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_set_request.py
--rw-r--r--   0        0        0     4763 2024-04-16 17:44:00.718152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_stage_binding.py
--rw-r--r--   0        0        0     3983 2024-04-16 17:44:00.722152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_stage_binding_request.py
--rw-r--r--   0        0        0     2641 2024-04-16 17:44:00.730152 authentik_client-2024.2.2.post1713289429/authentik_client/models/footer_link.py
--rw-r--r--   0        0        0     2531 2024-04-16 17:44:00.734152 authentik_client-2024.2.2.post1713289429/authentik_client/models/generic_error.py
--rw-r--r--   0        0        0      865 2024-04-16 17:44:00.738152 authentik_client-2024.2.2.post1713289429/authentik_client/models/geoip_binding_enum.py
--rw-r--r--   0        0        0     5445 2024-04-16 17:44:00.746152 authentik_client-2024.2.2.post1713289429/authentik_client/models/group.py
--rw-r--r--   0        0        0     4209 2024-04-16 17:44:00.750152 authentik_client-2024.2.2.post1713289429/authentik_client/models/group_member.py
--rw-r--r--   0        0        0     4006 2024-04-16 17:44:00.758152 authentik_client-2024.2.2.post1713289429/authentik_client/models/group_member_request.py
--rw-r--r--   0        0        0     3347 2024-04-16 17:44:00.766152 authentik_client-2024.2.2.post1713289429/authentik_client/models/group_request.py
--rw-r--r--   0        0        0     6080 2024-04-16 17:44:00.770152 authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_challenge.py
--rw-r--r--   0        0        0     3174 2024-04-16 17:44:00.778152 authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_challenge_response_request.py
--rw-r--r--   0        0        0     7503 2024-04-16 17:44:00.786152 authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_stage.py
--rw-r--r--   0        0        0     6533 2024-04-16 17:44:00.794152 authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_stage_request.py
--rw-r--r--   0        0        0     2438 2024-04-16 17:44:00.798152 authentik_client-2024.2.2.post1713289429/authentik_client/models/install_id.py
--rw-r--r--   0        0        0      771 2024-04-16 17:44:00.802152 authentik_client-2024.2.2.post1713289429/authentik_client/models/intent_enum.py
--rw-r--r--   0        0        0      800 2024-04-16 17:44:00.802152 authentik_client-2024.2.2.post1713289429/authentik_client/models/invalid_response_action_enum.py
--rw-r--r--   0        0        0     4878 2024-04-16 17:44:00.810152 authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation.py
--rw-r--r--   0        0        0     3895 2024-04-16 17:44:00.818152 authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation_request.py
--rw-r--r--   0        0        0     4508 2024-04-16 17:44:00.826152 authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation_stage.py
--rw-r--r--   0        0        0     3527 2024-04-16 17:44:00.834152 authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation_stage_request.py
--rw-r--r--   0        0        0      729 2024-04-16 17:44:00.838152 authentik_client-2024.2.2.post1713289429/authentik_client/models/issuer_mode_enum.py
--rw-r--r--   0        0        0     4386 2024-04-16 17:44:00.842152 authentik_client-2024.2.2.post1713289429/authentik_client/models/kubernetes_service_connection.py
--rw-r--r--   0        0        0     3454 2024-04-16 17:44:00.846152 authentik_client-2024.2.2.post1713289429/authentik_client/models/kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     2811 2024-04-16 17:44:00.858152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_debug.py
--rw-r--r--   0        0        0     5765 2024-04-16 17:44:00.862152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_outpost_config.py
--rw-r--r--   0        0        0     4378 2024-04-16 17:44:00.866152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_property_mapping.py
--rw-r--r--   0        0        0     3478 2024-04-16 17:44:00.874152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_property_mapping_request.py
--rw-r--r--   0        0        0     8694 2024-04-16 17:44:00.878152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_provider.py
--rw-r--r--   0        0        0     6192 2024-04-16 17:44:00.882152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_provider_request.py
--rw-r--r--   0        0        0    11791 2024-04-16 17:44:00.890152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_source.py
--rw-r--r--   0        0        0     9542 2024-04-16 17:44:00.898152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_source_request.py
--rw-r--r--   0        0        0     3129 2024-04-16 17:44:00.902152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_sync_status.py
--rw-r--r--   0        0        0      726 2024-04-16 17:44:00.850152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldapapi_access_mode.py
--rw-r--r--   0        0        0     3278 2024-04-16 17:44:00.910152 authentik_client-2024.2.2.post1713289429/authentik_client/models/license.py
--rw-r--r--   0        0        0     2897 2024-04-16 17:44:00.914152 authentik_client-2024.2.2.post1713289429/authentik_client/models/license_forecast.py
--rw-r--r--   0        0        0     2509 2024-04-16 17:44:00.922152 authentik_client-2024.2.2.post1713289429/authentik_client/models/license_request.py
--rw-r--r--   0        0        0     3222 2024-04-16 17:44:00.926152 authentik_client-2024.2.2.post1713289429/authentik_client/models/license_summary.py
--rw-r--r--   0        0        0     2411 2024-04-16 17:44:00.930152 authentik_client-2024.2.2.post1713289429/authentik_client/models/link.py
--rw-r--r--   0        0        0     2882 2024-04-16 17:44:00.934152 authentik_client-2024.2.2.post1713289429/authentik_client/models/log_event.py
--rw-r--r--   0        0        0      843 2024-04-16 17:44:00.934152 authentik_client-2024.2.2.post1713289429/authentik_client/models/log_level_enum.py
--rw-r--r--   0        0        0     6520 2024-04-16 17:44:00.938152 authentik_client-2024.2.2.post1713289429/authentik_client/models/login_challenge_types.py
--rw-r--r--   0        0        0     4171 2024-04-16 17:44:00.942152 authentik_client-2024.2.2.post1713289429/authentik_client/models/login_metrics.py
--rw-r--r--   0        0        0     3192 2024-04-16 17:44:00.942152 authentik_client-2024.2.2.post1713289429/authentik_client/models/login_source.py
--rw-r--r--   0        0        0     2513 2024-04-16 17:44:00.946152 authentik_client-2024.2.2.post1713289429/authentik_client/models/metadata.py
--rw-r--r--   0        0        0     7604 2024-04-16 17:44:00.950152 authentik_client-2024.2.2.post1713289429/authentik_client/models/model_enum.py
--rw-r--r--   0        0        0     9828 2024-04-16 17:44:00.954152 authentik_client-2024.2.2.post1713289429/authentik_client/models/model_request.py
--rw-r--r--   0        0        0     1559 2024-04-16 17:44:00.954152 authentik_client-2024.2.2.post1713289429/authentik_client/models/name_id_policy_enum.py
--rw-r--r--   0        0        0      831 2024-04-16 17:44:00.958152 authentik_client-2024.2.2.post1713289429/authentik_client/models/network_binding_enum.py
--rw-r--r--   0        0        0      764 2024-04-16 17:44:00.958152 authentik_client-2024.2.2.post1713289429/authentik_client/models/not_configured_action_enum.py
--rw-r--r--   0        0        0     3479 2024-04-16 17:44:00.962152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification.py
--rw-r--r--   0        0        0     2858 2024-04-16 17:44:00.966152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_request.py
--rw-r--r--   0        0        0     4010 2024-04-16 17:44:00.966152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_rule.py
--rw-r--r--   0        0        0     3549 2024-04-16 17:44:00.970152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_rule_request.py
--rw-r--r--   0        0        0     3760 2024-04-16 17:44:00.974152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport.py
--rw-r--r--   0        0        0      818 2024-04-16 17:44:00.974152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport_mode_enum.py
--rw-r--r--   0        0        0     3500 2024-04-16 17:44:00.978152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport_request.py
--rw-r--r--   0        0        0     2503 2024-04-16 17:44:00.982152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport_test.py
--rw-r--r--   0        0        0     2707 2024-04-16 17:44:00.986152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_webhook_mapping.py
--rw-r--r--   0        0        0     2717 2024-04-16 17:44:00.990152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     8888 2024-04-16 17:44:00.994152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth2_provider.py
--rw-r--r--   0        0        0     6654 2024-04-16 17:44:00.998152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth2_provider_request.py
--rw-r--r--   0        0        0     3482 2024-04-16 17:44:01.002152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth2_provider_setup_urls.py
--rw-r--r--   0        0        0     4164 2024-04-16 17:44:01.006152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_challenge.py
--rw-r--r--   0        0        0     2846 2024-04-16 17:44:01.010152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_challenge_response_request.py
--rw-r--r--   0        0        0     4213 2024-04-16 17:44:01.014152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_finish_challenge.py
--rw-r--r--   0        0        0     2816 2024-04-16 17:44:01.018152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
--rw-r--r--   0        0        0    10563 2024-04-16 17:44:01.022152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_source.py
--rw-r--r--   0        0        0     8013 2024-04-16 17:44:01.026152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_source_request.py
--rw-r--r--   0        0        0     3922 2024-04-16 17:44:01.030152 authentik_client-2024.2.2.post1713289429/authentik_client/models/open_id_connect_configuration.py
--rw-r--r--   0        0        0     5545 2024-04-16 17:44:01.034152 authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost.py
--rw-r--r--   0        0        0     2541 2024-04-16 17:44:01.038152 authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_default_config.py
--rw-r--r--   0        0        0     3755 2024-04-16 17:44:01.042152 authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_health.py
--rw-r--r--   0        0        0     4050 2024-04-16 17:44:01.042152 authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_request.py
--rw-r--r--   0        0        0      752 2024-04-16 17:44:01.046152 authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_type_enum.py
--rw-r--r--   0        0        0     3322 2024-04-16 17:44:01.050152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_application_list.py
--rw-r--r--   0        0        0     3395 2024-04-16 17:44:01.050152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticated_session_list.py
--rw-r--r--   0        0        0     3404 2024-04-16 17:44:01.054152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_duo_stage_list.py
--rw-r--r--   0        0        0     3404 2024-04-16 17:44:01.058152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_sms_stage_list.py
--rw-r--r--   0        0        0     3428 2024-04-16 17:44:01.062152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_static_stage_list.py
--rw-r--r--   0        0        0     3412 2024-04-16 17:44:01.066152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_totp_stage_list.py
--rw-r--r--   0        0        0     3444 2024-04-16 17:44:01.070152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_validate_stage_list.py
--rw-r--r--   0        0        0     3445 2024-04-16 17:44:01.070152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
--rw-r--r--   0        0        0     3371 2024-04-16 17:44:01.074152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_blueprint_instance_list.py
--rw-r--r--   0        0        0     3274 2024-04-16 17:44:01.078152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_brand_list.py
--rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.082152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_captcha_stage_list.py
--rw-r--r--   0        0        0     3380 2024-04-16 17:44:01.082152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_certificate_key_pair_list.py
--rw-r--r--   0        0        0     3355 2024-04-16 17:44:01.086152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_connection_token_list.py
--rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.090152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_consent_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-16 17:44:01.094152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_deny_stage_list.py
--rw-r--r--   0        0        0     3420 2024-04-16 17:44:01.094152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_docker_service_connection_list.py
--rw-r--r--   0        0        0     3282 2024-04-16 17:44:01.098152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_domain_list.py
--rw-r--r--   0        0        0     3323 2024-04-16 17:44:01.102152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_dummy_policy_list.py
--rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.102152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_dummy_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-16 17:44:01.106152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_duo_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.110152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_email_stage_list.py
--rw-r--r--   0        0        0     3298 2024-04-16 17:44:01.114152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_endpoint_list.py
--rw-r--r--   0        0        0     3274 2024-04-16 17:44:01.114152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_event_list.py
--rw-r--r--   0        0        0     3380 2024-04-16 17:44:01.118152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_event_matcher_policy_list.py
--rw-r--r--   0        0        0     3413 2024-04-16 17:44:01.122152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_expiring_base_grant_model_list.py
--rw-r--r--   0        0        0     3363 2024-04-16 17:44:01.126152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_expression_policy_list.py
--rw-r--r--   0        0        0     3437 2024-04-16 17:44:01.126152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_extra_role_object_permission_list.py
--rw-r--r--   0        0        0     3437 2024-04-16 17:44:01.130152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_extra_user_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-16 17:44:01.134152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_flow_list.py
--rw-r--r--   0        0        0     3364 2024-04-16 17:44:01.138152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_flow_stage_binding_list.py
--rw-r--r--   0        0        0     3274 2024-04-16 17:44:01.138152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_group_list.py
--rw-r--r--   0        0        0     3387 2024-04-16 17:44:01.142152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_identification_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-16 17:44:01.146152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_invitation_list.py
--rw-r--r--   0        0        0     3355 2024-04-16 17:44:01.150152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_invitation_stage_list.py
--rw-r--r--   0        0        0     3452 2024-04-16 17:44:01.154152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_kubernetes_service_connection_list.py
--rw-r--r--   0        0        0     3372 2024-04-16 17:44:01.154152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_outpost_config_list.py
--rw-r--r--   0        0        0     3388 2024-04-16 17:44:01.158152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.162152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.166152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-16 17:44:01.170152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_license_list.py
--rw-r--r--   0        0        0     3330 2024-04-16 17:44:01.170152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_list.py
--rw-r--r--   0        0        0     3363 2024-04-16 17:44:01.174152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_rule_list.py
--rw-r--r--   0        0        0     3403 2024-04-16 17:44:01.178152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_transport_list.py
--rw-r--r--   0        0        0     3444 2024-04-16 17:44:01.182152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_webhook_mapping_list.py
--rw-r--r--   0        0        0     3348 2024-04-16 17:44:01.182152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_o_auth2_provider_list.py
--rw-r--r--   0        0        0     3324 2024-04-16 17:44:01.186152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_o_auth_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-16 17:44:01.190152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_outpost_list.py
--rw-r--r--   0        0        0     3396 2024-04-16 17:44:01.194152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_password_expiry_policy_list.py
--rw-r--r--   0        0        0     3347 2024-04-16 17:44:01.198152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_password_policy_list.py
--rw-r--r--   0        0        0     3339 2024-04-16 17:44:01.202152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_password_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-16 17:44:01.206152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_permission_list.py
--rw-r--r--   0        0        0     3396 2024-04-16 17:44:01.214152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_plex_source_connection_list.py
--rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.218152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_plex_source_list.py
--rw-r--r--   0        0        0     3339 2024-04-16 17:44:01.222152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_policy_binding_list.py
--rw-r--r--   0        0        0     3282 2024-04-16 17:44:01.226152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_policy_list.py
--rw-r--r--   0        0        0     3282 2024-04-16 17:44:01.230152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_prompt_list.py
--rw-r--r--   0        0        0     3323 2024-04-16 17:44:01.234152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_prompt_stage_list.py
--rw-r--r--   0        0        0     3355 2024-04-16 17:44:01.238152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_property_mapping_list.py
--rw-r--r--   0        0        0     3298 2024-04-16 17:44:01.238152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-16 17:44:01.242152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_proxy_outpost_config_list.py
--rw-r--r--   0        0        0     3339 2024-04-16 17:44:01.246152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_proxy_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-16 17:44:01.250152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_rac_property_mapping_list.py
--rw-r--r--   0        0        0     3323 2024-04-16 17:44:01.254152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_rac_provider_list.py
--rw-r--r--   0        0        0     3388 2024-04-16 17:44:01.254152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_radius_outpost_config_list.py
--rw-r--r--   0        0        0     3347 2024-04-16 17:44:01.258152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_radius_provider_list.py
--rw-r--r--   0        0        0     3314 2024-04-16 17:44:01.262152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_reputation_list.py
--rw-r--r--   0        0        0     3363 2024-04-16 17:44:01.266152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_reputation_policy_list.py
--rw-r--r--   0        0        0     3461 2024-04-16 17:44:01.266152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_role_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-16 17:44:01.270152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_role_list.py
--rw-r--r--   0        0        0     3388 2024-04-16 17:44:01.274152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_saml_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.278152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_saml_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.282152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_saml_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-16 17:44:01.286152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.286152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_provider_list.py
--rw-r--r--   0        0        0     3356 2024-04-16 17:44:01.290152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_source_group_list.py
--rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.294152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_source_list.py
--rw-r--r--   0        0        0     3348 2024-04-16 17:44:01.298152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_source_user_list.py
--rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.306152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scope_mapping_list.py
--rw-r--r--   0        0        0     3371 2024-04-16 17:44:01.310152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_service_connection_list.py
--rw-r--r--   0        0        0     3307 2024-04-16 17:44:01.302152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_sms_device_list.py
--rw-r--r--   0        0        0     3282 2024-04-16 17:44:01.314152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-16 17:44:01.318152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_source_stage_list.py
--rw-r--r--   0        0        0     3274 2024-04-16 17:44:01.322152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_stage_list.py
--rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.322152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_static_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.326152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_system_task_list.py
--rw-r--r--   0        0        0     3282 2024-04-16 17:44:01.334152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_tenant_list.py
--rw-r--r--   0        0        0     3274 2024-04-16 17:44:01.338152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_token_list.py
--rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.342152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_token_model_list.py
--rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.330152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_totp_device_list.py
--rw-r--r--   0        0        0     3461 2024-04-16 17:44:01.342152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3323 2024-04-16 17:44:01.346152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_consent_list.py
--rw-r--r--   0        0        0     3356 2024-04-16 17:44:01.350152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_delete_stage_list.py
--rw-r--r--   0        0        0     3266 2024-04-16 17:44:01.354152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_list.py
--rw-r--r--   0        0        0     3348 2024-04-16 17:44:01.358152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_login_stage_list.py
--rw-r--r--   0        0        0     3356 2024-04-16 17:44:01.362152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_logout_stage_list.py
--rw-r--r--   0        0        0     3438 2024-04-16 17:44:01.366152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_o_auth_source_connection_list.py
--rw-r--r--   0        0        0     3429 2024-04-16 17:44:01.370152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_saml_source_connection_list.py
--rw-r--r--   0        0        0     3396 2024-04-16 17:44:01.370152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_source_connection_list.py
--rw-r--r--   0        0        0     3348 2024-04-16 17:44:01.374152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_write_stage_list.py
--rw-r--r--   0        0        0     3348 2024-04-16 17:44:01.378152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_web_authn_device_list.py
--rw-r--r--   0        0        0     3381 2024-04-16 17:44:01.382152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_web_authn_device_type_list.py
--rw-r--r--   0        0        0     3076 2024-04-16 17:44:01.386152 authentik_client-2024.2.2.post1713289429/authentik_client/models/pagination.py
--rw-r--r--   0        0        0     4454 2024-04-16 17:44:01.390152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_challenge.py
--rw-r--r--   0        0        0     2819 2024-04-16 17:44:01.390152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_challenge_response_request.py
--rw-r--r--   0        0        0     4377 2024-04-16 17:44:01.394152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_expiry_policy.py
--rw-r--r--   0        0        0     3099 2024-04-16 17:44:01.398152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_expiry_policy_request.py
--rw-r--r--   0        0        0     6428 2024-04-16 17:44:01.398152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_policy.py
--rw-r--r--   0        0        0     5239 2024-04-16 17:44:01.402152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_policy_request.py
--rw-r--r--   0        0        0     5274 2024-04-16 17:44:01.402152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_stage.py
--rw-r--r--   0        0        0     4264 2024-04-16 17:44:01.406152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-16 17:44:01.410152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_application_request.py
--rw-r--r--   0        0        0     4833 2024-04-16 17:44:01.414152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     5701 2024-04-16 17:44:01.414152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4430 2024-04-16 17:44:01.418152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4256 2024-04-16 17:44:01.422152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     4931 2024-04-16 17:44:01.422152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5340 2024-04-16 17:44:01.426152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     3246 2024-04-16 17:44:01.430152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_blueprint_instance_request.py
--rw-r--r--   0        0        0     6352 2024-04-16 17:44:01.430152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_brand_request.py
--rw-r--r--   0        0        0     3860 2024-04-16 17:44:01.434152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_captcha_stage_request.py
--rw-r--r--   0        0        0     3051 2024-04-16 17:44:01.434152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_certificate_key_pair_request.py
--rw-r--r--   0        0        0     2717 2024-04-16 17:44:01.438152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_connection_token_request.py
--rw-r--r--   0        0        0     3607 2024-04-16 17:44:01.438152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_consent_stage_request.py
--rw-r--r--   0        0        0     3268 2024-04-16 17:44:01.442152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_deny_stage_request.py
--rw-r--r--   0        0        0     4149 2024-04-16 17:44:01.446152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_docker_service_connection_request.py
--rw-r--r--   0        0        0     2801 2024-04-16 17:44:01.446152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_domain_request.py
--rw-r--r--   0        0        0     3275 2024-04-16 17:44:01.450152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_dummy_policy_request.py
--rw-r--r--   0        0        0     3270 2024-04-16 17:44:01.454152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_dummy_stage_request.py
--rw-r--r--   0        0        0     2674 2024-04-16 17:44:01.454152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_duo_device_request.py
--rw-r--r--   0        0        0     5159 2024-04-16 17:44:01.458152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_email_stage_request.py
--rw-r--r--   0        0        0     3784 2024-04-16 17:44:01.462152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_endpoint_request.py
--rw-r--r--   0        0        0     4845 2024-04-16 17:44:01.466152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_event_matcher_policy_request.py
--rw-r--r--   0        0        0     4045 2024-04-16 17:44:01.474152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_event_request.py
--rw-r--r--   0        0        0     3047 2024-04-16 17:44:01.478152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_expression_policy_request.py
--rw-r--r--   0        0        0     4903 2024-04-16 17:44:01.482152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_flow_request.py
--rw-r--r--   0        0        0     4055 2024-04-16 17:44:01.486152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_flow_stage_binding_request.py
--rw-r--r--   0        0        0     3385 2024-04-16 17:44:01.486152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_group_request.py
--rw-r--r--   0        0        0     6571 2024-04-16 17:44:01.490152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_identification_stage_request.py
--rw-r--r--   0        0        0     3985 2024-04-16 17:44:01.494152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_invitation_request.py
--rw-r--r--   0        0        0     3565 2024-04-16 17:44:01.498152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_invitation_stage_request.py
--rw-r--r--   0        0        0     3492 2024-04-16 17:44:01.502152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     3550 2024-04-16 17:44:01.502152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_ldap_property_mapping_request.py
--rw-r--r--   0        0        0     6254 2024-04-16 17:44:01.506152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_ldap_provider_request.py
--rw-r--r--   0        0        0     9697 2024-04-16 17:44:01.510152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_ldap_source_request.py
--rw-r--r--   0        0        0     2557 2024-04-16 17:44:01.514152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_license_request.py
--rw-r--r--   0        0        0     2879 2024-04-16 17:44:01.514152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_request.py
--rw-r--r--   0        0        0     3587 2024-04-16 17:44:01.518152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_rule_request.py
--rw-r--r--   0        0        0     3538 2024-04-16 17:44:01.522152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_transport_request.py
--rw-r--r--   0        0        0     2782 2024-04-16 17:44:01.526152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     6716 2024-04-16 17:44:01.530152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_o_auth2_provider_request.py
--rw-r--r--   0        0        0     8185 2024-04-16 17:44:01.534152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_o_auth_source_request.py
--rw-r--r--   0        0        0     4139 2024-04-16 17:44:01.534152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_outpost_request.py
--rw-r--r--   0        0        0     3154 2024-04-16 17:44:01.538152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_password_expiry_policy_request.py
--rw-r--r--   0        0        0     5277 2024-04-16 17:44:01.542152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_password_policy_request.py
--rw-r--r--   0        0        0     4326 2024-04-16 17:44:01.546152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_password_stage_request.py
--rw-r--r--   0        0        0     2922 2024-04-16 17:44:01.550152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_permission_assign_request.py
--rw-r--r--   0        0        0     2784 2024-04-16 17:44:01.550152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_plex_source_connection_request.py
--rw-r--r--   0        0        0     5905 2024-04-16 17:44:01.554152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_plex_source_request.py
--rw-r--r--   0        0        0     4286 2024-04-16 17:44:01.558152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_policy_binding_request.py
--rw-r--r--   0        0        0     5023 2024-04-16 17:44:01.562152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_prompt_request.py
--rw-r--r--   0        0        0     3406 2024-04-16 17:44:01.566152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_prompt_stage_request.py
--rw-r--r--   0        0        0     6907 2024-04-16 17:44:01.570152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_proxy_provider_request.py
--rw-r--r--   0        0        0     3495 2024-04-16 17:44:01.570152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_rac_property_mapping_request.py
--rw-r--r--   0        0        0     4413 2024-04-16 17:44:01.574152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_rac_provider_request.py
--rw-r--r--   0        0        0     4563 2024-04-16 17:44:01.578152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_radius_provider_request.py
--rw-r--r--   0        0        0     3276 2024-04-16 17:44:01.582152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_reputation_policy_request.py
--rw-r--r--   0        0        0     2565 2024-04-16 17:44:01.582152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_role_request.py
--rw-r--r--   0        0        0     3901 2024-04-16 17:44:01.586152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_saml_property_mapping_request.py
--rw-r--r--   0        0        0     7539 2024-04-16 17:44:01.590152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_saml_provider_request.py
--rw-r--r--   0        0        0     8676 2024-04-16 17:44:01.590152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_saml_source_request.py
--rw-r--r--   0        0        0     3364 2024-04-16 17:44:01.594152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_mapping_request.py
--rw-r--r--   0        0        0     3888 2024-04-16 17:44:01.594152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_provider_request.py
--rw-r--r--   0        0        0     3095 2024-04-16 17:44:01.598152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_source_group_request.py
--rw-r--r--   0        0        0     3829 2024-04-16 17:44:01.602152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_source_request.py
--rw-r--r--   0        0        0     3098 2024-04-16 17:44:01.602152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_source_user_request.py
--rw-r--r--   0        0        0     3819 2024-04-16 17:44:01.610152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scope_mapping_request.py
--rw-r--r--   0        0        0     5079 2024-04-16 17:44:01.610152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_settings_request.py
--rw-r--r--   0        0        0     2674 2024-04-16 17:44:01.606152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_sms_device_request.py
--rw-r--r--   0        0        0     3562 2024-04-16 17:44:01.614152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_source_stage_request.py
--rw-r--r--   0        0        0     2686 2024-04-16 17:44:01.614152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_static_device_request.py
--rw-r--r--   0        0        0     2820 2024-04-16 17:44:01.618152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_tenant_request.py
--rw-r--r--   0        0        0     4419 2024-04-16 17:44:01.622152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_token_request.py
--rw-r--r--   0        0        0     2678 2024-04-16 17:44:01.618152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_totp_device_request.py
--rw-r--r--   0        0        0     3167 2024-04-16 17:44:01.626152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_delete_stage_request.py
--rw-r--r--   0        0        0     4766 2024-04-16 17:44:01.626152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_login_stage_request.py
--rw-r--r--   0        0        0     3167 2024-04-16 17:44:01.630152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_logout_stage_request.py
--rw-r--r--   0        0        0     3109 2024-04-16 17:44:01.630152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3934 2024-04-16 17:44:01.634152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_request.py
--rw-r--r--   0        0        0     2733 2024-04-16 17:44:01.634152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_saml_source_connection_request.py
--rw-r--r--   0        0        0     4450 2024-04-16 17:44:01.638152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_write_stage_request.py
--rw-r--r--   0        0        0     2625 2024-04-16 17:44:01.642152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_web_authn_device_request.py
--rw-r--r--   0        0        0     3548 2024-04-16 17:44:01.642152 authentik_client-2024.2.2.post1713289429/authentik_client/models/permission.py
--rw-r--r--   0        0        0     2884 2024-04-16 17:44:01.646152 authentik_client-2024.2.2.post1713289429/authentik_client/models/permission_assign_request.py
--rw-r--r--   0        0        0     4315 2024-04-16 17:44:01.646152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_authentication_challenge.py
--rw-r--r--   0        0        0     2726 2024-04-16 17:44:01.650152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_authentication_challenge_response_request.py
--rw-r--r--   0        0        0     7752 2024-04-16 17:44:01.654152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source.py
--rw-r--r--   0        0        0     3265 2024-04-16 17:44:01.654152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source_connection.py
--rw-r--r--   0        0        0     2719 2024-04-16 17:44:01.658152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source_connection_request.py
--rw-r--r--   0        0        0     5760 2024-04-16 17:44:01.662152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source_request.py
--rw-r--r--   0        0        0     2576 2024-04-16 17:44:01.666152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_token_redeem_request.py
--rw-r--r--   0        0        0     4055 2024-04-16 17:44:01.670152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy.py
--rw-r--r--   0        0        0     5643 2024-04-16 17:44:01.670152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_binding.py
--rw-r--r--   0        0        0     4231 2024-04-16 17:44:01.674152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_binding_request.py
--rw-r--r--   0        0        0      711 2024-04-16 17:44:01.674152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_engine_mode.py
--rw-r--r--   0        0        0     2817 2024-04-16 17:44:01.678152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_request.py
--rw-r--r--   0        0        0     2583 2024-04-16 17:44:01.678152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_test_request.py
--rw-r--r--   0        0        0     3281 2024-04-16 17:44:01.682152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_test_result.py
--rw-r--r--   0        0        0     4885 2024-04-16 17:44:01.686152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt.py
--rw-r--r--   0        0        0     4649 2024-04-16 17:44:01.690152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_challenge.py
--rw-r--r--   0        0        0     3325 2024-04-16 17:44:01.690152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_challenge_response_request.py
--rw-r--r--   0        0        0     4927 2024-04-16 17:44:01.694152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_request.py
--rw-r--r--   0        0        0     4321 2024-04-16 17:44:01.698152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_stage.py
--rw-r--r--   0        0        0     3351 2024-04-16 17:44:01.698152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_stage_request.py
--rw-r--r--   0        0        0     1185 2024-04-16 17:44:01.702152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_type_enum.py
--rw-r--r--   0        0        0     4264 2024-04-16 17:44:01.702152 authentik_client-2024.2.2.post1713289429/authentik_client/models/property_mapping.py
--rw-r--r--   0        0        0     2610 2024-04-16 17:44:01.706152 authentik_client-2024.2.2.post1713289429/authentik_client/models/property_mapping_preview.py
--rw-r--r--   0        0        0     2744 2024-04-16 17:44:01.706152 authentik_client-2024.2.2.post1713289429/authentik_client/models/property_mapping_test_result.py
--rw-r--r--   0        0        0      715 2024-04-16 17:44:01.706152 authentik_client-2024.2.2.post1713289429/authentik_client/models/protocol_enum.py
--rw-r--r--   0        0        0     5722 2024-04-16 17:44:01.710152 authentik_client-2024.2.2.post1713289429/authentik_client/models/provider.py
--rw-r--r--   0        0        0      713 2024-04-16 17:44:01.710152 authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_enum.py
--rw-r--r--   0        0        0     1314 2024-04-16 17:44:01.714152 authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_model_enum.py
--rw-r--r--   0        0        0     3397 2024-04-16 17:44:01.714152 authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_request.py
--rw-r--r--   0        0        0     1009 2024-04-16 17:44:01.714152 authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_type_enum.py
--rw-r--r--   0        0        0      754 2024-04-16 17:44:01.718152 authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_mode.py
--rw-r--r--   0        0        0     7819 2024-04-16 17:44:01.718152 authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_outpost_config.py
--rw-r--r--   0        0        0     9552 2024-04-16 17:44:01.722152 authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_provider.py
--rw-r--r--   0        0        0     6828 2024-04-16 17:44:01.722152 authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_provider_request.py
--rw-r--r--   0        0        0     4407 2024-04-16 17:44:01.726152 authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_property_mapping.py
--rw-r--r--   0        0        0     3440 2024-04-16 17:44:01.726152 authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_property_mapping_request.py
--rw-r--r--   0        0        0     6813 2024-04-16 17:44:01.730152 authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_provider.py
--rw-r--r--   0        0        0     4351 2024-04-16 17:44:01.730152 authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_provider_request.py
--rw-r--r--   0        0        0     3833 2024-04-16 17:44:01.734152 authentik_client-2024.2.2.post1713289429/authentik_client/models/radius_outpost_config.py
--rw-r--r--   0        0        0     6924 2024-04-16 17:44:01.734152 authentik_client-2024.2.2.post1713289429/authentik_client/models/radius_provider.py
--rw-r--r--   0        0        0     4501 2024-04-16 17:44:01.738152 authentik_client-2024.2.2.post1713289429/authentik_client/models/radius_provider_request.py
--rw-r--r--   0        0        0     4184 2024-04-16 17:44:01.738152 authentik_client-2024.2.2.post1713289429/authentik_client/models/redirect_challenge.py
--rw-r--r--   0        0        0     3642 2024-04-16 17:44:01.742152 authentik_client-2024.2.2.post1713289429/authentik_client/models/reputation.py
--rw-r--r--   0        0        0     4516 2024-04-16 17:44:01.746152 authentik_client-2024.2.2.post1713289429/authentik_client/models/reputation_policy.py
--rw-r--r--   0        0        0     3238 2024-04-16 17:44:01.750152 authentik_client-2024.2.2.post1713289429/authentik_client/models/reputation_policy_request.py
--rw-r--r--   0        0        0      795 2024-04-16 17:44:01.750152 authentik_client-2024.2.2.post1713289429/authentik_client/models/resident_key_requirement_enum.py
--rw-r--r--   0        0        0     2618 2024-04-16 17:44:01.750152 authentik_client-2024.2.2.post1713289429/authentik_client/models/role.py
--rw-r--r--   0        0        0     3333 2024-04-16 17:44:01.754152 authentik_client-2024.2.2.post1713289429/authentik_client/models/role_assigned_object_permission.py
--rw-r--r--   0        0        0     3293 2024-04-16 17:44:01.758152 authentik_client-2024.2.2.post1713289429/authentik_client/models/role_object_permission.py
--rw-r--r--   0        0        0     2517 2024-04-16 17:44:01.758152 authentik_client-2024.2.2.post1713289429/authentik_client/models/role_request.py
--rw-r--r--   0        0        0     2712 2024-04-16 17:44:01.762152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_metadata.py
--rw-r--r--   0        0        0     4718 2024-04-16 17:44:01.762152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_property_mapping.py
--rw-r--r--   0        0        0     3829 2024-04-16 17:44:01.766152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_property_mapping_request.py
--rw-r--r--   0        0        0    11056 2024-04-16 17:44:01.766152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_provider.py
--rw-r--r--   0        0        0     7460 2024-04-16 17:44:01.770152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_provider_request.py
--rw-r--r--   0        0        0    10563 2024-04-16 17:44:01.770152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_source.py
--rw-r--r--   0        0        0     8507 2024-04-16 17:44:01.774152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_source_request.py
--rw-r--r--   0        0        0     4248 2024-04-16 17:44:01.778152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_mapping.py
--rw-r--r--   0        0        0     3309 2024-04-16 17:44:01.778152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_mapping_request.py
--rw-r--r--   0        0        0     5454 2024-04-16 17:44:01.782152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_provider.py
--rw-r--r--   0        0        0     3802 2024-04-16 17:44:01.782152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_provider_request.py
--rw-r--r--   0        0        0     5999 2024-04-16 17:44:01.786152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source.py
--rw-r--r--   0        0        0     3369 2024-04-16 17:44:01.786152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_group.py
--rw-r--r--   0        0        0     3023 2024-04-16 17:44:01.790152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_group_request.py
--rw-r--r--   0        0        0     3708 2024-04-16 17:44:01.794152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_request.py
--rw-r--r--   0        0        0     3370 2024-04-16 17:44:01.794152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_user.py
--rw-r--r--   0        0        0     3026 2024-04-16 17:44:01.798152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_user_request.py
--rw-r--r--   0        0        0     3131 2024-04-16 17:44:01.802152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_sync_status.py
--rw-r--r--   0        0        0     4629 2024-04-16 17:44:01.806152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scope_mapping.py
--rw-r--r--   0        0        0     3740 2024-04-16 17:44:01.810152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scope_mapping_request.py
--rw-r--r--   0        0        0     2738 2024-04-16 17:44:01.814152 authentik_client-2024.2.2.post1713289429/authentik_client/models/selectable_stage.py
--rw-r--r--   0        0        0     3773 2024-04-16 17:44:01.814152 authentik_client-2024.2.2.post1713289429/authentik_client/models/service_connection.py
--rw-r--r--   0        0        0     2776 2024-04-16 17:44:01.818152 authentik_client-2024.2.2.post1713289429/authentik_client/models/service_connection_request.py
--rw-r--r--   0        0        0     2731 2024-04-16 17:44:01.818152 authentik_client-2024.2.2.post1713289429/authentik_client/models/service_connection_state.py
--rw-r--r--   0        0        0     3178 2024-04-16 17:44:01.822152 authentik_client-2024.2.2.post1713289429/authentik_client/models/session_user.py
--rw-r--r--   0        0        0     4931 2024-04-16 17:44:01.826152 authentik_client-2024.2.2.post1713289429/authentik_client/models/settings.py
--rw-r--r--   0        0        0     5058 2024-04-16 17:44:01.826152 authentik_client-2024.2.2.post1713289429/authentik_client/models/settings_request.py
--rw-r--r--   0        0        0      733 2024-04-16 17:44:01.830152 authentik_client-2024.2.2.post1713289429/authentik_client/models/severity_enum.py
--rw-r--r--   0        0        0     4175 2024-04-16 17:44:01.830152 authentik_client-2024.2.2.post1713289429/authentik_client/models/shell_challenge.py
--rw-r--r--   0        0        0     1492 2024-04-16 17:44:01.834152 authentik_client-2024.2.2.post1713289429/authentik_client/models/signature_algorithm_enum.py
--rw-r--r--   0        0        0     2906 2024-04-16 17:44:01.802152 authentik_client-2024.2.2.post1713289429/authentik_client/models/sms_device.py
--rw-r--r--   0        0        0     2619 2024-04-16 17:44:01.806152 authentik_client-2024.2.2.post1713289429/authentik_client/models/sms_device_request.py
--rw-r--r--   0        0        0     6945 2024-04-16 17:44:01.834152 authentik_client-2024.2.2.post1713289429/authentik_client/models/source.py
--rw-r--r--   0        0        0     4836 2024-04-16 17:44:01.838152 authentik_client-2024.2.2.post1713289429/authentik_client/models/source_request.py
--rw-r--r--   0        0        0     4438 2024-04-16 17:44:01.842152 authentik_client-2024.2.2.post1713289429/authentik_client/models/source_stage.py
--rw-r--r--   0        0        0     3507 2024-04-16 17:44:01.842152 authentik_client-2024.2.2.post1713289429/authentik_client/models/source_stage_request.py
--rw-r--r--   0        0        0     5355 2024-04-16 17:44:01.846152 authentik_client-2024.2.2.post1713289429/authentik_client/models/source_type.py
--rw-r--r--   0        0        0      714 2024-04-16 17:44:01.846152 authentik_client-2024.2.2.post1713289429/authentik_client/models/sp_binding_enum.py
--rw-r--r--   0        0        0     4070 2024-04-16 17:44:01.850152 authentik_client-2024.2.2.post1713289429/authentik_client/models/stage.py
--rw-r--r--   0        0        0     3437 2024-04-16 17:44:01.854152 authentik_client-2024.2.2.post1713289429/authentik_client/models/stage_prompt.py
--rw-r--r--   0        0        0     3089 2024-04-16 17:44:01.854152 authentik_client-2024.2.2.post1713289429/authentik_client/models/stage_request.py
--rw-r--r--   0        0        0     3385 2024-04-16 17:44:01.858152 authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device.py
--rw-r--r--   0        0        0     2631 2024-04-16 17:44:01.858152 authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device_request.py
--rw-r--r--   0        0        0     2546 2024-04-16 17:44:01.862152 authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device_token.py
--rw-r--r--   0        0        0     2581 2024-04-16 17:44:01.866152 authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device_token_request.py
--rw-r--r--   0        0        0      846 2024-04-16 17:44:01.866152 authentik_client-2024.2.2.post1713289429/authentik_client/models/sub_mode_enum.py
--rw-r--r--   0        0        0     4463 2024-04-16 17:44:01.870152 authentik_client-2024.2.2.post1713289429/authentik_client/models/system_info.py
--rw-r--r--   0        0        0     2934 2024-04-16 17:44:01.870152 authentik_client-2024.2.2.post1713289429/authentik_client/models/system_info_runtime.py
--rw-r--r--   0        0        0     4286 2024-04-16 17:44:01.874152 authentik_client-2024.2.2.post1713289429/authentik_client/models/system_task.py
--rw-r--r--   0        0        0      789 2024-04-16 17:44:01.874152 authentik_client-2024.2.2.post1713289429/authentik_client/models/system_task_status_enum.py
--rw-r--r--   0        0        0     2872 2024-04-16 17:44:01.882152 authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant.py
--rw-r--r--   0        0        0     2589 2024-04-16 17:44:01.886152 authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_admin_group_request_request.py
--rw-r--r--   0        0        0     2705 2024-04-16 17:44:01.886152 authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_recovery_key_request_request.py
--rw-r--r--   0        0        0     2599 2024-04-16 17:44:01.890152 authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_recovery_key_response.py
--rw-r--r--   0        0        0     2765 2024-04-16 17:44:01.894152 authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_request.py
--rw-r--r--   0        0        0     4802 2024-04-16 17:44:01.894152 authentik_client-2024.2.2.post1713289429/authentik_client/models/token.py
--rw-r--r--   0        0        0     4198 2024-04-16 17:44:01.898152 authentik_client-2024.2.2.post1713289429/authentik_client/models/token_model.py
--rw-r--r--   0        0        0     4329 2024-04-16 17:44:01.898152 authentik_client-2024.2.2.post1713289429/authentik_client/models/token_request.py
--rw-r--r--   0        0        0     2521 2024-04-16 17:44:01.902152 authentik_client-2024.2.2.post1713289429/authentik_client/models/token_set_key_request.py
--rw-r--r--   0        0        0     2494 2024-04-16 17:44:01.906152 authentik_client-2024.2.2.post1713289429/authentik_client/models/token_view.py
--rw-r--r--   0        0        0     2724 2024-04-16 17:44:01.878152 authentik_client-2024.2.2.post1713289429/authentik_client/models/totp_device.py
--rw-r--r--   0        0        0     2623 2024-04-16 17:44:01.882152 authentik_client-2024.2.2.post1713289429/authentik_client/models/totp_device_request.py
--rw-r--r--   0        0        0     3389 2024-04-16 17:44:01.906152 authentik_client-2024.2.2.post1713289429/authentik_client/models/transaction_application_request.py
--rw-r--r--   0        0        0     2595 2024-04-16 17:44:01.910152 authentik_client-2024.2.2.post1713289429/authentik_client/models/transaction_application_response.py
--rw-r--r--   0        0        0     2936 2024-04-16 17:44:01.910152 authentik_client-2024.2.2.post1713289429/authentik_client/models/type_create.py
--rw-r--r--   0        0        0      730 2024-04-16 17:44:01.914152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ui_theme_enum.py
--rw-r--r--   0        0        0     2808 2024-04-16 17:44:01.914152 authentik_client-2024.2.2.post1713289429/authentik_client/models/used_by.py
--rw-r--r--   0        0        0      795 2024-04-16 17:44:01.914152 authentik_client-2024.2.2.post1713289429/authentik_client/models/used_by_action_enum.py
--rw-r--r--   0        0        0     5459 2024-04-16 17:44:01.918152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user.py
--rw-r--r--   0        0        0     2458 2024-04-16 17:44:01.922152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_account_request.py
--rw-r--r--   0        0        0     4946 2024-04-16 17:44:01.922152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_assigned_object_permission.py
--rw-r--r--   0        0        0     3828 2024-04-16 17:44:01.926152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_consent.py
--rw-r--r--   0        0        0      811 2024-04-16 17:44:01.926152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_creation_mode_enum.py
--rw-r--r--   0        0        0     4110 2024-04-16 17:44:01.930152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_delete_stage.py
--rw-r--r--   0        0        0     3129 2024-04-16 17:44:01.930152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_delete_stage_request.py
--rw-r--r--   0        0        0      735 2024-04-16 17:44:01.934152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_fields_enum.py
--rw-r--r--   0        0        0     3909 2024-04-16 17:44:01.934152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_group.py
--rw-r--r--   0        0        0     4334 2024-04-16 17:44:01.938152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_challenge.py
--rw-r--r--   0        0        0     2805 2024-04-16 17:44:01.938152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_challenge_response_request.py
--rw-r--r--   0        0        0     5631 2024-04-16 17:44:01.942152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_stage.py
--rw-r--r--   0        0        0     4728 2024-04-16 17:44:01.942152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_stage_request.py
--rw-r--r--   0        0        0     4110 2024-04-16 17:44:01.946152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_logout_stage.py
--rw-r--r--   0        0        0     3129 2024-04-16 17:44:01.950152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_logout_stage_request.py
--rw-r--r--   0        0        0      853 2024-04-16 17:44:01.950152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_matching_mode_enum.py
--rw-r--r--   0        0        0     4160 2024-04-16 17:44:01.950152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_metrics.py
--rw-r--r--   0        0        0     3188 2024-04-16 17:44:01.954152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_o_auth_source_connection.py
--rw-r--r--   0        0        0     3054 2024-04-16 17:44:01.954152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3293 2024-04-16 17:44:01.958152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_object_permission.py
--rw-r--r--   0        0        0     2557 2024-04-16 17:44:01.958152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_password_set_request.py
--rw-r--r--   0        0        0     2491 2024-04-16 17:44:01.962152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_path.py
--rw-r--r--   0        0        0     3872 2024-04-16 17:44:01.962152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_request.py
--rw-r--r--   0        0        0     3107 2024-04-16 17:44:01.966152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_saml_source_connection.py
--rw-r--r--   0        0        0     2668 2024-04-16 17:44:01.970152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_saml_source_connection_request.py
--rw-r--r--   0        0        0     5465 2024-04-16 17:44:01.974152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_self.py
--rw-r--r--   0        0        0     2629 2024-04-16 17:44:01.974152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_self_groups.py
--rw-r--r--   0        0        0     3074 2024-04-16 17:44:01.978152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_service_account_request.py
--rw-r--r--   0        0        0     2844 2024-04-16 17:44:01.978152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_service_account_response.py
--rw-r--r--   0        0        0     2866 2024-04-16 17:44:01.982152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_setting.py
--rw-r--r--   0        0        0     3245 2024-04-16 17:44:01.986152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_source_connection.py
--rw-r--r--   0        0        0      817 2024-04-16 17:44:01.986152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_type_enum.py
--rw-r--r--   0        0        0      777 2024-04-16 17:44:01.986152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_verification_enum.py
--rw-r--r--   0        0        0     5382 2024-04-16 17:44:01.990152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_write_stage.py
--rw-r--r--   0        0        0     4412 2024-04-16 17:44:01.990152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_write_stage_request.py
--rw-r--r--   0        0        0     3197 2024-04-16 17:44:01.994152 authentik_client-2024.2.2.post1713289429/authentik_client/models/validation_error.py
--rw-r--r--   0        0        0     3589 2024-04-16 17:44:01.998152 authentik_client-2024.2.2.post1713289429/authentik_client/models/version.py
--rw-r--r--   0        0        0     3630 2024-04-16 17:44:01.998152 authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device.py
--rw-r--r--   0        0        0     2577 2024-04-16 17:44:02.002152 authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device_request.py
--rw-r--r--   0        0        0     2562 2024-04-16 17:44:02.002152 authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device_type.py
--rw-r--r--   0        0        0     2669 2024-04-16 17:44:02.006152 authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device_type_request.py
--rw-r--r--   0        0        0     2410 2024-04-16 17:44:02.006152 authentik_client-2024.2.2.post1713289429/authentik_client/models/workers.py
--rw-r--r--   0        0        0        0 2024-04-16 17:44:03.290151 authentik_client-2024.2.2.post1713289429/authentik_client/py.typed
--rw-r--r--   0        0        0     9196 2024-04-16 17:44:03.298151 authentik_client-2024.2.2.post1713289429/authentik_client/rest.py
--rw-r--r--   0        0        0     1936 2024-04-16 17:44:03.290151 authentik_client-2024.2.2.post1713289429/pyproject.toml
--rw-r--r--   0        0        0   144847 1970-01-01 00:00:00.000000 authentik_client-2024.2.2.post1713289429/PKG-INFO
+-rw-r--r--   0        0        0   143895 2024-04-17 13:18:33.219812 authentik_client-2024.2.3.post1713359900/README.md
+-rw-r--r--   0        0        0    48410 2024-04-17 13:18:33.227813 authentik_client-2024.2.3.post1713359900/authentik_client/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-17 13:18:33.231813 authentik_client-2024.2.3.post1713359900/authentik_client/api/__init__.py
+-rw-r--r--   0        0        0    97518 2024-04-17 13:18:32.939812 authentik_client-2024.2.3.post1713359900/authentik_client/api/admin_api.py
+-rw-r--r--   0        0        0   700271 2024-04-17 13:18:32.955812 authentik_client-2024.2.3.post1713359900/authentik_client/api/authenticators_api.py
+-rw-r--r--   0        0        0   701197 2024-04-17 13:18:32.979812 authentik_client-2024.2.3.post1713359900/authentik_client/api/core_api.py
+-rw-r--r--   0        0        0   116805 2024-04-17 13:18:32.991812 authentik_client-2024.2.3.post1713359900/authentik_client/api/crypto_api.py
+-rw-r--r--   0        0        0   107946 2024-04-17 13:18:32.999812 authentik_client-2024.2.3.post1713359900/authentik_client/api/enterprise_api.py
+-rw-r--r--   0        0        0   408008 2024-04-17 13:18:33.011812 authentik_client-2024.2.3.post1713359900/authentik_client/api/events_api.py
+-rw-r--r--   0        0        0   280806 2024-04-17 13:18:33.023812 authentik_client-2024.2.3.post1713359900/authentik_client/api/flows_api.py
+-rw-r--r--   0        0        0   101134 2024-04-17 13:18:33.031812 authentik_client-2024.2.3.post1713359900/authentik_client/api/managed_api.py
+-rw-r--r--   0        0        0   135649 2024-04-17 13:18:33.039812 authentik_client-2024.2.3.post1713359900/authentik_client/api/oauth2_api.py
+-rw-r--r--   0        0        0   413301 2024-04-17 13:18:33.047812 authentik_client-2024.2.3.post1713359900/authentik_client/api/outposts_api.py
+-rw-r--r--   0        0        0   725201 2024-04-17 13:18:33.067812 authentik_client-2024.2.3.post1713359900/authentik_client/api/policies_api.py
+-rw-r--r--   0        0        0   552586 2024-04-17 13:18:33.083812 authentik_client-2024.2.3.post1713359900/authentik_client/api/propertymappings_api.py
+-rw-r--r--   0        0        0   718066 2024-04-17 13:18:33.107812 authentik_client-2024.2.3.post1713359900/authentik_client/api/providers_api.py
+-rw-r--r--   0        0        0   150485 2024-04-17 13:18:33.119812 authentik_client-2024.2.3.post1713359900/authentik_client/api/rac_api.py
+-rw-r--r--   0        0        0   207550 2024-04-17 13:18:33.127812 authentik_client-2024.2.3.post1713359900/authentik_client/api/rbac_api.py
+-rw-r--r--   0        0        0    10391 2024-04-17 13:18:33.135812 authentik_client-2024.2.3.post1713359900/authentik_client/api/root_api.py
+-rw-r--r--   0        0        0    11845 2024-04-17 13:18:33.139812 authentik_client-2024.2.3.post1713359900/authentik_client/api/schema_api.py
+-rw-r--r--   0        0        0  1037225 2024-04-17 13:18:33.155812 authentik_client-2024.2.3.post1713359900/authentik_client/api/sources_api.py
+-rw-r--r--   0        0        0  1945986 2024-04-17 13:18:33.191813 authentik_client-2024.2.3.post1713359900/authentik_client/api/stages_api.py
+-rw-r--r--   0        0        0   157909 2024-04-17 13:18:33.207813 authentik_client-2024.2.3.post1713359900/authentik_client/api/tenants_api.py
+-rw-r--r--   0        0        0    25779 2024-04-17 13:18:33.231813 authentik_client-2024.2.3.post1713359900/authentik_client/api_client.py
+-rw-r--r--   0        0        0      652 2024-04-17 13:18:33.231813 authentik_client-2024.2.3.post1713359900/authentik_client/api_response.py
+-rw-r--r--   0        0        0    14724 2024-04-17 13:18:33.227813 authentik_client-2024.2.3.post1713359900/authentik_client/configuration.py
+-rw-r--r--   0        0        0     5934 2024-04-17 13:18:33.231813 authentik_client-2024.2.3.post1713359900/authentik_client/exceptions.py
+-rw-r--r--   0        0        0    46712 2024-04-17 13:18:33.227813 authentik_client-2024.2.3.post1713359900/authentik_client/models/__init__.py
+-rw-r--r--   0        0        0     4513 2024-04-17 13:18:30.283804 authentik_client-2024.2.3.post1713359900/authentik_client/models/access_denied_challenge.py
+-rw-r--r--   0        0        0     2482 2024-04-17 13:18:30.299804 authentik_client-2024.2.3.post1713359900/authentik_client/models/app.py
+-rw-r--r--   0        0        0     4230 2024-04-17 13:18:30.303804 authentik_client-2024.2.3.post1713359900/authentik_client/models/app_enum.py
+-rw-r--r--   0        0        0     2702 2024-04-17 13:18:30.315804 authentik_client-2024.2.3.post1713359900/authentik_client/models/apple_challenge_response_request.py
+-rw-r--r--   0        0        0     4508 2024-04-17 13:18:30.327804 authentik_client-2024.2.3.post1713359900/authentik_client/models/apple_login_challenge.py
+-rw-r--r--   0        0        0     6686 2024-04-17 13:18:30.335804 authentik_client-2024.2.3.post1713359900/authentik_client/models/application.py
+-rw-r--r--   0        0        0     4473 2024-04-17 13:18:30.343804 authentik_client-2024.2.3.post1713359900/authentik_client/models/application_request.py
+-rw-r--r--   0        0        0      711 2024-04-17 13:18:30.351804 authentik_client-2024.2.3.post1713359900/authentik_client/models/auth_mode_enum.py
+-rw-r--r--   0        0        0      709 2024-04-17 13:18:30.351804 authentik_client-2024.2.3.post1713359900/authentik_client/models/auth_type_enum.py
+-rw-r--r--   0        0        0     5195 2024-04-17 13:18:30.359804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session.py
+-rw-r--r--   0        0        0     3064 2024-04-17 13:18:30.375804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session_asn.py
+-rw-r--r--   0        0        0     2826 2024-04-17 13:18:30.383804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session_geo_ip.py
+-rw-r--r--   0        0        0     3865 2024-04-17 13:18:30.387804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session_user_agent.py
+-rw-r--r--   0        0        0     2646 2024-04-17 13:18:30.395804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session_user_agent_device.py
+-rw-r--r--   0        0        0     2792 2024-04-17 13:18:30.399804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session_user_agent_os.py
+-rw-r--r--   0        0        0     2725 2024-04-17 13:18:30.407804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session_user_agent_user_agent.py
+-rw-r--r--   0        0        0      895 2024-04-17 13:18:30.411804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authentication_enum.py
+-rw-r--r--   0        0        0      782 2024-04-17 13:18:30.415804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_attachment_enum.py
+-rw-r--r--   0        0        0     4686 2024-04-17 13:18:30.419804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_duo_challenge.py
+-rw-r--r--   0        0        0     2743 2024-04-17 13:18:30.427804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_duo_challenge_response_request.py
+-rw-r--r--   0        0        0     5327 2024-04-17 13:18:30.431804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_duo_stage.py
+-rw-r--r--   0        0        0     2768 2024-04-17 13:18:30.435804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_duo_stage_device_import_response.py
+-rw-r--r--   0        0        0     2785 2024-04-17 13:18:30.439804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
+-rw-r--r--   0        0        0     4744 2024-04-17 13:18:30.447804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-17 13:18:30.451804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_sms_challenge.py
+-rw-r--r--   0        0        0     3022 2024-04-17 13:18:30.459804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_sms_challenge_response_request.py
+-rw-r--r--   0        0        0     6409 2024-04-17 13:18:30.463804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_sms_stage.py
+-rw-r--r--   0        0        0     5595 2024-04-17 13:18:30.467804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4474 2024-04-17 13:18:30.475804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_static_challenge.py
+-rw-r--r--   0        0        0     2761 2024-04-17 13:18:30.479804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_static_challenge_response_request.py
+-rw-r--r--   0        0        0     5363 2024-04-17 13:18:30.487804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_static_stage.py
+-rw-r--r--   0        0        0     4392 2024-04-17 13:18:30.491804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4468 2024-04-17 13:18:30.495804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_totp_challenge.py
+-rw-r--r--   0        0        0     2858 2024-04-17 13:18:30.499804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_totp_challenge_response_request.py
+-rw-r--r--   0        0        0     5132 2024-04-17 13:18:30.507804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_totp_stage.py
+-rw-r--r--   0        0        0     4201 2024-04-17 13:18:30.511804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     6722 2024-04-17 13:18:30.515804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_validate_stage.py
+-rw-r--r--   0        0        0     4893 2024-04-17 13:18:30.523804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5717 2024-04-17 13:18:30.527804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_validation_challenge.py
+-rw-r--r--   0        0        0     3805 2024-04-17 13:18:30.535804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_validation_challenge_response_request.py
+-rw-r--r--   0        0        0     4499 2024-04-17 13:18:30.539804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_web_authn_challenge.py
+-rw-r--r--   0        0        0     2852 2024-04-17 13:18:30.547804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_web_authn_challenge_response_request.py
+-rw-r--r--   0        0        0     7081 2024-04-17 13:18:30.551804 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_web_authn_stage.py
+-rw-r--r--   0        0        0     5302 2024-04-17 13:18:30.555805 authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     2718 2024-04-17 13:18:30.559805 authentik_client-2024.2.3.post1713359900/authentik_client/models/auto_submit_challenge_response_request.py
+-rw-r--r--   0        0        0     4388 2024-04-17 13:18:30.567804 authentik_client-2024.2.3.post1713359900/authentik_client/models/autosubmit_challenge.py
+-rw-r--r--   0        0        0      950 2024-04-17 13:18:30.571805 authentik_client-2024.2.3.post1713359900/authentik_client/models/backends_enum.py
+-rw-r--r--   0        0        0      748 2024-04-17 13:18:30.571805 authentik_client-2024.2.3.post1713359900/authentik_client/models/binding_type_enum.py
+-rw-r--r--   0        0        0     2995 2024-04-17 13:18:30.575805 authentik_client-2024.2.3.post1713359900/authentik_client/models/blueprint_file.py
+-rw-r--r--   0        0        0     4453 2024-04-17 13:18:30.583804 authentik_client-2024.2.3.post1713359900/authentik_client/models/blueprint_instance.py
+-rw-r--r--   0        0        0     3208 2024-04-17 13:18:30.587805 authentik_client-2024.2.3.post1713359900/authentik_client/models/blueprint_instance_request.py
+-rw-r--r--   0        0        0      836 2024-04-17 13:18:30.591805 authentik_client-2024.2.3.post1713359900/authentik_client/models/blueprint_instance_status_enum.py
+-rw-r--r--   0        0        0     6255 2024-04-17 13:18:30.595805 authentik_client-2024.2.3.post1713359900/authentik_client/models/brand.py
+-rw-r--r--   0        0        0     6307 2024-04-17 13:18:30.599804 authentik_client-2024.2.3.post1713359900/authentik_client/models/brand_request.py
+-rw-r--r--   0        0        0     2501 2024-04-17 13:18:30.603805 authentik_client-2024.2.3.post1713359900/authentik_client/models/cache.py
+-rw-r--r--   0        0        0      875 2024-04-17 13:18:30.603805 authentik_client-2024.2.3.post1713359900/authentik_client/models/capabilities_enum.py
+-rw-r--r--   0        0        0     4476 2024-04-17 13:18:30.611805 authentik_client-2024.2.3.post1713359900/authentik_client/models/captcha_challenge.py
+-rw-r--r--   0        0        0     2797 2024-04-17 13:18:30.615805 authentik_client-2024.2.3.post1713359900/authentik_client/models/captcha_challenge_response_request.py
+-rw-r--r--   0        0        0     4438 2024-04-17 13:18:30.619805 authentik_client-2024.2.3.post1713359900/authentik_client/models/captcha_stage.py
+-rw-r--r--   0        0        0     3774 2024-04-17 13:18:30.623805 authentik_client-2024.2.3.post1713359900/authentik_client/models/captcha_stage_request.py
+-rw-r--r--   0        0        0     2522 2024-04-17 13:18:30.627805 authentik_client-2024.2.3.post1713359900/authentik_client/models/certificate_data.py
+-rw-r--r--   0        0        0     2861 2024-04-17 13:18:30.631805 authentik_client-2024.2.3.post1713359900/authentik_client/models/certificate_generation_request.py
+-rw-r--r--   0        0        0     6655 2024-04-17 13:18:30.635805 authentik_client-2024.2.3.post1713359900/authentik_client/models/certificate_key_pair.py
+-rw-r--r--   0        0        0     2989 2024-04-17 13:18:30.643805 authentik_client-2024.2.3.post1713359900/authentik_client/models/certificate_key_pair_request.py
+-rw-r--r--   0        0        0      747 2024-04-17 13:18:30.647805 authentik_client-2024.2.3.post1713359900/authentik_client/models/challenge_choices.py
+-rw-r--r--   0        0        0    24236 2024-04-17 13:18:30.655805 authentik_client-2024.2.3.post1713359900/authentik_client/models/challenge_types.py
+-rw-r--r--   0        0        0      729 2024-04-17 13:18:30.659805 authentik_client-2024.2.3.post1713359900/authentik_client/models/client_type_enum.py
+-rw-r--r--   0        0        0     3539 2024-04-17 13:18:30.663805 authentik_client-2024.2.3.post1713359900/authentik_client/models/config.py
+-rw-r--r--   0        0        0     4021 2024-04-17 13:18:30.667805 authentik_client-2024.2.3.post1713359900/authentik_client/models/connection_token.py
+-rw-r--r--   0        0        0     2662 2024-04-17 13:18:30.671805 authentik_client-2024.2.3.post1713359900/authentik_client/models/connection_token_request.py
+-rw-r--r--   0        0        0     5736 2024-04-17 13:18:30.675805 authentik_client-2024.2.3.post1713359900/authentik_client/models/consent_challenge.py
+-rw-r--r--   0        0        0     2838 2024-04-17 13:18:30.679805 authentik_client-2024.2.3.post1713359900/authentik_client/models/consent_challenge_response_request.py
+-rw-r--r--   0        0        0     2513 2024-04-17 13:18:30.683805 authentik_client-2024.2.3.post1713359900/authentik_client/models/consent_permission.py
+-rw-r--r--   0        0        0     4511 2024-04-17 13:18:30.687805 authentik_client-2024.2.3.post1713359900/authentik_client/models/consent_stage.py
+-rw-r--r--   0        0        0      783 2024-04-17 13:18:30.691805 authentik_client-2024.2.3.post1713359900/authentik_client/models/consent_stage_mode_enum.py
+-rw-r--r--   0        0        0     3569 2024-04-17 13:18:30.695805 authentik_client-2024.2.3.post1713359900/authentik_client/models/consent_stage_request.py
+-rw-r--r--   0        0        0     2891 2024-04-17 13:18:30.699805 authentik_client-2024.2.3.post1713359900/authentik_client/models/contextual_flow_info.py
+-rw-r--r--   0        0        0      879 2024-04-17 13:18:30.699805 authentik_client-2024.2.3.post1713359900/authentik_client/models/contextual_flow_info_layout_enum.py
+-rw-r--r--   0        0        0     2657 2024-04-17 13:18:30.703805 authentik_client-2024.2.3.post1713359900/authentik_client/models/coordinate.py
+-rw-r--r--   0        0        0     4704 2024-04-17 13:18:30.707805 authentik_client-2024.2.3.post1713359900/authentik_client/models/current_brand.py
+-rw-r--r--   0        0        0      771 2024-04-17 13:18:30.711805 authentik_client-2024.2.3.post1713359900/authentik_client/models/denied_action_enum.py
+-rw-r--r--   0        0        0     4200 2024-04-17 13:18:30.715805 authentik_client-2024.2.3.post1713359900/authentik_client/models/deny_stage.py
+-rw-r--r--   0        0        0     3230 2024-04-17 13:18:30.719805 authentik_client-2024.2.3.post1713359900/authentik_client/models/deny_stage_request.py
+-rw-r--r--   0        0        0     3522 2024-04-17 13:18:30.723805 authentik_client-2024.2.3.post1713359900/authentik_client/models/device.py
+-rw-r--r--   0        0        0     2657 2024-04-17 13:18:30.731805 authentik_client-2024.2.3.post1713359900/authentik_client/models/device_challenge.py
+-rw-r--r--   0        0        0     2792 2024-04-17 13:18:30.735805 authentik_client-2024.2.3.post1713359900/authentik_client/models/device_challenge_request.py
+-rw-r--r--   0        0        0      780 2024-04-17 13:18:30.739805 authentik_client-2024.2.3.post1713359900/authentik_client/models/device_classes_enum.py
+-rw-r--r--   0        0        0     1244 2024-04-17 13:18:30.743805 authentik_client-2024.2.3.post1713359900/authentik_client/models/digest_algorithm_enum.py
+-rw-r--r--   0        0        0      695 2024-04-17 13:18:30.747805 authentik_client-2024.2.3.post1713359900/authentik_client/models/digits_enum.py
+-rw-r--r--   0        0        0     4969 2024-04-17 13:18:30.751805 authentik_client-2024.2.3.post1713359900/authentik_client/models/docker_service_connection.py
+-rw-r--r--   0        0        0     4087 2024-04-17 13:18:30.759805 authentik_client-2024.2.3.post1713359900/authentik_client/models/docker_service_connection_request.py
+-rw-r--r--   0        0        0     2847 2024-04-17 13:18:30.763805 authentik_client-2024.2.3.post1713359900/authentik_client/models/domain.py
+-rw-r--r--   0        0        0     2746 2024-04-17 13:18:30.767805 authentik_client-2024.2.3.post1713359900/authentik_client/models/domain_request.py
+-rw-r--r--   0        0        0     4155 2024-04-17 13:18:30.775805 authentik_client-2024.2.3.post1713359900/authentik_client/models/dummy_challenge.py
+-rw-r--r--   0        0        0     2681 2024-04-17 13:18:30.779805 authentik_client-2024.2.3.post1713359900/authentik_client/models/dummy_challenge_response_request.py
+-rw-r--r--   0        0        0     4515 2024-04-17 13:18:30.783805 authentik_client-2024.2.3.post1713359900/authentik_client/models/dummy_policy.py
+-rw-r--r--   0        0        0     3237 2024-04-17 13:18:30.787805 authentik_client-2024.2.3.post1713359900/authentik_client/models/dummy_policy_request.py
+-rw-r--r--   0        0        0     4213 2024-04-17 13:18:30.791805 authentik_client-2024.2.3.post1713359900/authentik_client/models/dummy_stage.py
+-rw-r--r--   0        0        0     3232 2024-04-17 13:18:30.795805 authentik_client-2024.2.3.post1713359900/authentik_client/models/dummy_stage_request.py
+-rw-r--r--   0        0        0     2720 2024-04-17 13:18:30.799805 authentik_client-2024.2.3.post1713359900/authentik_client/models/duo_device.py
+-rw-r--r--   0        0        0     2575 2024-04-17 13:18:30.799805 authentik_client-2024.2.3.post1713359900/authentik_client/models/duo_device_enrollment_status.py
+-rw-r--r--   0        0        0     2619 2024-04-17 13:18:30.803805 authentik_client-2024.2.3.post1713359900/authentik_client/models/duo_device_request.py
+-rw-r--r--   0        0        0      748 2024-04-17 13:18:30.807805 authentik_client-2024.2.3.post1713359900/authentik_client/models/duo_response_enum.py
+-rw-r--r--   0        0        0     4090 2024-04-17 13:18:30.811805 authentik_client-2024.2.3.post1713359900/authentik_client/models/email_challenge.py
+-rw-r--r--   0        0        0     2770 2024-04-17 13:18:30.815805 authentik_client-2024.2.3.post1713359900/authentik_client/models/email_challenge_response_request.py
+-rw-r--r--   0        0        0     5902 2024-04-17 13:18:30.819805 authentik_client-2024.2.3.post1713359900/authentik_client/models/email_stage.py
+-rw-r--r--   0        0        0     5121 2024-04-17 13:18:30.823805 authentik_client-2024.2.3.post1713359900/authentik_client/models/email_stage_request.py
+-rw-r--r--   0        0        0     4707 2024-04-17 13:18:30.831805 authentik_client-2024.2.3.post1713359900/authentik_client/models/endpoint.py
+-rw-r--r--   0        0        0     3678 2024-04-17 13:18:30.835805 authentik_client-2024.2.3.post1713359900/authentik_client/models/endpoint_request.py
+-rw-r--r--   0        0        0     2530 2024-04-17 13:18:30.839805 authentik_client-2024.2.3.post1713359900/authentik_client/models/error_detail.py
+-rw-r--r--   0        0        0     3309 2024-04-17 13:18:30.843805 authentik_client-2024.2.3.post1713359900/authentik_client/models/error_reporting_config.py
+-rw-r--r--   0        0        0     4129 2024-04-17 13:18:30.847805 authentik_client-2024.2.3.post1713359900/authentik_client/models/event.py
+-rw-r--r--   0        0        0     1730 2024-04-17 13:18:30.851805 authentik_client-2024.2.3.post1713359900/authentik_client/models/event_actions.py
+-rw-r--r--   0        0        0     6006 2024-04-17 13:18:30.855805 authentik_client-2024.2.3.post1713359900/authentik_client/models/event_matcher_policy.py
+-rw-r--r--   0        0        0     4807 2024-04-17 13:18:30.859805 authentik_client-2024.2.3.post1713359900/authentik_client/models/event_matcher_policy_request.py
+-rw-r--r--   0        0        0     3990 2024-04-17 13:18:30.859805 authentik_client-2024.2.3.post1713359900/authentik_client/models/event_request.py
+-rw-r--r--   0        0        0     2697 2024-04-17 13:18:30.863805 authentik_client-2024.2.3.post1713359900/authentik_client/models/event_top_per_user.py
+-rw-r--r--   0        0        0     3926 2024-04-17 13:18:30.867805 authentik_client-2024.2.3.post1713359900/authentik_client/models/expiring_base_grant_model.py
+-rw-r--r--   0        0        0     4191 2024-04-17 13:18:30.875805 authentik_client-2024.2.3.post1713359900/authentik_client/models/expression_policy.py
+-rw-r--r--   0        0        0     2992 2024-04-17 13:18:30.879805 authentik_client-2024.2.3.post1713359900/authentik_client/models/expression_policy_request.py
+-rw-r--r--   0        0        0     4524 2024-04-17 13:18:30.879805 authentik_client-2024.2.3.post1713359900/authentik_client/models/extra_role_object_permission.py
+-rw-r--r--   0        0        0     4524 2024-04-17 13:18:30.883805 authentik_client-2024.2.3.post1713359900/authentik_client/models/extra_user_object_permission.py
+-rw-r--r--   0        0        0     2519 2024-04-17 13:18:30.887806 authentik_client-2024.2.3.post1713359900/authentik_client/models/file_path_request.py
+-rw-r--r--   0        0        0     6047 2024-04-17 13:18:30.891806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow.py
+-rw-r--r--   0        0        0    25850 2024-04-17 13:18:30.899806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_challenge_response_request.py
+-rw-r--r--   0        0        0      934 2024-04-17 13:18:30.899806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_designation_enum.py
+-rw-r--r--   0        0        0     2533 2024-04-17 13:18:30.903806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_diagram.py
+-rw-r--r--   0        0        0     4505 2024-04-17 13:18:30.907806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_error_challenge.py
+-rw-r--r--   0        0        0     3111 2024-04-17 13:18:30.915806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_import_result.py
+-rw-r--r--   0        0        0     3418 2024-04-17 13:18:30.915806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_inspection.py
+-rw-r--r--   0        0        0     3875 2024-04-17 13:18:30.919806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_inspector_plan.py
+-rw-r--r--   0        0        0      837 2024-04-17 13:18:30.919806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_layout_enum.py
+-rw-r--r--   0        0        0     4741 2024-04-17 13:18:30.923806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_request.py
+-rw-r--r--   0        0        0     5223 2024-04-17 13:18:30.927806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_set.py
+-rw-r--r--   0        0        0     4459 2024-04-17 13:18:30.931806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_set_request.py
+-rw-r--r--   0        0        0     4763 2024-04-17 13:18:30.935806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_stage_binding.py
+-rw-r--r--   0        0        0     3983 2024-04-17 13:18:30.939806 authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_stage_binding_request.py
+-rw-r--r--   0        0        0     2641 2024-04-17 13:18:30.943806 authentik_client-2024.2.3.post1713359900/authentik_client/models/footer_link.py
+-rw-r--r--   0        0        0     2531 2024-04-17 13:18:30.947806 authentik_client-2024.2.3.post1713359900/authentik_client/models/generic_error.py
+-rw-r--r--   0        0        0      865 2024-04-17 13:18:30.947806 authentik_client-2024.2.3.post1713359900/authentik_client/models/geoip_binding_enum.py
+-rw-r--r--   0        0        0     5445 2024-04-17 13:18:30.951806 authentik_client-2024.2.3.post1713359900/authentik_client/models/group.py
+-rw-r--r--   0        0        0     4209 2024-04-17 13:18:30.959806 authentik_client-2024.2.3.post1713359900/authentik_client/models/group_member.py
+-rw-r--r--   0        0        0     4006 2024-04-17 13:18:30.963806 authentik_client-2024.2.3.post1713359900/authentik_client/models/group_member_request.py
+-rw-r--r--   0        0        0     3347 2024-04-17 13:18:30.967806 authentik_client-2024.2.3.post1713359900/authentik_client/models/group_request.py
+-rw-r--r--   0        0        0     6080 2024-04-17 13:18:30.971806 authentik_client-2024.2.3.post1713359900/authentik_client/models/identification_challenge.py
+-rw-r--r--   0        0        0     3174 2024-04-17 13:18:30.975806 authentik_client-2024.2.3.post1713359900/authentik_client/models/identification_challenge_response_request.py
+-rw-r--r--   0        0        0     7503 2024-04-17 13:18:30.979806 authentik_client-2024.2.3.post1713359900/authentik_client/models/identification_stage.py
+-rw-r--r--   0        0        0     6533 2024-04-17 13:18:30.983806 authentik_client-2024.2.3.post1713359900/authentik_client/models/identification_stage_request.py
+-rw-r--r--   0        0        0     2438 2024-04-17 13:18:30.983806 authentik_client-2024.2.3.post1713359900/authentik_client/models/install_id.py
+-rw-r--r--   0        0        0      771 2024-04-17 13:18:30.987806 authentik_client-2024.2.3.post1713359900/authentik_client/models/intent_enum.py
+-rw-r--r--   0        0        0      800 2024-04-17 13:18:30.991806 authentik_client-2024.2.3.post1713359900/authentik_client/models/invalid_response_action_enum.py
+-rw-r--r--   0        0        0     4878 2024-04-17 13:18:30.995806 authentik_client-2024.2.3.post1713359900/authentik_client/models/invitation.py
+-rw-r--r--   0        0        0     3895 2024-04-17 13:18:30.999806 authentik_client-2024.2.3.post1713359900/authentik_client/models/invitation_request.py
+-rw-r--r--   0        0        0     4508 2024-04-17 13:18:31.003806 authentik_client-2024.2.3.post1713359900/authentik_client/models/invitation_stage.py
+-rw-r--r--   0        0        0     3527 2024-04-17 13:18:31.007806 authentik_client-2024.2.3.post1713359900/authentik_client/models/invitation_stage_request.py
+-rw-r--r--   0        0        0      729 2024-04-17 13:18:31.011806 authentik_client-2024.2.3.post1713359900/authentik_client/models/issuer_mode_enum.py
+-rw-r--r--   0        0        0     4386 2024-04-17 13:18:31.015806 authentik_client-2024.2.3.post1713359900/authentik_client/models/kubernetes_service_connection.py
+-rw-r--r--   0        0        0     3454 2024-04-17 13:18:31.015806 authentik_client-2024.2.3.post1713359900/authentik_client/models/kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     2811 2024-04-17 13:18:31.023806 authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_debug.py
+-rw-r--r--   0        0        0     5765 2024-04-17 13:18:31.027806 authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_outpost_config.py
+-rw-r--r--   0        0        0     4378 2024-04-17 13:18:31.027806 authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_property_mapping.py
+-rw-r--r--   0        0        0     3478 2024-04-17 13:18:31.031806 authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     8694 2024-04-17 13:18:31.035806 authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_provider.py
+-rw-r--r--   0        0        0     6192 2024-04-17 13:18:31.039806 authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_provider_request.py
+-rw-r--r--   0        0        0    11791 2024-04-17 13:18:31.043806 authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_source.py
+-rw-r--r--   0        0        0     9542 2024-04-17 13:18:31.047806 authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_source_request.py
+-rw-r--r--   0        0        0     3129 2024-04-17 13:18:31.051806 authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_sync_status.py
+-rw-r--r--   0        0        0      726 2024-04-17 13:18:31.019806 authentik_client-2024.2.3.post1713359900/authentik_client/models/ldapapi_access_mode.py
+-rw-r--r--   0        0        0     3278 2024-04-17 13:18:31.055806 authentik_client-2024.2.3.post1713359900/authentik_client/models/license.py
+-rw-r--r--   0        0        0     2897 2024-04-17 13:18:31.059806 authentik_client-2024.2.3.post1713359900/authentik_client/models/license_forecast.py
+-rw-r--r--   0        0        0     2509 2024-04-17 13:18:31.063806 authentik_client-2024.2.3.post1713359900/authentik_client/models/license_request.py
+-rw-r--r--   0        0        0     3222 2024-04-17 13:18:31.067806 authentik_client-2024.2.3.post1713359900/authentik_client/models/license_summary.py
+-rw-r--r--   0        0        0     2411 2024-04-17 13:18:31.071806 authentik_client-2024.2.3.post1713359900/authentik_client/models/link.py
+-rw-r--r--   0        0        0     2882 2024-04-17 13:18:31.075806 authentik_client-2024.2.3.post1713359900/authentik_client/models/log_event.py
+-rw-r--r--   0        0        0      843 2024-04-17 13:18:31.079806 authentik_client-2024.2.3.post1713359900/authentik_client/models/log_level_enum.py
+-rw-r--r--   0        0        0     6520 2024-04-17 13:18:31.083806 authentik_client-2024.2.3.post1713359900/authentik_client/models/login_challenge_types.py
+-rw-r--r--   0        0        0     4171 2024-04-17 13:18:31.083806 authentik_client-2024.2.3.post1713359900/authentik_client/models/login_metrics.py
+-rw-r--r--   0        0        0     3192 2024-04-17 13:18:31.087806 authentik_client-2024.2.3.post1713359900/authentik_client/models/login_source.py
+-rw-r--r--   0        0        0     2513 2024-04-17 13:18:31.087806 authentik_client-2024.2.3.post1713359900/authentik_client/models/metadata.py
+-rw-r--r--   0        0        0     7604 2024-04-17 13:18:31.091806 authentik_client-2024.2.3.post1713359900/authentik_client/models/model_enum.py
+-rw-r--r--   0        0        0     9828 2024-04-17 13:18:31.091806 authentik_client-2024.2.3.post1713359900/authentik_client/models/model_request.py
+-rw-r--r--   0        0        0     1559 2024-04-17 13:18:31.095806 authentik_client-2024.2.3.post1713359900/authentik_client/models/name_id_policy_enum.py
+-rw-r--r--   0        0        0      831 2024-04-17 13:18:31.103806 authentik_client-2024.2.3.post1713359900/authentik_client/models/network_binding_enum.py
+-rw-r--r--   0        0        0      764 2024-04-17 13:18:31.103806 authentik_client-2024.2.3.post1713359900/authentik_client/models/not_configured_action_enum.py
+-rw-r--r--   0        0        0     3479 2024-04-17 13:18:31.107806 authentik_client-2024.2.3.post1713359900/authentik_client/models/notification.py
+-rw-r--r--   0        0        0     2858 2024-04-17 13:18:31.111806 authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_request.py
+-rw-r--r--   0        0        0     4010 2024-04-17 13:18:31.115806 authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_rule.py
+-rw-r--r--   0        0        0     3549 2024-04-17 13:18:31.119806 authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_rule_request.py
+-rw-r--r--   0        0        0     3760 2024-04-17 13:18:31.119806 authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_transport.py
+-rw-r--r--   0        0        0      818 2024-04-17 13:18:31.123806 authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_transport_mode_enum.py
+-rw-r--r--   0        0        0     3500 2024-04-17 13:18:31.127806 authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_transport_request.py
+-rw-r--r--   0        0        0     2503 2024-04-17 13:18:31.131806 authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_transport_test.py
+-rw-r--r--   0        0        0     2707 2024-04-17 13:18:31.135806 authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_webhook_mapping.py
+-rw-r--r--   0        0        0     2717 2024-04-17 13:18:31.135806 authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     8888 2024-04-17 13:18:31.139806 authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth2_provider.py
+-rw-r--r--   0        0        0     6654 2024-04-17 13:18:31.143806 authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth2_provider_request.py
+-rw-r--r--   0        0        0     3482 2024-04-17 13:18:31.147806 authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth2_provider_setup_urls.py
+-rw-r--r--   0        0        0     4164 2024-04-17 13:18:31.151806 authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth_device_code_challenge.py
+-rw-r--r--   0        0        0     2846 2024-04-17 13:18:31.155806 authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth_device_code_challenge_response_request.py
+-rw-r--r--   0        0        0     4213 2024-04-17 13:18:31.159806 authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth_device_code_finish_challenge.py
+-rw-r--r--   0        0        0     2816 2024-04-17 13:18:31.163806 authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
+-rw-r--r--   0        0        0    10563 2024-04-17 13:18:31.167806 authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth_source.py
+-rw-r--r--   0        0        0     8013 2024-04-17 13:18:31.171806 authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth_source_request.py
+-rw-r--r--   0        0        0     3922 2024-04-17 13:18:31.175806 authentik_client-2024.2.3.post1713359900/authentik_client/models/open_id_connect_configuration.py
+-rw-r--r--   0        0        0     5545 2024-04-17 13:18:31.179806 authentik_client-2024.2.3.post1713359900/authentik_client/models/outpost.py
+-rw-r--r--   0        0        0     2541 2024-04-17 13:18:31.183806 authentik_client-2024.2.3.post1713359900/authentik_client/models/outpost_default_config.py
+-rw-r--r--   0        0        0     3755 2024-04-17 13:18:31.183806 authentik_client-2024.2.3.post1713359900/authentik_client/models/outpost_health.py
+-rw-r--r--   0        0        0     4050 2024-04-17 13:18:31.187806 authentik_client-2024.2.3.post1713359900/authentik_client/models/outpost_request.py
+-rw-r--r--   0        0        0      752 2024-04-17 13:18:31.191806 authentik_client-2024.2.3.post1713359900/authentik_client/models/outpost_type_enum.py
+-rw-r--r--   0        0        0     3322 2024-04-17 13:18:31.191806 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_application_list.py
+-rw-r--r--   0        0        0     3395 2024-04-17 13:18:31.195806 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticated_session_list.py
+-rw-r--r--   0        0        0     3404 2024-04-17 13:18:31.199807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticator_duo_stage_list.py
+-rw-r--r--   0        0        0     3404 2024-04-17 13:18:31.203806 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticator_sms_stage_list.py
+-rw-r--r--   0        0        0     3428 2024-04-17 13:18:31.207806 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticator_static_stage_list.py
+-rw-r--r--   0        0        0     3412 2024-04-17 13:18:31.211806 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticator_totp_stage_list.py
+-rw-r--r--   0        0        0     3444 2024-04-17 13:18:31.215807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticator_validate_stage_list.py
+-rw-r--r--   0        0        0     3445 2024-04-17 13:18:31.215807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
+-rw-r--r--   0        0        0     3371 2024-04-17 13:18:31.219807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_blueprint_instance_list.py
+-rw-r--r--   0        0        0     3274 2024-04-17 13:18:31.223806 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_brand_list.py
+-rw-r--r--   0        0        0     3331 2024-04-17 13:18:31.227806 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_captcha_stage_list.py
+-rw-r--r--   0        0        0     3380 2024-04-17 13:18:31.231807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_certificate_key_pair_list.py
+-rw-r--r--   0        0        0     3355 2024-04-17 13:18:31.235807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_connection_token_list.py
+-rw-r--r--   0        0        0     3331 2024-04-17 13:18:31.235807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_consent_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-17 13:18:31.239807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_deny_stage_list.py
+-rw-r--r--   0        0        0     3420 2024-04-17 13:18:31.243806 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_docker_service_connection_list.py
+-rw-r--r--   0        0        0     3282 2024-04-17 13:18:31.247807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_domain_list.py
+-rw-r--r--   0        0        0     3323 2024-04-17 13:18:31.251807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_dummy_policy_list.py
+-rw-r--r--   0        0        0     3315 2024-04-17 13:18:31.255807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_dummy_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-17 13:18:31.255807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_duo_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-17 13:18:31.259807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_email_stage_list.py
+-rw-r--r--   0        0        0     3298 2024-04-17 13:18:31.263807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_endpoint_list.py
+-rw-r--r--   0        0        0     3274 2024-04-17 13:18:31.267807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_event_list.py
+-rw-r--r--   0        0        0     3380 2024-04-17 13:18:31.271807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_event_matcher_policy_list.py
+-rw-r--r--   0        0        0     3413 2024-04-17 13:18:31.275807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_expiring_base_grant_model_list.py
+-rw-r--r--   0        0        0     3363 2024-04-17 13:18:31.279807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_expression_policy_list.py
+-rw-r--r--   0        0        0     3437 2024-04-17 13:18:31.279807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_extra_role_object_permission_list.py
+-rw-r--r--   0        0        0     3437 2024-04-17 13:18:31.283807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_extra_user_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-17 13:18:31.287807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_flow_list.py
+-rw-r--r--   0        0        0     3364 2024-04-17 13:18:31.291807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_flow_stage_binding_list.py
+-rw-r--r--   0        0        0     3274 2024-04-17 13:18:31.295807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_group_list.py
+-rw-r--r--   0        0        0     3387 2024-04-17 13:18:31.295807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_identification_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-17 13:18:31.299807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_invitation_list.py
+-rw-r--r--   0        0        0     3355 2024-04-17 13:18:31.303807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_invitation_stage_list.py
+-rw-r--r--   0        0        0     3452 2024-04-17 13:18:31.303807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_kubernetes_service_connection_list.py
+-rw-r--r--   0        0        0     3372 2024-04-17 13:18:31.307807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_ldap_outpost_config_list.py
+-rw-r--r--   0        0        0     3388 2024-04-17 13:18:31.311807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_ldap_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-17 13:18:31.315807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_ldap_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-17 13:18:31.315807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_ldap_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-17 13:18:31.319807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_license_list.py
+-rw-r--r--   0        0        0     3330 2024-04-17 13:18:31.323807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_notification_list.py
+-rw-r--r--   0        0        0     3363 2024-04-17 13:18:31.323807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_notification_rule_list.py
+-rw-r--r--   0        0        0     3403 2024-04-17 13:18:31.327807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_notification_transport_list.py
+-rw-r--r--   0        0        0     3444 2024-04-17 13:18:31.331807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_notification_webhook_mapping_list.py
+-rw-r--r--   0        0        0     3348 2024-04-17 13:18:31.335807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_o_auth2_provider_list.py
+-rw-r--r--   0        0        0     3324 2024-04-17 13:18:31.335807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_o_auth_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-17 13:18:31.339807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_outpost_list.py
+-rw-r--r--   0        0        0     3396 2024-04-17 13:18:31.343807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_password_expiry_policy_list.py
+-rw-r--r--   0        0        0     3347 2024-04-17 13:18:31.347807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_password_policy_list.py
+-rw-r--r--   0        0        0     3339 2024-04-17 13:18:31.351807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_password_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-17 13:18:31.355807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_permission_list.py
+-rw-r--r--   0        0        0     3396 2024-04-17 13:18:31.359807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_plex_source_connection_list.py
+-rw-r--r--   0        0        0     3315 2024-04-17 13:18:31.359807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_plex_source_list.py
+-rw-r--r--   0        0        0     3339 2024-04-17 13:18:31.363807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_policy_binding_list.py
+-rw-r--r--   0        0        0     3282 2024-04-17 13:18:31.367807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_policy_list.py
+-rw-r--r--   0        0        0     3282 2024-04-17 13:18:31.367807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_prompt_list.py
+-rw-r--r--   0        0        0     3323 2024-04-17 13:18:31.371807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_prompt_stage_list.py
+-rw-r--r--   0        0        0     3355 2024-04-17 13:18:31.375807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_property_mapping_list.py
+-rw-r--r--   0        0        0     3298 2024-04-17 13:18:31.375807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-17 13:18:31.379807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_proxy_outpost_config_list.py
+-rw-r--r--   0        0        0     3339 2024-04-17 13:18:31.379807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_proxy_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-17 13:18:31.383807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_rac_property_mapping_list.py
+-rw-r--r--   0        0        0     3323 2024-04-17 13:18:31.387807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_rac_provider_list.py
+-rw-r--r--   0        0        0     3388 2024-04-17 13:18:31.387807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_radius_outpost_config_list.py
+-rw-r--r--   0        0        0     3347 2024-04-17 13:18:31.395807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_radius_provider_list.py
+-rw-r--r--   0        0        0     3314 2024-04-17 13:18:31.399807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_reputation_list.py
+-rw-r--r--   0        0        0     3363 2024-04-17 13:18:31.399807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_reputation_policy_list.py
+-rw-r--r--   0        0        0     3461 2024-04-17 13:18:31.403807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_role_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-17 13:18:31.407807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_role_list.py
+-rw-r--r--   0        0        0     3388 2024-04-17 13:18:31.407807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_saml_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-17 13:18:31.411807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_saml_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-17 13:18:31.415807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_saml_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-17 13:18:31.415807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_scim_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-17 13:18:31.419807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_scim_provider_list.py
+-rw-r--r--   0        0        0     3356 2024-04-17 13:18:31.423807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_scim_source_group_list.py
+-rw-r--r--   0        0        0     3315 2024-04-17 13:18:31.423807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_scim_source_list.py
+-rw-r--r--   0        0        0     3348 2024-04-17 13:18:31.427807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_scim_source_user_list.py
+-rw-r--r--   0        0        0     3331 2024-04-17 13:18:31.431807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_scope_mapping_list.py
+-rw-r--r--   0        0        0     3371 2024-04-17 13:18:31.435807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_service_connection_list.py
+-rw-r--r--   0        0        0     3307 2024-04-17 13:18:31.431807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_sms_device_list.py
+-rw-r--r--   0        0        0     3282 2024-04-17 13:18:31.439807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-17 13:18:31.439807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_source_stage_list.py
+-rw-r--r--   0        0        0     3274 2024-04-17 13:18:31.443807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_stage_list.py
+-rw-r--r--   0        0        0     3331 2024-04-17 13:18:31.447807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_static_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-17 13:18:31.447807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_system_task_list.py
+-rw-r--r--   0        0        0     3282 2024-04-17 13:18:31.451807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_tenant_list.py
+-rw-r--r--   0        0        0     3274 2024-04-17 13:18:31.455807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_token_list.py
+-rw-r--r--   0        0        0     3315 2024-04-17 13:18:31.459807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_token_model_list.py
+-rw-r--r--   0        0        0     3315 2024-04-17 13:18:31.451807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_totp_device_list.py
+-rw-r--r--   0        0        0     3461 2024-04-17 13:18:31.463807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3323 2024-04-17 13:18:31.463807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_consent_list.py
+-rw-r--r--   0        0        0     3356 2024-04-17 13:18:31.467807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_delete_stage_list.py
+-rw-r--r--   0        0        0     3266 2024-04-17 13:18:31.471807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_list.py
+-rw-r--r--   0        0        0     3348 2024-04-17 13:18:31.471807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_login_stage_list.py
+-rw-r--r--   0        0        0     3356 2024-04-17 13:18:31.475807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_logout_stage_list.py
+-rw-r--r--   0        0        0     3438 2024-04-17 13:18:31.479807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_o_auth_source_connection_list.py
+-rw-r--r--   0        0        0     3429 2024-04-17 13:18:31.479807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_saml_source_connection_list.py
+-rw-r--r--   0        0        0     3396 2024-04-17 13:18:31.483807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_source_connection_list.py
+-rw-r--r--   0        0        0     3348 2024-04-17 13:18:31.487807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_write_stage_list.py
+-rw-r--r--   0        0        0     3348 2024-04-17 13:18:31.487807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_web_authn_device_list.py
+-rw-r--r--   0        0        0     3381 2024-04-17 13:18:31.491807 authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_web_authn_device_type_list.py
+-rw-r--r--   0        0        0     3076 2024-04-17 13:18:31.491807 authentik_client-2024.2.3.post1713359900/authentik_client/models/pagination.py
+-rw-r--r--   0        0        0     4454 2024-04-17 13:18:31.495807 authentik_client-2024.2.3.post1713359900/authentik_client/models/password_challenge.py
+-rw-r--r--   0        0        0     2819 2024-04-17 13:18:31.499807 authentik_client-2024.2.3.post1713359900/authentik_client/models/password_challenge_response_request.py
+-rw-r--r--   0        0        0     4377 2024-04-17 13:18:31.499807 authentik_client-2024.2.3.post1713359900/authentik_client/models/password_expiry_policy.py
+-rw-r--r--   0        0        0     3099 2024-04-17 13:18:31.503807 authentik_client-2024.2.3.post1713359900/authentik_client/models/password_expiry_policy_request.py
+-rw-r--r--   0        0        0     6428 2024-04-17 13:18:31.503807 authentik_client-2024.2.3.post1713359900/authentik_client/models/password_policy.py
+-rw-r--r--   0        0        0     5239 2024-04-17 13:18:31.507807 authentik_client-2024.2.3.post1713359900/authentik_client/models/password_policy_request.py
+-rw-r--r--   0        0        0     5274 2024-04-17 13:18:31.511807 authentik_client-2024.2.3.post1713359900/authentik_client/models/password_stage.py
+-rw-r--r--   0        0        0     4264 2024-04-17 13:18:31.511807 authentik_client-2024.2.3.post1713359900/authentik_client/models/password_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-17 13:18:31.515807 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_application_request.py
+-rw-r--r--   0        0        0     4833 2024-04-17 13:18:31.519807 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     5701 2024-04-17 13:18:31.523807 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4430 2024-04-17 13:18:31.523807 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4256 2024-04-17 13:18:31.527807 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     4931 2024-04-17 13:18:31.531808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5340 2024-04-17 13:18:31.531808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     3246 2024-04-17 13:18:31.535807 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_blueprint_instance_request.py
+-rw-r--r--   0        0        0     6352 2024-04-17 13:18:31.535807 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_brand_request.py
+-rw-r--r--   0        0        0     3860 2024-04-17 13:18:31.539807 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_captcha_stage_request.py
+-rw-r--r--   0        0        0     3051 2024-04-17 13:18:31.543808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_certificate_key_pair_request.py
+-rw-r--r--   0        0        0     2717 2024-04-17 13:18:31.543808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_connection_token_request.py
+-rw-r--r--   0        0        0     3607 2024-04-17 13:18:31.547808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_consent_stage_request.py
+-rw-r--r--   0        0        0     3268 2024-04-17 13:18:31.547808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_deny_stage_request.py
+-rw-r--r--   0        0        0     4149 2024-04-17 13:18:31.551807 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_docker_service_connection_request.py
+-rw-r--r--   0        0        0     2801 2024-04-17 13:18:31.551807 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_domain_request.py
+-rw-r--r--   0        0        0     3275 2024-04-17 13:18:31.555807 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_dummy_policy_request.py
+-rw-r--r--   0        0        0     3270 2024-04-17 13:18:31.559808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_dummy_stage_request.py
+-rw-r--r--   0        0        0     2674 2024-04-17 13:18:31.559808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_duo_device_request.py
+-rw-r--r--   0        0        0     5159 2024-04-17 13:18:31.563808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_email_stage_request.py
+-rw-r--r--   0        0        0     3784 2024-04-17 13:18:31.563808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_endpoint_request.py
+-rw-r--r--   0        0        0     4845 2024-04-17 13:18:31.567808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_event_matcher_policy_request.py
+-rw-r--r--   0        0        0     4045 2024-04-17 13:18:31.571807 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_event_request.py
+-rw-r--r--   0        0        0     3047 2024-04-17 13:18:31.571807 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_expression_policy_request.py
+-rw-r--r--   0        0        0     4903 2024-04-17 13:18:31.575808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_flow_request.py
+-rw-r--r--   0        0        0     4055 2024-04-17 13:18:31.579808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_flow_stage_binding_request.py
+-rw-r--r--   0        0        0     3385 2024-04-17 13:18:31.583808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_group_request.py
+-rw-r--r--   0        0        0     6571 2024-04-17 13:18:31.583808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_identification_stage_request.py
+-rw-r--r--   0        0        0     3985 2024-04-17 13:18:31.587808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_invitation_request.py
+-rw-r--r--   0        0        0     3565 2024-04-17 13:18:31.591808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_invitation_stage_request.py
+-rw-r--r--   0        0        0     3492 2024-04-17 13:18:31.595808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     3550 2024-04-17 13:18:31.595808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     6254 2024-04-17 13:18:31.599808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_ldap_provider_request.py
+-rw-r--r--   0        0        0     9697 2024-04-17 13:18:31.603808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_ldap_source_request.py
+-rw-r--r--   0        0        0     2557 2024-04-17 13:18:31.603808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_license_request.py
+-rw-r--r--   0        0        0     2879 2024-04-17 13:18:31.607808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_notification_request.py
+-rw-r--r--   0        0        0     3587 2024-04-17 13:18:31.607808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_notification_rule_request.py
+-rw-r--r--   0        0        0     3538 2024-04-17 13:18:31.611808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_notification_transport_request.py
+-rw-r--r--   0        0        0     2782 2024-04-17 13:18:31.611808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     6716 2024-04-17 13:18:31.615808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_o_auth2_provider_request.py
+-rw-r--r--   0        0        0     8185 2024-04-17 13:18:31.619808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_o_auth_source_request.py
+-rw-r--r--   0        0        0     4139 2024-04-17 13:18:31.619808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_outpost_request.py
+-rw-r--r--   0        0        0     3154 2024-04-17 13:18:31.623808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_password_expiry_policy_request.py
+-rw-r--r--   0        0        0     5277 2024-04-17 13:18:31.623808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_password_policy_request.py
+-rw-r--r--   0        0        0     4326 2024-04-17 13:18:31.627808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_password_stage_request.py
+-rw-r--r--   0        0        0     2922 2024-04-17 13:18:31.635808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_permission_assign_request.py
+-rw-r--r--   0        0        0     2784 2024-04-17 13:18:31.635808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_plex_source_connection_request.py
+-rw-r--r--   0        0        0     5905 2024-04-17 13:18:31.639808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_plex_source_request.py
+-rw-r--r--   0        0        0     4286 2024-04-17 13:18:31.643808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_policy_binding_request.py
+-rw-r--r--   0        0        0     5023 2024-04-17 13:18:31.647808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_prompt_request.py
+-rw-r--r--   0        0        0     3406 2024-04-17 13:18:31.647808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_prompt_stage_request.py
+-rw-r--r--   0        0        0     6907 2024-04-17 13:18:31.651808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_proxy_provider_request.py
+-rw-r--r--   0        0        0     3495 2024-04-17 13:18:31.655808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_rac_property_mapping_request.py
+-rw-r--r--   0        0        0     4413 2024-04-17 13:18:31.655808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_rac_provider_request.py
+-rw-r--r--   0        0        0     4563 2024-04-17 13:18:31.659808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_radius_provider_request.py
+-rw-r--r--   0        0        0     3276 2024-04-17 13:18:31.659808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_reputation_policy_request.py
+-rw-r--r--   0        0        0     2565 2024-04-17 13:18:31.663808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_role_request.py
+-rw-r--r--   0        0        0     3901 2024-04-17 13:18:31.663808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_saml_property_mapping_request.py
+-rw-r--r--   0        0        0     7539 2024-04-17 13:18:31.667808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_saml_provider_request.py
+-rw-r--r--   0        0        0     8676 2024-04-17 13:18:31.667808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_saml_source_request.py
+-rw-r--r--   0        0        0     3364 2024-04-17 13:18:31.671808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_scim_mapping_request.py
+-rw-r--r--   0        0        0     3888 2024-04-17 13:18:31.675808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_scim_provider_request.py
+-rw-r--r--   0        0        0     3095 2024-04-17 13:18:31.675808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_scim_source_group_request.py
+-rw-r--r--   0        0        0     3829 2024-04-17 13:18:31.679808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_scim_source_request.py
+-rw-r--r--   0        0        0     3098 2024-04-17 13:18:31.679808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_scim_source_user_request.py
+-rw-r--r--   0        0        0     3819 2024-04-17 13:18:31.687808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_scope_mapping_request.py
+-rw-r--r--   0        0        0     5079 2024-04-17 13:18:31.691808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_settings_request.py
+-rw-r--r--   0        0        0     2674 2024-04-17 13:18:31.683808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_sms_device_request.py
+-rw-r--r--   0        0        0     3562 2024-04-17 13:18:31.695808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_source_stage_request.py
+-rw-r--r--   0        0        0     2686 2024-04-17 13:18:31.695808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_static_device_request.py
+-rw-r--r--   0        0        0     2820 2024-04-17 13:18:31.703808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_tenant_request.py
+-rw-r--r--   0        0        0     4419 2024-04-17 13:18:31.703808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_token_request.py
+-rw-r--r--   0        0        0     2678 2024-04-17 13:18:31.699808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_totp_device_request.py
+-rw-r--r--   0        0        0     3167 2024-04-17 13:18:31.707808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_delete_stage_request.py
+-rw-r--r--   0        0        0     4766 2024-04-17 13:18:31.711808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_login_stage_request.py
+-rw-r--r--   0        0        0     3167 2024-04-17 13:18:31.715808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_logout_stage_request.py
+-rw-r--r--   0        0        0     3109 2024-04-17 13:18:31.719808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3934 2024-04-17 13:18:31.719808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_request.py
+-rw-r--r--   0        0        0     2733 2024-04-17 13:18:31.723808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     4450 2024-04-17 13:18:31.727808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_write_stage_request.py
+-rw-r--r--   0        0        0     2625 2024-04-17 13:18:31.731808 authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_web_authn_device_request.py
+-rw-r--r--   0        0        0     3548 2024-04-17 13:18:31.731808 authentik_client-2024.2.3.post1713359900/authentik_client/models/permission.py
+-rw-r--r--   0        0        0     2884 2024-04-17 13:18:31.735808 authentik_client-2024.2.3.post1713359900/authentik_client/models/permission_assign_request.py
+-rw-r--r--   0        0        0     4315 2024-04-17 13:18:31.739808 authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_authentication_challenge.py
+-rw-r--r--   0        0        0     2726 2024-04-17 13:18:31.743808 authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_authentication_challenge_response_request.py
+-rw-r--r--   0        0        0     7752 2024-04-17 13:18:31.743808 authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_source.py
+-rw-r--r--   0        0        0     3265 2024-04-17 13:18:31.747808 authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_source_connection.py
+-rw-r--r--   0        0        0     2719 2024-04-17 13:18:31.751808 authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_source_connection_request.py
+-rw-r--r--   0        0        0     5760 2024-04-17 13:18:31.755808 authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_source_request.py
+-rw-r--r--   0        0        0     2576 2024-04-17 13:18:31.755808 authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_token_redeem_request.py
+-rw-r--r--   0        0        0     4055 2024-04-17 13:18:31.759808 authentik_client-2024.2.3.post1713359900/authentik_client/models/policy.py
+-rw-r--r--   0        0        0     5643 2024-04-17 13:18:31.759808 authentik_client-2024.2.3.post1713359900/authentik_client/models/policy_binding.py
+-rw-r--r--   0        0        0     4231 2024-04-17 13:18:31.763808 authentik_client-2024.2.3.post1713359900/authentik_client/models/policy_binding_request.py
+-rw-r--r--   0        0        0      711 2024-04-17 13:18:31.763808 authentik_client-2024.2.3.post1713359900/authentik_client/models/policy_engine_mode.py
+-rw-r--r--   0        0        0     2817 2024-04-17 13:18:31.767808 authentik_client-2024.2.3.post1713359900/authentik_client/models/policy_request.py
+-rw-r--r--   0        0        0     2583 2024-04-17 13:18:31.771808 authentik_client-2024.2.3.post1713359900/authentik_client/models/policy_test_request.py
+-rw-r--r--   0        0        0     3281 2024-04-17 13:18:31.771808 authentik_client-2024.2.3.post1713359900/authentik_client/models/policy_test_result.py
+-rw-r--r--   0        0        0     4885 2024-04-17 13:18:31.775808 authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt.py
+-rw-r--r--   0        0        0     4649 2024-04-17 13:18:31.779808 authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt_challenge.py
+-rw-r--r--   0        0        0     3325 2024-04-17 13:18:31.783808 authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt_challenge_response_request.py
+-rw-r--r--   0        0        0     4927 2024-04-17 13:18:31.783808 authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt_request.py
+-rw-r--r--   0        0        0     4321 2024-04-17 13:18:31.787808 authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt_stage.py
+-rw-r--r--   0        0        0     3351 2024-04-17 13:18:31.791808 authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt_stage_request.py
+-rw-r--r--   0        0        0     1185 2024-04-17 13:18:31.791808 authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt_type_enum.py
+-rw-r--r--   0        0        0     4264 2024-04-17 13:18:31.795808 authentik_client-2024.2.3.post1713359900/authentik_client/models/property_mapping.py
+-rw-r--r--   0        0        0     2610 2024-04-17 13:18:31.795808 authentik_client-2024.2.3.post1713359900/authentik_client/models/property_mapping_preview.py
+-rw-r--r--   0        0        0     2744 2024-04-17 13:18:31.799808 authentik_client-2024.2.3.post1713359900/authentik_client/models/property_mapping_test_result.py
+-rw-r--r--   0        0        0      715 2024-04-17 13:18:31.799808 authentik_client-2024.2.3.post1713359900/authentik_client/models/protocol_enum.py
+-rw-r--r--   0        0        0     5722 2024-04-17 13:18:31.803808 authentik_client-2024.2.3.post1713359900/authentik_client/models/provider.py
+-rw-r--r--   0        0        0      713 2024-04-17 13:18:31.803808 authentik_client-2024.2.3.post1713359900/authentik_client/models/provider_enum.py
+-rw-r--r--   0        0        0     1314 2024-04-17 13:18:31.803808 authentik_client-2024.2.3.post1713359900/authentik_client/models/provider_model_enum.py
+-rw-r--r--   0        0        0     3397 2024-04-17 13:18:31.807808 authentik_client-2024.2.3.post1713359900/authentik_client/models/provider_request.py
+-rw-r--r--   0        0        0     1009 2024-04-17 13:18:31.807808 authentik_client-2024.2.3.post1713359900/authentik_client/models/provider_type_enum.py
+-rw-r--r--   0        0        0      754 2024-04-17 13:18:31.807808 authentik_client-2024.2.3.post1713359900/authentik_client/models/proxy_mode.py
+-rw-r--r--   0        0        0     7819 2024-04-17 13:18:31.811808 authentik_client-2024.2.3.post1713359900/authentik_client/models/proxy_outpost_config.py
+-rw-r--r--   0        0        0     9552 2024-04-17 13:18:31.811808 authentik_client-2024.2.3.post1713359900/authentik_client/models/proxy_provider.py
+-rw-r--r--   0        0        0     6828 2024-04-17 13:18:31.815808 authentik_client-2024.2.3.post1713359900/authentik_client/models/proxy_provider_request.py
+-rw-r--r--   0        0        0     4407 2024-04-17 13:18:31.815808 authentik_client-2024.2.3.post1713359900/authentik_client/models/rac_property_mapping.py
+-rw-r--r--   0        0        0     3440 2024-04-17 13:18:31.819808 authentik_client-2024.2.3.post1713359900/authentik_client/models/rac_property_mapping_request.py
+-rw-r--r--   0        0        0     6813 2024-04-17 13:18:31.819808 authentik_client-2024.2.3.post1713359900/authentik_client/models/rac_provider.py
+-rw-r--r--   0        0        0     4351 2024-04-17 13:18:31.823808 authentik_client-2024.2.3.post1713359900/authentik_client/models/rac_provider_request.py
+-rw-r--r--   0        0        0     3833 2024-04-17 13:18:31.823808 authentik_client-2024.2.3.post1713359900/authentik_client/models/radius_outpost_config.py
+-rw-r--r--   0        0        0     6924 2024-04-17 13:18:31.827808 authentik_client-2024.2.3.post1713359900/authentik_client/models/radius_provider.py
+-rw-r--r--   0        0        0     4501 2024-04-17 13:18:31.831808 authentik_client-2024.2.3.post1713359900/authentik_client/models/radius_provider_request.py
+-rw-r--r--   0        0        0     4184 2024-04-17 13:18:31.831808 authentik_client-2024.2.3.post1713359900/authentik_client/models/redirect_challenge.py
+-rw-r--r--   0        0        0     3642 2024-04-17 13:18:31.835808 authentik_client-2024.2.3.post1713359900/authentik_client/models/reputation.py
+-rw-r--r--   0        0        0     4516 2024-04-17 13:18:31.839808 authentik_client-2024.2.3.post1713359900/authentik_client/models/reputation_policy.py
+-rw-r--r--   0        0        0     3238 2024-04-17 13:18:31.839808 authentik_client-2024.2.3.post1713359900/authentik_client/models/reputation_policy_request.py
+-rw-r--r--   0        0        0      795 2024-04-17 13:18:31.839808 authentik_client-2024.2.3.post1713359900/authentik_client/models/resident_key_requirement_enum.py
+-rw-r--r--   0        0        0     2618 2024-04-17 13:18:31.843809 authentik_client-2024.2.3.post1713359900/authentik_client/models/role.py
+-rw-r--r--   0        0        0     3333 2024-04-17 13:18:31.843809 authentik_client-2024.2.3.post1713359900/authentik_client/models/role_assigned_object_permission.py
+-rw-r--r--   0        0        0     3293 2024-04-17 13:18:31.847808 authentik_client-2024.2.3.post1713359900/authentik_client/models/role_object_permission.py
+-rw-r--r--   0        0        0     2517 2024-04-17 13:18:31.847808 authentik_client-2024.2.3.post1713359900/authentik_client/models/role_request.py
+-rw-r--r--   0        0        0     2712 2024-04-17 13:18:31.851808 authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_metadata.py
+-rw-r--r--   0        0        0     4718 2024-04-17 13:18:31.855808 authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_property_mapping.py
+-rw-r--r--   0        0        0     3829 2024-04-17 13:18:31.855808 authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_property_mapping_request.py
+-rw-r--r--   0        0        0    11056 2024-04-17 13:18:31.859809 authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_provider.py
+-rw-r--r--   0        0        0     7460 2024-04-17 13:18:31.859809 authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_provider_request.py
+-rw-r--r--   0        0        0    10563 2024-04-17 13:18:31.863808 authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_source.py
+-rw-r--r--   0        0        0     8507 2024-04-17 13:18:31.867808 authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_source_request.py
+-rw-r--r--   0        0        0     4248 2024-04-17 13:18:31.867808 authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_mapping.py
+-rw-r--r--   0        0        0     3309 2024-04-17 13:18:31.871808 authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_mapping_request.py
+-rw-r--r--   0        0        0     5454 2024-04-17 13:18:31.875809 authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_provider.py
+-rw-r--r--   0        0        0     3802 2024-04-17 13:18:31.875809 authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_provider_request.py
+-rw-r--r--   0        0        0     5999 2024-04-17 13:18:31.879809 authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_source.py
+-rw-r--r--   0        0        0     3369 2024-04-17 13:18:31.883808 authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_source_group.py
+-rw-r--r--   0        0        0     3023 2024-04-17 13:18:31.883808 authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_source_group_request.py
+-rw-r--r--   0        0        0     3708 2024-04-17 13:18:31.887808 authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_source_request.py
+-rw-r--r--   0        0        0     3370 2024-04-17 13:18:31.895809 authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_source_user.py
+-rw-r--r--   0        0        0     3026 2024-04-17 13:18:31.899809 authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_source_user_request.py
+-rw-r--r--   0        0        0     3131 2024-04-17 13:18:31.903809 authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_sync_status.py
+-rw-r--r--   0        0        0     4629 2024-04-17 13:18:31.911809 authentik_client-2024.2.3.post1713359900/authentik_client/models/scope_mapping.py
+-rw-r--r--   0        0        0     3740 2024-04-17 13:18:31.911809 authentik_client-2024.2.3.post1713359900/authentik_client/models/scope_mapping_request.py
+-rw-r--r--   0        0        0     2738 2024-04-17 13:18:31.915809 authentik_client-2024.2.3.post1713359900/authentik_client/models/selectable_stage.py
+-rw-r--r--   0        0        0     3773 2024-04-17 13:18:31.919809 authentik_client-2024.2.3.post1713359900/authentik_client/models/service_connection.py
+-rw-r--r--   0        0        0     2776 2024-04-17 13:18:31.919809 authentik_client-2024.2.3.post1713359900/authentik_client/models/service_connection_request.py
+-rw-r--r--   0        0        0     2731 2024-04-17 13:18:31.923809 authentik_client-2024.2.3.post1713359900/authentik_client/models/service_connection_state.py
+-rw-r--r--   0        0        0     3178 2024-04-17 13:18:31.927809 authentik_client-2024.2.3.post1713359900/authentik_client/models/session_user.py
+-rw-r--r--   0        0        0     4931 2024-04-17 13:18:31.931809 authentik_client-2024.2.3.post1713359900/authentik_client/models/settings.py
+-rw-r--r--   0        0        0     5058 2024-04-17 13:18:31.931809 authentik_client-2024.2.3.post1713359900/authentik_client/models/settings_request.py
+-rw-r--r--   0        0        0      733 2024-04-17 13:18:31.935809 authentik_client-2024.2.3.post1713359900/authentik_client/models/severity_enum.py
+-rw-r--r--   0        0        0     4175 2024-04-17 13:18:31.939809 authentik_client-2024.2.3.post1713359900/authentik_client/models/shell_challenge.py
+-rw-r--r--   0        0        0     1492 2024-04-17 13:18:31.939809 authentik_client-2024.2.3.post1713359900/authentik_client/models/signature_algorithm_enum.py
+-rw-r--r--   0        0        0     2906 2024-04-17 13:18:31.903809 authentik_client-2024.2.3.post1713359900/authentik_client/models/sms_device.py
+-rw-r--r--   0        0        0     2619 2024-04-17 13:18:31.907809 authentik_client-2024.2.3.post1713359900/authentik_client/models/sms_device_request.py
+-rw-r--r--   0        0        0     6945 2024-04-17 13:18:31.943809 authentik_client-2024.2.3.post1713359900/authentik_client/models/source.py
+-rw-r--r--   0        0        0     4836 2024-04-17 13:18:31.947809 authentik_client-2024.2.3.post1713359900/authentik_client/models/source_request.py
+-rw-r--r--   0        0        0     4438 2024-04-17 13:18:31.951809 authentik_client-2024.2.3.post1713359900/authentik_client/models/source_stage.py
+-rw-r--r--   0        0        0     3507 2024-04-17 13:18:31.955809 authentik_client-2024.2.3.post1713359900/authentik_client/models/source_stage_request.py
+-rw-r--r--   0        0        0     5355 2024-04-17 13:18:31.955809 authentik_client-2024.2.3.post1713359900/authentik_client/models/source_type.py
+-rw-r--r--   0        0        0      714 2024-04-17 13:18:31.959809 authentik_client-2024.2.3.post1713359900/authentik_client/models/sp_binding_enum.py
+-rw-r--r--   0        0        0     4070 2024-04-17 13:18:31.959809 authentik_client-2024.2.3.post1713359900/authentik_client/models/stage.py
+-rw-r--r--   0        0        0     3437 2024-04-17 13:18:31.963809 authentik_client-2024.2.3.post1713359900/authentik_client/models/stage_prompt.py
+-rw-r--r--   0        0        0     3089 2024-04-17 13:18:31.967809 authentik_client-2024.2.3.post1713359900/authentik_client/models/stage_request.py
+-rw-r--r--   0        0        0     3385 2024-04-17 13:18:31.971809 authentik_client-2024.2.3.post1713359900/authentik_client/models/static_device.py
+-rw-r--r--   0        0        0     2631 2024-04-17 13:18:31.971809 authentik_client-2024.2.3.post1713359900/authentik_client/models/static_device_request.py
+-rw-r--r--   0        0        0     2546 2024-04-17 13:18:31.975809 authentik_client-2024.2.3.post1713359900/authentik_client/models/static_device_token.py
+-rw-r--r--   0        0        0     2581 2024-04-17 13:18:31.979809 authentik_client-2024.2.3.post1713359900/authentik_client/models/static_device_token_request.py
+-rw-r--r--   0        0        0      846 2024-04-17 13:18:31.979809 authentik_client-2024.2.3.post1713359900/authentik_client/models/sub_mode_enum.py
+-rw-r--r--   0        0        0     4463 2024-04-17 13:18:31.983809 authentik_client-2024.2.3.post1713359900/authentik_client/models/system_info.py
+-rw-r--r--   0        0        0     2934 2024-04-17 13:18:31.983809 authentik_client-2024.2.3.post1713359900/authentik_client/models/system_info_runtime.py
+-rw-r--r--   0        0        0     4286 2024-04-17 13:18:31.987809 authentik_client-2024.2.3.post1713359900/authentik_client/models/system_task.py
+-rw-r--r--   0        0        0      789 2024-04-17 13:18:31.991809 authentik_client-2024.2.3.post1713359900/authentik_client/models/system_task_status_enum.py
+-rw-r--r--   0        0        0     2872 2024-04-17 13:18:31.995809 authentik_client-2024.2.3.post1713359900/authentik_client/models/tenant.py
+-rw-r--r--   0        0        0     2589 2024-04-17 13:18:31.999809 authentik_client-2024.2.3.post1713359900/authentik_client/models/tenant_admin_group_request_request.py
+-rw-r--r--   0        0        0     2705 2024-04-17 13:18:32.003809 authentik_client-2024.2.3.post1713359900/authentik_client/models/tenant_recovery_key_request_request.py
+-rw-r--r--   0        0        0     2599 2024-04-17 13:18:32.003809 authentik_client-2024.2.3.post1713359900/authentik_client/models/tenant_recovery_key_response.py
+-rw-r--r--   0        0        0     2765 2024-04-17 13:18:32.007809 authentik_client-2024.2.3.post1713359900/authentik_client/models/tenant_request.py
+-rw-r--r--   0        0        0     4802 2024-04-17 13:18:32.011809 authentik_client-2024.2.3.post1713359900/authentik_client/models/token.py
+-rw-r--r--   0        0        0     4198 2024-04-17 13:18:32.015809 authentik_client-2024.2.3.post1713359900/authentik_client/models/token_model.py
+-rw-r--r--   0        0        0     4329 2024-04-17 13:18:32.015809 authentik_client-2024.2.3.post1713359900/authentik_client/models/token_request.py
+-rw-r--r--   0        0        0     2521 2024-04-17 13:18:32.019809 authentik_client-2024.2.3.post1713359900/authentik_client/models/token_set_key_request.py
+-rw-r--r--   0        0        0     2494 2024-04-17 13:18:32.023809 authentik_client-2024.2.3.post1713359900/authentik_client/models/token_view.py
+-rw-r--r--   0        0        0     2724 2024-04-17 13:18:31.991809 authentik_client-2024.2.3.post1713359900/authentik_client/models/totp_device.py
+-rw-r--r--   0        0        0     2623 2024-04-17 13:18:31.995809 authentik_client-2024.2.3.post1713359900/authentik_client/models/totp_device_request.py
+-rw-r--r--   0        0        0     3389 2024-04-17 13:18:32.023809 authentik_client-2024.2.3.post1713359900/authentik_client/models/transaction_application_request.py
+-rw-r--r--   0        0        0     2595 2024-04-17 13:18:32.027809 authentik_client-2024.2.3.post1713359900/authentik_client/models/transaction_application_response.py
+-rw-r--r--   0        0        0     2936 2024-04-17 13:18:32.031809 authentik_client-2024.2.3.post1713359900/authentik_client/models/type_create.py
+-rw-r--r--   0        0        0      730 2024-04-17 13:18:32.031809 authentik_client-2024.2.3.post1713359900/authentik_client/models/ui_theme_enum.py
+-rw-r--r--   0        0        0     2808 2024-04-17 13:18:32.035809 authentik_client-2024.2.3.post1713359900/authentik_client/models/used_by.py
+-rw-r--r--   0        0        0      795 2024-04-17 13:18:32.035809 authentik_client-2024.2.3.post1713359900/authentik_client/models/used_by_action_enum.py
+-rw-r--r--   0        0        0     5459 2024-04-17 13:18:32.039809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user.py
+-rw-r--r--   0        0        0     2458 2024-04-17 13:18:32.039809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_account_request.py
+-rw-r--r--   0        0        0     4946 2024-04-17 13:18:32.043809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_assigned_object_permission.py
+-rw-r--r--   0        0        0     3828 2024-04-17 13:18:32.047809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_consent.py
+-rw-r--r--   0        0        0      811 2024-04-17 13:18:32.047809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_creation_mode_enum.py
+-rw-r--r--   0        0        0     4110 2024-04-17 13:18:32.051809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_delete_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-17 13:18:32.051809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_delete_stage_request.py
+-rw-r--r--   0        0        0      735 2024-04-17 13:18:32.055809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_fields_enum.py
+-rw-r--r--   0        0        0     3909 2024-04-17 13:18:32.055809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_group.py
+-rw-r--r--   0        0        0     4334 2024-04-17 13:18:32.059809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_login_challenge.py
+-rw-r--r--   0        0        0     2805 2024-04-17 13:18:32.059809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_login_challenge_response_request.py
+-rw-r--r--   0        0        0     5631 2024-04-17 13:18:32.063809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_login_stage.py
+-rw-r--r--   0        0        0     4728 2024-04-17 13:18:32.063809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_login_stage_request.py
+-rw-r--r--   0        0        0     4110 2024-04-17 13:18:32.067809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_logout_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-17 13:18:32.067809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_logout_stage_request.py
+-rw-r--r--   0        0        0      853 2024-04-17 13:18:32.067809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_matching_mode_enum.py
+-rw-r--r--   0        0        0     4160 2024-04-17 13:18:32.071809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_metrics.py
+-rw-r--r--   0        0        0     3188 2024-04-17 13:18:32.071809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_o_auth_source_connection.py
+-rw-r--r--   0        0        0     3054 2024-04-17 13:18:32.075809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3293 2024-04-17 13:18:32.075809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_object_permission.py
+-rw-r--r--   0        0        0     2557 2024-04-17 13:18:32.079809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_password_set_request.py
+-rw-r--r--   0        0        0     2491 2024-04-17 13:18:32.079809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_path.py
+-rw-r--r--   0        0        0     3872 2024-04-17 13:18:32.083809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_request.py
+-rw-r--r--   0        0        0     3107 2024-04-17 13:18:32.087809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_saml_source_connection.py
+-rw-r--r--   0        0        0     2668 2024-04-17 13:18:32.087809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     5465 2024-04-17 13:18:32.091809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_self.py
+-rw-r--r--   0        0        0     2629 2024-04-17 13:18:32.091809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_self_groups.py
+-rw-r--r--   0        0        0     3074 2024-04-17 13:18:32.095809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_service_account_request.py
+-rw-r--r--   0        0        0     2844 2024-04-17 13:18:32.099809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_service_account_response.py
+-rw-r--r--   0        0        0     2866 2024-04-17 13:18:32.099809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_setting.py
+-rw-r--r--   0        0        0     3245 2024-04-17 13:18:32.103809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_source_connection.py
+-rw-r--r--   0        0        0      817 2024-04-17 13:18:32.103809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_type_enum.py
+-rw-r--r--   0        0        0      777 2024-04-17 13:18:32.103809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_verification_enum.py
+-rw-r--r--   0        0        0     5382 2024-04-17 13:18:32.107809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_write_stage.py
+-rw-r--r--   0        0        0     4412 2024-04-17 13:18:32.111809 authentik_client-2024.2.3.post1713359900/authentik_client/models/user_write_stage_request.py
+-rw-r--r--   0        0        0     3197 2024-04-17 13:18:32.111809 authentik_client-2024.2.3.post1713359900/authentik_client/models/validation_error.py
+-rw-r--r--   0        0        0     3589 2024-04-17 13:18:32.115809 authentik_client-2024.2.3.post1713359900/authentik_client/models/version.py
+-rw-r--r--   0        0        0     3630 2024-04-17 13:18:32.119809 authentik_client-2024.2.3.post1713359900/authentik_client/models/web_authn_device.py
+-rw-r--r--   0        0        0     2577 2024-04-17 13:18:32.119809 authentik_client-2024.2.3.post1713359900/authentik_client/models/web_authn_device_request.py
+-rw-r--r--   0        0        0     2562 2024-04-17 13:18:32.123809 authentik_client-2024.2.3.post1713359900/authentik_client/models/web_authn_device_type.py
+-rw-r--r--   0        0        0     2669 2024-04-17 13:18:32.123809 authentik_client-2024.2.3.post1713359900/authentik_client/models/web_authn_device_type_request.py
+-rw-r--r--   0        0        0     2410 2024-04-17 13:18:32.127809 authentik_client-2024.2.3.post1713359900/authentik_client/models/workers.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:18:33.223813 authentik_client-2024.2.3.post1713359900/authentik_client/py.typed
+-rw-r--r--   0        0        0     9196 2024-04-17 13:18:33.231813 authentik_client-2024.2.3.post1713359900/authentik_client/rest.py
+-rw-r--r--   0        0        0     1936 2024-04-17 13:18:33.223813 authentik_client-2024.2.3.post1713359900/pyproject.toml
+-rw-r--r--   0        0        0   144847 1970-01-01 00:00:00.000000 authentik_client-2024.2.3.post1713359900/PKG-INFO
```

### Comparing `authentik_client-2024.2.2.post1713289429/README.md` & `authentik_client-2024.2.3.post1713359900/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2024.2.2
-- Package version: 2024.2.2-1713289429
+- API version: 2024.2.3
+- Package version: 2024.2.3-1713359900
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/__init__.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2024.2.2-1713289429"
+__version__ = "2024.2.3-1713359900"
 
 # import apis into sdk package
 from authentik_client.api.admin_api import AdminApi
 from authentik_client.api.authenticators_api import AuthenticatorsApi
 from authentik_client.api.core_api import CoreApi
 from authentik_client.api.crypto_api import CryptoApi
 from authentik_client.api.enterprise_api import EnterpriseApi
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/__init__.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/admin_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/admin_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/authenticators_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/authenticators_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/core_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/core_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/crypto_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/crypto_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/enterprise_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/enterprise_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/events_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/events_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/flows_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/flows_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/managed_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/managed_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/oauth2_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/oauth2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/outposts_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/outposts_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/policies_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/policies_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/propertymappings_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/propertymappings_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/providers_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/providers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/rac_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/rac_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/rbac_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/rbac_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/root_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/root_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/schema_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/schema_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/sources_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/sources_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/stages_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/stages_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api/tenants_api.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api/tenants_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api_client.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2024.2.2-1713289429/python'
+        self.user_agent = 'OpenAPI-Generator/2024.2.3-1713359900/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/api_response.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/api_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/configuration.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -374,16 +374,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2024.2.2\n"\
-               "SDK Package Version: 2024.2.2-1713289429".\
+               "Version of the API: 2024.2.3\n"\
+               "SDK Package Version: 2024.2.3-1713359900".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/exceptions.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/__init__.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/access_denied_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/access_denied_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/app.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/app_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/app_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/apple_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/apple_challenge_response_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/apple_login_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/apple_login_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/application.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/application_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/application_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/auth_mode_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/auth_mode_enum.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/auth_type_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/auth_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_asn.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session_asn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_geo_ip.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session_geo_ip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session_user_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent_device.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session_user_agent_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent_os.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session_user_agent_os.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent_user_agent.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticated_session_user_agent_user_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authentication_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authentication_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_attachment_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_attachment_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_duo_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_duo_challenge_response_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_duo_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage_device_import_response.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_duo_stage_device_import_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_duo_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_sms_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_sms_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_sms_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_sms_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_static_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_static_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_static_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_static_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_totp_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_totp_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_totp_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_totp_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validate_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_validate_stage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validate_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_validate_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validation_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_validation_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validation_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_validation_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_web_authn_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_web_authn_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_web_authn_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/authenticator_web_authn_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/auto_submit_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/auto_submit_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/autosubmit_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/autosubmit_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/backends_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/backends_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/binding_type_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/binding_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_file.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/blueprint_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_instance.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/blueprint_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_instance_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/blueprint_instance_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_instance_status_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/blueprint_instance_status_enum.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/brand.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/brand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/brand_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/brand_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/cache.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/capabilities_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/capabilities_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/captcha_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/captcha_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/captcha_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/captcha_stage_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_data.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/certificate_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_generation_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/certificate_generation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_key_pair.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/certificate_key_pair.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_key_pair_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/certificate_key_pair_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/challenge_choices.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/challenge_choices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/challenge_types.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/challenge_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/client_type_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/client_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/config.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/connection_token.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/connection_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/connection_token_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/connection_token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/consent_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/consent_challenge_response_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_permission.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/consent_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/consent_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_stage_mode_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/consent_stage_mode_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/consent_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/contextual_flow_info.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/contextual_flow_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/contextual_flow_info_layout_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/contextual_flow_info_layout_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/coordinate.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/coordinate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/current_brand.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/current_brand.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/denied_action_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/denied_action_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/deny_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/deny_stage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/deny_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/deny_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/device.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/device_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/device_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/device_challenge_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/device_challenge_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/device_classes_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/device_classes_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/digest_algorithm_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/digest_algorithm_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/digits_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/intent_enum.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class DigitsEnum(str, Enum):
+class IntentEnum(str, Enum):
     """
-    DigitsEnum
+    IntentEnum
     """
 
     """
     allowed enum values
     """
-    ENUM_6 = '6'
-    ENUM_8 = '8'
+    VERIFICATION = 'verification'
+    API = 'api'
+    RECOVERY = 'recovery'
+    APP_PASSWORD = 'app_password'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of DigitsEnum from a JSON string"""
+        """Create an instance of IntentEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/docker_service_connection.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/docker_service_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/docker_service_connection_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/docker_service_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/domain.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/domain_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/domain_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/dummy_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/dummy_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_policy.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/dummy_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_policy_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/dummy_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/dummy_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/dummy_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_device.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/duo_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_device_enrollment_status.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/duo_device_enrollment_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_device_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/duo_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_response_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/provider_enum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class DuoResponseEnum(str, Enum):
+class ProviderEnum(str, Enum):
     """
-    DuoResponseEnum
+    ProviderEnum
     """
 
     """
     allowed enum values
     """
-    SUCCESS = 'success'
-    WAITING = 'waiting'
-    INVALID = 'invalid'
+    TWILIO = 'twilio'
+    GENERIC = 'generic'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of DuoResponseEnum from a JSON string"""
+        """Create an instance of ProviderEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/email_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/email_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/email_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/email_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/email_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/email_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/email_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/email_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/endpoint.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/endpoint_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/endpoint_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/error_detail.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/error_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/error_reporting_config.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/error_reporting_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/event.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/event_actions.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/event_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/event_matcher_policy.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/event_matcher_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/event_matcher_policy_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/event_matcher_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/event_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/event_top_per_user.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/event_top_per_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/expiring_base_grant_model.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/expiring_base_grant_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/expression_policy.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/expression_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/expression_policy_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/expression_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/extra_role_object_permission.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/extra_role_object_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/extra_user_object_permission.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/extra_user_object_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/file_path_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/file_path_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_designation_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_designation_enum.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_diagram.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_diagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_error_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_error_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_import_result.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_import_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_inspection.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_inspection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_inspector_plan.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_inspector_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_layout_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_layout_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_set.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_set_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_stage_binding.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_stage_binding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_stage_binding_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/flow_stage_binding_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/footer_link.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/footer_link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/generic_error.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/generic_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/geoip_binding_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/geoip_binding_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/group.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/group_member.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/group_member.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/group_member_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/group_member_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/group_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/identification_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/identification_challenge_response_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/identification_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/identification_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/install_id.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/install_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/intent_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/not_configured_action_enum.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class IntentEnum(str, Enum):
+class NotConfiguredActionEnum(str, Enum):
     """
-    IntentEnum
+    NotConfiguredActionEnum
     """
 
     """
     allowed enum values
     """
-    VERIFICATION = 'verification'
-    API = 'api'
-    RECOVERY = 'recovery'
-    APP_PASSWORD = 'app_password'
+    SKIP = 'skip'
+    DENY = 'deny'
+    CONFIGURE = 'configure'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of IntentEnum from a JSON string"""
+        """Create an instance of NotConfiguredActionEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/invalid_response_action_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/invalid_response_action_enum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/invitation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/invitation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/invitation_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/invitation_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/issuer_mode_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/issuer_mode_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/kubernetes_service_connection.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/kubernetes_service_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/kubernetes_service_connection_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/kubernetes_service_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_debug.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_outpost_config.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_outpost_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_property_mapping.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_property_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_property_mapping_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_property_mapping_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_provider.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_provider_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_source.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_source_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_sync_status.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/ldap_sync_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldapapi_access_mode.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/ldapapi_access_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/license.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/license.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/license_forecast.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/license_forecast.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/license_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/license_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/license_summary.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/license_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/link.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/log_event.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/log_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/log_level_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/log_level_enum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/login_challenge_types.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/login_challenge_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/login_metrics.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/login_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/login_source.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/login_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/metadata.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/model_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/model_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/model_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/model_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/name_id_policy_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/name_id_policy_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/network_binding_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/network_binding_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/not_configured_action_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_verification_enum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class NotConfiguredActionEnum(str, Enum):
+class UserVerificationEnum(str, Enum):
     """
-    NotConfiguredActionEnum
+    UserVerificationEnum
     """
 
     """
     allowed enum values
     """
-    SKIP = 'skip'
-    DENY = 'deny'
-    CONFIGURE = 'configure'
+    REQUIRED = 'required'
+    PREFERRED = 'preferred'
+    DISCOURAGED = 'discouraged'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of NotConfiguredActionEnum from a JSON string"""
+        """Create an instance of UserVerificationEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_rule.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_rule_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_rule_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport_mode_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_transport_mode_enum.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_transport_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport_test.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_transport_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_webhook_mapping.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_webhook_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_webhook_mapping_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/notification_webhook_mapping_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth2_provider.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth2_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth2_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth2_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth2_provider_setup_urls.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth2_provider_setup_urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth_device_code_challenge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth_device_code_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_finish_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth_device_code_finish_challenge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_source.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_source_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/o_auth_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/open_id_connect_configuration.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/open_id_connect_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/outpost.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_default_config.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/outpost_default_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_health.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/outpost_health.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/outpost_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_type_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/outpost_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_application_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_application_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticated_session_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticated_session_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_duo_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticator_duo_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_sms_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticator_sms_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_static_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticator_static_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_totp_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticator_totp_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_validate_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticator_validate_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_web_authn_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_authenticator_web_authn_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_blueprint_instance_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_blueprint_instance_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_brand_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_brand_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_captcha_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_captcha_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_certificate_key_pair_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_certificate_key_pair_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_connection_token_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_connection_token_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_consent_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_consent_stage_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_deny_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_deny_stage_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_docker_service_connection_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_docker_service_connection_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_domain_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_domain_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_dummy_policy_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_dummy_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_dummy_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_stage_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from authentik_client.models.dummy_stage import DummyStage
 from authentik_client.models.pagination import Pagination
+from authentik_client.models.stage import Stage
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedDummyStageList(BaseModel):
+class PaginatedStageList(BaseModel):
     """
-    PaginatedDummyStageList
+    PaginatedStageList
     """ # noqa: E501
     pagination: Pagination
-    results: List[DummyStage]
+    results: List[Stage]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedDummyStageList from a JSON string"""
+        """Create an instance of PaginatedStageList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedDummyStageList from a dict"""
+        """Create an instance of PaginatedStageList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [DummyStage.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [Stage.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_duo_device_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_duo_device_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_email_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_email_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_endpoint_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_event_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from authentik_client.models.endpoint import Endpoint
+from authentik_client.models.event import Event
 from authentik_client.models.pagination import Pagination
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedEndpointList(BaseModel):
+class PaginatedEventList(BaseModel):
     """
-    PaginatedEndpointList
+    PaginatedEventList
     """ # noqa: E501
     pagination: Pagination
-    results: List[Endpoint]
+    results: List[Event]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedEndpointList from a JSON string"""
+        """Create an instance of PaginatedEventList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedEndpointList from a dict"""
+        """Create an instance of PaginatedEventList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [Endpoint.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [Event.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_event_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_ldap_provider_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from authentik_client.models.event import Event
+from authentik_client.models.ldap_provider import LDAPProvider
 from authentik_client.models.pagination import Pagination
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedEventList(BaseModel):
+class PaginatedLDAPProviderList(BaseModel):
     """
-    PaginatedEventList
+    PaginatedLDAPProviderList
     """ # noqa: E501
     pagination: Pagination
-    results: List[Event]
+    results: List[LDAPProvider]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedEventList from a JSON string"""
+        """Create an instance of PaginatedLDAPProviderList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedEventList from a dict"""
+        """Create an instance of PaginatedLDAPProviderList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [Event.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [LDAPProvider.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_event_matcher_policy_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_event_matcher_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_expiring_base_grant_model_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_expiring_base_grant_model_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_expression_policy_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_expression_policy_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_extra_role_object_permission_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_extra_role_object_permission_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_extra_user_object_permission_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_extra_user_object_permission_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_flow_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_flow_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_flow_stage_binding_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_flow_stage_binding_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_group_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_group_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_identification_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_identification_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_invitation_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_invitation_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_invitation_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_invitation_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_kubernetes_service_connection_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_kubernetes_service_connection_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_outpost_config_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_ldap_outpost_config_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_property_mapping_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_ldap_property_mapping_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_provider_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_saml_provider_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from authentik_client.models.ldap_provider import LDAPProvider
 from authentik_client.models.pagination import Pagination
+from authentik_client.models.saml_provider import SAMLProvider
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedLDAPProviderList(BaseModel):
+class PaginatedSAMLProviderList(BaseModel):
     """
-    PaginatedLDAPProviderList
+    PaginatedSAMLProviderList
     """ # noqa: E501
     pagination: Pagination
-    results: List[LDAPProvider]
+    results: List[SAMLProvider]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedLDAPProviderList from a JSON string"""
+        """Create an instance of PaginatedSAMLProviderList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedLDAPProviderList from a dict"""
+        """Create an instance of PaginatedSAMLProviderList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [LDAPProvider.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [SAMLProvider.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_source_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_ldap_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_license_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_license_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_notification_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_rule_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_notification_rule_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_transport_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_notification_transport_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_webhook_mapping_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_notification_webhook_mapping_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_o_auth2_provider_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_o_auth2_provider_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_o_auth_source_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_o_auth_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_outpost_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_outpost_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_password_expiry_policy_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_password_expiry_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_password_policy_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_password_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_password_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_password_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_permission_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_permission_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_plex_source_connection_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_plex_source_connection_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_plex_source_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_plex_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_policy_binding_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_policy_binding_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_policy_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_prompt_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_prompt_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_prompt_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_prompt_stage_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_property_mapping_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_property_mapping_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_provider_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_proxy_provider_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,24 +17,24 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
 from authentik_client.models.pagination import Pagination
-from authentik_client.models.provider import Provider
+from authentik_client.models.proxy_provider import ProxyProvider
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedProviderList(BaseModel):
+class PaginatedProxyProviderList(BaseModel):
     """
-    PaginatedProviderList
+    PaginatedProxyProviderList
     """ # noqa: E501
     pagination: Pagination
-    results: List[Provider]
+    results: List[ProxyProvider]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedProviderList from a JSON string"""
+        """Create an instance of PaginatedProxyProviderList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedProviderList from a dict"""
+        """Create an instance of PaginatedProxyProviderList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [Provider.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [ProxyProvider.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_proxy_outpost_config_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_proxy_outpost_config_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_proxy_provider_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_provider_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,24 +17,24 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
 from authentik_client.models.pagination import Pagination
-from authentik_client.models.proxy_provider import ProxyProvider
+from authentik_client.models.provider import Provider
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedProxyProviderList(BaseModel):
+class PaginatedProviderList(BaseModel):
     """
-    PaginatedProxyProviderList
+    PaginatedProviderList
     """ # noqa: E501
     pagination: Pagination
-    results: List[ProxyProvider]
+    results: List[Provider]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedProxyProviderList from a JSON string"""
+        """Create an instance of PaginatedProviderList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedProxyProviderList from a dict"""
+        """Create an instance of PaginatedProviderList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [ProxyProvider.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [Provider.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_rac_property_mapping_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_rac_property_mapping_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_rac_provider_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_rac_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_radius_outpost_config_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_radius_outpost_config_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_radius_provider_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_radius_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_reputation_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_reputation_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_reputation_policy_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_reputation_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_role_assigned_object_permission_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_role_assigned_object_permission_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_role_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_role_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_saml_property_mapping_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_saml_property_mapping_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_saml_provider_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_totp_device_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,24 +17,24 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
 from authentik_client.models.pagination import Pagination
-from authentik_client.models.saml_provider import SAMLProvider
+from authentik_client.models.totp_device import TOTPDevice
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedSAMLProviderList(BaseModel):
+class PaginatedTOTPDeviceList(BaseModel):
     """
-    PaginatedSAMLProviderList
+    PaginatedTOTPDeviceList
     """ # noqa: E501
     pagination: Pagination
-    results: List[SAMLProvider]
+    results: List[TOTPDevice]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedSAMLProviderList from a JSON string"""
+        """Create an instance of PaginatedTOTPDeviceList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedSAMLProviderList from a dict"""
+        """Create an instance of PaginatedTOTPDeviceList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [SAMLProvider.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [TOTPDevice.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_saml_source_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_saml_source_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_mapping_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_scim_mapping_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_provider_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_scim_provider_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_source_group_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_scim_source_group_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_source_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_scim_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_source_user_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_scim_source_user_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scope_mapping_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_scope_mapping_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_service_connection_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_service_connection_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_sms_device_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_sms_device_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_source_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_source_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_source_stage_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_login_stage_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,24 +17,24 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
 from authentik_client.models.pagination import Pagination
-from authentik_client.models.stage import Stage
+from authentik_client.models.user_login_stage import UserLoginStage
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedStageList(BaseModel):
+class PaginatedUserLoginStageList(BaseModel):
     """
-    PaginatedStageList
+    PaginatedUserLoginStageList
     """ # noqa: E501
     pagination: Pagination
-    results: List[Stage]
+    results: List[UserLoginStage]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedStageList from a JSON string"""
+        """Create an instance of PaginatedUserLoginStageList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedStageList from a dict"""
+        """Create an instance of PaginatedUserLoginStageList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [Stage.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [UserLoginStage.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_static_device_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_static_device_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_system_task_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_system_task_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_tenant_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_tenant_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_token_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_token_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_token_model_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_token_model_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_totp_device_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_web_authn_device_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,24 +17,24 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
 from authentik_client.models.pagination import Pagination
-from authentik_client.models.totp_device import TOTPDevice
+from authentik_client.models.web_authn_device import WebAuthnDevice
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedTOTPDeviceList(BaseModel):
+class PaginatedWebAuthnDeviceList(BaseModel):
     """
-    PaginatedTOTPDeviceList
+    PaginatedWebAuthnDeviceList
     """ # noqa: E501
     pagination: Pagination
-    results: List[TOTPDevice]
+    results: List[WebAuthnDevice]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedTOTPDeviceList from a JSON string"""
+        """Create an instance of PaginatedWebAuthnDeviceList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedTOTPDeviceList from a dict"""
+        """Create an instance of PaginatedWebAuthnDeviceList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [TOTPDevice.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [WebAuthnDevice.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_assigned_object_permission_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_assigned_object_permission_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_consent_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_consent_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_delete_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_delete_stage_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_login_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_write_stage_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,24 +17,24 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
 from authentik_client.models.pagination import Pagination
-from authentik_client.models.user_login_stage import UserLoginStage
+from authentik_client.models.user_write_stage import UserWriteStage
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedUserLoginStageList(BaseModel):
+class PaginatedUserWriteStageList(BaseModel):
     """
-    PaginatedUserLoginStageList
+    PaginatedUserWriteStageList
     """ # noqa: E501
     pagination: Pagination
-    results: List[UserLoginStage]
+    results: List[UserWriteStage]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedUserLoginStageList from a JSON string"""
+        """Create an instance of PaginatedUserWriteStageList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedUserLoginStageList from a dict"""
+        """Create an instance of PaginatedUserWriteStageList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [UserLoginStage.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [UserWriteStage.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_logout_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_logout_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_o_auth_source_connection_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_o_auth_source_connection_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_saml_source_connection_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_saml_source_connection_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_source_connection_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_user_source_connection_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_write_stage_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_endpoint_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
+from authentik_client.models.endpoint import Endpoint
 from authentik_client.models.pagination import Pagination
-from authentik_client.models.user_write_stage import UserWriteStage
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedUserWriteStageList(BaseModel):
+class PaginatedEndpointList(BaseModel):
     """
-    PaginatedUserWriteStageList
+    PaginatedEndpointList
     """ # noqa: E501
     pagination: Pagination
-    results: List[UserWriteStage]
+    results: List[Endpoint]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedUserWriteStageList from a JSON string"""
+        """Create an instance of PaginatedEndpointList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedUserWriteStageList from a dict"""
+        """Create an instance of PaginatedEndpointList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [UserWriteStage.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [Endpoint.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_web_authn_device_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_web_authn_device_type_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,24 +17,24 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
 from authentik_client.models.pagination import Pagination
-from authentik_client.models.web_authn_device import WebAuthnDevice
+from authentik_client.models.web_authn_device_type import WebAuthnDeviceType
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedWebAuthnDeviceList(BaseModel):
+class PaginatedWebAuthnDeviceTypeList(BaseModel):
     """
-    PaginatedWebAuthnDeviceList
+    PaginatedWebAuthnDeviceTypeList
     """ # noqa: E501
     pagination: Pagination
-    results: List[WebAuthnDevice]
+    results: List[WebAuthnDeviceType]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedWebAuthnDeviceList from a JSON string"""
+        """Create an instance of PaginatedWebAuthnDeviceTypeList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedWebAuthnDeviceList from a dict"""
+        """Create an instance of PaginatedWebAuthnDeviceTypeList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [WebAuthnDevice.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [WebAuthnDeviceType.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_web_authn_device_type_list.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/paginated_dummy_stage_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
+from authentik_client.models.dummy_stage import DummyStage
 from authentik_client.models.pagination import Pagination
-from authentik_client.models.web_authn_device_type import WebAuthnDeviceType
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedWebAuthnDeviceTypeList(BaseModel):
+class PaginatedDummyStageList(BaseModel):
     """
-    PaginatedWebAuthnDeviceTypeList
+    PaginatedDummyStageList
     """ # noqa: E501
     pagination: Pagination
-    results: List[WebAuthnDeviceType]
+    results: List[DummyStage]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedWebAuthnDeviceTypeList from a JSON string"""
+        """Create an instance of PaginatedDummyStageList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedWebAuthnDeviceTypeList from a dict"""
+        """Create an instance of PaginatedDummyStageList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [WebAuthnDeviceType.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [DummyStage.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/pagination.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/password_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/password_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_expiry_policy.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/password_expiry_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_expiry_policy_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/password_expiry_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_policy.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/password_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_policy_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/password_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/password_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/password_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_application_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_application_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_duo_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_authenticator_duo_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_sms_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_authenticator_sms_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_static_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_authenticator_static_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_totp_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_authenticator_totp_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_validate_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_authenticator_validate_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_web_authn_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_authenticator_web_authn_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_blueprint_instance_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_blueprint_instance_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_brand_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_brand_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_captcha_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_captcha_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_certificate_key_pair_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_certificate_key_pair_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_connection_token_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_connection_token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_consent_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_consent_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_deny_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_deny_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_docker_service_connection_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_docker_service_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_domain_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_domain_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_dummy_policy_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_dummy_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_dummy_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_dummy_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_duo_device_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_duo_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_email_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_email_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_endpoint_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_endpoint_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_event_matcher_policy_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_event_matcher_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_event_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_expression_policy_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_expression_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_flow_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_flow_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_flow_stage_binding_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_flow_stage_binding_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_group_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_group_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_identification_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_identification_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_invitation_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_invitation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_invitation_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_invitation_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_kubernetes_service_connection_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_kubernetes_service_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_ldap_property_mapping_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_ldap_property_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_ldap_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_ldap_provider_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_ldap_source_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_ldap_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_license_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_license_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_rule_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_notification_rule_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_transport_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_notification_transport_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_webhook_mapping_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_notification_webhook_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_o_auth2_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_o_auth2_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_o_auth_source_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_o_auth_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_outpost_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_outpost_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_password_expiry_policy_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_password_expiry_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_password_policy_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_password_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_password_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_password_stage_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_permission_assign_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_permission_assign_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_plex_source_connection_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_plex_source_connection_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_plex_source_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_plex_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_policy_binding_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_policy_binding_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_prompt_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_prompt_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_prompt_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_prompt_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_proxy_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_proxy_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_rac_property_mapping_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_rac_property_mapping_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_rac_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_rac_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_radius_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_radius_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_reputation_policy_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_reputation_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_role_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_role_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_saml_property_mapping_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_saml_property_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_saml_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_saml_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_saml_source_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_saml_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_mapping_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_scim_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_scim_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_source_group_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_scim_source_group_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_source_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_scim_source_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_source_user_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_scim_source_user_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scope_mapping_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_scope_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_settings_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_sms_device_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_static_device_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -20,17 +20,17 @@
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PatchedSMSDeviceRequest(BaseModel):
+class PatchedStaticDeviceRequest(BaseModel):
     """
-    Serializer for sms authenticator devices
+    Serializer for static authenticator devices
     """ # noqa: E501
     name: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=64)]] = Field(default=None, description="The human-readable name of this device.")
     __properties: ClassVar[List[str]] = ["name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PatchedSMSDeviceRequest from a JSON string"""
+        """Create an instance of PatchedStaticDeviceRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,15 +70,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PatchedSMSDeviceRequest from a dict"""
+        """Create an instance of PatchedStaticDeviceRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_source_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_source_stage_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_static_device_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_sms_device_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -20,17 +20,17 @@
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PatchedStaticDeviceRequest(BaseModel):
+class PatchedSMSDeviceRequest(BaseModel):
     """
-    Serializer for static authenticator devices
+    Serializer for sms authenticator devices
     """ # noqa: E501
     name: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=64)]] = Field(default=None, description="The human-readable name of this device.")
     __properties: ClassVar[List[str]] = ["name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PatchedStaticDeviceRequest from a JSON string"""
+        """Create an instance of PatchedSMSDeviceRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,15 +70,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PatchedStaticDeviceRequest from a dict"""
+        """Create an instance of PatchedSMSDeviceRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_tenant_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_tenant_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_token_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_totp_device_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_totp_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_delete_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_delete_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_login_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_login_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_logout_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_logout_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_o_auth_source_connection_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_o_auth_source_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_saml_source_connection_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_saml_source_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_write_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_user_write_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_web_authn_device_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/patched_web_authn_device_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/permission.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/permission.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/permission_assign_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/permission_assign_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_authentication_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_authentication_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_authentication_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_authentication_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source_connection.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_source_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source_connection_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_source_connection_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_token_redeem_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/plex_token_redeem_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_binding.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/policy_binding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_binding_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/policy_binding_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_engine_mode.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/policy_engine_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/policy_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_test_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/policy_test_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_test_result.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/policy_test_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_type_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/prompt_type_enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/property_mapping.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/property_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/property_mapping_preview.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/property_mapping_preview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/property_mapping_test_result.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/property_mapping_test_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/protocol_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/protocol_enum.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/provider.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/severity_enum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class ProviderEnum(str, Enum):
+class SeverityEnum(str, Enum):
     """
-    ProviderEnum
+    SeverityEnum
     """
 
     """
     allowed enum values
     """
-    TWILIO = 'twilio'
-    GENERIC = 'generic'
+    NOTICE = 'notice'
+    WARNING = 'warning'
+    ALERT = 'alert'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ProviderEnum from a JSON string"""
+        """Create an instance of SeverityEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_model_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/provider_model_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_type_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/provider_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_mode.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/proxy_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_outpost_config.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/proxy_outpost_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_provider.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/proxy_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/proxy_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_property_mapping.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/rac_property_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_property_mapping_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/rac_property_mapping_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_provider.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/rac_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/rac_provider_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/radius_outpost_config.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/radius_outpost_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/radius_provider.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/radius_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/radius_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/radius_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/redirect_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/redirect_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/reputation.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/reputation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/reputation_policy.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/reputation_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/reputation_policy_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/reputation_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/resident_key_requirement_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/resident_key_requirement_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/role.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/role_assigned_object_permission.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/role_assigned_object_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/role_object_permission.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/role_object_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/role_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/role_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_metadata.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_property_mapping.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_property_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_property_mapping_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_property_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_provider.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_source.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_source_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/saml_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_mapping.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_mapping_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_mapping_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_provider.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_provider_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_group.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_source_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_group_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_source_group_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_source_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_user.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_source_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_user_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_source_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_sync_status.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/scim_sync_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/scope_mapping.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/scope_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/scope_mapping_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/scope_mapping_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/selectable_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/selectable_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/service_connection.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/service_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/service_connection_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/service_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/service_connection_state.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/service_connection_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/session_user.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/session_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/settings.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/settings_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/severity_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_type_enum.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class SeverityEnum(str, Enum):
+class UserTypeEnum(str, Enum):
     """
-    SeverityEnum
+    UserTypeEnum
     """
 
     """
     allowed enum values
     """
-    NOTICE = 'notice'
-    WARNING = 'warning'
-    ALERT = 'alert'
+    INTERNAL = 'internal'
+    EXTERNAL = 'external'
+    SERVICE_ACCOUNT = 'service_account'
+    INTERNAL_SERVICE_ACCOUNT = 'internal_service_account'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of SeverityEnum from a JSON string"""
+        """Create an instance of UserTypeEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/shell_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/shell_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/signature_algorithm_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/signature_algorithm_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/sms_device.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/sms_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/sms_device_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/static_device_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -20,17 +20,17 @@
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SMSDeviceRequest(BaseModel):
+class StaticDeviceRequest(BaseModel):
     """
-    Serializer for sms authenticator devices
+    Serializer for static authenticator devices
     """ # noqa: E501
     name: Annotated[str, Field(min_length=1, strict=True, max_length=64)] = Field(description="The human-readable name of this device.")
     __properties: ClassVar[List[str]] = ["name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SMSDeviceRequest from a JSON string"""
+        """Create an instance of StaticDeviceRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,15 +70,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SMSDeviceRequest from a dict"""
+        """Create an instance of StaticDeviceRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/source.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/source_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/source_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/source_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/source_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/source_stage_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/source_type.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/source_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/sp_binding_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/sp_binding_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/stage_prompt.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/stage_prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/static_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/totp_device_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -20,17 +20,17 @@
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class StaticDeviceRequest(BaseModel):
+class TOTPDeviceRequest(BaseModel):
     """
-    Serializer for static authenticator devices
+    Serializer for totp authenticator devices
     """ # noqa: E501
     name: Annotated[str, Field(min_length=1, strict=True, max_length=64)] = Field(description="The human-readable name of this device.")
     __properties: ClassVar[List[str]] = ["name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of StaticDeviceRequest from a JSON string"""
+        """Create an instance of TOTPDeviceRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,15 +70,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of StaticDeviceRequest from a dict"""
+        """Create an instance of TOTPDeviceRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device_token.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/static_device_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device_token_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/static_device_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/sub_mode_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/sub_mode_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/system_info.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/system_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/system_info_runtime.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/system_info_runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/system_task.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/system_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/system_task_status_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/system_task_status_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/tenant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_admin_group_request_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/tenant_admin_group_request_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_recovery_key_request_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/tenant_recovery_key_request_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_recovery_key_response.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/tenant_recovery_key_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/tenant_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/token.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/token_model.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/token_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/token_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/token_set_key_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/token_set_key_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/token_view.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/token_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/totp_device.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/totp_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/totp_device_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/sms_device_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -20,17 +20,17 @@
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TOTPDeviceRequest(BaseModel):
+class SMSDeviceRequest(BaseModel):
     """
-    Serializer for totp authenticator devices
+    Serializer for sms authenticator devices
     """ # noqa: E501
     name: Annotated[str, Field(min_length=1, strict=True, max_length=64)] = Field(description="The human-readable name of this device.")
     __properties: ClassVar[List[str]] = ["name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TOTPDeviceRequest from a JSON string"""
+        """Create an instance of SMSDeviceRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,15 +70,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TOTPDeviceRequest from a dict"""
+        """Create an instance of SMSDeviceRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/transaction_application_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/transaction_application_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/transaction_application_response.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/transaction_application_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/type_create.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/type_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/ui_theme_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/ui_theme_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/used_by.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/used_by.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/used_by_action_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/used_by_action_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_account_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_account_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_assigned_object_permission.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_assigned_object_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_consent.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_consent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_creation_mode_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_creation_mode_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_delete_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_delete_stage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_delete_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_delete_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_fields_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_fields_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_group.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_challenge.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_login_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_challenge_response_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_login_challenge_response_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_login_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_login_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_logout_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_logout_stage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_logout_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_logout_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_matching_mode_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_matching_mode_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_metrics.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_o_auth_source_connection.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_o_auth_source_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_o_auth_source_connection_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_o_auth_source_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_object_permission.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_object_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_password_set_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_password_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_path.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_saml_source_connection.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_saml_source_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_saml_source_connection_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_saml_source_connection_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_self.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_self.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_self_groups.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_self_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_service_account_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_service_account_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_service_account_response.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_service_account_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_setting.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_source_connection.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_source_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_type_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/duo_response_enum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class UserTypeEnum(str, Enum):
+class DuoResponseEnum(str, Enum):
     """
-    UserTypeEnum
+    DuoResponseEnum
     """
 
     """
     allowed enum values
     """
-    INTERNAL = 'internal'
-    EXTERNAL = 'external'
-    SERVICE_ACCOUNT = 'service_account'
-    INTERNAL_SERVICE_ACCOUNT = 'internal_service_account'
+    SUCCESS = 'success'
+    WAITING = 'waiting'
+    INVALID = 'invalid'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of UserTypeEnum from a JSON string"""
+        """Create an instance of DuoResponseEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_verification_enum.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/digits_enum.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class UserVerificationEnum(str, Enum):
+class DigitsEnum(str, Enum):
     """
-    UserVerificationEnum
+    DigitsEnum
     """
 
     """
     allowed enum values
     """
-    REQUIRED = 'required'
-    PREFERRED = 'preferred'
-    DISCOURAGED = 'discouraged'
+    ENUM_6 = '6'
+    ENUM_8 = '8'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of UserVerificationEnum from a JSON string"""
+        """Create an instance of DigitsEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_write_stage.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_write_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_write_stage_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/user_write_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/validation_error.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/validation_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/version.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/web_authn_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/web_authn_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device_type.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/web_authn_device_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device_type_request.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/web_authn_device_type_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/models/workers.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/models/workers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/authentik_client/rest.py` & `authentik_client-2024.2.3.post1713359900/authentik_client/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.2.2
+    The version of the OpenAPI document: 2024.2.3
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.2.2.post1713289429/pyproject.toml` & `authentik_client-2024.2.3.post1713359900/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "authentik_client"
-version = "2024.2.2-1713289429"
+version = "2024.2.3-1713359900"
 description = "authentik"
 authors = ["authentik Team <hello@goauthentik.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/goauthentik/authentik"
 keywords = ["OpenAPI", "OpenAPI-Generator", "authentik"]
 include = ["authentik_client/py.typed"]
```

### Comparing `authentik_client-2024.2.2.post1713289429/PKG-INFO` & `authentik_client-2024.2.3.post1713359900/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authentik_client
-Version: 2024.2.2.post1713289429
+Version: 2024.2.3.post1713359900
 Summary: authentik
 Home-page: https://github.com/goauthentik/authentik
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,authentik
 Author: authentik Team
 Author-email: hello@goauthentik.io
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2024.2.2
-- Package version: 2024.2.2-1713289429
+- API version: 2024.2.3
+- Package version: 2024.2.3-1713359900
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

