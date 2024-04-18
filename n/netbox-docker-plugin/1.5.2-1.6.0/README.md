# Comparing `tmp/netbox_docker_plugin-1.5.2.tar.gz` & `tmp/netbox_docker_plugin-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_docker_plugin-1.5.2.tar", last modified: Tue Apr 16 08:03:35 2024, max compression
+gzip compressed data, was "netbox_docker_plugin-1.6.0.tar", last modified: Thu Apr 18 14:48:47 2024, max compression
```

## Comparing `netbox_docker_plugin-1.5.2.tar` & `netbox_docker_plugin-1.6.0.tar`

### file list

```diff
@@ -1,130 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.201006 netbox_docker_plugin-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-16 08:03:35.201006 netbox_docker_plugin-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.181005 netbox_docker_plugin-1.5.2/netbox_docker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.181005 netbox_docker_plugin-1.5.2/netbox_docker_plugin/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14679 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.185006 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/network_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.189005 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0002_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0003_image_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0004_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0005_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0011_host_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0012_host_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0013_host_netbox_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0014_container_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0016_alter_env_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0017_network_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0020_container_hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0021_registry_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0023_delete_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0025_alter_image_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.189005 netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.177005 netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.193005 netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/netbox_docker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/netbox_docker_plugin/container.html
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/netbox_docker_plugin/host.html
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/netbox_docker_plugin/image.html
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/netbox_docker_plugin/network.html
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.193005 netbox_docker_plugin-1.5.2/netbox_docker_plugin/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/templatetags/host.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.193005 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.193005 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/container/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/container/test_container_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/container/test_container_operation_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/container/test_container_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/container/test_container_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.193005 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/host/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/host/test_host_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/host/test_host_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/host/test_replace_password.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.193005 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/image/test_image_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/image/test_image_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.197006 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/network/test_network_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/network/test_network_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.197006 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/registry/test_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/registry/test_registry_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.197006 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/volume/test_volume_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/volume/test_volume_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.197006 netbox_docker_plugin-1.5.2/netbox_docker_plugin/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.197006 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/label.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/network_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:35.197006 netbox_docker_plugin-1.5.2/netbox_docker_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-16 08:03:35.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-16 08:03:35.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:03:35.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 08:03:35.000000 netbox_docker_plugin-1.5.2/netbox_docker_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 08:03:31.000000 netbox_docker_plugin-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:03:35.201006 netbox_docker_plugin-1.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.041770 netbox_docker_plugin-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-18 14:48:47.041770 netbox_docker_plugin-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.025770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.029770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.029770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/network_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.033770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0002_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0003_image_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0004_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0005_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0011_host_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0012_host_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0014_container_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0016_alter_env_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0017_network_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0020_container_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0021_registry_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0023_delete_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0025_alter_image_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0026_image_digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0027_container_restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.033770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10657 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.025770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.037770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/netbox_docker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.037770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/templatetags/host.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.037770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.037770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/container/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/container/test_container_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/container/test_container_operation_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/container/test_container_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/container/test_container_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.037770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/host/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/host/test_host_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/host/test_host_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/host/test_replace_password.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.037770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/image/test_image_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/image/test_image_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.037770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/network/test_network_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/network/test_network_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.041770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/registry/test_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/registry/test_registry_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.041770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/volume/test_volume_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/volume/test_volume_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.041770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.041770 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/network_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:48:47.041770 netbox_docker_plugin-1.6.0/netbox_docker_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-18 14:48:47.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-18 14:48:47.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:48:47.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 14:48:47.000000 netbox_docker_plugin-1.6.0/netbox_docker_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-18 14:48:43.000000 netbox_docker_plugin-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:48:47.041770 netbox_docker_plugin-1.6.0/setup.cfg
```

### Comparing `netbox_docker_plugin-1.5.2/LICENSE` & `netbox_docker_plugin-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/PKG-INFO` & `netbox_docker_plugin-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-docker-plugin
-Version: 1.5.2
+Version: 1.6.0
 Summary: Manage Docker with Netbox & style.
 Author-email: Vincent Simonin <vincent@saashup.com>
 Project-URL: Homepage, https://github.com/SaaShup/netbox-docker-plugin
 Project-URL: Bug Tracker, https://github.com/SaaShup/netbox-docker-plugin/issues
 Keywords: netbox,netbox-plugin,docker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `netbox_docker_plugin-1.5.2/README.md` & `netbox_docker_plugin-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/__init__.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class NetBoxDockerConfig(PluginConfig):
     """Plugin Config Class"""
 
     name = "netbox_docker_plugin"
     verbose_name = " NetBox Docker Plugin"
     description = "Manage Docker"
-    version = "1.5.2"
+    version = "1.6.0"
     base_url = "docker"
     author= "Vincent Simonin"
     author_email= "vincent@saashup.com"
 
     def ready(self):
         post_migrate.connect(create_webhook)
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/api/serializers.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/api/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,15 @@
             "id",
             "url",
             "display",
             "name",
             "version",
             "size",
             "ImageID",
+            "Digest",
         )
 
 
 class NestedVolumeSerializer(WritableNestedSerializer):
     """Nested Volume Serializer class"""
 
     url = serializers.HyperlinkedIdentityField(
@@ -122,14 +123,15 @@
         fields = (
             "id",
             "url",
             "name",
             "ContainerID",
             "state",
             "status",
+            "restart_policy",
             "operation",
             "hostname",
         )
 
 
 class NestedMountSerializer(WritableNestedSerializer):
     """Nested Mount Serializer class"""
@@ -199,14 +201,15 @@
             "display",
             "host",
             "name",
             "version",
             "registry",
             "size",
             "ImageID",
+            "Digest",
             "custom_fields",
             "created",
             "last_updated",
             "containers",
             "tags",
         )
 
@@ -375,14 +378,15 @@
             "image",
             "name",
             "state",
             "operation",
             "status",
             "ContainerID",
             "hostname",
+            "restart_policy",
             "ports",
             "env",
             "labels",
             "mounts",
             "binds",
             "network_settings",
             "custom_fields",
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/api/views.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/filtersets.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/filtersets.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         label="Image (ID)",
     )
 
     class Meta:
         """Container filterset definition meta class"""
 
         model = Container
-        fields = ("id", "name", "state", "hostname")
+        fields = ("id", "name", "state", "hostname", "restart_policy")
 
     # pylint: disable=W0613
     def search(self, queryset, name, value):
         """override"""
         if not value.strip():
             return queryset
         return queryset.filter(Q(name__icontains=value))
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/bind.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/container.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/container.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,19 @@
     NetBoxModelForm,
     NetBoxModelImportForm,
     NetBoxModelFilterSetForm,
     NetBoxModelBulkEditForm,
 )
 from ..models.volume import Volume
 from ..models.host import Host
-from ..models.container import Container, ContainerStateChoices
+from ..models.container import (
+    Container,
+    ContainerStateChoices,
+    ContainerRestartPolicyChoices,
+)
 from ..models.image import Image
 
 
 class ContainerForm(NetBoxModelForm):
     """Container form definition class"""
 
     host = DynamicModelChoiceField(
@@ -37,22 +41,24 @@
         model = Container
         fields = (
             "host",
             "image",
             "name",
             "hostname",
             "state",
+            "restart_policy",
             "tags",
         )
         labels = {
             "name": "Name",
             "host": "Host",
             "image": "Image",
             "hostname": "Hostname",
             "state": "State",
+            "restart_policy": "Restart Policy",
         }
 
 
 class ContainerFilterForm(NetBoxModelFilterSetForm):
     """Container filter form definition class"""
 
     model = Volume
@@ -72,26 +78,36 @@
         queryset=Image.objects.all(),
         required=False,
         label="Image",
     )
     state = forms.ChoiceField(
         label="State", choices=ContainerStateChoices, required=False
     )
+    restart_policy = forms.ChoiceField(
+        label="Restart Policy", choices=ContainerRestartPolicyChoices, required=False
+    )
     tag = TagFilterField(model)
 
 
 class ContainerImportForm(NetBoxModelImportForm):
     """Container importation form definition class"""
 
     state = forms.ChoiceField(
         label="State",
         choices=ContainerStateChoices,
         required=False,
         help_text="Container State. Can be `created`, `restarting`, "
-        + "`running`, `paused`, `exited`or `dead`.",
+        + "`running`, `paused`, `exited` or `dead`.",
+    )
+    restart_policy = forms.ChoiceField(
+        label="Restart Policy",
+        choices=ContainerRestartPolicyChoices,
+        required=False,
+        help_text="Container restart policy. Can be `no`, `on-failure`, "
+        + "`always`, `unless-stopped`.",
     )
 
     class Meta:
         """Container importation form definition Meta class"""
 
         model = Container
         fields = (
@@ -101,34 +117,36 @@
             "state",
             "hostname",
         )
         labels = {
             "name": "Unique container name",
             "host": "Host identifier",
             "image": "Image identifier",
-            "state": "Container State. Can be `created`, `restarting`, "
-            + "`running`, `paused`, `exited`or `dead`.",
-            "hostname": "Container hostname"
         }
 
 
 class ContainerBulkEditForm(NetBoxModelBulkEditForm):
     """Container bulk edit form definition class"""
 
     state = forms.ChoiceField(
         label="State",
         choices=ContainerStateChoices,
         required=True,
     )
+    restart_policy = forms.ChoiceField(
+        label="Restart Policy",
+        choices=ContainerRestartPolicyChoices,
+        required=True,
+    )
     hostname = forms.CharField(
         label="Hostname", max_length=256, min_length=1, required=False
     )
 
     model = Container
-    fieldsets = (("General", ("state", "hostname")),)
+    fieldsets = (("General", ("state", "restart_policy", "hostname")),)
 
 
 class ContainerOperationForm(NetBoxModelForm):
     """Container Operation form definition class"""
 
     class Meta:
         """Container form definition Meta class"""
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/env.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/env.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/host.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/host.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/image.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/label.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/label.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/mount.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/mount.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/network.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/network_setting.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/network_setting.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/port.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/port.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/registry.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/forms/volume.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/forms/volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0001_initial.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0002_image.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0002_image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0003_image_size.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0003_image_size.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0004_volume.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0004_volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0005_network.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0005_network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0011_host_token.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0011_host_token.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0012_host_state.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0012_host_state.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0013_host_netbox_url.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0016_alter_env_value.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0016_alter_env_value.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0020_container_hostname.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0020_container_hostname.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0021_registry_and_more.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0021_registry_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0023_delete_hosts.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0023_delete_hosts.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/0025_alter_image_version.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/0025_alter_image_version.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/migrations/__init__.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/container.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/container.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,29 @@
         ("restart", "Restart", "blue"),
         ("stop", "Stop", "blue"),
         ("recreate", "Recreate", "blue"),
         ("none", "None", "white"),
     ]
 
 
+class ContainerRestartPolicyChoices(ChoiceSet):
+    """Container restart policy choices definition class"""
+
+    key = "Container.restart_policy"
+
+    DEFAULT_VALUE = "no"
+
+    CHOICES = [
+        ("no", "no", "dark"),
+        ("on-failure", "on-failure", "blue"),
+        ("always", "always", "blue"),
+        ("unless-stopped", "unless-stopped", "blue"),
+    ]
+
+
 class PortTypeChoices(ChoiceSet):
     """Port type choices definition class"""
 
     key = "Port.type"
 
     DEFAULT_VALUE = "tcp"
 
@@ -108,14 +123,19 @@
         validators=[
             MinLengthValidator(limit_value=1),
             MaxLengthValidator(limit_value=256),
         ],
         blank=True,
         null=True,
     )
+    restart_policy = models.CharField(
+        max_length=32,
+        choices=ContainerRestartPolicyChoices,
+        default=ContainerRestartPolicyChoices.DEFAULT_VALUE,
+    )
 
     class Meta:
         """Image Model Meta Class"""
 
         ordering = ("name",)
         constraints = (
             models.UniqueConstraint(
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/host.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/host.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/image.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,23 @@
         validators=[
             MinLengthValidator(limit_value=1),
             MaxLengthValidator(limit_value=128),
         ],
         blank=True,
         null=True,
     )
+    Digest = models.CharField(
+        max_length=512,
+        validators=[
+            MinLengthValidator(limit_value=1),
+            MaxLengthValidator(limit_value=512),
+        ],
+        blank=True,
+        null=True,
+    )
 
     class Meta:
         """Image Model Meta Class"""
 
         ordering = ("name", "version")
         constraints = (
             models.UniqueConstraint(
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/network.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/registry.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/models/volume.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/models/volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/navigation.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tables.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,14 +251,15 @@
             "host",
             "name",
             "image",
             "state",
             "status",
             "ContainerID",
             "hostname",
+            "restart_policy",
             "port_count",
             "mount_count",
             "bind_count",
             "networksetting_count",
             "env_count",
             "label_count",
             "tags",
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/netbox_docker_plugin/container.html` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,18 @@
             <td>{{ object.hostname|placeholder }}</td>
           </tr>
           <tr>
             <th scope="row">State</th>
             <td>{{ object.get_state_display }}</td>
           </tr>
           <tr>
+            <th scope="row">Restart Policy</th>
+            <td>{{ object.get_restart_policy_display }}</td>
+          </tr>
+          <tr>
             <th scope="row">Status</th>
             <td>{{ object.status|placeholder }}</td>
           </tr>
           <tr>
             <th scope="row">Operation</th>
             <td>{{ object.get_operation_display }}</td>
           </tr>
```

#### html2text {}

```diff
@@ -2,22 +2,23 @@
 %}
 {% csrf_token %} Start
 {% csrf_token %} Stop
 {% csrf_token %} Restart
 {% csrf_token %} Recreate
 {% endblock %} {% block content %}
 **** CCOONNTTAAIINNEERR ****
-HHoosstt        _{_{_ _o_b_j_e_c_t_._h_o_s_t_ _}_}
-IImmaaggee       _{_{_ _o_b_j_e_c_t_._i_m_a_g_e_ _}_}
-NNaammee        {{ object.name }}
-CCoonnttaaiinneerrIIDD {{ object.ContainerID|placeholder }}
-HHoossttnnaammee    {{ object.hostname|placeholder }}
-SSttaattee       {{ object.get_state_display }}
-SSttaattuuss      {{ object.status|placeholder }}
-OOppeerraattiioonn   {{ object.get_operation_display }}
+HHoosstt           _{_{_ _o_b_j_e_c_t_._h_o_s_t_ _}_}
+IImmaaggee          _{_{_ _o_b_j_e_c_t_._i_m_a_g_e_ _}_}
+NNaammee           {{ object.name }}
+CCoonnttaaiinneerrIIDD    {{ object.ContainerID|placeholder }}
+HHoossttnnaammee       {{ object.hostname|placeholder }}
+SSttaattee          {{ object.get_state_display }}
+RReessttaarrtt PPoolliiccyy {{ object.get_restart_policy_display }}
+SSttaattuuss         {{ object.status|placeholder }}
+OOppeerraattiioonn      {{ object.get_operation_display }}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/tags.html'
 %} {% plugin_left_page object %}
 **** PPOORRTT MMAAPPPPIINNGGSS ****
 {% if perms.netbox_docker_plugin.add_env %}
 _A_d_d_ _a_ _P_o_r_t_ _M_a_p_p_i_n_g
 {% endif %}
 **** MMOOUUNNTTSS ****
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/netbox_docker_plugin/host.html` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/netbox_docker_plugin/image.html` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html`

 * *Files 9% similar despite different names*

```diff
@@ -2,48 +2,40 @@
 
 {% load plugins %}
 
 {% block content %}
 <div class="row mb-3">
   <div class="col col-md-6">
     <div class="card">
-      <h5 class="card-header">IMAGE</h5>
+      <h5 class="card-header">VOLUME</h5>
       <div class="card-body">
         <table class="table table-hover attr-table">
           <tr>
             <th scope="row">Host</th>
             <td><a href="{{ object.host.get_absolute_url }}">{{ object.host }}</a></td>
           </tr>
           <tr>
-            <th scope="row">Name & Version</th>
-            <td>{{ object.name }}:{{ object.version }}</td>
+            <th scope="row">Name</th>
+            <td>{{ object.name }}</td>
           </tr>
           <tr>
-            <th scope="row">Registry</th>
-            <td><a href="{{ object.registry.get_absolute_url }}">{{ object.registry }}</a></td>
-          </tr>
-          <tr>
-            <th scope="row">Size</th>
-            <td>{{ object.size }}&nbsp;MByte</td>
-          </tr>
-          <tr>
-            <th scope="row">ImageID</th>
-            <td>{{ object.ImageID|placeholder }}</td>
+            <th scope="row">Driver</th>
+            <td>{{ object.get_driver_display }}</td>
           </tr>
         </table>
       </div>
     </div>
     {% include 'inc/panels/custom_fields.html' %}
     {% include 'inc/panels/tags.html' %}
     {% plugin_left_page object %}
   </div>
   <div class="col col-md-6">
     <div class="card">
       <h5 class="card-header">USED BY</h5>
       <div class="card-body htmx-container table-responsive"
-        hx-get="{% url 'plugins:netbox_docker_plugin:container_list' %}?image_id={{ object.pk }}"
+        hx-get="{% url 'plugins:netbox_docker_plugin:mount_list' %}?volume_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
     </div>
   </div>
 </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,11 +1,9 @@
 {% extends 'generic/object.html' %} {% load plugins %} {% block content %}
-**** IIMMAAGGEE ****
-HHoosstt           _{_{_ _o_b_j_e_c_t_._h_o_s_t_ _}_}
-NNaammee && VVeerrssiioonn {{ object.name }}:{{ object.version }}
-RReeggiissttrryy       _{_{_ _o_b_j_e_c_t_._r_e_g_i_s_t_r_y_ _}_}
-SSiizzee           {{ object.size }} MByte
-IImmaaggeeIIDD        {{ object.ImageID|placeholder }}
+**** VVOOLLUUMMEE ****
+HHoosstt   _{_{_ _o_b_j_e_c_t_._h_o_s_t_ _}_}
+NNaammee   {{ object.name }}
+DDrriivveerr {{ object.get_driver_display }}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/tags.html'
 %} {% plugin_left_page object %}
 **** UUSSEEDD BBYY ****
 {% endblock content %}
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/netbox_docker_plugin/network.html` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html`

 * *Files 21% similar despite different names*

```diff
@@ -2,40 +2,58 @@
 
 {% load plugins %}
 
 {% block content %}
 <div class="row mb-3">
   <div class="col col-md-6">
     <div class="card">
-      <h5 class="card-header">VOLUME</h5>
+      <h5 class="card-header">IMAGE</h5>
       <div class="card-body">
         <table class="table table-hover attr-table">
           <tr>
             <th scope="row">Host</th>
             <td><a href="{{ object.host.get_absolute_url }}">{{ object.host }}</a></td>
           </tr>
           <tr>
-            <th scope="row">Name</th>
-            <td>{{ object.name }}</td>
+            <th scope="row">Name & Version</th>
+            <td>{{ object.name }}:{{ object.version }}</td>
           </tr>
           <tr>
-            <th scope="row">Driver</th>
-            <td>{{ object.get_driver_display }}</td>
+            <th scope="row">Registry</th>
+            <td><a href="{{ object.registry.get_absolute_url }}">{{ object.registry }}</a></td>
+          </tr>
+          <tr>
+            <th scope="row">Size</th>
+            <td>{{ object.size }}&nbsp;MByte</td>
+          </tr>
+          <tr>
+            <th scope="row">ImageID</th>
+            <td>{{ object.ImageID|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Digest</th>
+            <td>
+              {% if object.Digest is None %}
+                {{ object.Digest|placeholder }}
+              {% else %}
+                {{ object.Digest|truncatechars:32 }}
+              {% endif %}
+            </td>
           </tr>
         </table>
       </div>
     </div>
     {% include 'inc/panels/custom_fields.html' %}
     {% include 'inc/panels/tags.html' %}
     {% plugin_left_page object %}
   </div>
   <div class="col col-md-6">
     <div class="card">
       <h5 class="card-header">USED BY</h5>
       <div class="card-body htmx-container table-responsive"
-        hx-get="{% url 'plugins:netbox_docker_plugin:mount_list' %}?volume_id={{ object.pk }}"
+        hx-get="{% url 'plugins:netbox_docker_plugin:container_list' %}?image_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
     </div>
   </div>
 </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,9 +1,13 @@
 {% extends 'generic/object.html' %} {% load plugins %} {% block content %}
-**** VVOOLLUUMMEE ****
-HHoosstt   _{_{_ _o_b_j_e_c_t_._h_o_s_t_ _}_}
-NNaammee   {{ object.name }}
-DDrriivveerr {{ object.get_driver_display }}
+**** IIMMAAGGEE ****
+HHoosstt           _{_{_ _o_b_j_e_c_t_._h_o_s_t_ _}_}
+NNaammee && VVeerrssiioonn {{ object.name }}:{{ object.version }}
+RReeggiissttrryy       _{_{_ _o_b_j_e_c_t_._r_e_g_i_s_t_r_y_ _}_}
+SSiizzee           {{ object.size }} MByte
+IImmaaggeeIIDD        {{ object.ImageID|placeholder }}
+DDiiggeesstt         {% if object.Digest is None %} {{ object.Digest|placeholder }}
+               {% else %} {{ object.Digest|truncatechars:32 }} {% endif %}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/tags.html'
 %} {% plugin_left_page object %}
 **** UUSSEEDD BBYY ****
 {% endblock content %}
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/base.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/container/test_container_api.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/container/test_container_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     model = Container
     brief_fields = [
         "ContainerID",
         "hostname",
         "id",
         "name",
         "operation",
+        "restart_policy",
         "state",
         "status",
         "url",
     ]
     validation_excluded_fields = [
         "ports",
         "env",
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/container/test_container_operation_view.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/container/test_container_operation_view.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/container/test_container_validation.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/container/test_container_validation.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/container/test_container_views.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/container/test_container_views.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,35 +27,39 @@
             host=host2, name="registry2", serveraddress="http://localhost:8082"
         )
 
         image1 = Image.objects.create(host=host1, name="image1", registry=registry1)
         image2 = Image.objects.create(host=host2, name="image2", registry=registry2)
 
         container1 = Container.objects.create(
-            host=host1, image=image1, name="container1"
+            host=host1, image=image1, name="container1", restart_policy="always"
         )
         container2 = Container.objects.create(
             host=host1, image=image1, name="container2"
         )
         Container.objects.create(host=host2, image=image2, name="container3")
         Container.objects.create(host=host2, image=image2, name="container4")
 
         cls.form_data = {
             "name": "container5",
             "host": host1.pk,
             "image": image1.pk,
             "state": "created",
+            "restart_policy": "unless-stopped",
         }
 
         cls.csv_data = (
             "name,host,image,hostname",
             f"container6,{host1.pk},{image1.pk},",
             f"container7,{host2.pk},{image2.pk},container7",
         )
 
-        cls.bulk_edit_data = {"state": "running"}
+        cls.bulk_edit_data = {
+            "state": "running",
+            "restart_policy": "always",
+        }
 
         cls.csv_update_data = (
-            "id,name,host,image,state,hostname",
-            f"{container1.pk},container1,{host1.pk},{image1.pk},paused,",
-            f"{container2.pk},container2,{host1.pk},{image1.pk},running,container2",
+            "id,name,host,image,state,hostname,restart_policy",
+            f"{container1.pk},container1,{host1.pk},{image1.pk},paused,,on-failure",
+            f"{container2.pk},container2,{host1.pk},{image1.pk},running,container2,unless-stopped",
         )
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/host/test_host_api.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/host/test_host_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/host/test_host_views.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/host/test_host_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/host/test_replace_password.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/host/test_replace_password.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/image/test_image_api.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/image/test_image_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     APIViewTestCases.UpdateObjectViewTestCase,
     APIViewTestCases.DeleteObjectViewTestCase,
 ):
     """Image Test Case Class"""
 
     model = Image
     brief_fields = [
+        "Digest",
         "ImageID",
         "display",
         "id",
         "name",
         "size",
         "url",
         "version",
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/image/test_image_views.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/image/test_image_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/network/test_network_api.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/network/test_network_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/network/test_network_views.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/network/test_network_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/registry/test_registry_api.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/registry/test_registry_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/registry/test_registry_views.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/registry/test_registry_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/test_init.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/volume/test_volume_api.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/volume/test_volume_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/tests/volume/test_volume_views.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/tests/volume/test_volume_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/urls.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/utilities/__init__.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/bind.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/container.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/container.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/env.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/env.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/host.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/host.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/image.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/label.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/label.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/mount.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/mount.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/network.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/network_setting.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/network_setting.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/port.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/port.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/registry.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin/views/volume.py` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin/views/volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin.egg-info/PKG-INFO` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-docker-plugin
-Version: 1.5.2
+Version: 1.6.0
 Summary: Manage Docker with Netbox & style.
 Author-email: Vincent Simonin <vincent@saashup.com>
 Project-URL: Homepage, https://github.com/SaaShup/netbox-docker-plugin
 Project-URL: Bug Tracker, https://github.com/SaaShup/netbox-docker-plugin/issues
 Keywords: netbox,netbox-plugin,docker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `netbox_docker_plugin-1.5.2/netbox_docker_plugin.egg-info/SOURCES.txt` & `netbox_docker_plugin-1.6.0/netbox_docker_plugin.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
 netbox_docker_plugin/migrations/0020_container_hostname.py
 netbox_docker_plugin/migrations/0021_registry_and_more.py
 netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
 netbox_docker_plugin/migrations/0023_delete_hosts.py
 netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
 netbox_docker_plugin/migrations/0025_alter_image_version.py
+netbox_docker_plugin/migrations/0026_image_digest.py
+netbox_docker_plugin/migrations/0027_container_restart_policy.py
 netbox_docker_plugin/migrations/__init__.py
 netbox_docker_plugin/models/__init__.py
 netbox_docker_plugin/models/container.py
 netbox_docker_plugin/models/host.py
 netbox_docker_plugin/models/image.py
 netbox_docker_plugin/models/network.py
 netbox_docker_plugin/models/registry.py
```

### Comparing `netbox_docker_plugin-1.5.2/pyproject.toml` & `netbox_docker_plugin-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-docker-plugin"
-version = "1.5.2"
+version = "1.6.0"
 authors = [
   { name="Vincent Simonin", email="vincent@saashup.com" },
 ]
 description = "Manage Docker with Netbox & style."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

