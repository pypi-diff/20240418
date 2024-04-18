# Comparing `tmp/iac_init-0.4.3.tar.gz` & `tmp/iac_init-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.4.3.tar", max compression
+gzip compressed data, was "iac_init-0.4.4.tar", max compression
```

## Comparing `iac_init-0.4.3.tar` & `iac_init-0.4.4.tar`

### file list

```diff
@@ -1,104 +1,102 @@
--rw-r--r--   0        0        0    16295 2024-04-18 06:52:34.671088 iac_init-0.4.3/LICENSE
--rw-r--r--   0        0        0        0 2024-04-18 06:52:34.671088 iac_init-0.4.3/README.md
--rw-r--r--   0        0        0      389 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/__main__.py
--rw-r--r--   0        0        0     7671 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/cli/main.py
--rw-r--r--   0        0        0      206 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/cli/options.py
--rw-r--r--   0        0        0     2064 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     2832 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0      747 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2595 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     6788 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      453 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0      263 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0     3778 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6823 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1464 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0     1950 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/main.yml
--rw-r--r--   0        0        0       22 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/exp_files
--rw-r--r--   0        0        0     5432 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0     1944 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/main.yml
--rw-r--r--   0        0        0     6876 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/cimc_precheck_tool.py
--rw-r--r--   0        0        0      197 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0      206 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/testenv.yml
--rw-r--r--   0        0        0       22 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/files/exp_files
--rw-r--r--   0        0        0     1016 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.j2
--rw-r--r--   0        0        0     3585 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.j2
--rw-r--r--   0        0        0     1656 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.j2
--rw-r--r--   0        0        0     1994 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/vars/main.yml
--rw-r--r--   0        0        0      181 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/12-config_backup/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4910 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/utils/functional.py
--rw-r--r--   0        0        0    11200 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/validator.py
--rw-r--r--   0        0        0     5093 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5222 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1601 2024-04-18 06:52:34.679088 iac_init-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 iac_init-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-04-18 07:16:46.040060 iac_init-0.4.4/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.040060 iac_init-0.4.4/README.md
+-rw-r--r--   0        0        0      389 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/__main__.py
+-rw-r--r--   0        0        0     7671 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/cli/main.py
+-rw-r--r--   0        0        0      206 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/cli/options.py
+-rw-r--r--   0        0        0     2064 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     2832 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0      747 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2595 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     6788 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      453 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0      263 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0     3778 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6823 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1464 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5432 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0       22 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/files/exp_files
+-rw-r--r--   0        0        0     1016 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.j2
+-rw-r--r--   0        0        0     3585 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.j2
+-rw-r--r--   0        0        0     1656 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.j2
+-rw-r--r--   0        0        0     1994 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/vars/main.yml
+-rw-r--r--   0        0        0      181 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4910 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    11462 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/validator.py
+-rw-r--r--   0        0        0     5093 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5222 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1601 2024-04-18 07:16:46.048060 iac_init-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 iac_init-0.4.4/PKG-INFO
```

### Comparing `iac_init-0.4.3/LICENSE` & `iac_init-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/cli/main.py` & `iac_init-0.4.4/iac_init/cli/main.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/conf/__init__.py` & `iac_init-0.4.4/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/conf/global_settings.py` & `iac_init-0.4.4/iac_init/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/scripts/ansible_tool.py` & `iac_init-0.4.4/iac_init/scripts/ansible_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.4.4/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.4.4/iac_init/scripts/cimc_precheck_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/main.yml` & `iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/vars/main.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ---
 fabric:
   global_policies:
     aci_local_username: admin
-    aci_local_password: Cisco123
+    aci_local_password: Cisco123  # Must be a very strong password for version 6.x
     apic_cimc_username: admin
     apic_cimc_password: P@ssw0rd
     fabric_name: dlc-aci01
     fabric_id: 1
     fabric_active_controllers: 1
     standby_apic_cluster: no
     tep_pool: 10.0.0.0/16
     infra_vlan: 3967
     gipo: 225.0.0.0/15
     strong_password: N
     aci_version: 5.2(1h)
     aci_image_path: http://10.124.145.88/Images/ACI/4/4.2/
-    apic_image: aci-apic-dk9.6.0.2j.iso
-    switch_image32: aci-n9000-dk9.16.0.3d.bin
-    switch_image64: aci-n9000-dk9.16.0.3d-cs_64.bin
+    apic_image: aci-apic-dk9.4.2.7q.iso
+    switch_image32: aci-n9000-dk9.14.2.7f.bin
+    switch_image64: aci-n9000-dk9.14.2.7r.bin
     dns_server: 64.104.76.247
     ntp_server: ntp.esl.cisco.com
     timezone: Asia/Shanghai
     apic_netmask: 24
     apic_gateway: 10.124.145.1
     aci_switch_pid_64_bit:
       - N9K-C93108TC-FX
```

### Comparing `iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.j2` & `iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.j2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.j2` & `iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.j2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.j2` & `iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.j2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/utils/functional.py` & `iac_init-0.4.4/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/validator.py` & `iac_init-0.4.4/iac_init/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,18 +154,24 @@
         try:
             image32 = settings.global_policy['fabric']['global_policies']['switch_image32']
             image64 = settings.global_policy['fabric']['global_policies']['switch_image64']
 
             pattern_32 = r"^(.+)\.bin"
             pattern_64 = r'(.+)-cs_64.bin'
 
-            if not re.match(pattern_32, image32).group(1) == re.match(pattern_64, image64).group(1):
-                msg = "Validate error: switch_image32 and switch_image64 checking failed."
-                logger.error(msg)
-                return True
+            if image32 == image64:
+                if not image32.endwith(".bin"):
+                    msg = "Validate error: Image name must end with .bin."
+                    logger.error(msg)
+                    return True
+            else:
+                if not re.match(pattern_32, image32).group(1) == re.match(pattern_64, image64).group(1):
+                    msg = "Validate error: switch_image32 and switch_image64 checking failed."
+                    logger.error(msg)
+                    return True
 
         except Exception as e:
             msg = "Validate error: Yaml configuration switch_image32 and switch_image64 checking failed."
             logger.error(msg)
             msg = e
             logger.error(msg)
             self.errors.append(str(msg))
```

### Comparing `iac_init-0.4.3/iac_init/yaml_conf/yaml.py` & `iac_init-0.4.4/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.4.4/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.3/pyproject.toml` & `iac_init-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.4.3"
+version = "0.4.4"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.4.3/PKG-INFO` & `iac_init-0.4.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

