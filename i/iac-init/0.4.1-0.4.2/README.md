# Comparing `tmp/iac_init-0.4.1.tar.gz` & `tmp/iac_init-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.4.1.tar", max compression
+gzip compressed data, was "iac_init-0.4.2.tar", max compression
```

## Comparing `iac_init-0.4.1.tar` & `iac_init-0.4.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0    16295 2024-04-17 09:23:31.013977 iac_init-0.4.1/LICENSE
--rw-r--r--   0        0        0        0 2024-04-17 09:23:31.013977 iac_init-0.4.1/README.md
--rw-r--r--   0        0        0      389 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/__main__.py
--rw-r--r--   0        0        0     5880 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/cli/main.py
--rw-r--r--   0        0        0      206 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/cli/options.py
--rw-r--r--   0        0        0     2064 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     2057 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0      747 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2595 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     6788 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      453 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0      263 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0      388 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 09:23:31.013977 iac_init-0.4.1/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 09:23:31.017977 iac_init-0.4.1/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/templates/12-config_backup/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4910 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/utils/functional.py
--rw-r--r--   0        0        0    10270 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/validator.py
--rw-r--r--   0        0        0     5093 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5222 2024-04-17 09:23:31.021977 iac_init-0.4.1/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1601 2024-04-17 09:23:31.021977 iac_init-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 iac_init-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-04-17 10:12:01.659483 iac_init-0.4.2/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-17 10:12:01.659483 iac_init-0.4.2/README.md
+-rw-r--r--   0        0        0      389 2024-04-17 10:12:01.659483 iac_init-0.4.2/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-04-17 10:12:01.659483 iac_init-0.4.2/iac_init/__main__.py
+-rw-r--r--   0        0        0     5880 2024-04-17 10:12:01.659483 iac_init-0.4.2/iac_init/cli/main.py
+-rw-r--r--   0        0        0      206 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/cli/options.py
+-rw-r--r--   0        0        0     2064 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     2057 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0      747 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2595 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     6788 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      453 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0      263 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      388 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4910 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    11200 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/validator.py
+-rw-r--r--   0        0        0     5093 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5222 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1601 2024-04-17 10:12:01.667483 iac_init-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 iac_init-0.4.2/PKG-INFO
```

### Comparing `iac_init-0.4.1/LICENSE` & `iac_init-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.1/iac_init/cli/main.py` & `iac_init-0.4.2/iac_init/cli/main.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.1/iac_init/conf/__init__.py` & `iac_init-0.4.2/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.1/iac_init/conf/global_settings.py` & `iac_init-0.4.2/iac_init/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.1/iac_init/scripts/ansible_tool.py` & `iac_init-0.4.2/iac_init/scripts/ansible_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.1/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.4.2/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.1/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.4.2/iac_init/scripts/cimc_precheck_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.1/iac_init/utils/functional.py` & `iac_init-0.4.2/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.1/iac_init/validator.py` & `iac_init-0.4.2/iac_init/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,20 +138,43 @@
                 if not p.match(ip):
                     msg = msg + "{}".format(ip)
 
             if msg != "Validate error :Below IP can not meet IP Address Format.\n":
                 logger.error(msg)
                 self.errors.append(msg)
                 return True
+            else:
+                return self._validate_image_version()
         else:
             msg = "Validate error: Pls provide APIC/Switch IP configuration"
             logger.error(msg)
             self.errors.append(msg)
             return True
 
+    def _validate_image_version(self):
+        try:
+            image32 = settings.global_policy['fabric']['global_policies']['switch_image32']
+            image64 = settings.global_policy['fabric']['global_policies']['switch_image64']
+
+            pattern_32 = r"^(.+)\.bin"
+            pattern_64 = r'(.+)-cs_64.bin'
+
+            if not re.match(pattern_32, image32).group(1) == re.match(pattern_64, image64).group(1):
+                msg = "Validate error: switch_image32 and switch_image64 checking failed."
+                logger.error(msg)
+                return True
+
+        except Exception as e:
+            msg = "Validate error: Yaml configuration switch_image32 and switch_image64 checking failed."
+            logger.error(msg)
+            msg = e
+            logger.error(msg)
+            self.errors.append(str(msg))
+            return True
+
     def validate_ssh_telnet_connection(self):
         apic_error_msg = "Validate error: APIC CIMC SSH Fail.\n"
         apic_fail_list = []
 
         for ip in self.cimc_address:
             logger.info("Start SSH Connection Validate for {}, timeout 5 minustes".format(ip))
             connection_state = check_ssh_connection(ip, self.apic_cimc_credential[0], self.apic_cimc_credential[1])
```

### Comparing `iac_init-0.4.1/iac_init/yaml_conf/yaml.py` & `iac_init-0.4.2/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.1/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.4.2/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.1/pyproject.toml` & `iac_init-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.4.1/PKG-INFO` & `iac_init-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

