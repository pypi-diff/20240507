# Comparing `tmp/netbox-routing-0.1.0.tar.gz` & `tmp/netbox-routing-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/netbox-routing-0.1.0.tar", last modified: Thu Aug 24 20:20:22 2023, max compression
+gzip compressed data, was "dist/netbox-routing-0.1.1.tar", last modified: Tue May  7 17:49:42 2024, max compression
```

## Comparing `netbox-routing-0.1.0.tar` & `netbox-routing-0.1.1.tar`

### file list

```diff
@@ -1,110 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (999)    11357 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      120 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)      537 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2443 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/
--rw-r--r--   0 runner    (1001) docker     (999)      557 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/api/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/api/nested_serializers/
--rw-r--r--   0 runner    (1001) docker     (999)      384 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/nested_serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1407 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/nested_serializers/objects.py
--rw-r--r--   0 runner    (1001) docker     (999)     1341 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/nested_serializers/ospf.py
--rw-r--r--   0 runner    (1001) docker     (999)      508 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/nested_serializers/static.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/api/serializers/
--rw-r--r--   0 runner    (1001) docker     (999)      665 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1542 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/serializers/objects.py
--rw-r--r--   0 runner    (1001) docker     (999)     1548 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/serializers/ospf.py
--rw-r--r--   0 runner    (1001) docker     (999)      712 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/serializers/static.py
--rw-r--r--   0 runner    (1001) docker     (999)      702 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/api/views/
--rw-r--r--   0 runner    (1001) docker     (999)      443 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1078 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/views/objects.py
--rw-r--r--   0 runner    (1001) docker     (999)      930 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/views/ospf.py
--rw-r--r--   0 runner    (1001) docker     (999)      388 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/api/views/static.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/choices/
--rw-r--r--   0 runner    (1001) docker     (999)       39 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/choices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      347 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/choices/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     1980 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/choices/bgp.py
--rw-r--r--   0 runner    (1001) docker     (999)      207 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/choices/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/constants/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      885 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/constants/bgp.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/fields/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1236 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/fields/ip.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/filtersets/
--rw-r--r--   0 runner    (1001) docker     (999)      415 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2198 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/filtersets/objects.py
--rw-r--r--   0 runner    (1001) docker     (999)     2896 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/filtersets/ospf.py
--rw-r--r--   0 runner    (1001) docker     (999)     1614 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/filtersets/static.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/forms/
--rw-r--r--   0 runner    (1001) docker     (999)      788 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/forms/bulk_edit/
--rw-r--r--   0 runner    (1001) docker     (999)      217 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/bulk_edit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1008 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/bulk_edit/objects.py
--rw-r--r--   0 runner    (1001) docker     (999)      859 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/bulk_edit/ospf.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/forms/bulk_import/
--rw-r--r--   0 runner    (1001) docker     (999)      101 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/bulk_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1531 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/bulk_import/ospf.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/forms/filtersets/
--rw-r--r--   0 runner    (1001) docker     (999)      543 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      464 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/filtersets/objects.py
--rw-r--r--   0 runner    (1001) docker     (999)     2297 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/filtersets/ospf.py
--rw-r--r--   0 runner    (1001) docker     (999)      599 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/filtersets/static.py
--rw-r--r--   0 runner    (1001) docker     (999)      660 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/objects.py
--rw-r--r--   0 runner    (1001) docker     (999)     2151 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/ospf.py
--rw-r--r--   0 runner    (1001) docker     (999)     1098 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/forms/static.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/helpers/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/migrations/
--rw-r--r--   0 runner    (1001) docker     (999)     5526 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (999)     1388 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/migrations/0002_netboxmodel_updates.py
--rw-r--r--   0 runner    (1001) docker     (999)     2433 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/migrations/0003_model_ordering_and_constraints.py
--rw-r--r--   0 runner    (1001) docker     (999)      616 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/migrations/0004_alter_prefixlistentry_ge_alter_prefixlistentry_le.py
--rw-r--r--   0 runner    (1001) docker     (999)     3997 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/migrations/0005_ospf.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/models/
--rw-r--r--   0 runner    (1001) docker     (999)      330 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)       37 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/models/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     8382 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/models/bgp.py
--rw-r--r--   0 runner    (1001) docker     (999)     5483 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/models/objects.py
--rw-r--r--   0 runner    (1001) docker     (999)     3087 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/models/ospf.py
--rw-r--r--   0 runner    (1001) docker     (999)     1894 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/models/static.py
--rw-r--r--   0 runner    (1001) docker     (999)     3146 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/tables/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1390 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/tables/objects.py
--rw-r--r--   0 runner    (1001) docker     (999)     1299 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/tables/ospf.py
--rw-r--r--   0 runner    (1001) docker     (999)      518 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/tables/static.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/
--rw-r--r--   0 runner    (1001) docker     (999)      557 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/object_children.html
--rw-r--r--   0 runner    (1001) docker     (999)     1820 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/objecttable.html
--rw-r--r--   0 runner    (1001) docker     (999)      601 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/ospfarea.html
--rw-r--r--   0 runner    (1001) docker     (999)     1374 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/ospfinstance.html
--rw-r--r--   0 runner    (1001) docker     (999)     2075 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/ospfinterface.html
--rw-r--r--   0 runner    (1001) docker     (999)      932 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/prefixlist.html
--rw-r--r--   0 runner    (1001) docker     (999)     1704 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/prefixlistentry.html
--rw-r--r--   0 runner    (1001) docker     (999)      932 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/routemap.html
--rw-r--r--   0 runner    (1001) docker     (999)     1282 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/routemapentry.html
--rw-r--r--   0 runner    (1001) docker     (999)     1823 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/staticroute.html
--rw-r--r--   0 runner    (1001) docker     (999)      593 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/staticroute_devices.html
--rw-r--r--   0 runner    (1001) docker     (999)     7073 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing/views/
--rw-r--r--   0 runner    (1001) docker     (999)     1985 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      893 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/views/core.py
--rw-r--r--   0 runner    (1001) docker     (999)     6032 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/views/objects.py
--rw-r--r--   0 runner    (1001) docker     (999)     5269 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/views/ospf.py
--rw-r--r--   0 runner    (1001) docker     (999)     1955 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/netbox_routing/views/static.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      537 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     3310 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)       19 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       15 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/netbox_routing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-24 20:20:22.000000 netbox-routing-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      820 2023-08-24 20:20:17.000000 netbox-routing-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/api/nested_serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/nested_serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/nested_serializers/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/nested_serializers/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/nested_serializers/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/nested_serializers/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/serializers/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/serializers/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/serializers/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/serializers/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/api/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/views/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/views/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/views/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/views/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/choices/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/choices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/choices/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/choices/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/choices/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/constants/bgp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/fields/ip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/filtersets/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/filtersets/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/filtersets/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/filtersets/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/bgp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_edit/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_edit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_edit/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_edit/ospf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_import/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_import/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/forms/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/filtersets/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/filtersets/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/filtersets/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/filtersets/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0002_netboxmodel_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0003_model_ordering_and_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0004_alter_prefixlistentry_ge_alter_prefixlistentry_le.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0005_ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0006_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0007_bgpsessiontemplate_asn_bgpsessiontemplate_bfd_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/models/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/models/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/models/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/models/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/navigation/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/navigation/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/navigation/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/navigation/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/navigation/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/tables/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/tables/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/tables/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/tables/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/bgpaddressfamily.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/bgprouter.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/bgpscope.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/inc/settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/object_children.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/objecttable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/ospfarea.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/ospfinstance.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/ospfinterface.html
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/prefixlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/prefixlistentry.html
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/routemap.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/routemapentry.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/staticroute.html
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/staticroute_devices.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/views/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/views/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/views/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/views/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/views/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/setup.py
```

### Comparing `netbox-routing-0.1.0/LICENSE` & `netbox-routing-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/PKG-INFO` & `netbox-routing-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-routing
-Version: 0.1.0
+Version: 0.1.1
 Summary: NetBox Routing
 Home-page: https://github.com/dansheps/netbox-routing/
 Download-URL: https://pypi.org/project/netbox-routing/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox-routing-0.1.0/netbox_routing/__init__.py` & `netbox-routing-0.1.1/netbox_routing/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from extras.plugins import PluginConfig
+from netbox.plugins import PluginConfig
 from importlib.metadata import metadata
 
 
 plugin = metadata('netbox_routing')
 
 
 class NetboxRouting(PluginConfig):
```

### Comparing `netbox-routing-0.1.0/netbox_routing/api/nested_serializers/objects.py` & `netbox-routing-0.1.1/netbox_routing/api/nested_serializers/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/api/nested_serializers/ospf.py` & `netbox-routing-0.1.1/netbox_routing/api/nested_serializers/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/api/serializers/__init__.py` & `netbox-routing-0.1.1/netbox_routing/api/nested_serializers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,19 @@
-from .static import StaticRouteSerializer
-from .ospf import *
-from .objects import PrefixListSerializer, PrefixListEntrySerializer, RouteMapSerializer, RouteMapEntrySerializer
-from ..nested_serializers import *
+from .static import NestedStaticRouteSerializer
+from .bgp import NestedBGPRouterSerializer, NestedBGPScopeSerializer, NestedBGPAddressFamilySerializer, \
+    NestedBGPSettingSerializer
+from .objects import NestedPrefixListSerializer, NestedPrefixListEntrySerializer, NestedRouteMapSerializer,\
+    NestedRouteMapEntrySerializer
 
 __all__ = (
-    'StaticRouteSerializer',
+    'NestedStaticRouteSerializer',
 
-    'OSPFInstanceSerializer',
-    'OSPFAreaSerializer',
-    'OSPFInterfaceSerializer',
+    'NestedBGPRouterSerializer',
+    'NestedBGPScopeSerializer',
+    'NestedBGPAddressFamilySerializer',
+    'NestedBGPSettingSerializer',
 
-    'PrefixListSerializer',
-    'PrefixListEntrySerializer',
-    'RouteMapSerializer',
-    'RouteMapEntrySerializer',
-
-    # Nested Serializers
     'NestedPrefixListSerializer',
     'NestedPrefixListEntrySerializer',
     'NestedRouteMapSerializer',
     'NestedRouteMapEntrySerializer',
-    'NestedStaticRouteSerializer'
-
 )
```

### Comparing `netbox-routing-0.1.0/netbox_routing/api/serializers/objects.py` & `netbox-routing-0.1.1/netbox_routing/api/serializers/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/api/serializers/ospf.py` & `netbox-routing-0.1.1/netbox_routing/api/serializers/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/api/serializers/static.py` & `netbox-routing-0.1.1/netbox_routing/api/serializers/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/api/urls.py` & `netbox-routing-0.1.1/netbox_routing/api/urls.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from netbox.api.routers import NetBoxRouter
 from .views import StaticRouteViewSet, PrefixListViewSet, RouteMapViewSet, PrefixListEntryViewSet, \
-    RouteMapEntryViewSet, OSPFInstanceViewSet, OSPFAreaViewSet, OSPFInterfaceViewSet
+    RouteMapEntryViewSet, OSPFInstanceViewSet, OSPFAreaViewSet, OSPFInterfaceViewSet, BGPRouterViewSet, \
+    BGPScopeViewSet, BGPAddressFamilyViewSet, BGPSettingViewSet
 
 router = NetBoxRouter()
 router.register('staticroute', StaticRouteViewSet)
+router.register('bgp-router', BGPRouterViewSet)
+router.register('bgp-scope', BGPScopeViewSet)
+router.register('bgp-addressfamily', BGPAddressFamilyViewSet)
+router.register('bgp-setting', BGPSettingViewSet)
 router.register('ospf-instance', OSPFInstanceViewSet)
 router.register('ospf-area', OSPFAreaViewSet)
 router.register('ospf-interface', OSPFInterfaceViewSet)
 router.register('prefix-list', PrefixListViewSet)
 router.register('prefix-list-entry', PrefixListEntryViewSet)
 router.register('route-map', RouteMapViewSet)
 router.register('route-map-entry', RouteMapEntryViewSet)
```

### Comparing `netbox-routing-0.1.0/netbox_routing/api/views/objects.py` & `netbox-routing-0.1.1/netbox_routing/api/views/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/api/views/ospf.py` & `netbox-routing-0.1.1/netbox_routing/api/views/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/constants/bgp.py` & `netbox-routing-0.1.1/netbox_routing/constants/bgp.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,20 @@
 BGPSETTING_ASSIGNMENT_MODELS = Q(
     Q(app_label='netbox_routing', model='bgprouter') |
     Q(app_label='netbox_routing', model='bgpscope')
 )
 
 BGPAF_ASSIGNMENT_MODELS = Q(
     Q(app_label='netbox_routing', model='bgprouter') |
-    Q(app_label='netbox_routing', model='bgpscope') |
-    Q(app_label='netbox_routing', model='bgpneighbor') |
-    Q(app_label='ipam', model='VRF')
+    Q(app_label='netbox_routing', model='bgpscope')
 )
 
 BGPPEER_ASSIGNMENT_MODELS = Q(
     Q(app_label='netbox_routing', model='bgprouter') |
-    Q(app_label='netbox_routing', model='bgpscope') |
-    Q(app_label='netbox_routing', model='bgpaddressfamily')
+    Q(app_label='netbox_routing', model='bgpscope')
 )
 
 BGPPEERAF_ASSIGNMENT_MODELS = Q(
     Q(app_label='netbox_routing', model='bgppeer') |
     Q(app_label='netbox_routing', model='bgppeergroup') |
     Q(app_label='netbox_routing', model='bgptemplatepeer') |
     Q(app_label='netbox_routing', model='bgptemplatepeerpolicy')
```

### Comparing `netbox-routing-0.1.0/netbox_routing/fields/ip.py` & `netbox-routing-0.1.1/netbox_routing/fields/ip.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/filtersets/objects.py` & `netbox-routing-0.1.1/netbox_routing/filtersets/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/filtersets/ospf.py` & `netbox-routing-0.1.1/netbox_routing/filtersets/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/filtersets/static.py` & `netbox-routing-0.1.1/netbox_routing/filtersets/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/forms/__init__.py` & `netbox-routing-0.1.1/netbox_routing/forms/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .filtersets import *
 from .bulk_edit import *
 from .bulk_import import *
 from .objects import PrefixListForm, PrefixListEntryForm, RouteMapForm, RouteMapEntryForm
 from .ospf import OSPFAreaForm, OSPFInstanceForm, OSPFInterfaceForm
+from .bgp import BGPRouterForm, BGPScopeForm, BGPAddressFamilyForm
 from .static import StaticRouteForm
 
 __all__ = (
     # Static Routes
     'StaticRouteForm',
     'StaticRouteFilterForm',
 
@@ -17,14 +18,22 @@
     'OSPFInstanceForm',
     'OSPFInstanceFilterForm',
 
     'OSPFInterfaceForm',
     'OSPFInterfaceFilterForm',
     'OSPFInterfaceBulkEditForm',
 
+    'BGPRouterForm',
+    'BGPScopeForm',
+    'BGPAddressFamilyForm',
+    'BGPRouterFilterForm',
+    'BGPScopeFilterForm',
+    'BGPAddressFamilyFilterForm',
+    'BGPSettingFilterForm',
+
     # Objects
     'PrefixListForm',
     'PrefixListEntryForm',
     'RouteMapForm',
     'RouteMapEntryForm',
     'PrefixListFilterForm',
     'PrefixListEntryFilterForm',
```

### Comparing `netbox-routing-0.1.0/netbox_routing/forms/bulk_edit/objects.py` & `netbox-routing-0.1.1/netbox_routing/forms/bulk_edit/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/forms/bulk_edit/ospf.py` & `netbox-routing-0.1.1/netbox_routing/forms/bulk_edit/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/forms/bulk_import/ospf.py` & `netbox-routing-0.1.1/netbox_routing/forms/bulk_import/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/forms/filtersets/ospf.py` & `netbox-routing-0.1.1/netbox_routing/forms/filtersets/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/forms/filtersets/static.py` & `netbox-routing-0.1.1/netbox_routing/forms/filtersets/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/forms/objects.py` & `netbox-routing-0.1.1/netbox_routing/forms/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/forms/ospf.py` & `netbox-routing-0.1.1/netbox_routing/forms/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/forms/static.py` & `netbox-routing-0.1.1/netbox_routing/forms/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/migrations/0001_initial.py` & `netbox-routing-0.1.1/netbox_routing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/migrations/0002_netboxmodel_updates.py` & `netbox-routing-0.1.1/netbox_routing/migrations/0002_netboxmodel_updates.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/migrations/0003_model_ordering_and_constraints.py` & `netbox-routing-0.1.1/netbox_routing/migrations/0003_model_ordering_and_constraints.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/migrations/0004_alter_prefixlistentry_ge_alter_prefixlistentry_le.py` & `netbox-routing-0.1.1/netbox_routing/migrations/0004_alter_prefixlistentry_ge_alter_prefixlistentry_le.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/migrations/0005_ospf.py` & `netbox-routing-0.1.1/netbox_routing/migrations/0005_ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/models/bgp.py` & `netbox-routing-0.1.1/netbox_routing/models/bgp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from django.contrib.contenttypes.fields import GenericForeignKey
+from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
+from django.utils.translation import gettext as _
 
 from netbox.models import NetBoxModel, NestedGroupModel
 from netbox_routing import choices
+from netbox_routing.choices.bgp import BGPSettingChoices, BGPAddressFamilyChoices, BFDChoices
 from netbox_routing.constants.bgp import BGPSETTING_ASSIGNMENT_MODELS, BGPAF_ASSIGNMENT_MODELS, \
     BGPPEER_ASSIGNMENT_MODELS, BGPPEERAF_ASSIGNMENT_MODELS
 from netbox_routing.fields.ip import IPAddressField
 
 
-class BGPSettings(NetBoxModel):
+class BGPSetting(NetBoxModel):
     assigned_object_type = models.ForeignKey(
         to=ContentType,
         limit_choices_to=BGPSETTING_ASSIGNMENT_MODELS,
         on_delete=models.PROTECT,
         related_name='+',
         blank=True,
         null=True
@@ -22,162 +24,216 @@
         blank=True,
         null=True
     )
     assigned_object = GenericForeignKey(
         ct_field='assigned_object_type',
         fk_field='assigned_object_id'
     )
-    router_id = IPAddressField()
-    auto_summary = models.BooleanField()
-    bgp_additional_paths_install = models.BooleanField()
-    bgp_additional_paths_receive = models.BooleanField()
-    bgp_additional_paths_send = models.BooleanField()
-    bgp_asnotation_dot = models.BooleanField()
-    bgp_graceful_restart = models.BooleanField()
-
-    default_information_originate = models.BooleanField(verbose_name='Default Information Originate')
-    default_metric = models.PositiveBigIntegerField(verbose_name='Default Metric')
-    distance_ebgp = models.PositiveSmallIntegerField(verbose_name='eBGP Distance')
-    distance_ibgp = models.PositiveSmallIntegerField(verbose_name='iBGP Distance')
-    distance_embgp = models.PositiveSmallIntegerField(verbose_name='eBGP Distance (MultiProtocol)')
-    distance_imbgp = models.PositiveSmallIntegerField(verbose_name='iBGP Distance (MultiProtocol)')
-    paths_maximum = models.PositiveSmallIntegerField(verbose_name='Maximum Paths')
-    paths_maximum_secondary = models.PositiveSmallIntegerField(verbose_name='Maximum Secondary Paths')
-    timers_keepalive = models.PositiveSmallIntegerField(verbose_name='Keepalive Timer')
-    timers_hold = models.PositiveSmallIntegerField(verbose_name='Hold Timer')
+    key = models.CharField(
+        choices=BGPSettingChoices,
+    )
+    value = models.CharField()
+
+    class Meta:
+        verbose_name = 'BGP Setting'
+
+    def __str__(self):
+        return f'{self.assigned_object}: {self.key}'
+
+    def get_absolute_url(self):
+        from django.urls import reverse
+        return reverse('plugins:netbox_routing:bgpsetting', args=[self.pk])
 
 
 class BGPRouter(NetBoxModel):
+    device = models.ForeignKey(
+        to='dcim.Device',
+        on_delete=models.PROTECT,
+        related_name='router',
+        verbose_name='Device'
+    )
     asn = models.ForeignKey(
         to='ipam.ASN',
         on_delete=models.PROTECT,
         related_name='router',
         verbose_name='ASN'
     )
+    settings = GenericRelation(
+        to='netbox_routing.BGPSetting',
+        related_name='router',
+        related_query_name='router',
+        content_type_field='assigned_object_type',
+        object_id_field='assigned_object_id'
+    )
+
+    class Meta:
+        verbose_name = 'BGP Router'
+
+    def __str__(self):
+        return f'{self.device} ({self.asn})'
+
+    def get_absolute_url(self):
+        from django.urls import reverse
+        return reverse('plugins:netbox_routing:bgprouter', args=[self.pk])
 
 
 class BGPScope(NetBoxModel):
     router = models.ForeignKey(
         to=BGPRouter,
         on_delete=models.PROTECT,
         related_name='scopes',
         blank=False,
         null=False
     )
     vrf = models.ForeignKey(
         to='ipam.VRF',
         on_delete=models.PROTECT,
         related_name='scopes',
-        blank=False,
-        null=False
+        blank=True,
+        null=True
     )
 
+    settings = GenericRelation(
+        to='netbox_routing.BGPSetting',
+        related_name='scope',
+        related_query_name='scope',
+        content_type_field='assigned_object_type',
+        object_id_field='assigned_object_id'
+    )
+
+    class Meta:
+        verbose_name = 'BGP Scope'
+
+    def __str__(self):
+        return f'{self.router}: {self.vrf or "Global VRF"}'
+
+    def get_absolute_url(self):
+        from django.urls import reverse
+        return reverse('plugins:netbox_routing:bgpscope', args=[self.pk])
+
 
 class BGPAddressFamily(NetBoxModel):
-    assigned_object_type = models.ForeignKey(
-        to=ContentType,
-        limit_choices_to=BGPAF_ASSIGNMENT_MODELS,
+    scope = models.ForeignKey(
+        to=BGPScope,
         on_delete=models.PROTECT,
-        related_name='+',
-        blank=True,
-        null=True
+        related_name='address_families',
+        verbose_name=_('BGP Scope')
     )
-    assigned_object_id = models.PositiveBigIntegerField(
-        blank=True,
-        null=True
+    address_family = models.CharField(
+        max_length=50,
+        choices=BGPAddressFamilyChoices,
+        verbose_name=_('PoE type')
     )
-    assigned_object = GenericForeignKey(
-        ct_field='assigned_object_type',
-        fk_field='assigned_object_id'
+    settings = GenericRelation(
+        to='netbox_routing.BGPSetting',
+        related_name='address_family',
+        related_query_name='address_family',
+        content_type_field='assigned_object_type',
+        object_id_field='assigned_object_id'
     )
 
+    class Meta:
+        verbose_name = 'BGP Address Family'
+
+    def __str__(self):
+        return f'{self.scope} ({self.get_address_family_display()})'
+
+    def get_absolute_url(self):
+        from django.urls import reverse
+        return reverse('plugins:netbox_routing:bgpaddressfamily', args=[self.pk])
 
-class BGPTemplateSession(NetBoxModel):
+
+class BGPSessionTemplate(NetBoxModel):
     name = models.CharField(
         verbose_name='Name',
         max_length=255
     )
     router = models.ForeignKey(
         to=BGPRouter,
         on_delete=models.PROTECT,
         related_name='session_templates',
-        blank=False,
-        null=False
     )
-    enabled = models.BooleanField(
+    parent = models.ForeignKey(
+        to='netbox_routing.BGPSessionTemplate',
+        on_delete=models.PROTECT,
+        related_name='children',
         blank=True,
         null=True
     )
-    prefixlist_out = models.ForeignKey(
-        to='netbox_routing.PrefixList',
-        on_delete=models.PROTECT,
-        related_name='template_afs_out',
+    enabled = models.BooleanField(
         blank=True,
         null=True
     )
-    prefixlist_in = models.ForeignKey(
-        to='netbox_routing.PrefixList',
+    asn = models.ForeignKey(
+        to='ipam.ASN',
         on_delete=models.PROTECT,
-        related_name='template_afs_in',
+        related_name='session_templates',
         blank=True,
         null=True
     )
-    routemap_out = models.ForeignKey(
-        to='netbox_routing.RouteMap',
-        on_delete=models.PROTECT,
-        related_name='template_afs_out',
+    bfd = models.CharField(
+        max_length=50,
+        choices=BFDChoices,
         blank=True,
-        null=True
+        null=True,
     )
-    routemap_in = models.ForeignKey(
-        to='netbox_routing.RouteMap',
-        on_delete=models.PROTECT,
-        related_name='template_afs_in',
+    password = models.CharField(
+        max_length=255,
         blank=True,
-        null=True
+        null=True,
     )
 
 
-class BGPTemplatePolicy(NetBoxModel):
+class BGPPoliyTemplate(NetBoxModel):
     name = models.CharField(
         verbose_name='Name',
         max_length=255
     )
     router = models.ForeignKey(
         to=BGPRouter,
         on_delete=models.PROTECT,
-        related_name='session_templates',
+        related_name='policy_templates',
         blank=False,
         null=False
     )
     enabled = models.BooleanField(
         blank=True,
         null=True
     )
-
-
-class BGPTemplatePeer(NetBoxModel):
-    name = models.CharField(
-        verbose_name='Name',
-        max_length=255
+    prefixlist_out = models.ForeignKey(
+        to='netbox_routing.PrefixList',
+        on_delete=models.PROTECT,
+        related_name='template_afs_out',
+        blank=True,
+        null=True
     )
-    remote_as = models.ForeignKey(
-        to='ipam.ASN',
+    prefixlist_in = models.ForeignKey(
+        to='netbox_routing.PrefixList',
         on_delete=models.PROTECT,
-        related_name='+',
+        related_name='template_afs_in',
         blank=True,
         null=True
     )
-    enabled = models.BooleanField(
+    routemap_out = models.ForeignKey(
+        to='netbox_routing.RouteMap',
+        on_delete=models.PROTECT,
+        related_name='template_afs_out',
+        blank=True,
+        null=True
+    )
+    routemap_in = models.ForeignKey(
+        to='netbox_routing.RouteMap',
+        on_delete=models.PROTECT,
+        related_name='template_afs_in',
         blank=True,
         null=True
     )
 
 
-class BGPPeerGroup(NetBoxModel):
+class BGPPeerTemplate(NetBoxModel):
     name = models.CharField(
         verbose_name='Name',
         max_length=255
     )
     remote_as = models.ForeignKey(
         to='ipam.ASN',
         on_delete=models.PROTECT,
@@ -206,29 +262,22 @@
     )
     assigned_object = GenericForeignKey(
         ct_field='assigned_object_type',
         fk_field='assigned_object_id'
     )
     peer = IPAddressField()
     peer_group = models.ForeignKey(
-        to=BGPPeerGroup,
-        on_delete=models.PROTECT,
-        related_name='peers',
-        blank=True,
-        null=True
-    )
-    peer_template = models.ForeignKey(
-        to=BGPTemplatePeer,
+        to=BGPPeerTemplate,
         on_delete=models.PROTECT,
         related_name='peers',
         blank=True,
         null=True
     )
     peer_policy = models.ForeignKey(
-        to=BGPTemplatePolicy,
+        to=BGPPoliyTemplate,
         on_delete=models.PROTECT,
         related_name='peers',
         blank=True,
         null=True
     )
     remote_as = models.ForeignKey(
         to='ipam.ASN',
@@ -256,26 +305,27 @@
         blank=True,
         null=True
     )
     assigned_object = GenericForeignKey(
         ct_field='assigned_object_type',
         fk_field='assigned_object_id'
     )
+    address_family = models.ForeignKey(
+        to=BGPAddressFamily,
+        on_delete=models.PROTECT,
+        related_name='address_families'
+    )
 
     peer_session = models.ForeignKey(
-        to=BGPTemplateSession,
+        to=BGPSessionTemplate,
         on_delete=models.PROTECT,
         related_name='peer_afs',
         blank=True,
         null=True
     )
-
-    address_family = models.CharField(
-        choices=choices.BGPAddressFamilies
-    )
     enabled = models.BooleanField(
         blank=True,
         null=True
     )
 
     prefixlist_out = models.ForeignKey(
         to='netbox_routing.PrefixList',
```

### Comparing `netbox-routing-0.1.0/netbox_routing/models/objects.py` & `netbox-routing-0.1.1/netbox_routing/models/objects.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.db.models.functions import Lower
+from django.utils.translation import gettext_lazy as _
 from django.urls import reverse
 
 from django.db import models
 from django.db.models import F, Q, CheckConstraint
 from django.core.exceptions import ValidationError
 
 from ipam.fields import IPNetworkField
@@ -52,14 +53,26 @@
         to="netbox_routing.RouteMap",
         on_delete=models.PROTECT,
         related_name='entries',
         verbose_name='Route Map'
     )
     type = models.CharField(max_length=6, choices=PermitDenyChoices)
     sequence = models.PositiveSmallIntegerField()
+    match = models.JSONField(
+        blank=True,
+        null=True,
+        verbose_name=_('Set parameters'),
+        help_text=_("JSON blob of options to match ")
+    )
+    set = models.JSONField(
+        blank=True,
+        null=True,
+        verbose_name=_('Set parameters'),
+        help_text=_("JSON blob of options to set ")
+    )
 
     clone_fields = (
         'route_map', 'type',
     )
     prerequisite_models = (
         'netbox_routing.RouteMap',
     )
```

### Comparing `netbox-routing-0.1.0/netbox_routing/models/ospf.py` & `netbox-routing-0.1.1/netbox_routing/models/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/models/static.py` & `netbox-routing-0.1.1/netbox_routing/models/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/navigation.py` & `netbox-routing-0.1.1/netbox_routing/navigation/ospf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,16 @@
-from extras.plugins import PluginMenuButton, PluginMenuItem, PluginMenu
-from utilities.choices import ButtonColorChoices
+from netbox.choices import ButtonColorChoices
+from netbox.plugins import PluginMenuItem, PluginMenuButton
 
-static = PluginMenuItem(
-    link='plugins:netbox_routing:staticroute_list',
-    link_text='Static Route',
-    permissions=['netbox_routing.view_staticroute'],
-    buttons=(
-        PluginMenuButton('plugins:netbox_routing:staticroute_add', 'Add', 'mdi mdi-plus', ButtonColorChoices.GREEN),
-        PluginMenuButton(
-            'plugins:netbox_routing:staticroute_import',
-            'Import',
-            'mdi mdi-upload',
-            ButtonColorChoices.CYAN
-        ),
-    )
+
+__all__ = (
+    'MENUITEMS',
 )
 
+
 ospf_instance = PluginMenuItem(
     link='plugins:netbox_routing:ospfinstance_list',
     link_text='Instances',
     permissions=['netbox_routing.view_ospfinstance'],
     buttons=(
         PluginMenuButton('plugins:netbox_routing:ospfinstance_add', 'Add', 'mdi mdi-plus', ButtonColorChoices.GREEN),
         PluginMenuButton(
@@ -55,35 +46,8 @@
             'Import',
             'mdi mdi-upload',
             ButtonColorChoices.CYAN
         ),
     )
 )
 
-prefixlist = PluginMenuItem(
-    link='plugins:netbox_routing:prefixlist_list',
-    link_text='Prefix Lists',
-    permissions=['netbox_routing.view_prefixlist'],
-    buttons=(
-        PluginMenuButton('plugins:netbox_routing:prefixlist_add', 'Add', 'mdi mdi-plus', ButtonColorChoices.GREEN),
-        PluginMenuButton('plugins:netbox_routing:prefixlist_import', 'Import', 'mdi mdi-upload', ButtonColorChoices.CYAN),
-    )
-)
-routemap = PluginMenuItem(
-    link='plugins:netbox_routing:routemap_list',
-    link_text='Route Maps',
-    permissions=['netbox_routing.view_routemap'],
-    buttons=(
-        PluginMenuButton('plugins:netbox_routing:routemap_add', 'Add', 'mdi mdi-plus', ButtonColorChoices.GREEN),
-        PluginMenuButton('plugins:netbox_routing:routemap_import', 'Import', 'mdi mdi-upload', ButtonColorChoices.CYAN),
-    )
-)
-
-menu = PluginMenu(
-    label='Netbox Routing',
-    groups=(
-        ('Routing Objects', (prefixlist, routemap)),
-        ('Static Routing', (static,)),
-        ('OSPF', (ospf_instance, ospf_area, ospf_interfaces)),
-    ),
-    icon_class='mdi mdi-router'
-)
+MENUITEMS = (ospf_instance, ospf_area, ospf_interfaces)
```

### Comparing `netbox-routing-0.1.0/netbox_routing/tables/objects.py` & `netbox-routing-0.1.1/netbox_routing/tables/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/tables/ospf.py` & `netbox-routing-0.1.1/netbox_routing/tables/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/object_children.html` & `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/object_children.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/objecttable.html` & `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/objecttable.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/ospfarea.html` & `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/ospfarea.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/ospfinstance.html` & `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/ospfinstance.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/ospfinterface.html` & `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/ospfinterface.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/prefixlist.html` & `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/prefixlist.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/prefixlistentry.html` & `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/prefixlistentry.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/routemap.html` & `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/routemap.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/routemapentry.html` & `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/routemapentry.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/staticroute.html` & `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/staticroute.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/templates/netbox_routing/staticroute_devices.html` & `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/staticroute_devices.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/urls.py` & `netbox-routing-0.1.1/netbox_routing/urls.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.urls import path
 
 from netbox.views.generic import ObjectChangeLogView
 
 from . import views
 from .models import StaticRoute, PrefixList, PrefixListEntry, RouteMap, RouteMapEntry, OSPFInstance, OSPFArea, \
-    OSPFInterface
+    OSPFInterface, BGPRouter, BGPScope, BGPAddressFamily
 
 urlpatterns = [
     path('routes/static/', views.StaticRouteListView.as_view(), name='staticroute_list'),
     path('routes/static/add/', views.StaticRouteEditView.as_view(), name='staticroute_add'),
     path('routes/static/import/', views.StaticRouteListView.as_view(), name='staticroute_import'),
     path('routes/static/<int:pk>/', views.StaticRouteView.as_view(), name='staticroute'),
     path('routes/static/<int:pk>/edit/', views.StaticRouteEditView.as_view(), name='staticroute_edit'),
@@ -38,22 +38,43 @@
     path('ospf/interface/add/', views.OSPFInterfaceEditView.as_view(), name='ospfinterface_add'),
     path('ospf/interface/import/', views.OSPFInterfaceListView.as_view(), name='ospfinterface_import'),
     path('ospf/interface/<int:pk>/', views.OSPFInterfaceView.as_view(), name='ospfinterface'),
     path('ospf/interface/<int:pk>/edit/', views.OSPFInterfaceEditView.as_view(), name='ospfinterface_edit'),
     path('ospf/interface/<int:pk>/delete/', views.OSPFInterfaceDeleteView.as_view(), name='ospfinterface_delete'),
     path('ospf/interface/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='ospfinterface_changelog', kwargs={'model': OSPFInterface}),
 
+    path('bgp/router/', views.BGPRouterListView.as_view(), name='bgprouter_list'),
+    path('bgp/router/add/', views.BGPRouterEditView.as_view(), name='bgprouter_add'),
+    path('bgp/router/<int:pk>/', views.BGPRouterView.as_view(), name='bgprouter'),
+    path('bgp/router/<int:pk>/edit', views.BGPRouterEditView.as_view(), name='bgprouter_edit'),
+    path('bgp/router/<int:pk>/delete', views.BGPRouterEditView.as_view(), name='bgprouter_delete'),
+    path('bgp/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='bgprouter_changelog', kwargs={'model': BGPRouter}),
+
+    path('bgp/scope/', views.BGPScopeListView.as_view(), name='bgpscope_list'),
+    path('bgp/scope/add/', views.BGPScopeEditView.as_view(), name='bgpscope_add'),
+    path('bgp/scope/<int:pk>/', views.BGPScopeView.as_view(), name='bgpscope'),
+    path('bgp/scope/<int:pk>/edit', views.BGPScopeEditView.as_view(), name='bgpscope_edit'),
+    path('bgp/scope/<int:pk>/delete', views.BGPScopeEditView.as_view(), name='bgpscope_delete'),
+    path('bgp/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='bgpscope_changelog', kwargs={'model': BGPScope}),
+
+    path('bgp/address_family/', views.BGPAddressFamilyListView.as_view(), name='bgpaddressfamily_list'),
+    path('bgp/address_family/add/', views.BGPAddressFamilyEditView.as_view(), name='bgpaddressfamily_add'),
+    path('bgp/address_family/<int:pk>/', views.BGPAddressFamilyView.as_view(), name='bgpaddressfamily'),
+    path('bgp/address_family/<int:pk>/edit', views.BGPAddressFamilyEditView.as_view(), name='bgpaddressfamily_edit'),
+    path('bgp/address_family/<int:pk>/delete', views.BGPAddressFamilyEditView.as_view(), name='bgpaddressfamily_delete'),
+    path('bgp/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='bgpaddressfamily_changelog', kwargs={'model': BGPAddressFamily}),
+
     path('prefix-list/', views.PrefixListListView.as_view(), name='prefixlist_list'),
     path('prefix-list/add/', views.PrefixListEditView.as_view(), name='prefixlist_add'),
     path('prefix-list/import/', views.PrefixListListView.as_view(), name='prefixlist_import'),
     path('prefix-list/<int:pk>/', views.PrefixListView.as_view(), name='prefixlist'),
-    path('prefix-list/<int:pk>/edit/', views.PrefixListView.as_view(), name='prefixlist_edit'),
+    path('prefix-list/<int:pk>/edit/', views.PrefixListEditView.as_view(), name='prefixlist_edit'),
     path('prefix-list/<int:pk>/entries/', views.PrefixListEntriesView.as_view(), name='prefixlist_entries'),
     path('prefix-list/<int:pk>/delete/', views.PrefixListView.as_view(), name='prefixlist_delete'),
-    path('prefix-list/<int:pk>/changelog/', views.PrefixListView.as_view(), name='prefixlist_changelog', kwargs={'model': PrefixList}),
+    path('prefix-list/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='prefixlist_changelog', kwargs={'model': PrefixList}),
 
     path('prefix-list-entry/', views.PrefixListEntryListView.as_view(), name='prefixlistentry_list'),
     path('prefix-list-entry/add/', views.PrefixListEntryEditView.as_view(), name='prefixlistentry_add'),
     path('prefix-list-entry/edit/', views.PrefixListEntryBulkEditView.as_view(), name='prefixlistentry_bulk_edit'),
     path('prefix-list-entry/delete/', views.PrefixListEntryBulkDeleteView.as_view(), name='prefixlistentry_bulk_delete'),
     path('prefix-list-entry/import/', views.PrefixListEntryListView.as_view(), name='prefixlistentry_import'),
     path('prefix-list-entry/<int:pk>/', views.PrefixListEntryView.as_view(), name='prefixlistentry'),
@@ -62,17 +83,17 @@
     path('prefix-list-entry/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='prefixlistentry_changelog', kwargs={'model': PrefixListEntry}),
 
     path('route-map/', views.RouteMapListView.as_view(), name='routemap_list'),
     path('route-map/add/', views.RouteMapEditView.as_view(), name='routemap_add'),
     path('route-map/import/', views.RouteMapListView.as_view(), name='routemap_import'),
     path('route-map/<int:pk>/', views.RouteMapView.as_view(), name='routemap'),
     path('route-map/<int:pk>/entries/', views.RouteMapEntriesView.as_view(), name='routemap_entries'),
-    path('route-map/<int:pk>/edit/', views.RouteMapView.as_view(), name='routemap_edit'),
+    path('route-map/<int:pk>/edit/', views.RouteMapEditView.as_view(), name='routemap_edit'),
     path('route-map/<int:pk>/delete/', views.RouteMapView.as_view(), name='routemap_delete'),
-    path('route-map/<int:pk>/changelog/', views.RouteMapView.as_view(), name='routemap_changelog', kwargs={'model': RouteMap}),
+    path('route-map/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='routemap_changelog', kwargs={'model': RouteMap}),
 
     path('route-map-entry/', views.RouteMapEntryListView.as_view(), name='routemapentry_list'),
     path('route-map-entry/add/', views.RouteMapEntryEditView.as_view(), name='routemapentry_add'),
     path('route-map-entry/edit/', views.RouteMapEntryBulkEditView.as_view(), name='routemapentry_bulk_edit'),
     path('route-map-entry/delete/', views.RouteMapEntryBulkDeleteView.as_view(), name='routemapentry_bulk_delete'),
     path('route-map-entry/import/', views.RouteMapEntryListView.as_view(), name='routemapentry_import'),
     path('route-map-entry/<int:pk>/', views.RouteMapEntryView.as_view(), name='routemapentry'),
```

### Comparing `netbox-routing-0.1.0/netbox_routing/views/__init__.py` & `netbox-routing-0.1.1/netbox_routing/views/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .objects import PrefixListView, PrefixListEditView, PrefixListListView, PrefixListDeleteView, RouteMapListView, \
     RouteMapView, RouteMapEditView, RouteMapDeleteView, PrefixListEntryListView, PrefixListEntryEditView, \
     PrefixListEntryDeleteView, PrefixListEntryView, RouteMapEntryListView, RouteMapEntryView, RouteMapEntryEditView, \
     RouteMapEntryDeleteView, PrefixListEntriesView, RouteMapEntriesView, RouteMapEntryBulkEditView, \
     RouteMapEntryBulkDeleteView, PrefixListEntryBulkDeleteView, PrefixListEntryBulkEditView
 
 from .ospf import *
+from .bgp import *
 from .core import *
 
 __all__ = (
     # Core View Extensions
     'DeviceStaticRoutesView',
 
     # Static
@@ -35,14 +36,16 @@
     'OSPFAreaDeleteView',
 
     'OSPFInterfaceListView',
     'OSPFInterfaceView',
     'OSPFInterfaceEditView',
     'OSPFInterfaceDeleteView',
 
+    'BGPRouterView',
+    'BGPRouterEditView',
 
     # Routing Objects
     'PrefixListListView',
     'PrefixListView',
     'PrefixListEntriesView',
     'PrefixListEditView',
     'PrefixListDeleteView',
```

### Comparing `netbox-routing-0.1.0/netbox_routing/views/core.py` & `netbox-routing-0.1.1/netbox_routing/views/core.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/views/objects.py` & `netbox-routing-0.1.1/netbox_routing/views/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/views/ospf.py` & `netbox-routing-0.1.1/netbox_routing/views/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.0/netbox_routing/views/static.py` & `netbox-routing-0.1.1/netbox_routing/views/static.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,8 +55,8 @@
 class StaticRouteEditView(ObjectEditView):
     queryset = StaticRoute.objects.all()
     form = StaticRouteForm
 
 
 @register_model_view(StaticRoute, name='delete')
 class StaticRouteDeleteView(ObjectDeleteView):
-    pass
+    queryset = StaticRoute.objects.all()
```

### Comparing `netbox-routing-0.1.0/netbox_routing.egg-info/PKG-INFO` & `netbox-routing-0.1.1/netbox_routing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-routing
-Version: 0.1.0
+Version: 0.1.1
 Summary: NetBox Routing
 Home-page: https://github.com/dansheps/netbox-routing/
 Download-URL: https://pypi.org/project/netbox-routing/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox-routing-0.1.0/netbox_routing.egg-info/SOURCES.txt` & `netbox-routing-0.1.1/netbox_routing.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,104 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 netbox_routing/__init__.py
-netbox_routing/navigation.py
 netbox_routing/urls.py
 netbox_routing.egg-info/PKG-INFO
 netbox_routing.egg-info/SOURCES.txt
 netbox_routing.egg-info/dependency_links.txt
 netbox_routing.egg-info/not-zip-safe
 netbox_routing.egg-info/requires.txt
 netbox_routing.egg-info/top_level.txt
 netbox_routing/api/__init__.py
 netbox_routing/api/urls.py
 netbox_routing/api/nested_serializers/__init__.py
+netbox_routing/api/nested_serializers/bgp.py
 netbox_routing/api/nested_serializers/objects.py
 netbox_routing/api/nested_serializers/ospf.py
 netbox_routing/api/nested_serializers/static.py
 netbox_routing/api/serializers/__init__.py
+netbox_routing/api/serializers/bgp.py
 netbox_routing/api/serializers/objects.py
 netbox_routing/api/serializers/ospf.py
 netbox_routing/api/serializers/static.py
 netbox_routing/api/views/__init__.py
+netbox_routing/api/views/bgp.py
 netbox_routing/api/views/objects.py
 netbox_routing/api/views/ospf.py
 netbox_routing/api/views/static.py
 netbox_routing/choices/__init__.py
 netbox_routing/choices/base.py
 netbox_routing/choices/bgp.py
 netbox_routing/choices/objects.py
 netbox_routing/constants/__init__.py
 netbox_routing/constants/bgp.py
 netbox_routing/fields/__init__.py
 netbox_routing/fields/ip.py
 netbox_routing/filtersets/__init__.py
+netbox_routing/filtersets/bgp.py
 netbox_routing/filtersets/objects.py
 netbox_routing/filtersets/ospf.py
 netbox_routing/filtersets/static.py
 netbox_routing/forms/__init__.py
+netbox_routing/forms/bgp.py
 netbox_routing/forms/fields.py
 netbox_routing/forms/objects.py
 netbox_routing/forms/ospf.py
 netbox_routing/forms/static.py
 netbox_routing/forms/bulk_edit/__init__.py
 netbox_routing/forms/bulk_edit/objects.py
 netbox_routing/forms/bulk_edit/ospf.py
 netbox_routing/forms/bulk_import/__init__.py
 netbox_routing/forms/bulk_import/ospf.py
 netbox_routing/forms/filtersets/__init__.py
+netbox_routing/forms/filtersets/bgp.py
 netbox_routing/forms/filtersets/objects.py
 netbox_routing/forms/filtersets/ospf.py
 netbox_routing/forms/filtersets/static.py
 netbox_routing/helpers/__init__.py
 netbox_routing/migrations/0001_initial.py
 netbox_routing/migrations/0002_netboxmodel_updates.py
 netbox_routing/migrations/0003_model_ordering_and_constraints.py
 netbox_routing/migrations/0004_alter_prefixlistentry_ge_alter_prefixlistentry_le.py
 netbox_routing/migrations/0005_ospf.py
+netbox_routing/migrations/0006_bgp.py
+netbox_routing/migrations/0007_bgpsessiontemplate_asn_bgpsessiontemplate_bfd_and_more.py
 netbox_routing/migrations/__init__.py
 netbox_routing/models/__init__.py
 netbox_routing/models/base.py
 netbox_routing/models/bgp.py
 netbox_routing/models/objects.py
 netbox_routing/models/ospf.py
 netbox_routing/models/static.py
+netbox_routing/navigation/__init__.py
+netbox_routing/navigation/bgp.py
+netbox_routing/navigation/objects.py
+netbox_routing/navigation/ospf.py
+netbox_routing/navigation/static.py
 netbox_routing/tables/__init__.py
+netbox_routing/tables/bgp.py
 netbox_routing/tables/objects.py
 netbox_routing/tables/ospf.py
 netbox_routing/tables/static.py
+netbox_routing/templates/netbox_routing/bgpaddressfamily.html
+netbox_routing/templates/netbox_routing/bgprouter.html
+netbox_routing/templates/netbox_routing/bgpscope.html
 netbox_routing/templates/netbox_routing/object_children.html
 netbox_routing/templates/netbox_routing/objecttable.html
 netbox_routing/templates/netbox_routing/ospfarea.html
 netbox_routing/templates/netbox_routing/ospfinstance.html
 netbox_routing/templates/netbox_routing/ospfinterface.html
 netbox_routing/templates/netbox_routing/prefixlist.html
 netbox_routing/templates/netbox_routing/prefixlistentry.html
 netbox_routing/templates/netbox_routing/routemap.html
 netbox_routing/templates/netbox_routing/routemapentry.html
 netbox_routing/templates/netbox_routing/staticroute.html
 netbox_routing/templates/netbox_routing/staticroute_devices.html
+netbox_routing/templates/netbox_routing/inc/settings.html
 netbox_routing/views/__init__.py
+netbox_routing/views/bgp.py
 netbox_routing/views/core.py
 netbox_routing/views/objects.py
 netbox_routing/views/ospf.py
 netbox_routing/views/static.py
```

### Comparing `netbox-routing-0.1.0/setup.py` & `netbox-routing-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox-routing',
-    version='0.1.0',
+    version='0.1.1',
     description='NetBox Routing',
     long_description='Plugin for documentation of routing configuration and objects',
     url='https://github.com/dansheps/netbox-routing/',
     download_url='https://pypi.org/project/netbox-routing/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     maintainer='Daniel Sheppard',
```

