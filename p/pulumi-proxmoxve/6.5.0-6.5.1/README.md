# Comparing `tmp/pulumi_proxmoxve-6.5.0.tar.gz` & `tmp/pulumi_proxmoxve-6.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-6.5.0.tar", last modified: Tue Apr 30 06:23:57 2024, max compression
+gzip compressed data, was "pulumi_proxmoxve-6.5.1.tar", last modified: Tue May  7 07:11:04 2024, max compression
```

## Comparing `pulumi_proxmoxve-6.5.0.tar` & `pulumi_proxmoxve-6.5.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.841352 pulumi_proxmoxve-6.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-30 06:23:57.841352 pulumi_proxmoxve-6.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.829352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.829352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    53365 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.833352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.833352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37038 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    64365 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    32232 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/dns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.833352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/download/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38162 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/download/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/get_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.833352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18333 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/ha_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.833352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/get_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.837352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/get_pci.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/get_usb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/pci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/usb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.837352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    33135 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    18078 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    24956 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/network_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/network_vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.841352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    25681 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.841352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30815 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.841352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    87552 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    75694 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   124005 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    18043 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.829352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:23:57.841352 pulumi_proxmoxve-6.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.014572 pulumi_proxmoxve-6.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-07 07:11:04.014572 pulumi_proxmoxve-6.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:03.998571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.002571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/get_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53365 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.002571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.002571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37038 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64365 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32232 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/dns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.002571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38162 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/download/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/get_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.006571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18333 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/ha_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.006571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/get_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.006571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/get_pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/get_usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.010572 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33135 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18078 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24956 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/network_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/network_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.010572 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25681 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.010572 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30815 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.014572 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87632 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75774 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124005 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.002571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:11:04.014572 pulumi_proxmoxve-6.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/setup.py
```

### Comparing `pulumi_proxmoxve-6.5.0/PKG-INFO` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_proxmoxve
-Version: 6.5.0
+Name: pulumi-proxmoxve
+Version: 6.5.1
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.5.0/README.md` & `pulumi_proxmoxve-6.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/_inputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/options.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/outputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/config/outputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/config/vars.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/download/file.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/download/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/get_node.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/get_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_group.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_groups.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_resource.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_resources.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_resources.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/ha_group.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/ha_resource.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/__init__.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/get_mappings.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/get_mappings.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/_inputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/get_pci.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/get_pci.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/get_usb.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/get_usb.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/outputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/pci.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/pci.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/usb.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/usb.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/outputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/__init__.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/_inputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_alias.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_ip_set.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_ip_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_options.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_rules.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_security_group.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_dns.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_hosts.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_time.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_version.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/network_bridge.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/network_bridge.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/network_vlan.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/network_vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/outputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/outputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_roles.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/role.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/provider.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/_inputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/time.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,15 +579,15 @@
         :param pulumi.Input[bool] backup: Whether the drive should be included when making backups (defaults to `true`).
         :param pulumi.Input[str] cache: The cache type (defaults to `none`).
         :param pulumi.Input[str] datastore_id: The identifier for the datastore to create the
                cloud-init disk in (defaults to `local-lvm`).
         :param pulumi.Input[str] discard: Whether to pass discard/trim requests to the
                underlying storage. Supported values are `on`/`ignore` (defaults
                to `ignore`).
-        :param pulumi.Input[str] file_format: The file format.
+        :param pulumi.Input[str] file_format: The file format (defaults to `raw`).
         :param pulumi.Input[str] file_id: The file ID for a disk image (experimental -
                might cause high CPU utilization during import, especially with large
                disk images).
         :param pulumi.Input[bool] iothread: Whether to use iothreads for this disk (defaults
                to `false`).
         :param pulumi.Input[str] path_in_datastore: The in-datastore path to the disk image.
                ***Experimental.***Use to attach another VM's disks,
@@ -706,15 +706,15 @@
     def discard(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "discard", value)
 
     @property
     @pulumi.getter(name="fileFormat")
     def file_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The file format.
+        The file format (defaults to `raw`).
         """
         return pulumi.get(self, "file_format")
 
     @file_format.setter
     def file_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "file_format", value)
 
@@ -956,15 +956,15 @@
                  datastore_id: Optional[pulumi.Input[str]] = None,
                  file_format: Optional[pulumi.Input[str]] = None,
                  pre_enrolled_keys: Optional[pulumi.Input[bool]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] datastore_id: The identifier for the datastore to create the
                cloud-init disk in (defaults to `local-lvm`).
-        :param pulumi.Input[str] file_format: The file format.
+        :param pulumi.Input[str] file_format: The file format (defaults to `raw`).
         :param pulumi.Input[bool] pre_enrolled_keys: Use am EFI vars template with
                distribution-specific and Microsoft Standard keys enrolled, if used with
                EFI type=`4m`. Ignored for VMs with cpu.architecture=`aarch64` (defaults
                to `false`).
         :param pulumi.Input[str] type: The VGA type (defaults to `std`).
         """
         if datastore_id is not None:
@@ -989,15 +989,15 @@
     def datastore_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_id", value)
 
     @property
     @pulumi.getter(name="fileFormat")
     def file_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The file format.
+        The file format (defaults to `raw`).
         """
         return pulumi.get(self, "file_format")
 
     @file_format.setter
     def file_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "file_format", value)
```

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/get_virtual_machines.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -542,15 +542,15 @@
         :param bool backup: Whether the drive should be included when making backups (defaults to `true`).
         :param str cache: The cache type (defaults to `none`).
         :param str datastore_id: The identifier for the datastore to create the
                cloud-init disk in (defaults to `local-lvm`).
         :param str discard: Whether to pass discard/trim requests to the
                underlying storage. Supported values are `on`/`ignore` (defaults
                to `ignore`).
-        :param str file_format: The file format.
+        :param str file_format: The file format (defaults to `raw`).
         :param str file_id: The file ID for a disk image (experimental -
                might cause high CPU utilization during import, especially with large
                disk images).
         :param bool iothread: Whether to use iothreads for this disk (defaults
                to `false`).
         :param str path_in_datastore: The in-datastore path to the disk image.
                ***Experimental.***Use to attach another VM's disks,
@@ -645,15 +645,15 @@
         """
         return pulumi.get(self, "discard")
 
     @property
     @pulumi.getter(name="fileFormat")
     def file_format(self) -> Optional[str]:
         """
-        The file format.
+        The file format (defaults to `raw`).
         """
         return pulumi.get(self, "file_format")
 
     @property
     @pulumi.getter(name="fileId")
     def file_id(self) -> Optional[str]:
         """
@@ -879,15 +879,15 @@
                  datastore_id: Optional[str] = None,
                  file_format: Optional[str] = None,
                  pre_enrolled_keys: Optional[bool] = None,
                  type: Optional[str] = None):
         """
         :param str datastore_id: The identifier for the datastore to create the
                cloud-init disk in (defaults to `local-lvm`).
-        :param str file_format: The file format.
+        :param str file_format: The file format (defaults to `raw`).
         :param bool pre_enrolled_keys: Use am EFI vars template with
                distribution-specific and Microsoft Standard keys enrolled, if used with
                EFI type=`4m`. Ignored for VMs with cpu.architecture=`aarch64` (defaults
                to `false`).
         :param str type: The VGA type (defaults to `std`).
         """
         if datastore_id is not None:
@@ -908,15 +908,15 @@
         """
         return pulumi.get(self, "datastore_id")
 
     @property
     @pulumi.getter(name="fileFormat")
     def file_format(self) -> Optional[str]:
         """
-        The file format.
+        The file format (defaults to `raw`).
         """
         return pulumi.get(self, "file_format")
 
     @property
     @pulumi.getter(name="preEnrolledKeys")
     def pre_enrolled_keys(self) -> Optional[bool]:
         """
```

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm2.py` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm2.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,19 +257,18 @@
                  template: Optional[pulumi.Input[bool]] = None,
                  timeouts: Optional[pulumi.Input[pulumi.InputType['Vm2TimeoutsArgs']]] = None,
                  __props__=None):
         """
         !> **DO NOT USE**
         This is an experimental implementation of a Proxmox VM resource using Plugin Framework.<br><br>It is a Proof of Concept, highly experimental and **will** change in future. It does not support all features of the Proxmox API for VMs and **MUST NOT** be used in production.
 
-        > Note: Many attributes are marked as **optional** _and_ **computed** in the schema,
+        > Many attributes are marked as **optional** _and_ **computed** in the schema,
         hence you may seem added to the plan with "(known after apply)" status, even if they are not set in the configuration.
         This is done to support the `clone` operation, when a VM is created from an existing one,
-        and attributes of the original VM are copied to the new one.
-
+        and attributes of the original VM are copied to the new one.<br><br>
         Computed attributes allow the provider to set those attributes without user input.
         The attributes are marked as optional to allow the user to set (or overwrite) them if needed.
         In order to remove the computed attribute from the plan, you can set it to an empty value (e.g. `""` for string, `[]` for collection).
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['Vm2CloneArgs']] clone: The cloning configuration.
@@ -285,19 +284,18 @@
                  resource_name: str,
                  args: Vm2Args,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         !> **DO NOT USE**
         This is an experimental implementation of a Proxmox VM resource using Plugin Framework.<br><br>It is a Proof of Concept, highly experimental and **will** change in future. It does not support all features of the Proxmox API for VMs and **MUST NOT** be used in production.
 
-        > Note: Many attributes are marked as **optional** _and_ **computed** in the schema,
+        > Many attributes are marked as **optional** _and_ **computed** in the schema,
         hence you may seem added to the plan with "(known after apply)" status, even if they are not set in the configuration.
         This is done to support the `clone` operation, when a VM is created from an existing one,
-        and attributes of the original VM are copied to the new one.
-
+        and attributes of the original VM are copied to the new one.<br><br>
         Computed attributes allow the provider to set those attributes without user input.
         The attributes are marked as optional to allow the user to set (or overwrite) them if needed.
         In order to remove the computed attribute from the plan, you can set it to an empty value (e.g. `""` for string, `[]` for collection).
 
         :param str resource_name: The name of the resource.
         :param Vm2Args args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
```

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-6.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-proxmoxve
-Version: 6.5.0
+Name: pulumi_proxmoxve
+Version: 6.5.1
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.0/setup.py` & `pulumi_proxmoxve-6.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.5.0"
+VERSION = "6.5.1"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "proxmoxve Pulumi Package - Development Version"
```

