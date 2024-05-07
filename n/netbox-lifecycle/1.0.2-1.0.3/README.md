# Comparing `tmp/netbox-lifecycle-1.0.2.tar.gz` & `tmp/netbox_lifecycle-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-lifecycle-1.0.2.tar", last modified: Wed Mar 20 01:55:06 2024, max compression
+gzip compressed data, was "netbox_lifecycle-1.0.3.tar", last modified: Tue May  7 18:55:08 2024, max compression
```

## Comparing `netbox-lifecycle-1.0.2.tar` & `netbox_lifecycle-1.0.3.tar`

### file list

```diff
@@ -1,88 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.946021 netbox-lifecycle-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-20 01:55:06.946021 netbox-lifecycle-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.934021 netbox-lifecycle-1.0.2/netbox_lifecycle/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.934021 netbox-lifecycle-1.0.2/netbox_lifecycle/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.938021 netbox-lifecycle-1.0.2/netbox_lifecycle/api/nested_serializers/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/nested_serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/nested_serializers/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/nested_serializers/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/nested_serializers/license.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.938021 netbox-lifecycle-1.0.2/netbox_lifecycle/api/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/serializers/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/serializers/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/serializers/license.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.938021 netbox-lifecycle-1.0.2/netbox_lifecycle/api/views/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/views/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/views/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/api/views/license.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.938021 netbox-lifecycle-1.0.2/netbox_lifecycle/filtersets/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/filtersets/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/filtersets/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/filtersets/license.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.938021 netbox-lifecycle-1.0.2/netbox_lifecycle/forms/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/forms/bulk_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/forms/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/forms/model_forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.942021 netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0002_license_licenseassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0003_remove_supportcontract_devices_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0004_supportcontractassignment_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0005_remove_supportcontract_manufacturer_supportsku_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0006_alter_supportcontractassignment_assigned_object_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0007_alter_hardwarelifecycle_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0008_alter_supportcontractassignment_contract_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0009_alter_licenseassignment_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0010_licenseassignment_quantity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0011_alter_supportcontractassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.942021 netbox-lifecycle-1.0.2/netbox_lifecycle/models/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/models/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/models/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/models/license.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/models/netbox_polymprohic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.942021 netbox-lifecycle-1.0.2/netbox_lifecycle/tables/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/tables/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/tables/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/tables/license.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.934021 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.946021 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.946021 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/generic/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/generic/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle.html
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.946021 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/license/
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/license/assignments.html
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/license.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.946021 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/assignments.html
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/supportcontract.html
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/supportcontractassignment_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/supportsku.html
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/vendor.html
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.946021 netbox-lifecycle-1.0.2/netbox_lifecycle/views/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/views/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/views/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/netbox_lifecycle/views/license.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:55:06.946021 netbox-lifecycle-1.0.2/netbox_lifecycle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-20 01:55:06.000000 netbox-lifecycle-1.0.2/netbox_lifecycle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-03-20 01:55:06.000000 netbox-lifecycle-1.0.2/netbox_lifecycle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 01:55:06.000000 netbox-lifecycle-1.0.2/netbox_lifecycle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 01:55:06.000000 netbox-lifecycle-1.0.2/netbox_lifecycle.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-20 01:55:06.000000 netbox-lifecycle-1.0.2/netbox_lifecycle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 01:55:06.946021 netbox-lifecycle-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-20 01:55:02.000000 netbox-lifecycle-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.124794 netbox_lifecycle-1.0.3/netbox_lifecycle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.124794 netbox_lifecycle-1.0.3/netbox_lifecycle/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.128794 netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/license.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.128794 netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.128794 netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/license.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.128794 netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/license.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.128794 netbox_lifecycle-1.0.3/netbox_lifecycle/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/forms/bulk_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/forms/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/forms/model_forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.132794 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0002_license_licenseassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0003_remove_supportcontract_devices_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0004_supportcontractassignment_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0005_remove_supportcontract_manufacturer_supportsku_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0006_alter_supportcontractassignment_assigned_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0007_alter_hardwarelifecycle_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0008_alter_supportcontractassignment_contract_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0009_alter_licenseassignment_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0010_licenseassignment_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0011_alter_supportcontractassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.132794 netbox_lifecycle-1.0.3/netbox_lifecycle/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/models/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/models/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/models/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/models/netbox_polymprohic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.132794 netbox_lifecycle-1.0.3/netbox_lifecycle/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/tables/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/tables/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/tables/license.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.124794 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/generic/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/license/
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/license/assignments.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/license.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/assignments.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontract.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontractassignment_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportsku.html
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/vendor.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/views/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/views/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/views/license.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-07 18:55:08.000000 netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-07 18:55:08.000000 netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:55:08.000000 netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:55:08.000000 netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 18:55:08.000000 netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/setup.py
```

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/__init__.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from extras.plugins import PluginConfig
 from importlib.metadata import metadata
 
+from netbox.plugins import PluginConfig
+
 metadata = metadata('netbox_lifecycle')
 
 
 class NetBoxLifeCycle(PluginConfig):
     name = metadata.get('Name').replace('-', '_')
     verbose_name = metadata.get('Summary')
     description = metadata.get('Description')
     version = metadata.get('Version')
     author = metadata.get('Author')
     author_email = metadata.get('Author-email')
     base_url = 'lifecycle'
     min_version = '3.5.0'
-    max_version = '3.7.99'
+    max_version = '4.0.99'
     required_settings = []
     default_settings = {}
     queues = []
 
     def ready(self):
 
         super().ready()
```

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/api/nested_serializers/contract.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/contract.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/api/nested_serializers/hardware.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/hardware.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/api/nested_serializers/license.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/license.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/api/serializers/contract.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/contract.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/api/serializers/hardware.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/hardware.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/api/serializers/license.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/license.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/api/views/contract.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/contract.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 class SupportContractViewSet(ModelViewSet):
     queryset = SupportContract.objects.all()
     serializer_class = SupportContractSerializer
 
 
 class SupportContractAssignmentViewSet(ModelViewSet):
     queryset = SupportContractAssignment.objects.all()
-    serializer_class = SupportContractAssignmentSerializer
+    serializer_class = SupportContractAssignmentSerializer
```

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/api/views/license.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/license.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/filtersets/contract.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/contract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import django_filters
-from django.contrib.contenttypes.models import ContentType
 from django.db.models import Q
 from django.utils.translation import gettext as _
 
 from dcim.models import Manufacturer, Device
 from netbox.filtersets import NetBoxModelFilterSet
 from netbox_lifecycle.models import Vendor, SupportContract, SupportContractAssignment, SupportSKU, LicenseAssignment, \
     License
@@ -11,16 +10,14 @@
 __all__ = (
     'SupportContractFilterSet',
     'SupportSKUFilterSet',
     'VendorFilterSet',
     'SupportContractAssignmentFilterSet'
 )
 
-from utilities.filters import MultiValueCharFilter, MultiValueNumberFilter
-
 
 class VendorFilterSet(NetBoxModelFilterSet):
 
     class Meta:
         model = Vendor
         fields = ('id', 'q', )
 
@@ -56,15 +53,14 @@
         qs_filter = (
             Q(sku__icontains=value) |
             Q(manufacturer__name__icontains=value)
         )
         return queryset.filter(qs_filter).distinct()
 
 
-
 class SupportContractFilterSet(NetBoxModelFilterSet):
     vendor_id = django_filters.ModelMultipleChoiceFilter(
         field_name='vendor',
         queryset=Vendor.objects.all(),
         label=_('Vendor'),
     )
```

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/filtersets/hardware.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/hardware.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from netbox_lifecycle.models import HardwareLifecycle
 
 
 __all__ = (
     'HardwareLifecycleFilterSet',
 )
 
-from utilities.filters import MultiValueCharFilter, MultiValueNumberFilter
-
 
 class HardwareLifecycleFilterSet(NetBoxModelFilterSet):
     assigned_object_type_id = django_filters.ModelMultipleChoiceFilter(
         queryset=ContentType.objects.all()
     )
     device_type = django_filters.ModelMultipleChoiceFilter(
         field_name='device_type__model',
```

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/filtersets/license.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/license.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/forms/bulk_edit.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/forms/bulk_edit.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/forms/filtersets.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/forms/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/forms/model_forms.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/forms/model_forms.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0001_initial.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0002_license_licenseassignment.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0002_license_licenseassignment.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0003_remove_supportcontract_devices_and_more.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0003_remove_supportcontract_devices_and_more.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Generated by Django 4.1.7 on 2023-05-11 01:35
 
 from django.db import migrations, models
 import django.db.models.deletion
 import taggit.managers
 import utilities.json
 
+
 def migrate_to_assignments(apps, schema_editor):
     SupportContractDeviceAssignment = apps.get_model('netbox_lifecycle', 'SupportContractDeviceAssignment')
     SupportContract = apps.get_model('netbox_lifecycle', 'SupportContract')
 
     for contract in SupportContract.objects.all():
         for device in contract.devices.all():
             SupportContractDeviceAssignment.objects.create(contract=contract, device=device)
 
+
 def migrate_from_assignments(apps, schema_editor):
     SupportContractDeviceAssignment = apps.get_model('netbox_lifecycle', 'SupportContractDeviceAssignment')
 
     for contract in SupportContractDeviceAssignment.objects.all():
         contract.contract.devices.add(contract.device)
```

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0004_supportcontractassignment_and_more.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0004_supportcontractassignment_and_more.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 4.1.7 on 2023-05-11 13:12
 from django.db import migrations, models
 import django.db.models.deletion
 import taggit.managers
 import utilities.json
 
+
 def migrate_to_assignments(apps, schema_editor):
     from django.contrib.contenttypes.models import ContentType
     SupportContractDeviceAssignment = apps.get_model('netbox_lifecycle', 'SupportContractDeviceAssignment')
     SupportContractAssignment = apps.get_model('netbox_lifecycle', 'SupportContractAssignment')
     Device = apps.get_model('dcim', 'Device')
     assigned_object_type = ContentType.objects.get_for_model(Device)
 
@@ -18,14 +19,15 @@
             last_updated=contract.last_updated,
             custom_field_data=contract.custom_field_data,
             assigned_object_type_id=assigned_object_type.pk,
             assigned_object_id=contract.device.pk,
             contract=contract.contract,
         )
 
+
 def migrate_from_assignments(apps, schema_editor):
     SupportContractDeviceAssignment = apps.get_model('netbox_lifecycle', 'SupportContractDeviceAssignment')
     SupportContractAssignment = apps.get_model('netbox_lifecycle', 'SupportContractAssignment')
     Device = apps.get_model('dcim', 'Device')
     for contract in SupportContractAssignment.objects.all():
         if isinstance(contract.assigned_object, Device):
             assignment = SupportContractDeviceAssignment.objects.create(
```

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0005_remove_supportcontract_manufacturer_supportsku_and_more.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0005_remove_supportcontract_manufacturer_supportsku_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0006_alter_supportcontractassignment_assigned_object_type.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0006_alter_supportcontractassignment_assigned_object_type.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0007_alter_hardwarelifecycle_options_and_more.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0007_alter_hardwarelifecycle_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0008_alter_supportcontractassignment_contract_and_more.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0008_alter_supportcontractassignment_contract_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0009_alter_licenseassignment_device.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0009_alter_licenseassignment_device.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/migrations/0011_alter_supportcontractassignment.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0011_alter_supportcontractassignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
             assignment.save()
         else:
             license_assignment = LicenseAssignment.objects.get(pk=assignment.assigned_object_id)
             assignment.device = license_assignment.device
             assignment.license = license_assignment
             assignment.save()
 
+
 def migrate_assigned_object_reverse(apps, schema_editor):
     SupportContractAssignment = apps.get_model('netbox_lifecycle', 'SupportContractAssignment')
     ContentType = apps.get_model('contenttypes', 'ContentType')
 
     device_type = ContentType.objects.get(app_label='dcim', model='device')
     license_type = ContentType.objects.get(app_label='netbox_lifecycle', model='licenseassignment')
```

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/models/contract.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/models/contract.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
+from django.core.exceptions import ValidationError
 from django.db import models
 from django.db.models import Q
 from django.db.models.functions import Lower
 from django.urls import reverse
 from django.utils.translation import gettext as _
 
 from dcim.choices import DeviceStatusChoices
@@ -68,14 +69,15 @@
 
     def __str__(self):
         return f'{self.sku}'
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_lifecycle:supportsku', args=[self.pk])
 
+
 class SupportContract(NetBoxModel):
     vendor = models.ForeignKey(
         to='netbox_lifecycle.Vendor',
         on_delete=models.SET_NULL,
         related_name='contracts',
         null=True,
         blank=True,
@@ -173,7 +175,21 @@
             return self.end
         return self.contract.end
 
     def get_device_status_color(self):
         if self.device is None:
             return
         return DeviceStatusChoices.colors.get(self.device.status)
+
+    def clean(self):
+        if self.device and self.license and SupportContractAssignment.objects.filter(
+                contract=self.contract, device=self.device, license=self.license, sku=self.sku
+        ).exclude(pk=self.pk).count() > 0:
+            raise ValidationError('Device or License must be unique')
+        elif self.device and not self.license and SupportContractAssignment.objects.filter(
+                contract=self.contract, device=self.device, license=self.license
+        ).exclude(pk=self.pk).count() > 0:
+            raise ValidationError('Device must be unique')
+        elif not self.device and self.license and SupportContractAssignment.objects.filter(
+                contract=self.contract, device=self.device, license=self.license
+        ).exclude(pk=self.pk).count() > 0:
+            raise ValidationError('License must be unique')
```

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/models/hardware.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/models/hardware.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/models/license.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/models/license.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/navigation.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/navigation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from extras.plugins import PluginMenu, PluginMenuButton, PluginMenuItem
-from utilities.choices import ButtonColorChoices
+from netbox.plugins import PluginMenuItem, PluginMenu
 
 lifecycle = PluginMenuItem(
     link='plugins:netbox_lifecycle:hardwarelifecycle_list',
     link_text='Hardware Lifecycle',
     permissions=['netbox_lifecycle.view_hardwarelifecycle'],
 )
```

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/tables/contract.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/tables/contract.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/tables/hardware.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/tables/hardware.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/tables/license.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/tables/license.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle.html` & `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle.html`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle_edit.html` & `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/license/assignments.html` & `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/license/assignments.html`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/license.html` & `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/license.html`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/assignments.html` & `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/assignments.html`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/supportcontract.html` & `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontract.html`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/supportcontractassignment_edit.html` & `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontractassignment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/supportsku.html` & `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportsku.html`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/templates/netbox_lifecycle/vendor.html` & `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/vendor.html`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/urls.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/views/contract.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/views/contract.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/views/hardware.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/views/hardware.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 __all__ = (
     'HardwareLifecycleListView',
     'HardwareLifecycleView',
     'HardwareLifecycleEditView',
     'HardwareLifecycleDeleteView',
 )
 
+
 @register_model_view(HardwareLifecycle, name='list')
 class HardwareLifecycleListView(ObjectListView):
     queryset = HardwareLifecycle.objects.all()
     table = HardwareLifecycleTable
     filterset = HardwareLifecycleFilterSet
     filterset_form = HardwareLifecycleFilterForm
 
@@ -28,21 +29,17 @@
 
     def get_extra_context(self, request, instance):
 
         return {
         }
 
 
-
 @register_model_view(HardwareLifecycle, 'edit')
 class HardwareLifecycleEditView(ObjectEditView):
     template_name = 'netbox_lifecycle/hardwarelifecycle_edit.html'
     queryset = HardwareLifecycle.objects.all()
     form = HardwareLifecycleForm
 
 
-
-
 @register_model_view(HardwareLifecycle, 'delete')
 class HardwareLifecycleDeleteView(ObjectDeleteView):
     queryset = HardwareLifecycle.objects.all()
-
```

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle/views/license.py` & `netbox_lifecycle-1.0.3/netbox_lifecycle/views/license.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     'LicenseAssignmentListView',
     'LicenseAssignmentEditView',
     'LicenseAssignmentDeleteView',
     'LicenseAssignmentBulkEditView',
     'LicenseAssignmentBulkDeleteView',
 )
 
+
 @register_model_view(License, name='list')
 class LicenseListView(ObjectListView):
     queryset = License.objects.all()
     table = LicenseTable
     filterset = LicenseFilterSet
     filterset_form = LicenseFilterForm
```

### Comparing `netbox-lifecycle-1.0.2/netbox_lifecycle.egg-info/SOURCES.txt` & `netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,11 +58,13 @@
 netbox_lifecycle/templates/netbox_lifecycle/supportcontract.html
 netbox_lifecycle/templates/netbox_lifecycle/supportcontractassignment_edit.html
 netbox_lifecycle/templates/netbox_lifecycle/supportsku.html
 netbox_lifecycle/templates/netbox_lifecycle/vendor.html
 netbox_lifecycle/templates/netbox_lifecycle/generic/base.html
 netbox_lifecycle/templates/netbox_lifecycle/license/assignments.html
 netbox_lifecycle/templates/netbox_lifecycle/supportcontract/assignments.html
+netbox_lifecycle/tests/__init__.py
+netbox_lifecycle/tests/test_models.py
 netbox_lifecycle/views/__init__.py
 netbox_lifecycle/views/contract.py
 netbox_lifecycle/views/hardware.py
 netbox_lifecycle/views/license.py
```

### Comparing `netbox-lifecycle-1.0.2/setup.py` & `netbox_lifecycle-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox-lifecycle',
-    version='1.0.2',
+    version='1.0.3',
     description='NetBox Lifecycle',
     long_description='NetBox Support Contract and EOL/EOS management',
     url='https://github.com/dansheps/netbox-lifecycle/',
     download_url='https://pypi.org/project/netbox-lifecycle/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     maintainer='Daniel Sheppard',
```

