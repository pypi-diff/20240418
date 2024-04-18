# Comparing `tmp/iac_init-0.4.2.tar.gz` & `tmp/iac_init-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.4.2.tar", max compression
+gzip compressed data, was "iac_init-0.4.3.tar", max compression
```

## Comparing `iac_init-0.4.2.tar` & `iac_init-0.4.3.tar`

### file list

```diff
@@ -1,80 +1,104 @@
--rw-r--r--   0        0        0    16295 2024-04-17 10:12:01.659483 iac_init-0.4.2/LICENSE
--rw-r--r--   0        0        0        0 2024-04-17 10:12:01.659483 iac_init-0.4.2/README.md
--rw-r--r--   0        0        0      389 2024-04-17 10:12:01.659483 iac_init-0.4.2/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-04-17 10:12:01.659483 iac_init-0.4.2/iac_init/__main__.py
--rw-r--r--   0        0        0     5880 2024-04-17 10:12:01.659483 iac_init-0.4.2/iac_init/cli/main.py
--rw-r--r--   0        0        0      206 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/cli/options.py
--rw-r--r--   0        0        0     2064 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     2057 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0      747 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2595 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     6788 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      453 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0      263 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0      388 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 10:12:01.663483 iac_init-0.4.2/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/templates/12-config_backup/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4910 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/utils/functional.py
--rw-r--r--   0        0        0    11200 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/validator.py
--rw-r--r--   0        0        0     5093 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5222 2024-04-17 10:12:01.667483 iac_init-0.4.2/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1601 2024-04-17 10:12:01.667483 iac_init-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 iac_init-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-04-18 06:52:34.671088 iac_init-0.4.3/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-18 06:52:34.671088 iac_init-0.4.3/README.md
+-rw-r--r--   0        0        0      389 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/__main__.py
+-rw-r--r--   0        0        0     7671 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/cli/main.py
+-rw-r--r--   0        0        0      206 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/cli/options.py
+-rw-r--r--   0        0        0     2064 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     2832 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0      747 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2595 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     6788 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      453 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0      263 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0     3778 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6823 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1464 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0     1950 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/main.yml
+-rw-r--r--   0        0        0       22 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/exp_files
+-rw-r--r--   0        0        0     5432 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0     1944 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/main.yml
+-rw-r--r--   0        0        0     6876 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      197 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-04-18 06:52:34.671088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0      206 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/01-wipe_aci_fabric/testenv.yml
+-rw-r--r--   0        0        0       22 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/files/exp_files
+-rw-r--r--   0        0        0     1016 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.j2
+-rw-r--r--   0        0        0     3585 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.j2
+-rw-r--r--   0        0        0     1656 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.j2
+-rw-r--r--   0        0        0     1994 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/apic_discovery/vars/main.yml
+-rw-r--r--   0        0        0      181 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 06:52:34.675088 iac_init-0.4.3/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4910 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    11200 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/validator.py
+-rw-r--r--   0        0        0     5093 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5222 2024-04-18 06:52:34.679088 iac_init-0.4.3/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1601 2024-04-18 06:52:34.679088 iac_init-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 iac_init-0.4.3/PKG-INFO
```

### Comparing `iac_init-0.4.2/LICENSE` & `iac_init-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.2/iac_init/cli/main.py` & `iac_init-0.4.3/iac_init/cli/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -54,15 +54,48 @@
     error = validator._wrapped()
     if error:
         exit()
     logger.info("Initial Validation of Yamls Directory Success!!")
 
     for option in option_choice:
         logger.info("Start proceeding step {}.".format(option))
-        if int(option) in [1, 2]:
+        if int(option) in [1]:
+            error = validator.validate_ssh_telnet_connection()
+            if error:
+                exit()
+            yaml_path = validator.validate_yaml_exist(settings.DEFAULT_DATA_PATH)
+            if not yaml_path:
+                exit()
+            error = validator.validate_cimc_precheck()
+            if error:
+                exit()
+            try:
+                writer = yaml_writer.YamlWriter([yaml_path])
+                writer.write(settings.TEMPLATE_DIR[int(option) - 1], output)
+                logger.info("Generate Step {} working directory forder in {} Success!!".format(option, output))
+
+                dir_path = os.path.join(output, os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
+                                        'aci_switch_reimage', 'vars')
+                if os.path.exists(dir_path) and os.path.isdir(dir_path):
+                    yaml_cp_output_path = os.path.join(dir_path, 'main.yml')
+                    shutil.copy(option_yaml_path, yaml_cp_output_path)
+                    logger.info("Copied Yaml file to {} success.".format(yaml_cp_output_path))
+
+                dir_path = os.path.join(output, os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
+                                        'apic_reimage', 'vars')
+                if os.path.exists(dir_path) and os.path.isdir(dir_path):
+                    yaml_cp_output_path = os.path.join(dir_path, 'main.yml')
+                    shutil.copy(option_yaml_path, yaml_cp_output_path)
+                    logger.info("Copied Yaml file to {} success.".format(yaml_cp_output_path))
+
+            except Exception as e:
+                msg = "Generate working directory fail, detail: {}".format(e)
+                logger.error(msg)
+                exit()
+        elif int(option) in [2]:
             error = validator.validate_ssh_telnet_connection()
             if error:
                 exit()
             yaml_path = validator.validate_yaml_exist(settings.DEFAULT_DATA_PATH)
             if not yaml_path:
                 exit()
             error = validator.validate_cimc_precheck()
```

### Comparing `iac_init-0.4.2/iac_init/conf/__init__.py` & `iac_init-0.4.3/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.2/iac_init/conf/global_settings.py` & `iac_init-0.4.3/iac_init/conf/global_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,12 +52,30 @@
     os.path.join(BASE_DIR, "templates", "08-inb_mgmt"),
     os.path.join(BASE_DIR, "templates", "09-smart_licensing"),
     os.path.join(BASE_DIR, "templates", "10-confg_aaa"),
     os.path.join(BASE_DIR, "templates", "11-config_monitor"),
     os.path.join(BASE_DIR, "templates", "12-config_backup")
 ]
 
+OUTPUT_DIR = [
+    os.path.join(OUTPUT_BASE_DIR, "01-wipe_aci_fabric"),
+    os.path.join(OUTPUT_BASE_DIR, "02-discover_apic"),
+    os.path.join(OUTPUT_BASE_DIR, "03-node_registration"),
+    os.path.join(OUTPUT_BASE_DIR, "04-oob_mgmt"),
+    os.path.join(OUTPUT_BASE_DIR, "05-aci_system_settings"),
+    os.path.join(OUTPUT_BASE_DIR, "06-fabric_policy"),
+    os.path.join(OUTPUT_BASE_DIR, "07-access_policy"),
+    os.path.join(OUTPUT_BASE_DIR, "08-inb_mgmt"),
+    os.path.join(OUTPUT_BASE_DIR, "09-smart_licensing"),
+    os.path.join(OUTPUT_BASE_DIR, "10-confg_aaa"),
+    os.path.join(OUTPUT_BASE_DIR, "11-config_monitor"),
+    os.path.join(OUTPUT_BASE_DIR, "12-config_backup")
+]
+
+os.environ["iac_init_option_1"] = OUTPUT_DIR[0]
+os.environ["iac_init_option_2"] = OUTPUT_DIR[1]
+
 ANSIBLE_STEP = [
     'iac-validate',
     'deploy',
     'iac-test'
 ]
```

### Comparing `iac_init-0.4.2/iac_init/scripts/ansible_tool.py` & `iac_init-0.4.3/iac_init/scripts/ansible_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.2/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.4.3/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.2/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.4.3/iac_init/scripts/cimc_precheck_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.2/iac_init/utils/functional.py` & `iac_init-0.4.3/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.2/iac_init/validator.py` & `iac_init-0.4.3/iac_init/validator.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.2/iac_init/yaml_conf/yaml.py` & `iac_init-0.4.3/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.2/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.4.3/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.2/pyproject.toml` & `iac_init-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.4.2"
+version = "0.4.3"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.4.2/PKG-INFO` & `iac_init-0.4.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.4.2
+Version: 0.4.3
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

