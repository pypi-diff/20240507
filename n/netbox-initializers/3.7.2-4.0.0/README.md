# Comparing `tmp/netbox_initializers-3.7.2.tar.gz` & `tmp/netbox_initializers-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_initializers-3.7.2.tar", max compression
+gzip compressed data, was "netbox_initializers-4.0.0.tar", max compression
```

## Comparing `netbox_initializers-3.7.2.tar` & `netbox_initializers-4.0.0.tar`

### file list

```diff
@@ -1,107 +1,109 @@
--rw-r--r--   0        0        0    11358 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/LICENSE
--rw-r--r--   0        0        0     1503 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/README.md
--rw-r--r--   0        0        0      753 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/pyproject.toml
--rw-r--r--   0        0        0      353 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/__init__.py
--rw-r--r--   0        0        0     6934 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/__init__.py
--rw-r--r--   0        0        0     1636 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/aggregates.py
--rw-r--r--   0        0        0     1288 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/asns.py
--rw-r--r--   0        0        0     9076 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/cables.py
--rw-r--r--   0        0        0      932 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/circuit_types.py
--rw-r--r--   0        0        0     1547 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/circuits.py
--rw-r--r--   0        0        0      815 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/cluster_groups.py
--rw-r--r--   0        0        0      801 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/cluster_types.py
--rw-r--r--   0        0        0     1620 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/clusters.py
--rw-r--r--   0        0        0     2135 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/config_contexts.py
--rw-r--r--   0        0        0     1312 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/config_templates.py
--rw-r--r--   0        0        0     1258 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/contact_groups.py
--rw-r--r--   0        0        0      932 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/contact_roles.py
--rw-r--r--   0        0        0     1168 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/contacts.py
--rw-r--r--   0        0        0     6054 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/custom_fields.py
--rw-r--r--   0        0        0     1432 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/custom_links.py
--rw-r--r--   0        0        0     1046 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/device_roles.py
--rw-r--r--   0        0        0     5547 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/device_types.py
--rw-r--r--   0        0        0     2149 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/devices.py
--rw-r--r--   0        0        0      860 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/groups.py
--rw-r--r--   0        0        0     3345 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/interfaces.py
--rw-r--r--   0        0        0     3156 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/ip_addresses.py
--rw-r--r--   0        0        0     1050 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/locations.py
--rw-r--r--   0        0        0      794 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/manufacturers.py
--rw-r--r--   0        0        0     3110 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/object_permissions.py
--rw-r--r--   0        0        0     1142 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/platforms.py
--rw-r--r--   0        0        0     1539 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/power_feeds.py
--rw-r--r--   0        0        0     1557 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/power_panels.py
--rw-r--r--   0        0        0      701 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/prefix_vlan_roles.py
--rw-r--r--   0        0        0     1537 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/prefixes.py
--rw-r--r--   0        0        0     2240 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/primary_ips.py
--rw-r--r--   0        0        0     1321 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/providers.py
--rw-r--r--   0        0        0     1019 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/rack_roles.py
--rw-r--r--   0        0        0     1542 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/racks.py
--rw-r--r--   0        0        0      993 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/regions.py
--rw-r--r--   0        0        0      651 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/rirs.py
--rw-r--r--   0        0        0     1269 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/route_targets.py
--rw-r--r--   0        0        0      881 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/service_templates.py
--rw-r--r--   0        0        0     1208 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/services.py
--rw-r--r--   0        0        0     1988 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/sites.py
--rw-r--r--   0        0        0     1351 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/tags.py
--rw-r--r--   0        0        0      793 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/tenant_groups.py
--rw-r--r--   0        0        0     1152 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/tenants.py
--rw-r--r--   0        0        0      935 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/users.py
--rw-r--r--   0        0        0     2050 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/virtual_machines.py
--rw-r--r--   0        0        0     1319 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/virtualization_interfaces.py
--rw-r--r--   0        0        0     2123 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/vlan_groups.py
--rw-r--r--   0        0        0     1375 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/vlans.py
--rw-r--r--   0        0        0     1161 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/vrfs.py
--rw-r--r--   0        0        0     1053 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/webhooks.py
--rw-r--r--   0        0        0      152 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/aggregates.yml
--rw-r--r--   0        0        0      108 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/asns.yml
--rw-r--r--   0        0        0     2299 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/cables.yml
--rw-r--r--   0        0        0       98 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/circuit_types.yml
--rw-r--r--   0        0        0      146 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/circuits.yml
--rw-r--r--   0        0        0       72 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/cluster_groups.yml
--rw-r--r--   0        0        0       36 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/cluster_types.yml
--rw-r--r--   0        0        0      130 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/clusters.yml
--rw-r--r--   0        0        0      710 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/config_contexts.yml
--rw-r--r--   0        0        0      148 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/config_templates.yml
--rw-r--r--   0        0        0      264 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/contact_groups.yml
--rw-r--r--   0        0        0      110 2024-01-31 09:36:07.351162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/contact_roles.yml
--rw-r--r--   0        0        0      694 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/contacts.yml
--rw-r--r--   0        0        0     2416 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/custom_fields.yml
--rw-r--r--   0        0        0      472 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/custom_links.yml
--rw-r--r--   0        0        0      272 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/device_roles.yml
--rw-r--r--   0        0        0     1511 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/device_types.yml
--rw-r--r--   0        0        0     1105 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/devices.yml
--rw-r--r--   0        0        0      124 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/groups.yml
--rw-r--r--   0        0        0      769 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/interfaces.yml
--rw-r--r--   0        0        0      953 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/ip_addresses.yml
--rw-r--r--   0        0        0      219 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/locations.yml
--rw-r--r--   0        0        0      136 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/manufacturers.yml
--rw-r--r--   0        0        0     1079 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/object_permissions.yml
--rw-r--r--   0        0        0      255 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/platforms.yml
--rw-r--r--   0        0        0      316 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/power_feeds.yml
--rw-r--r--   0        0        0      117 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/power_panels.yml
--rw-r--r--   0        0        0       52 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/prefix_vlan_roles.yml
--rw-r--r--   0        0        0      522 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/prefixes.yml
--rw-r--r--   0        0        0      102 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/providers.yml
--rw-r--r--   0        0        0      200 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/rack_roles.yml
--rw-r--r--   0        0        0      723 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/racks.yml
--rw-r--r--   0        0        0      198 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/regions.yml
--rw-r--r--   0        0        0      179 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/rirs.yml
--rw-r--r--   0        0        0       62 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/route_targets.yml
--rw-r--r--   0        0        0      166 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/service_templates.yml
--rw-r--r--   0        0        0      265 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/services.yml
--rw-r--r--   0        0        0      697 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/sites.yml
--rw-r--r--   0        0        0      301 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/tags.yml
--rw-r--r--   0        0        0      100 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/tenant_groups.yml
--rw-r--r--   0        0        0       98 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/tenants.yml
--rw-r--r--   0        0        0      449 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/users.yml
--rw-r--r--   0        0        0      779 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/virtual_machines.yml
--rw-r--r--   0        0        0      346 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/virtualization_interfaces.yml
--rw-r--r--   0        0        0      585 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/vlan_groups.yml
--rw-r--r--   0        0        0      309 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/vlans.yml
--rw-r--r--   0        0        0      166 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/vrfs.yml
--rw-r--r--   0        0        0      211 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/webhooks.yml
--rw-r--r--   0        0        0        0 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/management/__init__.py
--rw-r--r--   0        0        0        0 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/management/commands/__init__.py
--rw-r--r--   0        0        0     1705 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/management/commands/copy_initializers_examples.py
--rw-r--r--   0        0        0     1359 2024-01-31 09:36:07.355162 netbox_initializers-3.7.2/src/netbox_initializers/management/commands/load_initializer_data.py
--rw-r--r--   0        0        0     2454 1970-01-01 00:00:00.000000 netbox_initializers-3.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-07 05:25:43.786314 netbox_initializers-4.0.0/LICENSE
+-rw-r--r--   0        0        0     1503 2024-05-07 05:25:43.786314 netbox_initializers-4.0.0/README.md
+-rw-r--r--   0        0        0      753 2024-05-07 05:25:43.786314 netbox_initializers-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0      357 2024-05-07 05:25:43.786314 netbox_initializers-4.0.0/src/netbox_initializers/__init__.py
+-rw-r--r--   0        0        0     6972 2024-05-07 05:25:43.786314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/__init__.py
+-rw-r--r--   0        0        0     1636 2024-05-07 05:25:43.786314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/aggregates.py
+-rw-r--r--   0        0        0     1288 2024-05-07 05:25:43.786314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/asns.py
+-rw-r--r--   0        0        0     9076 2024-05-07 05:25:43.786314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/cables.py
+-rw-r--r--   0        0        0      932 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/circuit_types.py
+-rw-r--r--   0        0        0     1547 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/circuits.py
+-rw-r--r--   0        0        0      815 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/cluster_groups.py
+-rw-r--r--   0        0        0      801 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/cluster_types.py
+-rw-r--r--   0        0        0     1620 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/clusters.py
+-rw-r--r--   0        0        0     2135 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/config_contexts.py
+-rw-r--r--   0        0        0     1312 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/config_templates.py
+-rw-r--r--   0        0        0     1258 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/contact_groups.py
+-rw-r--r--   0        0        0      932 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/contact_roles.py
+-rw-r--r--   0        0        0     1168 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/contacts.py
+-rw-r--r--   0        0        0     6028 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/custom_fields.py
+-rw-r--r--   0        0        0     1405 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/custom_links.py
+-rw-r--r--   0        0        0     1043 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/device_roles.py
+-rw-r--r--   0        0        0     5547 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/device_types.py
+-rw-r--r--   0        0        0     2142 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/devices.py
+-rw-r--r--   0        0        0      833 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/groups.py
+-rw-r--r--   0        0        0     3495 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/interfaces.py
+-rw-r--r--   0        0        0     3156 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/ip_addresses.py
+-rw-r--r--   0        0        0     1050 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/locations.py
+-rw-r--r--   0        0        0      794 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/manufacturers.py
+-rw-r--r--   0        0        0     3059 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/object_permissions.py
+-rw-r--r--   0        0        0     1142 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/platforms.py
+-rw-r--r--   0        0        0     1539 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/power_feeds.py
+-rw-r--r--   0        0        0     1557 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/power_panels.py
+-rw-r--r--   0        0        0      701 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/prefix_vlan_roles.py
+-rw-r--r--   0        0        0     1537 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/prefixes.py
+-rw-r--r--   0        0        0     2240 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/primary_ips.py
+-rw-r--r--   0        0        0     1321 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/providers.py
+-rw-r--r--   0        0        0     1016 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/rack_roles.py
+-rw-r--r--   0        0        0     1542 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/racks.py
+-rw-r--r--   0        0        0      993 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/regions.py
+-rw-r--r--   0        0        0      651 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/rirs.py
+-rw-r--r--   0        0        0     1269 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/route_targets.py
+-rw-r--r--   0        0        0      881 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/service_templates.py
+-rw-r--r--   0        0        0     1208 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/services.py
+-rw-r--r--   0        0        0     1074 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/site_groups.py
+-rw-r--r--   0        0        0     2044 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/sites.py
+-rw-r--r--   0        0        0     1323 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/tags.py
+-rw-r--r--   0        0        0      793 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/tenant_groups.py
+-rw-r--r--   0        0        0     1152 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/tenants.py
+-rw-r--r--   0        0        0      887 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/users.py
+-rw-r--r--   0        0        0     2050 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/virtual_machines.py
+-rw-r--r--   0        0        0     1319 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/virtualization_interfaces.py
+-rw-r--r--   0        0        0     2123 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/vlan_groups.py
+-rw-r--r--   0        0        0     1375 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/vlans.py
+-rw-r--r--   0        0        0     1161 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/vrfs.py
+-rw-r--r--   0        0        0     1053 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/webhooks.py
+-rw-r--r--   0        0        0      152 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/aggregates.yml
+-rw-r--r--   0        0        0      108 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/asns.yml
+-rw-r--r--   0        0        0     2299 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/cables.yml
+-rw-r--r--   0        0        0       98 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/circuit_types.yml
+-rw-r--r--   0        0        0      146 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/circuits.yml
+-rw-r--r--   0        0        0       72 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/cluster_groups.yml
+-rw-r--r--   0        0        0       36 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/cluster_types.yml
+-rw-r--r--   0        0        0      130 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/clusters.yml
+-rw-r--r--   0        0        0      710 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/config_contexts.yml
+-rw-r--r--   0        0        0      148 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/config_templates.yml
+-rw-r--r--   0        0        0      264 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/contact_groups.yml
+-rw-r--r--   0        0        0      110 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/contact_roles.yml
+-rw-r--r--   0        0        0      694 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/contacts.yml
+-rw-r--r--   0        0        0     2416 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/custom_fields.yml
+-rw-r--r--   0        0        0      472 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/custom_links.yml
+-rw-r--r--   0        0        0      272 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/device_roles.yml
+-rw-r--r--   0        0        0     1691 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/device_types.yml
+-rw-r--r--   0        0        0     1192 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/devices.yml
+-rw-r--r--   0        0        0      124 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/groups.yml
+-rw-r--r--   0        0        0      879 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/interfaces.yml
+-rw-r--r--   0        0        0      953 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/ip_addresses.yml
+-rw-r--r--   0        0        0      219 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/locations.yml
+-rw-r--r--   0        0        0      136 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/manufacturers.yml
+-rw-r--r--   0        0        0     1079 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/object_permissions.yml
+-rw-r--r--   0        0        0      255 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/platforms.yml
+-rw-r--r--   0        0        0      316 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/power_feeds.yml
+-rw-r--r--   0        0        0      117 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/power_panels.yml
+-rw-r--r--   0        0        0       52 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/prefix_vlan_roles.yml
+-rw-r--r--   0        0        0      522 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/prefixes.yml
+-rw-r--r--   0        0        0      102 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/providers.yml
+-rw-r--r--   0        0        0      200 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/rack_roles.yml
+-rw-r--r--   0        0        0      723 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/racks.yml
+-rw-r--r--   0        0        0      198 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/regions.yml
+-rw-r--r--   0        0        0      179 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/rirs.yml
+-rw-r--r--   0        0        0       62 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/route_targets.yml
+-rw-r--r--   0        0        0      166 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/service_templates.yml
+-rw-r--r--   0        0        0      265 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/services.yml
+-rw-r--r--   0        0        0      140 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/site_groups.yml
+-rw-r--r--   0        0        0      715 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/sites.yml
+-rw-r--r--   0        0        0      301 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/tags.yml
+-rw-r--r--   0        0        0      100 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/tenant_groups.yml
+-rw-r--r--   0        0        0       98 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/tenants.yml
+-rw-r--r--   0        0        0      449 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/users.yml
+-rw-r--r--   0        0        0      779 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/virtual_machines.yml
+-rw-r--r--   0        0        0      346 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/virtualization_interfaces.yml
+-rw-r--r--   0        0        0      585 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/vlan_groups.yml
+-rw-r--r--   0        0        0      309 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/vlans.yml
+-rw-r--r--   0        0        0      166 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/vrfs.yml
+-rw-r--r--   0        0        0      211 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/webhooks.yml
+-rw-r--r--   0        0        0        0 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/management/commands/__init__.py
+-rw-r--r--   0        0        0     1705 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/management/commands/copy_initializers_examples.py
+-rw-r--r--   0        0        0     1359 2024-05-07 05:25:43.790314 netbox_initializers-4.0.0/src/netbox_initializers/management/commands/load_initializer_data.py
+-rw-r--r--   0        0        0     2454 1970-01-01 00:00:00.000000 netbox_initializers-4.0.0/PKG-INFO
```

### Comparing `netbox_initializers-3.7.2/LICENSE` & `netbox_initializers-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/README.md` & `netbox_initializers-4.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Load data from YAML files into Netbox
 
 ## Installation
 
 First activate your virtual environment where Netbox is installed, the install the plugin version correspondig to your Netbox version.
 ```bash
-pip install "netbox-initializers==3.7.*"
+pip install "netbox-initializers==4.0.*"
 ```
 Then you need to add the plugin to the `PLUGINS` array in the Netbox configuration.
 ```python
 PLUGINS = [
     'netbox_initializers',
 ]
 ```
@@ -32,10 +32,10 @@
 
 ## Netbox Docker image
 
 The initializers where a part of the Docker image and where then extracted into a Netbox plugin. This was done to split the release cycle of the initializers and the image.
 To use the new plugin in a the Netbox Docker image, it musst be installad into the image. To this, the following example can be used as a starting point:
 
 ```dockerfile
-FROM netboxcommunity/netbox:v3.7
-RUN /opt/netbox/venv/bin/pip install "netbox-initializers==3.7.*"
+FROM netboxcommunity/netbox:v4.0
+RUN /opt/netbox/venv/bin/pip install "netbox-initializers==4.0.*"
 ```
```

### Comparing `netbox_initializers-3.7.2/pyproject.toml` & `netbox_initializers-4.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
   "Topic :: System :: Systems Administration"
 ]
 description = "Load initial data into Netbox"
 license = "Apache-2.0"
 name = "netbox-initializers"
 readme = "README.md"
 repository = "https://github.com/tobiasge/netbox-initializers"
-version = "3.7.2"
+version = "4.0.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-"ruamel.yaml" = "0.18.5"
+"ruamel.yaml" = "0.18.6"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.black]
 line_length = 100
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/__init__.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import Tuple
 
-from django.contrib.contenttypes.models import ContentType
+from core.models import ObjectType
 from django.core.exceptions import ObjectDoesNotExist
 from extras.models import CustomField, Tag
 from ruamel.yaml import YAML
 
 INITIALIZER_ORDER = (
     "users",
     "groups",
@@ -13,14 +13,15 @@
     "custom_fields",
     "custom_links",
     "tags",
     "config_templates",
     "webhooks",
     "tenant_groups",
     "tenants",
+    "site_groups",
     "regions",
     "rirs",
     "asns",
     "sites",
     "locations",
     "rack_roles",
     "racks",
@@ -100,16 +101,16 @@
         save = False
         for key, value in custom_field_data.items():
             try:
                 cf = CustomField.objects.get(name=key)
             except ObjectDoesNotExist:
                 missing_cfs.append(key)
             else:
-                ct = ContentType.objects.get_for_model(entity)
-                if ct not in cf.content_types.all():
+                ct = ObjectType.objects.get_for_model(entity)
+                if ct not in cf.object_types.all():
                     print(
                         f"⚠️ Custom field {key} is not enabled for {entity}'s model!"
                         "Please check the 'on_objects' for that custom field in custom_fields.yml"
                     )
                 elif key not in entity.custom_field_data:
                     entity.custom_field_data[key] = value
                     save = True
@@ -126,15 +127,15 @@
     def set_tags(self, entity, tags):
         if not tags:
             return
 
         if not hasattr(entity, "tags"):
             raise Exception(f"⚠️ Tags cannot be applied to {entity}'s model")
 
-        ct = ContentType.objects.get_for_model(entity)
+        ct = ObjectType.objects.get_for_model(entity)
 
         save = False
         for tag in Tag.objects.filter(name__in=tags):
             restricted_cts = tag.object_types.all()
             if restricted_cts and ct not in restricted_cts:
                 raise Exception(f"⚠️ Tag {tag} cannot be applied to {entity}'s model")
 
@@ -201,14 +202,15 @@
 from .rack_roles import RackRoleInitializer
 from .racks import RackInitializer
 from .regions import RegionInitializer
 from .rirs import RIRInitializer
 from .route_targets import RouteTargetInitializer
 from .service_templates import ServiceTemplateInitializer
 from .services import ServiceInitializer
+from .site_groups import SiteGroupInitializer
 from .sites import SiteInitializer
 from .tags import TagInitializer
 from .tenant_groups import TenantGroupInitializer
 from .tenants import TenantInitializer
 from .users import UserInitializer
 from .virtual_machines import VirtualMachineInitializer
 from .virtualization_interfaces import VMInterfaceInitializer
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/aggregates.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/aggregates.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/asns.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/asns.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/cables.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/cables.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/circuit_types.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/circuit_types.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/circuits.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/circuits.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/cluster_groups.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/cluster_groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/cluster_types.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/cluster_types.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/clusters.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/clusters.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/config_contexts.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/config_contexts.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/config_templates.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/config_templates.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/contact_groups.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/contact_groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/contact_roles.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/contact_roles.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/contacts.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/contacts.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/custom_fields.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/custom_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 from . import BaseInitializer, register_initializer
 
 
 def get_class_for_class_path(class_path):
     import importlib
 
-    from django.contrib.contenttypes.models import ContentType
+    from core.models import ObjectType
 
     module_name, class_name = class_path.rsplit(".", 1)
     module = importlib.import_module(module_name)
     clazz = getattr(module, class_name)
-    return ContentType.objects.get_for_model(clazz)
+    return ObjectType.objects.get_for_model(clazz)
 
 
 class CustomFieldInitializer(BaseInitializer):
     data_file_name = "custom_fields.yml"
 
     def load_data(self):
         customfields = self.load_yaml()
@@ -31,15 +31,15 @@
                 if cf_details.get("description", False):
                     custom_field.description = cf_details["description"]
 
                 if cf_details.get("label", False):
                     custom_field.label = cf_details["label"]
 
                 for object_type in cf_details.get("on_objects", []):
-                    custom_field.content_types.add(get_class_for_class_path(object_type))
+                    custom_field.object_types.add(get_class_for_class_path(object_type))
 
                 if cf_details.get("required", False):
                     custom_field.required = cf_details["required"]
 
                 if cf_details.get("type", False):
                     custom_field.type = cf_details["type"]
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/custom_links.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/custom_links.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from django.contrib.contenttypes.models import ContentType
+from core.models import ObjectType
 from extras.models import CustomLink
 
 from . import BaseInitializer, register_initializer
 
 
 def get_content_type(content_type):
     try:
-        return ContentType.objects.get(model=content_type)
-    except ContentType.DoesNotExist:
+        return ObjectType.objects.get(model=content_type)
+    except ObjectType.DoesNotExist:
         pass
     return None
 
 
 class CustomLinkInitializer(BaseInitializer):
     data_file_name = "custom_links.yml"
 
@@ -32,13 +32,13 @@
 
             matching_params, defaults = self.split_params(link)
             custom_link, created = CustomLink.objects.get_or_create(
                 **matching_params, defaults=defaults
             )
 
             if created:
-                custom_link.content_types.add(content_type)
+                custom_link.object_types.add(content_type)
                 custom_link.save()
                 print("🔗 Created Custom Link '{0}'".format(custom_link.name))
 
 
 register_initializer("custom_links", CustomLinkInitializer)
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/device_roles.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/device_roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dcim.models import DeviceRole
-from utilities.choices import ColorChoices
+from netbox.choices import ColorChoices
 
 from . import BaseInitializer, register_initializer
 
 
 class DeviceRoleInitializer(BaseInitializer):
     data_file_name = "device_roles.yml"
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/device_types.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/device_types.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/devices.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/devices.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from tenancy.models import Tenant
 from virtualization.models import Cluster
 
 from . import BaseInitializer, register_initializer
 
 MATCH_PARAMS = ["device_type", "name", "site"]
 REQUIRED_ASSOCS = {
-    "device_role": (DeviceRole, "name"),
+    "role": (DeviceRole, "name"),
     "device_type": (DeviceType, "model"),
     "site": (Site, "name"),
 }
 OPTIONAL_ASSOCS = {
     "cluster": (Cluster, "name"),
     "config_template": (ConfigTemplate, "name"),
     "location": (Location, "name"),
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/groups.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/groups.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from users.models import NetBoxGroup, NetBoxUser
+from users.models import Group, User
 
 from . import BaseInitializer, register_initializer
 
 
 class GroupInitializer(BaseInitializer):
     data_file_name = "groups.yml"
 
     def load_data(self):
         groups = self.load_yaml()
         if groups is None:
             return
 
         for groupname, group_details in groups.items():
-            group, created = NetBoxGroup.objects.get_or_create(name=groupname)
+            group, created = Group.objects.get_or_create(name=groupname)
             if created:
                 print("👥 Created group", groupname)
             for username in group_details.get("users", []):
-                user = NetBoxUser.objects.get(username=username)
+                user = User.objects.get(username=username)
                 if user:
-                    group.user_set.add(user)
+                    group.users.add(user)
                     print(" 👤 Assigned user %s to group %s" % (username, group.name))
             group.save()
 
 
 register_initializer("groups", GroupInitializer)
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/interfaces.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/interfaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,18 @@
             matching_params, defaults = self.split_params(params, MATCH_PARAMS)
             interface, created = Interface.objects.get_or_create(
                 **matching_params, defaults=defaults
             )
 
             if created:
                 print(f"🧷 Created interface {interface} on {interface.device}")
+            else:
+                for name in defaults:
+                    setattr(interface, name, defaults[name])
+                interface.save()
 
             self.set_custom_fields_values(interface, custom_field_data)
             self.set_tags(interface, tags)
 
             for related_field, related_value in related_interfaces.items():
                 if not related_value:
                     continue
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/ip_addresses.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/ip_addresses.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/locations.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/locations.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/manufacturers.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/manufacturers.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/object_permissions.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/object_permissions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from django.contrib.contenttypes.models import ContentType
-from users.models import NetBoxGroup, NetBoxUser, ObjectPermission
+from core.models import ObjectType
+from users.models import Group, ObjectPermission, User
 
 from . import BaseInitializer, register_initializer
 
 
 class ObjectPermissionInitializer(BaseInitializer):
     data_file_name = "object_permissions.yml"
 
@@ -24,46 +24,46 @@
             if permission_details.get("constraints", 0):
                 object_permission.constraints = permission_details["constraints"]
 
             if permission_details.get("object_types", 0):
                 object_types = permission_details["object_types"]
 
                 if object_types == "all":
-                    object_permission.object_types.set(ContentType.objects.all())
+                    object_permission.object_types.set(ObjectType.objects.all())
 
                 else:
                     for app_label, models in object_types.items():
                         if models == "all":
-                            app_models = ContentType.objects.filter(app_label=app_label)
+                            app_models = ObjectType.objects.filter(app_label=app_label)
 
                             for app_model in app_models:
                                 object_permission.object_types.add(app_model.id)
                         else:
                             # There is
                             for model in models:
                                 object_permission.object_types.add(
-                                    ContentType.objects.get(app_label=app_label, model=model)
+                                    ObjectType.objects.get(app_label=app_label, model=model)
                                 )
             if created:
                 print("🔓 Created object permission", object_permission.name)
 
             if permission_details.get("groups", 0):
                 for groupname in permission_details["groups"]:
-                    group = NetBoxGroup.objects.filter(name=groupname).first()
+                    group = Group.objects.filter(name=groupname).first()
 
                     if group:
                         object_permission.groups.add(group)
                         print(
                             " 👥 Assigned group %s object permission of %s"
                             % (groupname, object_permission.name)
                         )
 
             if permission_details.get("users", 0):
                 for username in permission_details["users"]:
-                    user = NetBoxUser.objects.filter(username=username).first()
+                    user = User.objects.filter(username=username).first()
 
                     if user:
                         object_permission.users.add(user)
                         print(
                             " 👤 Assigned user %s object permission of %s"
                             % (username, object_permission.name)
                         )
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/platforms.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/platforms.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/power_feeds.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/power_feeds.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/power_panels.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/power_panels.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/prefix_vlan_roles.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/prefix_vlan_roles.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/prefixes.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/prefixes.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/primary_ips.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/primary_ips.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/providers.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/providers.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/rack_roles.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/rack_roles.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dcim.models import RackRole
-from utilities.choices import ColorChoices
+from netbox.choices import ColorChoices
 
 from . import BaseInitializer, register_initializer
 
 
 class RackRoleInitializer(BaseInitializer):
     data_file_name = "rack_roles.yml"
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/racks.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/racks.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/regions.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/regions.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/rirs.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/rirs.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/route_targets.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/route_targets.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/service_templates.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/service_templates.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/services.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/services.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/sites.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/sites.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from dcim.models import Region, Site
+from dcim.models import Region, Site, SiteGroup
 from ipam.models import ASN
 from tenancy.models import Tenant
 
 from . import BaseInitializer, register_initializer
 
-OPTIONAL_ASSOCS = {"region": (Region, "name"), "tenant": (Tenant, "name")}
+OPTIONAL_ASSOCS = {
+    "region": (Region, "name"),
+    "group": (SiteGroup, "name"),
+    "tenant": (Tenant, "name"),
+}
 
 
 class SiteInitializer(BaseInitializer):
     data_file_name = "sites.yml"
 
     def load_data(self):
         sites = self.load_yaml()
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/tags.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from django.contrib.contenttypes.models import ContentType
+from core.models import ObjectType
 from extras.models import Tag
-from utilities.choices import ColorChoices
+from netbox.choices import ColorChoices
 
 from . import BaseInitializer, register_initializer
 
 
 class TagInitializer(BaseInitializer):
     data_file_name = "tags.yml"
 
@@ -25,15 +25,15 @@
             tag, created = Tag.objects.get_or_create(**matching_params, defaults=defaults)
 
             if created:
                 print("🎨 Created Tag", tag.name)
 
                 if object_types:
                     for ot in object_types:
-                        ct = ContentType.objects.get(
+                        ct = ObjectType.objects.get(
                             app_label=ot["app"],
                             model=ot["model"],
                         )
                         tag.object_types.add(ct)
                         print(f"🎨 Restricted Tag {tag.name} to {ot['app']}.{ot['model']}")
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/tenant_groups.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/tenant_groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/tenants.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/tenants.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/users.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/users.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from users.models import NetBoxUser, Token
+from users.models import Token, User
 
 from . import BaseInitializer, register_initializer
 
 
 class UserInitializer(BaseInitializer):
     data_file_name = "users.yml"
 
     def load_data(self):
         users = self.load_yaml()
         if users is None:
             return
 
         for username, user_details in users.items():
             api_token = user_details.pop("api_token", Token.generate_key())
-            password = user_details.pop("password", NetBoxUser.objects.make_random_password())
-            user, created = NetBoxUser.objects.get_or_create(
-                username=username, defaults=user_details
-            )
+            password = user_details.pop("password", User.objects.make_random_password())
+            user, created = User.objects.get_or_create(username=username, defaults=user_details)
             if created:
                 user.set_password(password)
                 user.save()
                 if api_token:
                     Token.objects.get_or_create(user=user, key=api_token)
                 print("👤 Created user", username)
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/virtual_machines.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/virtual_machines.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/virtualization_interfaces.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/virtualization_interfaces.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/vlan_groups.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/vlan_groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/vlans.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/vlans.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/vrfs.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/vrfs.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/webhooks.py` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/webhooks.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/cables.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/cables.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/config_contexts.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/config_contexts.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/contacts.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/contacts.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/custom_fields.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/custom_fields.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/device_types.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/device_types.yml`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 # - model: Model 3
 #   manufacturer: Manufacturer 1
 #   slug: model-3
 #   is_full_depth: false
 #   u_height: 0
 #   custom_field_data:
 #     text_field: Description
+# - model: TOR-8P
+#   manufacturer: No Name
+#   part_number: vlab-eos
+#   slug: tor-8p
+#   interfaces:
+#     - name: Ethernet1
+#       type: 1000base-t
+#       description: UPLINK
 # - model: Other
 #   manufacturer: No Name
 #   slug: other
 #   custom_field_data:
 #     text_field: Description
 #   interfaces:
 #     - name: eth0
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/devices.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/devices.yml`

 * *Files 6% similar despite different names*

```diff
@@ -10,48 +10,54 @@
 ##   - failed
 ##   - inventory
 ##   - decommissioning
 ##
 ## Examples:
 
 # - name: server01
-#   device_role: server
+#   role: server
 #   device_type: Other
 #   site: AMS 1
 #   rack: rack-01
 #   face: front
 #   position: 1
 #   custom_field_data:
 #     text_field: Description
 # - name: server02
-#   device_role: server
+#   role: server
 #   device_type: Other
 #   site: AMS 2
 #   rack: rack-02
 #   face: front
 #   position: 2
 #   primary_ip4: 10.1.1.2/24
 #   primary_ip4_vrf: vrf1
 #   primary_ip6: 2001:db8:a000:1::2/64
 #   primary_ip6_vrf: vrf1
 #   custom_field_data:
 #     text_field: Description
 # - name: server03
-#   device_role: server
+#   role: server
 #   device_type: Other
 #   site: SING 1
 #   rack: rack-03
 #   face: front
 #   position: 3
 #   custom_field_data:
 #     text_field: Description
 # - name: server04
-#   device_role: server
+#   role: server
 #   device_type: Other
 #   site: SING 1
 #   location: cage 101
 #   face: front
 #   position: 3
 #   config_template: configtemplate1
 #   custom_field_data:
 #     text_field: Description
 #
+## Templated device
+# - name: gns3-tor
+#   role: switch
+#   device_type: TOR-8P
+#   site: SING 1
+#   rack: rack-03
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/interfaces.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/interfaces.yml`

 * *Files 12% similar despite different names*

```diff
@@ -30,7 +30,12 @@
 #   type: 1000base-t
 #   name: eth0
 #   untagged_vlan: vlan2
 # - device: server02
 #   enabled: true
 #   type: virtual
 #   name: loopback
+
+## Example to add attributes on a templated interface
+# - name: Ethernet1
+#   mtu: 9100
+#   device: gns3-tor
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/ip_addresses.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/ip_addresses.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/object_permissions.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/object_permissions.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/prefixes.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/prefixes.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/racks.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/racks.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/sites.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/sites.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # - name: AMS 1
 #   slug: ams1
 #   region: Downtown
 #   status: active
 #   facility: Amsterdam 1
+#.  group: Office
 #   custom_field_data:
 #     text_field: Description for AMS1
 # - name: AMS 2
 #   slug: ams2
 #   asns:
 #   - 2
 #   region: Downtown
```

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/virtual_machines.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/virtual_machines.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/initializers/yaml/vlan_groups.yml` & `netbox_initializers-4.0.0/src/netbox_initializers/initializers/yaml/vlan_groups.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/management/commands/copy_initializers_examples.py` & `netbox_initializers-4.0.0/src/netbox_initializers/management/commands/copy_initializers_examples.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/src/netbox_initializers/management/commands/load_initializer_data.py` & `netbox_initializers-4.0.0/src/netbox_initializers/management/commands/load_initializer_data.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.7.2/PKG-INFO` & `netbox_initializers-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-initializers
-Version: 3.7.2
+Version: 4.0.0
 Summary: Load initial data into Netbox
 Home-page: https://github.com/tobiasge/netbox-initializers
 License: Apache-2.0
 Author: Tobias Genannt
 Author-email: tobias.genannt@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Plugins
@@ -14,27 +14,27 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
-Requires-Dist: ruamel.yaml (==0.18.5)
+Requires-Dist: ruamel.yaml (==0.18.6)
 Project-URL: Repository, https://github.com/tobiasge/netbox-initializers
 Description-Content-Type: text/markdown
 
 # Netbox Initializers Plugin
 
 Load data from YAML files into Netbox
 
 ## Installation
 
 First activate your virtual environment where Netbox is installed, the install the plugin version correspondig to your Netbox version.
 ```bash
-pip install "netbox-initializers==3.7.*"
+pip install "netbox-initializers==4.0.*"
 ```
 Then you need to add the plugin to the `PLUGINS` array in the Netbox configuration.
 ```python
 PLUGINS = [
     'netbox_initializers',
 ]
 ```
@@ -56,11 +56,11 @@
 
 ## Netbox Docker image
 
 The initializers where a part of the Docker image and where then extracted into a Netbox plugin. This was done to split the release cycle of the initializers and the image.
 To use the new plugin in a the Netbox Docker image, it musst be installad into the image. To this, the following example can be used as a starting point:
 
 ```dockerfile
-FROM netboxcommunity/netbox:v3.7
-RUN /opt/netbox/venv/bin/pip install "netbox-initializers==3.7.*"
+FROM netboxcommunity/netbox:v4.0
+RUN /opt/netbox/venv/bin/pip install "netbox-initializers==4.0.*"
 ```
```

