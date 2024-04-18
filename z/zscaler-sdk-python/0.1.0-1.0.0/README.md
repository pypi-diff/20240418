# Comparing `tmp/zscaler-sdk-python-0.1.0.tar.gz` & `tmp/zscaler-sdk-python-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler-sdk-python-0.1.0.tar", last modified: Thu Apr 18 09:09:45 2024, max compression
+gzip compressed data, was "zscaler-sdk-python-1.0.0.tar", last modified: Wed Apr 17 07:21:40 2024, max compression
```

## Comparing `zscaler-sdk-python-0.1.0.tar` & `zscaler-sdk-python-1.0.0.tar`

### file list

```diff
@@ -1,214 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.112415 zscaler-sdk-python-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/LONG_DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-18 09:09:45.112415 zscaler-sdk-python-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.084415 zscaler-sdk-python-0.1.0/docsrc/
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.084415 zscaler-sdk-python-0.1.0/docsrc/zs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.088415 zscaler-sdk-python-0.1.0/docsrc/zs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/guides/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/guides/support.rst
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/guides/troubleshooting.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.088415 zscaler-sdk-python-0.1.0/docsrc/zs/zia/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/activate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/admin_and_role_management.rst
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/apptotal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/audit_logs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/authentication_settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/cloud_apps.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/device_management.rst
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/dlp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/firewall.rst
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/forwarding_control.rst
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/isolation_profile.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/locations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/rule_labels.rst
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/sandbox.rst
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/security.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/ssl_inspection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/traffic.rst
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/url_categories.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/url_filtering.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/users.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/web_dlp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/workload_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/zpa_gateway.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.092415 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/app_segments.rst
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/app_segments_inspection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/app_segments_pra.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/certificates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/cloud_connector_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/connectors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/emergency_access.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/idp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/inspection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/isolation_profile.rst
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/lss.rst
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/machine_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/policies.rst
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/posture_profiles.rst
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/privileged_remote_access.rst
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/provisioning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/saml_attributes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/scim_attributes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/scim_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/segment_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/server_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/servers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/service_edges.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/trusted_networks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-18 09:09:45.112415 zscaler-sdk-python-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1794 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.092415 zscaler-sdk-python-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.084415 zscaler-sdk-python-0.1.0/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.096415 zscaler-sdk-python-0.1.0/tests/integration/zia/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_admin_and_role_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_authentication_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_cloud_firewall_ip_destination_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_cloud_firewall_ip_source_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_cloud_firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_engines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_icap_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_idm_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_incident_receiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_web_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_location_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    14466 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_location_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_rule_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_security.py
--rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_traffic_gre_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_traffic_static_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_traffic_vpn_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_url_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_url_filtering_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.100415 zscaler-sdk-python-0.1.0/tests/integration/zpa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_access_policy_forwarding_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_access_policy_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_access_policy_timeout_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_app_connector_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_application_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_application_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_ba_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_enrolment_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_idp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_machine_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_posture_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_pra_approval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_pra_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_pra_portal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_provisioning_key_app_connector_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_provisioning_key_service_edge_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_saml_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_scim_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_scim_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_segment_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_server_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_service_edge_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_trusted_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.100415 zscaler-sdk-python-0.1.0/zscaler/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.100415 zscaler-sdk-python-0.1.0/zscaler/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/cache/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/cache/no_op_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/cache/zscaler_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.100415 zscaler-sdk-python-0.1.0/zscaler/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/errors/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/errors/zscaler_api_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.100415 zscaler-sdk-python-0.1.0/zscaler/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.100415 zscaler-sdk-python-0.1.0/zscaler/ratelimiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/ratelimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/ratelimiter/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    19443 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.104415 zscaler-sdk-python-0.1.0/zscaler/zia/
--rw-r--r--   0 runner    (1001) docker     (127)    22024 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/activate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/admin_and_role_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/apptotal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/authentication_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18549 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/cloud_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/device_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    27588 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/dlp.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    40386 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/forwarding_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    30972 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/ssl_inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    31279 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/traffic.py
--rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/url_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/url_filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/web_dlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/workload_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/zpa_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.108415 zscaler-sdk-python-0.1.0/zscaler/zpa/
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    24790 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/app_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12657 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/app_segments_inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/app_segments_pra.py
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/cloud_connector_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    20602 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/emergency_access.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/idp.py
--rw-r--r--   0 runner    (1001) docker     (127)    34889 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/lss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/machine_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    30654 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/posture_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    32581 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/privileged_remote_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/provisioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/saml_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/scim_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/scim_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/segment_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/server_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/servers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15606 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/service_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/trusted_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.112415 zscaler-sdk-python-0.1.0/zscaler_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-18 09:09:45.000000 zscaler-sdk-python-0.1.0/zscaler_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-04-18 09:09:45.000000 zscaler-sdk-python-0.1.0/zscaler_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:09:45.000000 zscaler-sdk-python-0.1.0/zscaler_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-18 09:09:45.000000 zscaler-sdk-python-0.1.0/zscaler_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 09:09:45.000000 zscaler-sdk-python-0.1.0/zscaler_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 wguilherme   (503) staff       (20)        0 2024-04-17 07:21:40.721482 zscaler-sdk-python-1.0.0/
+-rw-r--r--   0 wguilherme   (503) staff       (20)      293 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/CHANGELOG.md
+-rw-r--r--   0 wguilherme   (503) staff       (20)     1113 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/LICENSE.md
+-rw-r--r--   0 wguilherme   (503) staff       (20)      739 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/LONG_DESCRIPTION.md
+-rw-r--r--   0 wguilherme   (503) staff       (20)      112 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/MANIFEST.in
+-rw-r--r--   0 wguilherme   (503) staff       (20)     1941 2024-04-17 07:21:40.721402 zscaler-sdk-python-1.0.0/PKG-INFO
+-rw-r--r--   0 wguilherme   (503) staff       (20)     9871 2024-04-17 07:02:00.000000 zscaler-sdk-python-1.0.0/README.md
+-rw-r--r--   0 wguilherme   (503) staff       (20)      349 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/requirements.txt
+-rw-r--r--   0 wguilherme   (503) staff       (20)      105 2024-04-17 07:21:40.721719 zscaler-sdk-python-1.0.0/setup.cfg
+-rwxr-xr-x   0 wguilherme   (503) staff       (20)     1944 2024-04-17 07:15:26.000000 zscaler-sdk-python-1.0.0/setup.py
+drwxr-xr-x   0 wguilherme   (503) staff       (20)        0 2024-04-17 07:21:40.700578 zscaler-sdk-python-1.0.0/tests/
+-rw-r--r--   0 wguilherme   (503) staff       (20)        0 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/__init__.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     1202 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/conftest.py
+drwxr-xr-x   0 wguilherme   (503) staff       (20)        0 2024-04-17 07:21:40.698236 zscaler-sdk-python-1.0.0/tests/integration/
+drwxr-xr-x   0 wguilherme   (503) staff       (20)        0 2024-04-17 07:21:40.704607 zscaler-sdk-python-1.0.0/tests/integration/zia/
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2091 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/conftest.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2161 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_activation.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2896 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_admin_and_role_management.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2481 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_authentication_settings.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4421 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_cloud_firewall_ip_destination_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4094 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_cloud_firewall_ip_source_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     6056 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_cloud_firewall_rule.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4391 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_dlp_dictionary.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4860 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_dlp_engines.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2887 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_dlp_icap_server.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3099 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_dlp_idm_profile.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3127 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_dlp_incident_receiver.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4096 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_dlp_web_rule.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3147 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_isolation_profile.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     5199 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_location_group.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    14466 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_location_management.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4080 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_rule_labels.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     6194 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_sandbox.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4558 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_security.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    15809 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_traffic_gre_tunnel.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4179 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_traffic_static_ip.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     5073 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_traffic_vpn_credential.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     9234 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_url_categories.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4394 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_url_filtering_rule.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    10152 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zia/test_users.py
+drwxr-xr-x   0 wguilherme   (503) staff       (20)        0 2024-04-17 07:21:40.708879 zscaler-sdk-python-1.0.0/tests/integration/zpa/
+-rw-r--r--   0 wguilherme   (503) staff       (20)        0 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/__init__.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2055 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/conftest.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4345 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_access_policy_forwarding_rules.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     5361 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_access_policy_rules.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4287 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_access_policy_timeout_rules.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4749 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_app_connector_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     6722 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_application_segment.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3729 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_application_servers.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3187 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_ba_certificates.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2534 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_enrolment_certificates.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3006 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_idp.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2775 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_isolation_profile.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3267 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_machine_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3412 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_posture_profiles.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     9208 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_pra_approval.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4453 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_pra_credential.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4701 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_pra_portal.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     6118 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_provisioning_key_app_connector_group.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     6209 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_provisioning_key_service_edge_group.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3410 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_saml_attributes.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2957 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_scim_attributes.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2812 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_scim_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3686 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_segment_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     5321 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_server_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     5488 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_service_edge_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3557 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/integration/zpa/test_trusted_networks.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3658 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tests/test_utils.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)      222 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/tox.ini
+drwxr-xr-x   0 wguilherme   (503) staff       (20)        0 2024-04-17 07:21:40.709545 zscaler-sdk-python-1.0.0/zscaler/
+-rw-r--r--   0 wguilherme   (503) staff       (20)     1248 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/__init__.py
+drwxr-xr-x   0 wguilherme   (503) staff       (20)        0 2024-04-17 07:21:40.710024 zscaler-sdk-python-1.0.0/zscaler/cache/
+-rw-r--r--   0 wguilherme   (503) staff       (20)        0 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/cache/__init__.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3195 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/cache/cache.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     1485 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/cache/no_op_cache.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4997 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/cache/zscaler_cache.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)      738 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/constants.py
+drwxr-xr-x   0 wguilherme   (503) staff       (20)        0 2024-04-17 07:21:40.710541 zscaler-sdk-python-1.0.0/zscaler/errors/
+-rw-r--r--   0 wguilherme   (503) staff       (20)        0 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/errors/__init__.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)      172 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/errors/error.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)      638 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/errors/http_error.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)      664 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/errors/zscaler_api_error.py
+drwxr-xr-x   0 wguilherme   (503) staff       (20)        0 2024-04-17 07:21:40.710876 zscaler-sdk-python-1.0.0/zscaler/exceptions/
+-rw-r--r--   0 wguilherme   (503) staff       (20)       63 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/exceptions/__init__.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2025 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/exceptions/exceptions.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2099 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/logger.py
+drwxr-xr-x   0 wguilherme   (503) staff       (20)        0 2024-04-17 07:21:40.711099 zscaler-sdk-python-1.0.0/zscaler/ratelimiter/
+-rw-r--r--   0 wguilherme   (503) staff       (20)        0 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/ratelimiter/__init__.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     1487 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/ratelimiter/ratelimiter.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)      663 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/user_agent.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    19443 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/utils.py
+drwxr-xr-x   0 wguilherme   (503) staff       (20)        0 2024-04-17 07:21:40.714818 zscaler-sdk-python-1.0.0/zscaler/zia/
+-rw-r--r--   0 wguilherme   (503) staff       (20)    22024 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/__init__.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     1535 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/activate.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    14292 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/admin_and_role_management.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2372 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/apptotal.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3014 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/audit_logs.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3184 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/authentication_settings.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2754 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/client.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    18549 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/cloud_apps.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2872 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/device_management.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    27588 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/dlp.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)      794 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/errors.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    40386 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/firewall.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    11754 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/forwarding_control.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2917 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/isolation_profile.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     5865 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/labels.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    30972 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/locations.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     5796 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/sandbox.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     6846 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/security.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     5364 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/ssl_inspection.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    31279 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/traffic.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    14744 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/url_categories.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    14387 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/url_filtering.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    13841 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/users.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    12436 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/web_dlp.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     1897 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/workload_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     6972 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zia/zpa_gateway.py
+drwxr-xr-x   0 wguilherme   (503) staff       (20)        0 2024-04-17 07:21:40.718908 zscaler-sdk-python-1.0.0/zscaler/zpa/
+-rw-r--r--   0 wguilherme   (503) staff       (20)    24826 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/__init__.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    13391 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/app_segments.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    12655 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/app_segments_inspection.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    12215 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/app_segments_pra.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     8006 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/certificates.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3804 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/client.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2667 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/cloud_connector_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    20602 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/connectors.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     6293 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/emergency_access.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)      844 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/errors.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2764 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/idp.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    34889 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/inspection.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3176 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/isolation_profile.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    21471 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/lss.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     2734 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/machine_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    30654 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/policies.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4339 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/posture_profiles.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    32836 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/privileged_remote_access.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     9995 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/provisioning.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     3678 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/saml_attributes.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4194 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/scim_attributes.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     5451 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/scim_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     6215 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/segment_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     7858 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/server_groups.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     6513 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/servers.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)    15606 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/service_edges.py
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4399 2024-04-17 06:16:38.000000 zscaler-sdk-python-1.0.0/zscaler/zpa/trusted_networks.py
+drwxr-xr-x   0 wguilherme   (503) staff       (20)        0 2024-04-17 07:21:40.720991 zscaler-sdk-python-1.0.0/zscaler_sdk_python.egg-info/
+-rw-r--r--   0 wguilherme   (503) staff       (20)     1941 2024-04-17 07:21:40.000000 zscaler-sdk-python-1.0.0/zscaler_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 wguilherme   (503) staff       (20)     4724 2024-04-17 07:21:40.000000 zscaler-sdk-python-1.0.0/zscaler_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 wguilherme   (503) staff       (20)        1 2024-04-17 07:21:40.000000 zscaler-sdk-python-1.0.0/zscaler_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 wguilherme   (503) staff       (20)      169 2024-04-17 07:21:40.000000 zscaler-sdk-python-1.0.0/zscaler_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 wguilherme   (503) staff       (20)        8 2024-04-17 07:21:40.000000 zscaler-sdk-python-1.0.0/zscaler_sdk_python.egg-info/top_level.txt
```

### Comparing `zscaler-sdk-python-0.1.0/LICENSE.md` & `zscaler-sdk-python-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/LONG_DESCRIPTION.md` & `zscaler-sdk-python-1.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 # Official Python SDK for the Zscaler Products
 
-[![CI/CD](https://github.com/zscaler/zscaler-sdk-python/actions/workflows/ci.yml/badge.svg)](https://github.com/zscaler/zscaler-sdk-python/actions/workflows/ci.yml)
-[![Documentation Status](https://readthedocs.org/projects/zscaler-sdk-python/badge/?version=latest)](https://zscaler-sdk-python.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/github/license/zscaler/zscaler-sdk-python.svg)](https://github.com/zscaler/zscaler-sdk-python)
-[![Latest version released on PyPi](https://img.shields.io/pypi/v/zscaler-sdk-python.svg)](https://pypi.org/project/zscaler-sdk-python)
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/zscaler-sdk-python.svg)](https://pypi.python.org/pypi/zscaler-sdk-python/)
-[![GitHub Release](https://img.shields.io/github/release/zscaler/zscaler-sdk-python.svg)](https://github.com/zscaler/zscaler-sdk-python/releases/)
 [![Zscaler Community](https://img.shields.io/badge/zscaler-community-blue)](https://community.zscaler.com/)
 
 ## Support Disclaimer
 
 -> **Disclaimer:** Please refer to our [General Support Statement](docs/guides/support.md) before proceeding with the use of this provider. You can also refer to our [troubleshooting guide](docs/guides/troubleshooting.md) for guidance on typical problems.
 
-## Zscaler Python SDK Overview
-
-This repository contains the Zscaler SDK for Python. This SDK can be used to interact with several Zscaler services such as:
+## Zscaler Python Management SDK Overview
 
+This repository contains the Zscaler management SDK for Python. This SDK can be used to interact with several Zscaler services such as:
 * Zscaler Private Access (ZPA)
 * Zscaler Internet Access (ZIA)
-* [Documentation](http://zscaler-sdk-python.readthedocs.io)
-
------
 
 Each Zscaler product has separate developer documentation and authentication methods. This SDK aims to simplify
 software development using the Zscaler API for both customers and partners.
 
 - [Release Status](#release-status)
 - [Need help?](#need-help)
 - [Getting Started](#getting-started)
@@ -46,28 +37,28 @@
 - Support [customer support portal][zscaler-support]
 
 ## Getting started
 
 To install the Zscaler Python SDK in your project:
 
 ```sh
-pip install zscaler-sdk-python
+pip install zscaler
 ```
 
 ## Usage
 
 Before you can interact with any of the Zscaler APIs, you need to generate API keys or retrieve tenancy information for each product that you are interfacing with. Once you have the requirements and you have installed Zscaler SDK Python, you're ready to go.
 
 ### Quick ZIA Example
 
 ```python
 from zscaler import ZIAClientHelper
 from pprint import pprint
 
-zia = ZIAClientHelper(username='ZIA_USERNAME', password='ZIA_PASSWORD', api_key='ZIA_API_KEY', cloud='ZIA_CLOUD')
+zia = ZIAClientHelper(username='USERNAME', password='PASSWORD', api_key='ZIA_API_KEY', cloud='ZIA_CLOUD')
 for user in zia.users.list_users():
     pprint(user)
 ```
 
 ### Quick ZPA Example
 
 ```python
@@ -187,29 +178,22 @@
 - Run `make build:dist` from the root of the project (assuming Python is installed)
 - Ensure tests run succesfully. 
 - Install `tox` if not installed already using: `pip install tox`. 
 - Run tests using `tox` in the root directory of the project.
 
 ## Contributing
 
-At this moment we are not accepting contributions, but we welcome suggestions on how to improve this SDK or feature requests, which can then be added in  future releases.
+We're happy to accept contributions and PRs! Please see the [Contribution Guide](CONTRIBUTING.md) to understand how to structure a contribution.
 
 [zenith]: https://community.zscaler.com/
 [zscaler-support]: https://help.zscaler.com/contact-support
 [github-issues]: https://github.com/zscaler/zscaler-sdk-python/issues
 [rate-limiting-zpa]: https://help.zscaler.com/zpa/understanding-rate-limiting
 [rate-limiting-zia]: https://help.zscaler.com/zia/understanding-rate-limiting
 
-Contributors
-------------
-
-- William Guilherme - [willguibr](https://github.com/willguibr)
-- Eddie Parra - [eparra](https://github.com/eparra)
-- Paul Abbot - [abbottp](https://github.com/abbottp)
-
 ## License
 MIT License
 
 =======
 
 Copyright (c) 2023 [Zscaler](https://github.com/zscaler)
```

### Comparing `zscaler-sdk-python-0.1.0/setup.py` & `zscaler-sdk-python-1.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 # -*- coding: utf-8 -*-
-from setuptools import setup
 import os
 import re
 
-def read(rel_path):
-    here = os.path.abspath(os.path.dirname(__file__))
-    with open(os.path.join(here, rel_path), encoding='utf-8') as fp:
-        return fp.read()
-    
+from setuptools import find_packages, setup
+
+
 def get_version():
     # Define the path to the __init__.py file
     init_path = os.path.join(os.path.dirname(__file__), "zscaler", "__init__.py")
     # Use a regular expression to find the version number
     version_pattern = re.compile(r"^__version__ = ['\"]([^'\"]*)['\"]")
     with open(init_path, "rt") as version_file:
         for line in version_file:
             match = version_pattern.search(line)
             if match:
                 return match.group(1)
     raise RuntimeError("Unable to find version string.")
 
 
-packages = [
-    "zscaler",
-    "zscaler.cache",
-    "zscaler.errors",
-    "zscaler.exceptions",
-    "zscaler.ratelimiter",
-    "zscaler.zia",
-    "zscaler.zpa",
-]
-
-package_data = {"": ["*"]}
-
 setup(
     name="zscaler-sdk-python",
     version=get_version(),
-    description="Official Python SDK for the Zscaler Products",
-    long_description=read('LONG_DESCRIPTION.md'),  # Read the content of the Markdown file
-    long_description_content_type='text/markdown',  # Specify the content type as Markdown
-    author="Zscaler Technology Alliances",
+    author="Zscaler, Inc.",
     author_email="devrel@zscaler.com",
     url="https://github.com/zscaler/zscaler-sdk-python",
-    packages=packages,
-    package_data=package_data,
+    license="MIT",
+    description="Official Python SDK for the Zscaler Products",
+    long_description=open("LONG_DESCRIPTION.md").read(),
+    long_description_content_type="text/markdown",
+    test_suite="tests",
+    packages=find_packages(exclude=("tests",)),
+    python_requires=">=3.8",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "License :: OSI Approved :: MIT License",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+    ],
     install_requires=[
-        "arrow", "certifi", "charset-normalizer", "idna", "python-box",
-        "python-dateutil", "requests", "responses", "restfly", "six",
-        "urllib3", "flatdict", "pyyaml", "xmltodict", "yarl",
-        "pycryptodomex", "aenum", "pydash", "flake8",
+        "arrow",
+        "certifi",
+        "charset-normalizer",
+        "idna",
+        "python-box",
+        "python-dateutil",
+        "requests",
+        "responses",
+        "restfly",
+        "six",
+        "urllib3",
+        "flatdict",
+        "pyyaml",
+        "xmltodict",
+        "yarl",
+        "pycryptodomex",
+        "aenum",
+        "pydash",
+        "flake8",
     ],
-    python_requires=">=3.8,<4.0",
-)
+)
```

### Comparing `zscaler-sdk-python-0.1.0/tests/conftest.py` & `zscaler-sdk-python-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/conftest.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/conftest.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_activation.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_activation.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_admin_and_role_management.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_admin_and_role_management.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_authentication_settings.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_authentication_settings.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_cloud_firewall_ip_destination_groups.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_cloud_firewall_ip_destination_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_cloud_firewall_ip_source_groups.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_cloud_firewall_ip_source_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_cloud_firewall_rule.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_cloud_firewall_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_dictionary.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_dlp_dictionary.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_engines.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_dlp_engines.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_icap_server.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_dlp_icap_server.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_idm_profile.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_dlp_idm_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_incident_receiver.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_dlp_incident_receiver.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_web_rule.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_dlp_web_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_isolation_profile.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_location_group.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_location_group.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_location_management.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_location_management.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_rule_labels.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_rule_labels.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_sandbox.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_sandbox.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_security.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_security.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_traffic_gre_tunnel.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_traffic_gre_tunnel.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_traffic_static_ip.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_traffic_static_ip.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_traffic_vpn_credential.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_traffic_vpn_credential.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_url_categories.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_url_categories.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_url_filtering_rule.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_url_filtering_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_users.py` & `zscaler-sdk-python-1.0.0/tests/integration/zia/test_users.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/conftest.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/conftest.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_access_policy_forwarding_rules.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_access_policy_forwarding_rules.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_access_policy_rules.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_access_policy_rules.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_access_policy_timeout_rules.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_access_policy_timeout_rules.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_app_connector_groups.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_app_connector_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_application_segment.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_application_segment.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_application_servers.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_application_servers.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_ba_certificates.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_ba_certificates.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_enrolment_certificates.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_enrolment_certificates.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_idp.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_idp.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_isolation_profile.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_machine_groups.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_machine_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_posture_profiles.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_posture_profiles.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_pra_approval.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_pra_approval.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_pra_credential.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_pra_credential.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_pra_portal.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_pra_portal.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_provisioning_key_app_connector_group.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_provisioning_key_app_connector_group.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_provisioning_key_service_edge_group.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_provisioning_key_service_edge_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """
 
     @pytest.mark.asyncio
     async def test_provisioning_key_operations(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
-        svc_edge_group_id = None
+        group_id = None
         svc_edge_group_key_id = None
 
         try:
             try:
                 # Prerequisite: Create an Service Edge Group for the SERVICE_EDGE_GRP Provisioning Key
                 svc_edge_group_name = "tests-" + generate_random_string()
                 svc_edge_group_description = "tests-" + generate_random_string()
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_saml_attributes.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_saml_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_scim_attributes.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_scim_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_scim_groups.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_scim_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_segment_groups.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_segment_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_server_groups.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_server_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_service_edge_groups.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_service_edge_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_trusted_networks.py` & `zscaler-sdk-python-1.0.0/tests/integration/zpa/test_trusted_networks.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/test_utils.py` & `zscaler-sdk-python-1.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/__init__.py` & `zscaler-sdk-python-1.0.0/zscaler/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,25 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
+"""Zscaler SDK for Python
+
+Zscaler SDK Python is an SDK that provides a uniform and easy-to-use interface for each of the Zscaler product APIs.
+
+Documentation available at https://zscaler-sdk-python.readthedocs.io
+
+"""
+
 __author__ = "Zscaler Inc"
 __email__ = "devrel@zscaler.com"
 __license__ = "MIT"
 __contributors__ = [
     "William Guilherme",
 ]
-__version__ = "0.1.0"
+__version__ = "1.0.0"
 
 from zscaler.zia import ZIAClientHelper  # noqa
 from zscaler.zpa import ZPAClientHelper  # noqa
```

### Comparing `zscaler-sdk-python-0.1.0/zscaler/cache/cache.py` & `zscaler-sdk-python-1.0.0/zscaler/cache/cache.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/cache/no_op_cache.py` & `zscaler-sdk-python-1.0.0/zscaler/cache/no_op_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/cache/zscaler_cache.py` & `zscaler-sdk-python-1.0.0/zscaler/cache/zscaler_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/constants.py` & `zscaler-sdk-python-1.0.0/zscaler/constants.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/errors/http_error.py` & `zscaler-sdk-python-1.0.0/zscaler/errors/http_error.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/errors/zscaler_api_error.py` & `zscaler-sdk-python-1.0.0/zscaler/errors/zscaler_api_error.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/exceptions/exceptions.py` & `zscaler-sdk-python-1.0.0/zscaler/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/logger.py` & `zscaler-sdk-python-1.0.0/zscaler/logger.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/ratelimiter/ratelimiter.py` & `zscaler-sdk-python-1.0.0/zscaler/ratelimiter/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/user_agent.py` & `zscaler-sdk-python-1.0.0/zscaler/user_agent.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/utils.py` & `zscaler-sdk-python-1.0.0/zscaler/utils.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/__init__.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/activate.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/activate.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 
 from zscaler.zia import ZIAClient
 
 
 class ActivationAPI:
+
     def __init__(self, client: ZIAClient):
         self.rest = client
 
     def status(self) -> str:
         """
         Returns the activation status for a configuration change.
```

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/admin_and_role_management.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/admin_and_role_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
+
+import logging
+
 from box import Box, BoxList
 from requests import Response
 
 from zscaler.utils import Iterator, snake_to_camel
 from zscaler.zia import ZIAClient
 
-
 class AdminAndRoleManagementAPI:
     def __init__(self, client: ZIAClient):
         self.rest = client
 
     def list_users(self, **kwargs) -> BoxList:
         """
         Returns a list of admin users.
```

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/apptotal.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/apptotal.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/audit_logs.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/audit_logs.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/authentication_settings.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/authentication_settings.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/client.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/client.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/cloud_apps.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/cloud_apps.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/device_management.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/device_management.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/dlp.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/errors.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/firewall.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/firewall.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/forwarding_control.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/forwarding_control.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/isolation_profile.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/isolation_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             **kwargs: Optional keyword arguments to refine the search query.
 
         Returns:
             :obj:`BoxList`: A list of isolation profile resource records.
 
         Examples:
             >>> isolation_profiles = zia.isolation_profiles.list_isolation_profiles()
-
+        
         """
         payload = {snake_to_camel(key): value for key, value in kwargs.items()}
         return self.rest.get("browserIsolation/profiles", json=payload)
 
     def get_profiles_by_name(self, name: str):
         """
         Retrieves a specific isolation profile by its name.
```

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/labels.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/labels.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/locations.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/locations.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/sandbox.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/sandbox.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/security.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/security.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/ssl_inspection.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/ssl_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/traffic.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/traffic.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/url_categories.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/url_categories.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/url_filtering.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/url_filtering.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/users.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/users.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/web_dlp.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/web_dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/workload_groups.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/workload_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/zpa_gateway.py` & `zscaler-sdk-python-1.0.0/zscaler/zia/zpa_gateway.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/__init__.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,15 @@
             api_version (str): Specifies the version of the API to be used. Helps in routing within the API service.
             search (str): Search query to filter the results based on specific conditions.
             search_field (str): The field name against which to search the query. Default is "name".
             max_pages (int): The maximum number of pages to fetch. If None, fetches all available pages.
             max_items (int): The maximum number of items to fetch across all pages. Stops fetching once reached.
             sort_order (str): Specifies the order of sorting (e.g., 'ASC' or 'DSC').
             sort_by (str): Specifies the field name by which the results should be sorted.
-            sort_dir (str): Specifies the direction of sorting. Supported values: ASC, DESC.
+            sort_dir (str): Specifies the direction of sorting. This is similar to `sort_order` and can be used interchangeably.
             start_time (str): The start of a time range for filtering data based on modification time.
             end_time (str): The end of a time range for filtering data based on modification time.
             idp_group_id (str): Identifier for a specific IDP group, used for fetching data related to that group.
             scim_user_id (str): Identifier for a specific SCIM user, used for fetching data related to that user.
             page (int): Specific page number to fetch. Overrides automatic pagination.
             pagesize (int): Number of items per page, default is 20 as per API specification, maximum is 500.
```

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/app_segments.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/app_segments.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,17 +292,17 @@
 
         # Handle the clientless_app_ids directly within this function without a separate helper
         if kwargs.get("clientless_app_ids"):
             # Here you would implement any necessary formatting directly
             formatted_clientless_apps = [
                 {"id": app.get("id")} for app in kwargs.pop("clientless_app_ids")
             ]
-            payload["clientlessApps"] = (
-                formatted_clientless_apps  # use the correct key expected by your API
-            )
+            payload[
+                "clientlessApps"
+            ] = formatted_clientless_apps  # use the correct key expected by your API
 
         # Convert other keys in payload
         add_id_groups(self.reformat_params, kwargs, payload)
 
         # Add remaining optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
```

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/app_segments_inspection.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/app_segments_inspection.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,17 +289,17 @@
                 for ports in kwargs.pop("udp_port_ranges")
             ]
 
         if common_apps_dto:
             camel_common_apps_dto = recursive_snake_to_camel(
                 common_apps_dto
             )  # use the recursive function
-            payload["commonAppsDto"] = (
-                camel_common_apps_dto  # ensure commonAppsDto gets added to payload
-            )
+            payload[
+                "commonAppsDto"
+            ] = camel_common_apps_dto  # ensure commonAppsDto gets added to payload
 
         # Convert other keys in payload
         add_id_groups(self.reformat_params, kwargs, payload)
 
         # Add remaining optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
```

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/app_segments_pra.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/app_segments_pra.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,17 +288,17 @@
                 for ports in kwargs.pop("udp_port_ranges")
             ]
 
         if common_apps_dto:
             camel_common_apps_dto = recursive_snake_to_camel(
                 common_apps_dto
             )  # use the recursive function
-            payload["commonAppsDto"] = (
-                camel_common_apps_dto  # ensure commonAppsDto gets added to payload
-            )
+            payload[
+                "commonAppsDto"
+            ] = camel_common_apps_dto  # ensure commonAppsDto gets added to payload
 
         # Convert other keys in payload
         add_id_groups(self.reformat_params, kwargs, payload)
 
         # Add remaining optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
```

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/certificates.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/certificates.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
     def add_certificate(self, name: str, cert_blob: str, **kwargs) -> Box:
         """
         Add a new Certificate.
 
         Args:
             name (str): The name of the certificate.
-            cert_blob (str): The content of the certificate. Must include the certificate and private key (in PEM format).
+            cert_blob (str): The content of the certificate. Must include the certificate and private key (in PEM format) in the JSON payload.
             **kwargs: Optional keyword args.
 
         Keyword Args:
             description (str): The description of the certificate.
 
         Returns:
             :obj:`Box`: The resource record for the newly created server.
```

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/client.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/client.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/cloud_connector_groups.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/cloud_connector_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/connectors.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/connectors.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/emergency_access.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/emergency_access.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/errors.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/idp.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/idp.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/inspection.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/isolation_profile.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/isolation_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,12 +76,10 @@
 
         Examples:
             >>> profile = zpa.isolation_profiles.get_profile_by_id('12345')
             >>> print(profile)
         """
         profiles = self.list_profiles()
         for profile in profiles:
-            if str(profile.get("id")) == str(
-                profile_id
-            ):  # Ensuring ID comparison as strings
+            if str(profile.get("id")) == str(profile_id):  # Ensuring ID comparison as strings
                 return profile
         return None
```

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/lss.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/lss.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/machine_groups.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/machine_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/policies.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/policies.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/posture_profiles.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/posture_profiles.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/privileged_remote_access.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/privileged_remote_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             **search (str, optional):
                 The search string used to match against features and fields.
 
         Returns:
             :obj:`BoxList`: A list of all configured privileged remote access portals.
 
         Examples:
-            >>> for pra_portal in zpa.privileged_remote_access.list_portals():
+            >>> for pra_portal in zpa.privilegedremoteaccess.list_portals():
             ...    pprint(pra_portal)
 
         """
         list, _ = self.rest.get_paginated_data(
             path="/praPortal", **kwargs, api_version="v1"
         )
         return list
@@ -63,15 +63,15 @@
             portal_id (str):
                 The unique identifier for the pra portal.
 
         Returns:
             :obj:`Box`: The resource record for the pra portal.
 
         Examples:
-            >>> pprint(zpa.privileged_remote_access.get_portal('99999'))
+            >>> pprint(zpa.privilegedremoteaccess.get_portal('99999'))
 
         """
         return self.rest.get(f"praPortal/{portal_id}")
 
     def add_portal(
         self,
         name: str,
@@ -99,22 +99,21 @@
         Keyword Args:
             description (str):
                 The description of the privileged portal.
             user_notification (str):
                 The notification message displayed in the banner of the privileged portallink, if enabled.
             user_notification_enabled (bool):
                 Indicates if the Notification Banner is enabled (true) or disabled (false)
-
         Returns:
             :obj:`Box`: The resource record for the newly created portal.
 
         Examples:
             Create a pra portal with the minimum required parameters:
 
-            >>> zpa.privileged_remote_access.add_portal(
+            >>> zpa.privilegedremoteaccess.add_portal(
             ...   name='PRA Portal Example',
             ...   certificate_id='123456789',
             ...   user_notification_enabled=True)
         """
         payload = {
             "name": name,
             "enabled": enabled,
@@ -162,21 +161,21 @@
 
         Returns:
             :obj:`Box`: The resource record for the updated portal.
 
         Examples:
             Update the name of a portal:
 
-            >>> zpa.privileged_remote_access.update_portal(
+            >>> zpa.privilegedremoteaccess.update_portal(
             ...   '99999',
             ...   name='Updated PRA Portal')
 
             Update the pra portal:
 
-            >>> zpa.privileged_remote_access.update_portal(
+            >>> zpa.privilegedremoteaccess.update_portal(
             ...    '99999',
             ...    name='Updated PRA Portal')
 
         """
         # Set payload to value of existing record
         payload = {snake_to_camel(k): v for k, v in self.get_portal(portal_id).items()}
 
@@ -196,15 +195,15 @@
         Args:
             portal_id (str): The unique identifier for the portal to be deleted.
 
         Returns:
             :obj:`int`: The response code for the operation.
 
         Examples:
-            >>> zpa.privileged_remote_access.delete_portal('99999')
+            >>> zpa.privilegedremoteaccess.delete_portal('99999')
 
         """
         return self.rest.delete(f"praPortal/{portal_id}").status_code
 
     def list_consoles(self, **kwargs) -> BoxList:
         """
         Returns a list of all privileged remote access consoles.
@@ -219,15 +218,15 @@
             **search (str, optional):
                 The search string used to match against features and fields.
 
         Returns:
             :obj:`BoxList`: A list of all configured privileged remote access consoles.
 
         Examples:
-            >>> for pra_console in zpa.privileged_remote_access.list_consoles():
+            >>> for pra_console in zpa.privilegedremoteaccess.list_consoles():
             ...    pprint(pra_console)
 
         """
         list, _ = self.rest.get_paginated_data(
             path="/praConsole", **kwargs, api_version="v1"
         )
         return list
@@ -240,15 +239,15 @@
             console_id (str):
                 The unique identifier for the pra console.
 
         Returns:
             :obj:`Box`: The resource record for the pra console.
 
         Examples:
-            >>> pprint(zpa.privileged_remote_access.get_console('99999'))
+            >>> pprint(zpa.privilegedremoteaccess.get_console('99999'))
 
         """
         return self.rest.get(f"praConsole/{console_id}")
 
     def get_console_portal(self, portal_id: str) -> Box:
         """
         Returns information on the specified pra console of the privileged portal.
@@ -257,15 +256,15 @@
             portal_id (str):
                 The unique identifier of the privileged portal.
 
         Returns:
             :obj:`Box`: The resource record for the privileged portal.
 
         Examples:
-            >>> pprint(zpa.privileged_remote_access.get_console_portal('99999'))
+            >>> pprint(zpa.privilegedremoteaccess.get_console_portal('99999'))
 
         """
         return self.rest.get(f"praConsole/praPortal/{portal_id}")
 
     def add_console(
         self,
         name: str,
@@ -286,15 +285,15 @@
         Keyword Args:
             description (str, optional): A description for the PRA console.
 
         Returns:
             Box: A Box object containing the details of the newly created console.
 
         Examples:
-            >>> zpa.privileged_remote_access.add_console(
+            >>> zpa.privilegedremoteaccess.add_console(
             ...     name='PRA Console Example',
             ...     pra_application_id='999999999',
             ...     pra_portal_ids=['999999999'],
             ...     description='PRA Console Description',
             ...     enabled=True
             ... )
         """
@@ -333,21 +332,21 @@
             console_id (str): The unique identifier of the console being updated.
 
         Keyword Args:
             name (str): The new name of the PRA console.
             description (str): The new description of the PRA console.
             enabled (bool): Indicates whether the console should be enabled.
             pra_application_id (str): The unique identifier of the associated PRA application to be linked with the console.
-            pra_portal_ids (list of str): List of unique IDs for the associated PRA portals to be linked with the console.
+            pra_portal_ids (list of str): A list of unique identifiers for the associated PRA portals to be linked with the console.
 
         Returns:
             Box: A Box object containing the details of the updated console.
 
         Examples:
-            >>> zpa.privileged_remote_access.update_console(
+            >>> zpa.privilegedremoteaccess.update_console(
             ...     console_id='99999',
             ...     name='Updated PRA Console',
             ...     description='Updated Description',
             ...     enabled=True,
             ...     pra_application_id='999999999',
             ...     pra_portal_ids=['999999999']
             ... )
@@ -378,15 +377,15 @@
         Args:
             console_id (str): The unique identifier for the console to be deleted.
 
         Returns:
             :obj:`int`: The response code for the operation.
 
         Examples:
-            >>> zpa.privileged_remote_access.delete_console('99999')
+            >>> zpa.privilegedremoteaccess.delete_console('99999')
 
         """
         response = self.rest.delete(f"/praConsole/{console_id}")
         if response.status_code != 204:
             raise Exception(f"Failed to delete console: {response.text}")
         return response.status_code
 
@@ -400,15 +399,15 @@
                 'name', 'pra_application_id', and 'pra_portal_ids'. Optionally, 'enabled' and 'description'
                 can also be included.
 
         Returns:
             Box: A Box object containing the details of the newly created consoles.
 
         Examples:
-            >>> zpa.privileged_remote_access.add_bulk_console([
+            >>> zpa.privilegedremoteaccess.add_bulk_console([
             ...     {
             ...         'name': 'PRA Console Example 1',
             ...         'pra_application_id': '999999999',
             ...         'pra_portal_ids': ['999999998'],
             ...         'description': 'PRA Console Description 1',
             ...         'enabled': True
             ...     },
@@ -456,15 +455,15 @@
             **search (str, optional):
                 The search string used to match against features and fields.
 
         Returns:
             :obj:`BoxList`: A list of all configured privileged remote access credentials.
 
         Examples:
-            >>> for pra_credential in zpa.privileged_remote_access.list_credentials():
+            >>> for pra_credential in zpa.privilegedremoteaccess.list_credentials():
             ...    pprint(pra_credential)
 
         """
         list, _ = self.rest.get_paginated_data(
             path="/credential", **kwargs, api_version="v1"
         )
         return list
@@ -477,15 +476,15 @@
             credential_id (str):
                 The unique identifier for the pra credential.
 
         Returns:
             :obj:`Box`: The resource record for the pra credential.
 
         Examples:
-            >>> pprint(zpa.privileged_remote_access.get_credential('99999'))
+            >>> pprint(zpa.privilegedremoteaccess.get_credential('99999'))
 
         """
         return self.rest.get(f"credential/{credential_id}")
         # response = self.rest.get("/credential/%s" % (credential_id))
         # if isinstance(response, Response):
         #     status_code = response.status_code
         #     if status_code != 200:
@@ -565,15 +564,15 @@
             Box: The resource record for the updated credential.
 
         Raises:
             Exception: If fetching the credential fails or the required parameters are missing based on the credential type.
 
         Examples:
             Update a USERNAME_PASSWORD credential:
-            >>> zpa.privileged_remote_access.update_credential(
+            >>> zpa.privilegedremoteaccess.update_credential(
             ...     credential_id='2223',
             ...     username='jdoe',
             ...     name='John Doe',
             ...     credential_type='USERNAME_PASSWORD',
             ...     password='**********',
             ...     description='Updated credential description'
             ... )
@@ -619,59 +618,55 @@
         Args:
             credential_id (str): The unique identifier for the credential to be deleted.
 
         Returns:
             :obj:`int`: The response code for the operation.
 
         Examples:
-            >>> zpa.privileged_remote_access.delete_credential('99999')
+            >>> zpa.privilegedremoteaccess.delete_credential('99999')
 
         """
         return self.rest.delete(f"credential/{credential_id}").status_code
+        # response = self.rest.delete(f"/credential/{credential_id}")
+        # if response.status_code != 204:
+        #     raise Exception(f"Failed to delete credential: {response.text}")
+        # return response.status_code
 
     def list_approval(self, **kwargs) -> BoxList:
         """
         Returns a list of all privileged remote access approvals.
 
         Keyword Args:
             max_items (int):
                 The maximum number of items to request before stopping iteration.
             max_pages (int):
                 The maximum number of pages to request before stopping iteration.
             pagesize (int):
-                Specifies the page size. Default is 20, maximum is 500.
+                Specifies the page size. The default size is 20, but the maximum size is 500.
             search (str, optional):
                 The search string used to match against features and fields.
             search_field (str, optional):
-                The field to search against. Defaults to 'name'. Commonly used fields
-                include 'name' and 'email_ids'.
+                The field to search against. Defaults to 'name'. Commonly used fields include 'name' and 'email_ids'.
 
         Returns:
             :obj:`BoxList`: A list of all configured privileged remote access approvals.
 
         Examples:
             Search by default field 'name':
-
-            >>> for pra_approval in zpa.privileged_remote_access.list_approval(
-            ...     search='Example_Name'):
+            >>> for pra_approval in zpa.privilegedremoteaccess.list_approval(search='Example_Name'):
             ...     pprint(pra_approval)
 
             Search by 'email_ids':
-
-            >>> for approval in zpa.privileged_remote_access.list_approval(
-            ...     search='jdoe@example.com', search_field='email_ids'):
-            ...     pprint(approval)
+            >>> for pra_approval in zpa.privilegedremoteaccess.list_approval(search='jdoe@example.com', search_field='email_ids'):
+            ...     pprint(pra_approval)
 
             Specify maximum items and use an explicit search field:
-
-            >>> approvals = zpa.privileged_remote_access.list_approval(
-            ...     search='Example_Name', search_field='name', max_items=10)
-            ... for approval in approvals:
+            >>> approvals = zpa.privilegedremoteaccess.list_approval(search='Example_Name', search_field='name', max_items=10)
+            >>> for approval in approvals:
             ...     pprint(approval)
-
         """
         list, _ = self.rest.get_paginated_data(
             path="/approval", **kwargs, api_version="v1"
         )
         return list
 
     def get_approval(self, approval_id: str) -> Box:
@@ -682,15 +677,15 @@
             approval_id (str):
                 The unique identifier for the pra approval.
 
         Returns:
             :obj:`Box`: The resource record for the pra approval.
 
         Examples:
-            >>> pprint(zpa.privileged_remote_access.get_approval('99999'))
+            >>> pprint(zpa.privilegedremoteaccess.get_approval('99999'))
 
         """
         return self.rest.get(f"approval/{approval_id}")
 
     def add_approval(
         self,
         email_ids: list,
@@ -706,26 +701,26 @@
 
         Args:
             email_ids (list): The email addresses of the users that you are assigning the privileged approval to.
             application_ids (list of str): A list of unique identifiers for the associated application segment ids.
             start_time (str): The start timestamp in UNIX format for when the approval begins.
             end_time (str): The end timestamp in UNIX format for when the approval ends.
             status (str): The status of the privileged approval. Supported values are: INVALID, ACTIVE, FUTURE, EXPIRED.
-            working_hours (dict): Dictionary containing details of working hours.
+            working_hours (dict): A dictionary containing the details of working hours including cron expressions for start and end times, actual start and end times, days of the week, and time zone.
 
         Keyword Args:
             Any additional optional parameters that can be included in the payload.
 
         Returns:
             Box: The resource record for the newly created approval.
 
         Examples:
             Create a PRA approval with the minimum required parameters and working hours:
 
-            >>> zpa.privileged_remote_access.add_approval(
+            >>> zpa.privilegedremoteaccess.add_approval(
             ...   email_ids=['jdoe@example.com'],
             ...   application_ids=['999999999'],
             ...   start_time='1712856502',
             ...   end_time='1714498102',
             ...   status='ACTIVE',
             ...   working_hours={
             ...       "start_time_cron": "0 0 16 ? * SUN,MON,TUE,WED,THU,FRI,SAT",
@@ -844,24 +839,24 @@
         Args:
             approval_id (str): The unique identifier for the approval to be deleted.
 
         Returns:
             :obj:`int`: The response code for the operation.
 
         Examples:
-            >>> zpa.privileged_remote_access.delete_approval('99999')
+            >>> zpa.privilegedremoteaccess.delete_approval('99999')
 
         """
         return self.rest.delete(f"approval/{approval_id}").status_code
 
     def expired_approval(self) -> int:
         """
         Deletes all expired privileged approvals.
 
         Returns:
             :obj:`int`: The response code for the operation.
 
         Examples:
-            >>> zpa.privileged_remote_access.expired_approval('99999')
+            >>> zpa.privilegedremoteaccess.expired_approval('99999')
 
         """
         return self.rest.delete("approval/expired").status_code
```

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/provisioning.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/provisioning.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/saml_attributes.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/saml_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/scim_attributes.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/scim_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/scim_groups.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/scim_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,25 @@
         """
         list, _ = self.rest.get_paginated_data(
             path=f"/scimgroup/idpId/{idp_id}",
             **kwargs,
             api_version="userconfig_v1",
         )
         return list
+        # params = {}
+        # if sort_order != "" and sort_by != "":
+        #     params["sortBy"] = sort_by
+        #     params["sortOrder"] = sort_order
+        # list, _ = self.rest.get_paginated_data(
+        #     path=f"/scimgroup/idpId/{idp_id}",
+        #     params=params,
+        #     **kwargs,
+        #     api_version="userconfig_v1",
+        # )
+        # return list
 
     def get_group(self, group_id: str, **kwargs) -> Box:
         """
         Returns information on the specified SCIM group.
 
         Args:
             group_id (str):
```

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/segment_groups.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/segment_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/server_groups.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/server_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/servers.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/servers.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/service_edges.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/service_edges.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/trusted_networks.py` & `zscaler-sdk-python-1.0.0/zscaler/zpa/trusted_networks.py`

 * *Files identical despite different names*

