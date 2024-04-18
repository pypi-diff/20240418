# Comparing `tmp/iac_init-0.4.4.tar.gz` & `tmp/iac_init-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.4.4.tar", max compression
+gzip compressed data, was "iac_init-0.4.5.tar", max compression
```

## Comparing `iac_init-0.4.4.tar` & `iac_init-0.4.5.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0    16295 2024-04-18 07:16:46.040060 iac_init-0.4.4/LICENSE
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.040060 iac_init-0.4.4/README.md
--rw-r--r--   0        0        0      389 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/__main__.py
--rw-r--r--   0        0        0     7671 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/cli/main.py
--rw-r--r--   0        0        0      206 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/cli/options.py
--rw-r--r--   0        0        0     2064 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     2832 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0      747 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2595 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     6788 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      453 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0      263 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0     3778 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6823 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1464 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5432 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0       22 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/files/exp_files
--rw-r--r--   0        0        0     1016 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.j2
--rw-r--r--   0        0        0     3585 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.j2
--rw-r--r--   0        0        0     1656 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.j2
--rw-r--r--   0        0        0     1994 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/vars/main.yml
--rw-r--r--   0        0        0      181 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 07:16:46.040060 iac_init-0.4.4/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.044060 iac_init-0.4.4/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/templates/12-config_backup/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4910 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/utils/functional.py
--rw-r--r--   0        0        0    11462 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/validator.py
--rw-r--r--   0        0        0     5093 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5222 2024-04-18 07:16:46.048060 iac_init-0.4.4/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1601 2024-04-18 07:16:46.048060 iac_init-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 iac_init-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-04-18 07:52:22.792345 iac_init-0.4.5/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.792345 iac_init-0.4.5/README.md
+-rw-r--r--   0        0        0      389 2024-04-18 07:52:22.792345 iac_init-0.4.5/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-04-18 07:52:22.792345 iac_init-0.4.5/iac_init/__main__.py
+-rw-r--r--   0        0        0     8661 2024-04-18 07:52:22.792345 iac_init-0.4.5/iac_init/cli/main.py
+-rw-r--r--   0        0        0      206 2024-04-18 07:52:22.792345 iac_init-0.4.5/iac_init/cli/options.py
+-rw-r--r--   0        0        0     2064 2024-04-18 07:52:22.792345 iac_init-0.4.5/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     2873 2024-04-18 07:52:22.792345 iac_init-0.4.5/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0      747 2024-04-18 07:52:22.792345 iac_init-0.4.5/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2595 2024-04-18 07:52:22.792345 iac_init-0.4.5/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     6788 2024-04-18 07:52:22.792345 iac_init-0.4.5/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      453 2024-04-18 07:52:22.792345 iac_init-0.4.5/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0      263 2024-04-18 07:52:22.792345 iac_init-0.4.5/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0     3778 2024-04-18 07:52:22.792345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-04-18 07:52:22.792345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6823 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1464 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5432 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0       22 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/02-discover_apic/apic_discovery/files/exp_files
+-rw-r--r--   0        0        0     1016 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.j2
+-rw-r--r--   0        0        0     3585 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.j2
+-rw-r--r--   0        0        0     1656 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.j2
+-rw-r--r--   0        0        0     1994 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/02-discover_apic/apic_discovery/vars/main.yml
+-rw-r--r--   0        0        0      181 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:52:22.796345 iac_init-0.4.5/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4910 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    11462 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/validator.py
+-rw-r--r--   0        0        0     5093 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5222 2024-04-18 07:52:22.800345 iac_init-0.4.5/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1636 2024-04-18 07:52:22.804345 iac_init-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.4.5/PKG-INFO
```

### Comparing `iac_init-0.4.4/LICENSE` & `iac_init-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/cli/main.py` & `iac_init-0.4.5/iac_init/cli/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,14 +64,17 @@
                 exit()
             yaml_path = validator.validate_yaml_exist(settings.DEFAULT_DATA_PATH)
             if not yaml_path:
                 exit()
             error = validator.validate_cimc_precheck()
             if error:
                 exit()
+            option_yaml_path = validator.validate_yaml_exist(settings.DATA_PATH[int(option) - 1])
+            if not option_yaml_path:
+                exit()
             try:
                 writer = yaml_writer.YamlWriter([yaml_path])
                 writer.write(settings.TEMPLATE_DIR[int(option) - 1], output)
                 logger.info("Generate Step {} working directory forder in {} Success!!".format(option, output))
 
                 dir_path = os.path.join(output, os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
                                         'aci_switch_reimage', 'vars')
@@ -87,24 +90,43 @@
                     shutil.copy(option_yaml_path, yaml_cp_output_path)
                     logger.info("Copied Yaml file to {} success.".format(yaml_cp_output_path))
 
             except Exception as e:
                 msg = "Generate working directory fail, detail: {}".format(e)
                 logger.error(msg)
                 exit()
+
+            try:
+                playbook_dir = os.path.join(os.getcwd(), output,
+                                                    os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
+                                                    'playbook_apic_init.yaml')
+
+                deploy_result = run_ansible_playbook(settings.ANSIBLE_STEP[3], option, None,
+                                                    playbook_dir)
+                if not deploy_result:
+                    exit()
+
+
+            except Exception as e:
+                msg = "Run NAC ansible-playbook fail detail:\nError: {}".format(e)
+                logger.error(msg)
+                exit()
         elif int(option) in [2]:
             error = validator.validate_ssh_telnet_connection()
             if error:
                 exit()
             yaml_path = validator.validate_yaml_exist(settings.DEFAULT_DATA_PATH)
             if not yaml_path:
                 exit()
             error = validator.validate_cimc_precheck()
             if error:
                 exit()
+            option_yaml_path = validator.validate_yaml_exist(settings.DATA_PATH[int(option) - 1])
+            if not option_yaml_path:
+                exit()
             try:
                 writer = yaml_writer.YamlWriter([yaml_path])
                 writer.write(settings.TEMPLATE_DIR[int(option) - 1], output)
                 logger.info("Generate Step {} working directory forder in {} Success!!".format(option, output))
             except Exception as e:
                 msg = "Generate working directory fail, detail: {}".format(e)
                 logger.error(msg)
```

### Comparing `iac_init-0.4.4/iac_init/conf/__init__.py` & `iac_init-0.4.5/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/conf/global_settings.py` & `iac_init-0.4.5/iac_init/conf/global_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,9 +73,11 @@
 
 os.environ["iac_init_option_1"] = OUTPUT_DIR[0]
 os.environ["iac_init_option_2"] = OUTPUT_DIR[1]
 
 ANSIBLE_STEP = [
     'iac-validate',
     'deploy',
-    'iac-test'
+    'iac-test',
+    'wipe_aci_fabric',
+    'apic_setup'
 ]
```

### Comparing `iac_init-0.4.4/iac_init/scripts/ansible_tool.py` & `iac_init-0.4.5/iac_init/scripts/ansible_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.4.5/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.4.5/iac_init/scripts/cimc_precheck_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.4.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.4.5/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.j2` & `iac_init-0.4.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.j2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.j2` & `iac_init-0.4.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.j2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.j2` & `iac_init-0.4.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.j2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/templates/02-discover_apic/apic_discovery/vars/main.yml` & `iac_init-0.4.5/iac_init/templates/02-discover_apic/apic_discovery/vars/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/utils/functional.py` & `iac_init-0.4.5/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/validator.py` & `iac_init-0.4.5/iac_init/validator.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/yaml_conf/yaml.py` & `iac_init-0.4.5/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.4.5/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.4/pyproject.toml` & `iac_init-0.4.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.4.4"
+version = "0.4.5"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
 
@@ -16,14 +16,16 @@
 ruamel-yaml = ">0.16.10"
 yamale = "^4.0.3"
 paramiko = "^3.4.0"
 requests = "^2.31.0"
 loguru = "^0.7.2"
 jmespath = "^1.0.1"
 ansible-runner = "^2.3.5"
+lxml = "^5.2.1"
+xmljson = "^0.2.1"
 
 [tool.poetry.group.dev.dependencies]
 ansible-core = "^2.13.2"
 black = "^22.10.0"
 flake8 = "^5.0.4"
 isort = "^5.10.1"
 mypy = "^0.990"
```

### Comparing `iac_init-0.4.4/PKG-INFO` & `iac_init-0.4.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.4.4
+Version: 0.4.5
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ansible-runner (>=2.3.5,<3.0.0)
 Requires-Dist: click (>=8.0.4,<9.0.0)
 Requires-Dist: errorhandler (>=2.0.1,<3.0.0)
 Requires-Dist: importlib-metadata (>=2.0.0,<3.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: paramiko (>=3.4.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ruamel-yaml (>0.16.10)
+Requires-Dist: xmljson (>=0.2.1,<0.3.0)
 Requires-Dist: yamale (>=4.0.3,<5.0.0)
 Description-Content-Type: text/markdown
```

