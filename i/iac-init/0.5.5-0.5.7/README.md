# Comparing `tmp/iac_init-0.5.5.tar.gz` & `tmp/iac_init-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.5.5.tar", max compression
+gzip compressed data, was "iac_init-0.5.7.tar", max compression
```

## Comparing `iac_init-0.5.5.tar` & `iac_init-0.5.7.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0    16295 2024-05-06 11:15:05.051650 iac_init-0.5.5/LICENSE
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.051650 iac_init-0.5.5/README.md
--rw-r--r--   0        0        0      389 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/__main__.py
--rw-r--r--   0        0        0    13247 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/cli/main.py
--rw-r--r--   0        0        0      206 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/cli/options.py
--rw-r--r--   0        0        0     2064 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     2886 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0     1041 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2595 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     7490 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      453 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0      263 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0     3778 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6823 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1464 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.051650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1494 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 11:15:05.055650 iac_init-0.5.5/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/templates/12-config_backup/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4910 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/utils/functional.py
--rw-r--r--   0        0        0    11463 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/validator.py
--rw-r--r--   0        0        0     5093 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5222 2024-05-06 11:15:05.059650 iac_init-0.5.5/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1636 2024-05-06 11:15:05.059650 iac_init-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-07 04:32:27.682029 iac_init-0.5.7/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.682029 iac_init-0.5.7/README.md
+-rw-r--r--   0        0        0      389 2024-05-07 04:32:27.682029 iac_init-0.5.7/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-07 04:32:27.682029 iac_init-0.5.7/iac_init/__main__.py
+-rw-r--r--   0        0        0    13247 2024-05-07 04:32:27.682029 iac_init-0.5.7/iac_init/cli/main.py
+-rw-r--r--   0        0        0      206 2024-05-07 04:32:27.682029 iac_init-0.5.7/iac_init/cli/options.py
+-rw-r--r--   0        0        0     2064 2024-05-07 04:32:27.682029 iac_init-0.5.7/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     2886 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     1041 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2595 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7490 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      453 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0      263 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0     3778 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1573 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-07 04:32:27.686029 iac_init-0.5.7/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-07 04:32:27.690029 iac_init-0.5.7/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-07 04:32:27.694028 iac_init-0.5.7/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-05-07 04:32:27.694028 iac_init-0.5.7/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4910 2024-05-07 04:32:27.694028 iac_init-0.5.7/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    11463 2024-05-07 04:32:27.694028 iac_init-0.5.7/iac_init/validator.py
+-rw-r--r--   0        0        0     5093 2024-05-07 04:32:27.694028 iac_init-0.5.7/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5222 2024-05-07 04:32:27.694028 iac_init-0.5.7/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1636 2024-05-07 04:32:27.694028 iac_init-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.5.7/PKG-INFO
```

### Comparing `iac_init-0.5.5/LICENSE` & `iac_init-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/cli/main.py` & `iac_init-0.5.7/iac_init/cli/main.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/conf/__init__.py` & `iac_init-0.5.7/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/conf/global_settings.py` & `iac_init-0.5.7/iac_init/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/scripts/ansible_tool.py` & `iac_init-0.5.7/iac_init/scripts/ansible_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.5.7/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.5.7/iac_init/scripts/cimc_precheck_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -16,72 +16,80 @@
 # 64-bit switch models
 set aci_switch_pid_64_bit {
 {% for item in fabric.global_policies.aci_switch_pid_64_bit %}
     "{{ item }}"
 {% endfor %}
 }
 
+# Human-like send procedure
+proc send_human {cmd} {
+    global send_human
+    send -- $cmd
+    sleep 1
+}
+
 # Default is 32-bit image
 set filename $switch_image32
 
 set b64script "IyEvYmluL2Jhc2gKCiMgU2NyaXB0IGRlc2NyaXB0aW9uIGFuZCB1c2FnZQojIFVzYWdlOiAuL2NoYW5nZWltYWdlLnNoCiMgRGVzY3JpcHRpb246CiMgYmFzZTY0IGVuY29kZSB0aGlzIHNjcmlwdCBmb3IgY29kZSB0cmFuc2ZlciAiIGJhc2U2NCBjaGFuZ2VpbWFnZS5zaCAtdyAwICIKIyBvbmUtbGluZXIgYmFja2dyb3VuZCBleGVjdXRpb246IFNDUklQVD0nTDNOamNtbHdkLi4uJyAmJiBub2h1cCBiYXNoIC1jICJlY2hvICRTQ1JJUFQgfCBiYXNlNjQgLWQgfCBiYXNoIgoKIyBDb3B5cmlnaHQ6IChjKSAyMDIyLCBMaW51cyBYdSA8bGlueHUzQGNpc2NvLmNvbT4KCiMgR2xvYmFsIHZhcmlhYmxlIGZvciB0aGUgZmlsZW5hbWUKIyBGSUxFU0VSVkVSPSJodHRwOi8vZmlsZXNlcnZlci9JbWFnZXMvQUNJLzUvNS4wIiAgPDwgYSBmaWxlIHNlcnZlciBwYXRoCiMgRklMRU5BTUU9ImFjaS1uOTAwMC1kazkuMTUuMC4yaC5iaW4iICAgPDw8IGdldCBmcm9tIGdsb2JhbCBlbnZpcm9uZW1udCB2YXJzCgojIExvZyBmaWxlIHNldHVwClRJTUVTVEFNUD0kKGRhdGUgJyslWS0lbS0lZF8lSC0lTS0lUycpCkxPR0ZJTEU9Ii90bXAvc2NyaXB0XyR7VElNRVNUQU1QfS5sb2ciCmV4ZWMgPiA+KHRlZSAiJExPR0ZJTEUiKSAyPiYxCmVjaG8gIlNjcmlwdCBleGVjdXRpb24gc3RhcnRlZDogJChkYXRlKSIKCgojIEZ1bmN0aW9uIHRvIGV4ZWN1dGUgYSBzY3JpcHQgYW5kIGNoZWNrIGZvciAiRG9uZSIgaW4gdGhlIG91dHB1dApleGVjdXRlX2FuZF9jaGVjaygpIHsKICAgICMgRXhlY3V0ZSBzY3JpcHQgcGFzc2VkIGFzIHBhcmFtZXRlciBhbmQgY2FwdHVyZSB0aGUgb3V0cHV0CiAgICBvdXRwdXQ9JCgiJEAiKSAjIFVzaW5nICIkQCIgdG8gYWxsb3cgcGFzc2luZyB3aG9sZSBjb21tYW5kIHdpdGggcGFyYW1ldGVycwoKICAgIGVjaG8gJG91dHB1dAogICAgIyBDaGVjayBpZiBvdXRwdXQgY29udGFpbnMgIkRvbmUiCiAgICBpZiBbWyAkb3V0cHV0ID09ICoiRG9uZSIqIF1dOyB0aGVuCiAgICAgICAgZWNobyAiJDEgZXhlY3V0ZWQgc3VjY2Vzc2Z1bGx5LiIKICAgIGVsc2UKICAgICAgICBlY2hvICJbIV0gRXJyb3I6ICQxIGRpZCBub3QgY29tcGxldGUgc3VjY2Vzc2Z1bGx5LiIKICAgICAgICBleGl0IDEKICAgIGZpCn0KCgojIEZ1bmN0aW9uIHRvIGNoZWNrIGlmIGEgZGlyZWN0b3J5IGlzIGVtcHR5CmNoZWNrX2RpcmVjdG9yeV9lbXB0eSgpIHsKICAgIGRpcj0kMQogICAgaWYgWyAiJChmaW5kICIkZGlyIiAtbWluZGVwdGggMSAtcHJpbnQgLXF1aXQgMj4vZGV2L251bGwpIiBdOyB0aGVuCiAgICAgICAgZWNobyAiWyFdIEVycm9yOiBEaXJlY3RvcnkgJGRpciBpcyBub3QgZW1wdHkuIgogICAgICAgIGV4aXQgMQogICAgZWxzZQogICAgICAgIGVjaG8gIkRpcmVjdG9yeSAkZGlyIGlzIGVtcHR5LiBDb250aW51aW5nLi4uIgogICAgZmkKfQoKIyBGdW5jdGlvbiB0byBmaW5kIGFuZCBkZWxldGUgZmlsZXMgc3RhcnRpbmcgd2l0aCBhIHNwZWNpZmljIHByZWZpeApkZWxldGVfZmlsZXNfd2l0aF9wcmVmaXgoKSB7CiAgICBwcmVmaXg9JDEKICAgIGVjaG8gImRlbGV0ZWluZyBhbGwgaW1hZ2VzIgogICAgcm0gLWYgJHByZWZpeAp9CgojIEZ1bmN0aW9uIHRvIGRvd25sb2FkIGEgZmlsZSBhbmQgY2hlY2sgaWYgaXQgd2FzIHNhdmVkIHN1Y2Nlc3NmdWxseQpkb3dubG9hZF9hbmRfY2hlY2soKSB7CiAgICB1cmw9JDEKICAgIGRlc3RpbmF0aW9uPSIvYm9vdGZsYXNoLyRGSUxFTkFNRSIKICAgIHdnZXQgIiR1cmwiIC1PICIkZGVzdGluYXRpb24iIDI+L2Rldi9udWxsCiAgICBpZiBbIC1mICIkZGVzdGluYXRpb24iIF07IHRoZW4KICAgICAgICBlY2hvICJGaWxlICckZGVzdGluYXRpb24nIGRvd25sb2FkZWQgYW5kIHNhdmVkIHN1Y2Nlc3NmdWxseS4iCiAgICBlbHNlCiAgICAgICAgZWNobyAiWyFdIEVycm9yOiBGaWxlICckZGVzdGluYXRpb24nIGNvdWxkIG5vdCBiZSBkb3dubG9hZGVkLiIKICAgICAgICBleGl0IDEKICAgIGZpCn0KCiMgRnVuY3Rpb24gdG8gY2hlY2sgZm9yIHRoZSBleGlzdGVuY2Ugb2YgYSBmaWxlIGFuZCBzcGVjaWZpYyBjb250ZW50IHdpdGhpbgpjaGVja19maWxlX2FuZF9jb250ZW50KCkgewogICAgZmlsZV9wYXRoPSQxCiAgICBzZWFyY2hfY29udGVudD0iYm9vdCAkRklMRU5BTUUiCiAgICBpZiBbICEgLWYgIiRmaWxlX3BhdGgiIF07IHRoZW4KICAgICAgICBlY2hvICJbIV0gRXJyb3I6IEZpbGUgJGZpbGVfcGF0aCBkb2VzIG5vdCBleGlzdC4iCiAgICAgICAgZXhpdCAxCiAgICBlbGlmICEgZ3JlcCAtcSAiJHNlYXJjaF9jb250ZW50IiAiJGZpbGVfcGF0aCI7IHRoZW4KICAgICAgICBlY2hvICJbIV0gRXJyb3I6IFRoZSByZXF1aXJlZCBjb250ZW50ICckc2VhcmNoX2NvbnRlbnQnIGlzIG5vdCBpbiAkZmlsZV9wYXRoLiIKICAgICAgICBleGl0IDEKICAgIGVsc2UKICAgICAgICBlY2hvICJGaWxlICRmaWxlX3BhdGggY29udGFpbnMgdGhlIHJlcXVpcmVkIGNvbnRlbnQuIgogICAgZmkKfQoKIyBNYWluIGxvZ2ljIG9mIHRoZSBzY3JpcHQKbWFpbigpIHsKICAgIGVjaG8gIlsrXSBDSEVDS0lORyB0YXJnZXQgaW1hZ2UgaW5mb3JtYXRpb24iCiAgICBlY2hvICJUYXJnZXRJbWFnZTogJEZJTEVOQU1FIgogICAgZWNobyAiRmlsZVNlcnZlcjogJEZJTEVTRVJWRVIiCgogICAgZWNobyAiWytdIENMRUFOSU5HIGNvbmZpZ3MgJiBib290dmFycyIKICAgIGV4ZWN1dGVfYW5kX2NoZWNrICJzZXR1cC1jbGVhbi1jb25maWcuc2giCiAgICBleGVjdXRlX2FuZF9jaGVjayAiY2xlYXItYm9vdHZhcnMuc2giCgogICAgZWNobyAiWytdIENIRUNLSU5HIGdydWIgZGlyZWN0b3J5IGluZm9ybWF0aW9uIgogICAgY2hlY2tfZGlyZWN0b3J5X2VtcHR5ICIvbW50L2NmZy8wL2Jvb3QvZ3J1Yi8iCiAgICBjaGVja19kaXJlY3RvcnlfZW1wdHkgIi9tbnQvY2ZnLzEvYm9vdC9ncnViLyIKCiAgICBlY2hvICJbK10gREVMRVRJTkcgJiBET1dOTE9BRCBpbWFnZSIKICAgIGRlbGV0ZV9maWxlc193aXRoX3ByZWZpeCAiL2Jvb3RmbGFzaC9hY2ktbjkwMDAqIgogICAgZG93bmxvYWRfYW5kX2NoZWNrICIkRklMRVNFUlZFUi8kRklMRU5BTUUiCgogICAgZWNobyAiWytdIFNFVElOR1VQIGJvb3R2YXJzIgogICAgb3V0cHV0PSQoYmFzaCAtYyAic2V0dXAtYm9vdHZhcnMuc2ggJEZJTEVOQU1FIikgICAjICAiJEAiICBpbiBub3Qgd29yawogICAgZWNobyAkb3V0cHV0CiAgICBpZiBbWyAkb3V0cHV0ID09ICoiRG9uZSIqIF1dOyB0aGVuCiAgICAgICAgZWNobyAic2V0dXAtYm9vdHZhcnMuc2ggZXhlY3V0ZWQgc3VjY2Vzc2Z1bGx5LiIKICAgIGVsc2UKICAgICAgICBlY2hvICJbIV0gRXJyb3I6IHNldHVwLWJvb3R2YXJzLnNoIGRpZCBub3QgY29tcGxldGUgc3VjY2Vzc2Z1bGx5LiIKICAgICAgICBleGl0IDEKICAgIGZpCgogICAgZWNobyAiWytdIENIRUNLSU5HIGlmIG1lbnUubHN0LmxvY2FsIGZpbGVzIGV4aXN0IGFuZCBjb250YWluIHRoZSByZXF1aXJlZCBib290IGVudHJ5IgogICAgY2hlY2tfZmlsZV9hbmRfY29udGVudCAiL21udC9jZmcvMC9ib290L2dydWIvbWVudS5sc3QubG9jYWwiCiAgICBjaGVja19maWxlX2FuZF9jb250ZW50ICIvbW50L2NmZy8xL2Jvb3QvZ3J1Yi9tZW51LmxzdC5sb2NhbCIKCiAgICBlY2hvICJbK11BbGwgY2hlY2tzIHBhc3NlZC4gQ29udGludWUgdG8gcmVib290Li4uIgogICAgdnNoIC1jICJyZWxvYWQiCn0KCiMgU2NyaXB0IGVudHJ5IHBvaW50Cm1haW4gIiRAIgplY2hvICJTY3JpcHQgZXhlY3V0aW9uIGZpbmlzaGVkOiAkKGRhdGUpIg=="
 
 set ip {{ item.console_address }}
 set port {{ item.console_port }}
 puts "============================================================"
 puts "connecting to $ip:$port ..."
 
+# Start Telnet session
 spawn telnet $ip $port
 
 sleep 2
-send -h -- "\n"
+send_human "\n"
 
+# Interaction sequence
 expect {
     "# " {
     }
     -re "--More--" {
-        send -h -- "q\r"
+        send_human "q\r"
         exp_continue
     }
     "login: " {
-        send -h -- "$username\n"
-        sleep 1
+        send_human "$username\n"
         exp_continue
     }
     "Password:" {
-        send -h -- "$password\n"
+        send_human "$password\n"
         exp_continue
     }
     "password:" {
-        send -h -- "$password\n"
+        send_human "$password\n"
         exp_continue
     }
 }
 
 # Retrieve switch platform
-send "show inventory\n"
+send_human "show inventory\n"
 expect "# "
 set output $expect_out(buffer)
 
 foreach pid $aci_switch_pid_64_bit {
     if {[string match "*$pid*" $output]} {
         set filename $switch_image64
     }
 }
 
-send "bash\n"
+send_human "bash\n"
 expect "#"
 
 set payload "bash -c 'export FILESERVER=$fileserver && export FILENAME=$filename && echo $b64script | base64 -d | bash' \r"
 
-send $payload
+send_human $payload
 expect "Script execution started"
 
 puts $filename
 
-send "\035"
+send_human "\035"
 expect "telnet>"
 
-send "quit\r"
+send_human "quit\r"
 expect eof
 
 puts "Telnet session complete!"
```

### Comparing `iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 #!/usr/bin/expect -f
 
 # Copyright: (c) 2022, Rudy Lei <shlei@cisco.com>
 
 # Common Setup
 set send_human {.1 .3 1 .05 2}
-set timeout 600
+set timeout 900
+set RETRY 600
 set username {{ fabric.global_policies.aci_local_username }}
-set password {{ fabric.global_policies.aci_local_password }}
 
 set switch_image {
     {{ fabric.global_policies.switch_image32 }}
     {{ fabric.global_policies.switch_image64 }}
 }
 
+# Human-like send procedure
+proc send_human {cmd} {
+    global send_human
+    send -- $cmd
+    sleep 1
+}
+
 set validator false
 
 set ip {{ item.console_address }}
 set port {{ item.console_port }}
 puts "============================================================"
 puts "connecting to $ip:$port ..."
 
+# Start Telnet session
 spawn telnet $ip $port
 
 sleep 2
-send -h -- "\n"
+send_human "\n"
 
+# Interaction sequence
 expect {
-    "# " {
-    }
-    -re "--More--" {
-        send -h -- "q\r"
-        exp_continue
+    "(none)# " {
     }
     "login: " {
+        sleep 60
         send -h -- "$username\n"
-        sleep 1
-        exp_continue
-    }
-    "Password:" {
-        send -h -- "$password\n"
-        exp_continue
-    }
-    "password:" {
-        send -h -- "$password\n"
         exp_continue
     }
 }
 
 # Retrieve current switch version
 send "show version | grep 'kickstart'\n"
 expect "# "
@@ -55,21 +52,21 @@
 foreach image $switch_image {
     if {[string match "*$image*" $output]} {
         puts "ACI switch installation complete!"
         set validator true
     }
 }
 
-send "bash\n"
-expect "#"
+send_human "exit\n"
+expect "logout"
 
-send "\035"
+send_human "\035"
 expect "telnet>"
 
-send "quit\r"
+send_human "quit\r"
 expect eof
 
 puts "Telnet session complete!"
 
 if {[string match "false" $validator]} {
     puts "ACI switch is not in target version!!"
     exit 1
```

### Comparing `iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.5.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.5.7/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,17 @@
         timeout: 500
         content: |
           <!-- CIMC hard reset -->
           <configConfMo><inConfig>
             <computeRackUnit dn="sys/rack-unit-1" adminPower="hard-reset-immediate" />
           </inConfig></configConfMo>
 
+      delegate_to: localhost
+      loop: "{{ fabric.apic_nodes_connection }}"
+
     - name: Render APIC discovery script
       template:
         src: apic_discovery{{ apic_version.stdout }}.exp.jinja2
         dest: apic_discovery/files/apic_discovery_{{ item.hostname }}.exp
       delegate_to: localhost
       loop: "{{ fabric.apic_nodes_connection }}"
```

### Comparing `iac_init-0.5.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.5.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.5.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.5.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/utils/functional.py` & `iac_init-0.5.7/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/validator.py` & `iac_init-0.5.7/iac_init/validator.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/yaml_conf/yaml.py` & `iac_init-0.5.7/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.5.7/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.5/pyproject.toml` & `iac_init-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.5.5"
+version = "0.5.7"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.5.5/PKG-INFO` & `iac_init-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.5.5
+Version: 0.5.7
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

