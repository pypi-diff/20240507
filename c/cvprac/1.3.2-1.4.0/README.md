# Comparing `tmp/cvprac-1.3.2.tar.gz` & `tmp/cvprac-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprac-1.3.2.tar", last modified: Thu Dec 14 23:43:51 2023, max compression
+gzip compressed data, was "cvprac-1.4.0.tar", last modified: Tue May  7 15:23:17 2024, max compression
```

## Comparing `cvprac-1.3.2.tar` & `cvprac-1.4.0.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.739082 cvprac-1.3.2/
--rw-r--r--   0 mhartzel   (501) staff       (20)    16636 2020-02-04 01:08:03.000000 cvprac-1.3.2/.pylintrc
--rw-r--r--   0 mhartzel   (501) staff       (20)     1522 2019-09-25 14:39:35.000000 cvprac-1.3.2/LICENSE
--rw-r--r--   0 mhartzel   (501) staff       (20)      505 2022-10-07 20:29:41.000000 cvprac-1.3.2/MANIFEST.in
--rw-r--r--   0 mhartzel   (501) staff       (20)     2377 2022-05-20 17:35:24.000000 cvprac-1.3.2/Makefile
--rw-r--r--   0 mhartzel   (501) staff       (20)    19753 2023-12-14 23:43:51.738534 cvprac-1.3.2/PKG-INFO
--rw-r--r--   0 mhartzel   (501) staff       (20)    18810 2023-12-14 23:40:27.000000 cvprac-1.3.2/README.md
--rw-r--r--   0 mhartzel   (501) staff       (20)        6 2023-12-14 23:40:27.000000 cvprac-1.3.2/VERSION
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.510229 cvprac-1.3.2/cvprac/
--rw-r--r--   0 mhartzel   (501) staff       (20)     1649 2023-12-14 23:40:27.000000 cvprac-1.3.2/cvprac/__init__.py
--rw-r--r--   0 mhartzel   (501) staff       (20)   189114 2023-12-14 23:40:27.000000 cvprac-1.3.2/cvprac/cvp_api.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    50314 2023-12-14 23:40:27.000000 cvprac-1.3.2/cvprac/cvp_client.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     2477 2019-09-25 14:39:35.000000 cvprac-1.3.2/cvprac/cvp_client_errors.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.516327 cvprac-1.3.2/cvprac.egg-info/
--rw-r--r--   0 mhartzel   (501) staff       (20)    19753 2023-12-14 23:43:51.000000 cvprac-1.3.2/cvprac.egg-info/PKG-INFO
--rw-r--r--   0 mhartzel   (501) staff       (20)     4453 2023-12-14 23:43:51.000000 cvprac-1.3.2/cvprac.egg-info/SOURCES.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)        1 2023-12-14 23:43:51.000000 cvprac-1.3.2/cvprac.egg-info/dependency_links.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)       83 2023-12-14 23:43:51.000000 cvprac-1.3.2/cvprac.egg-info/requires.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)       26 2023-12-14 23:43:51.000000 cvprac-1.3.2/cvprac.egg-info/top_level.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)      855 2019-09-25 14:39:35.000000 cvprac-1.3.2/cvprac.spec
--rw-r--r--   0 mhartzel   (501) staff       (20)       68 2022-10-07 20:29:41.000000 cvprac-1.3.2/dev-requirements.txt
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.537222 cvprac-1.3.2/docs/
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.538421 cvprac-1.3.2/docs/labs/
--rw-r--r--   0 mhartzel   (501) staff       (20)     2595 2023-12-14 23:40:27.000000 cvprac-1.3.2/docs/labs/README.md
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.539595 cvprac-1.3.2/docs/labs/lab01-cvp-info/
--rw-r--r--   0 mhartzel   (501) staff       (20)      519 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab01-cvp-info/get_cvp_info.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.549469 cvprac-1.3.2/docs/labs/lab02-inventory-operations/
--rw-r--r--   0 mhartzel   (501) staff       (20)     2514 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab02-inventory-operations/compliance_check.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1010 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab02-inventory-operations/get_running_configs.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1139 2022-10-07 20:29:41.000000 cvprac-1.3.2/docs/labs/lab02-inventory-operations/get_running_configs_by_time.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1208 2022-10-07 20:29:41.000000 cvprac-1.3.2/docs/labs/lab02-inventory-operations/remove_all_devices_legacy.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1287 2022-10-07 20:29:41.000000 cvprac-1.3.2/docs/labs/lab02-inventory-operations/remove_and_decommission_device.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1289 2022-10-07 20:29:41.000000 cvprac-1.3.2/docs/labs/lab02-inventory-operations/remove_devices_from_container_legacy.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1315 2022-10-07 20:29:41.000000 cvprac-1.3.2/docs/labs/lab02-inventory-operations/remove_devices_legacy.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.627554 cvprac-1.3.2/docs/labs/lab03-configlet-management/
--rw-r--r--   0 mhartzel   (501) staff       (20)      707 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab03-configlet-management/assign_configlet_to_device.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      669 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab03-configlet-management/backup_configlets.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1514 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab03-configlet-management/backup_configletsV2.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      124 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab03-configlet-management/common.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     2100 2022-10-07 20:29:41.000000 cvprac-1.3.2/docs/labs/lab03-configlet-management/config_search.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      121 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab03-configlet-management/configlet_list.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)      648 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab03-configlet-management/create_configlet.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      615 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab03-configlet-management/create_configlet_from_file.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1351 2023-03-07 16:02:05.000000 cvprac-1.3.2/docs/labs/lab03-configlet-management/get_applied_netelements.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1616 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab03-configlet-management/get_configlets.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      861 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab03-configlet-management/reorder_configlet_on_device.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      766 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab03-configlet-management/update_configlet.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.638824 cvprac-1.3.2/docs/labs/lab04-container-management/
--rw-r--r--   0 mhartzel   (501) staff       (20)      673 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab04-container-management/add_image_to_container.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      721 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab04-container-management/assign_configlet_to_container.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      655 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab04-container-management/create_container.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      676 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab04-container-management/remove_image_from_container.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1026 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab04-container-management/rename_container.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.646176 cvprac-1.3.2/docs/labs/lab05-device-management/
--rw-r--r--   0 mhartzel   (501) staff       (20)      659 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab05-device-management/add_image_to_devices.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     4334 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab05-device-management/add_image_wo_tempaction.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      662 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab05-device-management/remove_image_from_device.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1244 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab05-device-management/set_mgmt_ip.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.664604 cvprac-1.3.2/docs/labs/lab06-provisioning/
--rw-r--r--   0 mhartzel   (501) staff       (20)     5781 2023-03-07 16:02:05.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/atd_e2e_provisioning_workflow.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     2864 2022-10-07 20:29:41.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/auto_reconcile_on_rc_change.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     3562 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/change_control_custom_rapi.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      890 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/change_control_workflow.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1506 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/change_control_workflow_rapi.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.674822 cvprac-1.3.2/docs/labs/lab06-provisioning/configlets/
--rw-r--r--   0 mhartzel   (501) staff       (20)     6573 2023-03-07 16:02:05.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/configlets/AVD_leaf1.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     6573 2023-03-07 16:02:05.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/configlets/AVD_leaf2.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     6577 2023-03-07 16:02:05.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/configlets/AVD_leaf3.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     6581 2023-03-07 16:02:05.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/configlets/AVD_leaf4.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     3654 2023-03-07 16:02:05.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/configlets/AVD_spine1.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     3658 2023-03-07 16:02:05.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/configlets/AVD_spine2.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     2184 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/gen_builder.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     8347 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/mlag_issu.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      781 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/move_device.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     4909 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab06-provisioning/vc_task_retrigger.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.691443 cvprac-1.3.2/docs/labs/lab07-aaa/
--rw-r--r--   0 mhartzel   (501) staff       (20)      263 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab07-aaa/aaa_users.csv
--rw-r--r--   0 mhartzel   (501) staff       (20)      964 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab07-aaa/add_new_user_cvaas.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      823 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab07-aaa/add_new_user_onprem.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1078 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab07-aaa/add_users_from_csv_cvaas.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      786 2022-10-07 20:29:41.000000 cvprac-1.3.2/docs/labs/lab07-aaa/create_svc_account.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      854 2022-10-07 20:29:41.000000 cvprac-1.3.2/docs/labs/lab07-aaa/create_svc_account_token.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1106 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab07-aaa/create_terminattr_tokens.py
--rw-r--r--   0 mhartzel   (501) staff       (20)       33 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab07-aaa/cvaas.tok
--rw-r--r--   0 mhartzel   (501) staff       (20)      576 2022-10-07 20:29:41.000000 cvprac-1.3.2/docs/labs/lab07-aaa/delete_all_expired_svc_account_tokens.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      590 2022-10-07 20:29:41.000000 cvprac-1.3.2/docs/labs/lab07-aaa/delete_svc_account.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      808 2023-03-07 16:02:05.000000 cvprac-1.3.2/docs/labs/lab07-aaa/delete_svc_account_created_by_user.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      673 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab07-aaa/get_user_info.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1013 2022-10-07 20:29:41.000000 cvprac-1.3.2/docs/labs/lab07-aaa/svc_account_misc.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.693960 cvprac-1.3.2/docs/labs/lab08-resource-apis/
--rw-r--r--   0 mhartzel   (501) staff       (20)     6229 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/lab08-resource-apis/resource_cvprac.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     4449 2023-03-07 16:02:05.000000 cvprac-1.3.2/docs/labs/lab08-resource-apis/topology_tag_assignment.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.700116 cvprac-1.3.2/docs/labs/static/
--rw-r--r--   0 mhartzel   (501) staff       (20)   117691 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/static/serviceaccount1.png
--rw-r--r--   0 mhartzel   (501) staff       (20)   123315 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/static/serviceaccount2.png
--rw-r--r--   0 mhartzel   (501) staff       (20)   106538 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/labs/static/serviceaccount3.png
--rw-r--r--   0 mhartzel   (501) staff       (20)     1999 2019-09-25 14:39:35.000000 cvprac-1.3.2/docs/release-notes-0.7.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     2157 2019-09-25 14:39:35.000000 cvprac-1.3.2/docs/release-notes-0.8.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     2384 2019-09-25 14:39:35.000000 cvprac-1.3.2/docs/release-notes-0.9.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     3171 2019-09-25 14:39:35.000000 cvprac-1.3.2/docs/release-notes-1.0.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1759 2019-09-25 14:39:35.000000 cvprac-1.3.2/docs/release-notes-1.0.1.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     3148 2020-02-04 01:24:48.000000 cvprac-1.3.2/docs/release-notes-1.0.2.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)      303 2020-06-04 16:29:41.000000 cvprac-1.3.2/docs/release-notes-1.0.3.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     3328 2020-08-18 17:37:36.000000 cvprac-1.3.2/docs/release-notes-1.0.4.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1588 2021-05-17 20:03:41.000000 cvprac-1.3.2/docs/release-notes-1.0.5.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     2154 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/release-notes-1.0.6.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1407 2022-05-20 17:35:24.000000 cvprac-1.3.2/docs/release-notes-1.0.7.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     3350 2022-05-20 21:38:36.000000 cvprac-1.3.2/docs/release-notes-1.2.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1523 2022-10-10 14:46:28.000000 cvprac-1.3.2/docs/release-notes-1.2.2.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1716 2023-03-07 20:14:16.000000 cvprac-1.3.2/docs/release-notes-1.3.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)      206 2023-04-13 23:02:47.000000 cvprac-1.3.2/docs/release-notes-1.3.1.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1152 2023-12-14 23:40:27.000000 cvprac-1.3.2/docs/release-notes-1.3.2.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)       24 2023-03-07 16:02:05.000000 cvprac-1.3.2/requirements.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)       38 2023-12-14 23:43:51.739316 cvprac-1.3.2/setup.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     4721 2023-03-07 16:02:05.000000 cvprac-1.3.2/setup.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.494159 cvprac-1.3.2/test/
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.704481 cvprac-1.3.2/test/fixtures/
--rw-r--r--   0 mhartzel   (501) staff       (20)      450 2023-12-14 23:40:27.000000 cvprac-1.3.2/test/fixtures/cvp_nodes.yaml
--rw-r--r--   0 mhartzel   (501) staff       (20)  3941571 2019-09-25 14:39:35.000000 cvprac-1.3.2/test/fixtures/image-file.swix
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.725496 cvprac-1.3.2/test/lib/
--rw-r--r--   0 mhartzel   (501) staff       (20)     2634 2023-03-07 16:02:05.000000 cvprac-1.3.2/test/lib/systestlib.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.732056 cvprac-1.3.2/test/system/
--rw-r--r--   0 mhartzel   (501) staff       (20)     6699 2023-03-07 16:02:05.000000 cvprac-1.3.2/test/system/test_cvp_base.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    34474 2023-12-14 23:40:27.000000 cvprac-1.3.2/test/system/test_cvp_change_control_api.py
--rwxr-xr-x   0 mhartzel   (501) staff       (20)    20078 2023-12-14 23:40:27.000000 cvprac-1.3.2/test/system/test_cvp_client.py
--rw-r--r--   0 mhartzel   (501) staff       (20)   119502 2023-12-14 23:40:27.000000 cvprac-1.3.2/test/system/test_cvp_client_api.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-12-14 23:43:51.736797 cvprac-1.3.2/test/unit/
--rw-r--r--   0 mhartzel   (501) staff       (20)    10898 2023-04-13 15:49:42.000000 cvprac-1.3.2/test/unit/test_api.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    26712 2023-03-07 16:02:05.000000 cvprac-1.3.2/test/unit/test_client.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.511640 cvprac-1.4.0/
+-rw-r--r--   0 mhartzel   (501) staff       (20)    16636 2020-02-04 01:08:03.000000 cvprac-1.4.0/.pylintrc
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1522 2019-09-25 14:39:35.000000 cvprac-1.4.0/LICENSE
+-rw-r--r--   0 mhartzel   (501) staff       (20)      505 2022-10-07 20:29:41.000000 cvprac-1.4.0/MANIFEST.in
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2510 2024-04-25 20:36:28.000000 cvprac-1.4.0/Makefile
+-rw-r--r--   0 mhartzel   (501) staff       (20)    20014 2024-05-07 15:23:17.510732 cvprac-1.4.0/PKG-INFO
+-rw-r--r--   0 mhartzel   (501) staff       (20)    18810 2023-12-14 23:40:27.000000 cvprac-1.4.0/README.md
+-rw-r--r--   0 mhartzel   (501) staff       (20)        6 2024-05-06 17:49:39.000000 cvprac-1.4.0/VERSION
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.306339 cvprac-1.4.0/cvprac/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1649 2024-05-06 17:49:25.000000 cvprac-1.4.0/cvprac/__init__.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)   188108 2024-05-03 22:45:54.000000 cvprac-1.4.0/cvprac/cvp_api.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)    50262 2024-04-25 20:36:28.000000 cvprac-1.4.0/cvprac/cvp_client.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2477 2019-09-25 14:39:35.000000 cvprac-1.4.0/cvprac/cvp_client_errors.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.311532 cvprac-1.4.0/cvprac.egg-info/
+-rw-r--r--   0 mhartzel   (501) staff       (20)    20014 2024-05-07 15:23:17.000000 cvprac-1.4.0/cvprac.egg-info/PKG-INFO
+-rw-r--r--   0 mhartzel   (501) staff       (20)     4482 2024-05-07 15:23:17.000000 cvprac-1.4.0/cvprac.egg-info/SOURCES.txt
+-rw-r--r--   0 mhartzel   (501) staff       (20)        1 2024-05-07 15:23:17.000000 cvprac-1.4.0/cvprac.egg-info/dependency_links.txt
+-rw-r--r--   0 mhartzel   (501) staff       (20)       99 2024-05-07 15:23:17.000000 cvprac-1.4.0/cvprac.egg-info/requires.txt
+-rw-r--r--   0 mhartzel   (501) staff       (20)       26 2024-05-07 15:23:17.000000 cvprac-1.4.0/cvprac.egg-info/top_level.txt
+-rw-r--r--   0 mhartzel   (501) staff       (20)      855 2019-09-25 14:39:35.000000 cvprac-1.4.0/cvprac.spec
+-rw-r--r--   0 mhartzel   (501) staff       (20)       63 2024-04-29 20:36:54.000000 cvprac-1.4.0/dev-requirements.txt
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.331022 cvprac-1.4.0/docs/
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.332902 cvprac-1.4.0/docs/labs/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2595 2023-12-14 23:40:27.000000 cvprac-1.4.0/docs/labs/README.md
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.334819 cvprac-1.4.0/docs/labs/lab01-cvp-info/
+-rw-r--r--   0 mhartzel   (501) staff       (20)      519 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab01-cvp-info/get_cvp_info.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.346700 cvprac-1.4.0/docs/labs/lab02-inventory-operations/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2514 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab02-inventory-operations/compliance_check.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1010 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab02-inventory-operations/get_running_configs.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1139 2022-10-07 20:29:41.000000 cvprac-1.4.0/docs/labs/lab02-inventory-operations/get_running_configs_by_time.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1208 2022-10-07 20:29:41.000000 cvprac-1.4.0/docs/labs/lab02-inventory-operations/remove_all_devices_legacy.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1287 2022-10-07 20:29:41.000000 cvprac-1.4.0/docs/labs/lab02-inventory-operations/remove_and_decommission_device.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1289 2022-10-07 20:29:41.000000 cvprac-1.4.0/docs/labs/lab02-inventory-operations/remove_devices_from_container_legacy.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1315 2022-10-07 20:29:41.000000 cvprac-1.4.0/docs/labs/lab02-inventory-operations/remove_devices_legacy.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.372796 cvprac-1.4.0/docs/labs/lab03-configlet-management/
+-rw-r--r--   0 mhartzel   (501) staff       (20)      707 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab03-configlet-management/assign_configlet_to_device.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      669 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab03-configlet-management/backup_configlets.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1514 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab03-configlet-management/backup_configletsV2.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      124 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab03-configlet-management/common.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2100 2022-10-07 20:29:41.000000 cvprac-1.4.0/docs/labs/lab03-configlet-management/config_search.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      121 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab03-configlet-management/configlet_list.txt
+-rw-r--r--   0 mhartzel   (501) staff       (20)      648 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab03-configlet-management/create_configlet.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      615 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab03-configlet-management/create_configlet_from_file.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1351 2023-03-07 16:02:05.000000 cvprac-1.4.0/docs/labs/lab03-configlet-management/get_applied_netelements.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1616 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab03-configlet-management/get_configlets.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      861 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab03-configlet-management/reorder_configlet_on_device.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      766 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab03-configlet-management/update_configlet.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.391741 cvprac-1.4.0/docs/labs/lab04-container-management/
+-rw-r--r--   0 mhartzel   (501) staff       (20)      673 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab04-container-management/add_image_to_container.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      721 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab04-container-management/assign_configlet_to_container.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      655 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab04-container-management/create_container.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      676 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab04-container-management/remove_image_from_container.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1026 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab04-container-management/rename_container.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.407937 cvprac-1.4.0/docs/labs/lab05-device-management/
+-rw-r--r--   0 mhartzel   (501) staff       (20)      659 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab05-device-management/add_image_to_devices.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     4334 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab05-device-management/add_image_wo_tempaction.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      662 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab05-device-management/remove_image_from_device.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1244 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab05-device-management/set_mgmt_ip.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.428748 cvprac-1.4.0/docs/labs/lab06-provisioning/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     5781 2023-03-07 16:02:05.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/atd_e2e_provisioning_workflow.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2864 2022-10-07 20:29:41.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/auto_reconcile_on_rc_change.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3562 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/change_control_custom_rapi.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      890 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/change_control_workflow.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1506 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/change_control_workflow_rapi.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.441966 cvprac-1.4.0/docs/labs/lab06-provisioning/configlets/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     6573 2023-03-07 16:02:05.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/configlets/AVD_leaf1.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     6573 2023-03-07 16:02:05.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/configlets/AVD_leaf2.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     6577 2023-03-07 16:02:05.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/configlets/AVD_leaf3.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     6581 2023-03-07 16:02:05.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/configlets/AVD_leaf4.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3654 2023-03-07 16:02:05.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/configlets/AVD_spine1.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3658 2023-03-07 16:02:05.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/configlets/AVD_spine2.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2184 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/gen_builder.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     8347 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/mlag_issu.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      781 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/move_device.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     4889 2024-04-17 15:09:51.000000 cvprac-1.4.0/docs/labs/lab06-provisioning/vc_task_retrigger.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.464664 cvprac-1.4.0/docs/labs/lab07-aaa/
+-rw-r--r--   0 mhartzel   (501) staff       (20)      263 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab07-aaa/aaa_users.csv
+-rw-r--r--   0 mhartzel   (501) staff       (20)      964 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab07-aaa/add_new_user_cvaas.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      823 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab07-aaa/add_new_user_onprem.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1078 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab07-aaa/add_users_from_csv_cvaas.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      786 2022-10-07 20:29:41.000000 cvprac-1.4.0/docs/labs/lab07-aaa/create_svc_account.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      854 2022-10-07 20:29:41.000000 cvprac-1.4.0/docs/labs/lab07-aaa/create_svc_account_token.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1106 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab07-aaa/create_terminattr_tokens.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)       33 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab07-aaa/cvaas.tok
+-rw-r--r--   0 mhartzel   (501) staff       (20)      576 2022-10-07 20:29:41.000000 cvprac-1.4.0/docs/labs/lab07-aaa/delete_all_expired_svc_account_tokens.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      590 2022-10-07 20:29:41.000000 cvprac-1.4.0/docs/labs/lab07-aaa/delete_svc_account.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      808 2023-03-07 16:02:05.000000 cvprac-1.4.0/docs/labs/lab07-aaa/delete_svc_account_created_by_user.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      673 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab07-aaa/get_user_info.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1013 2022-10-07 20:29:41.000000 cvprac-1.4.0/docs/labs/lab07-aaa/svc_account_misc.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.467939 cvprac-1.4.0/docs/labs/lab08-resource-apis/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     6229 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/lab08-resource-apis/resource_cvprac.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     4449 2023-03-07 16:02:05.000000 cvprac-1.4.0/docs/labs/lab08-resource-apis/topology_tag_assignment.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.476395 cvprac-1.4.0/docs/labs/static/
+-rw-r--r--   0 mhartzel   (501) staff       (20)   117691 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/static/serviceaccount1.png
+-rw-r--r--   0 mhartzel   (501) staff       (20)   123315 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/static/serviceaccount2.png
+-rw-r--r--   0 mhartzel   (501) staff       (20)   106538 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/labs/static/serviceaccount3.png
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1999 2019-09-25 14:39:35.000000 cvprac-1.4.0/docs/release-notes-0.7.0.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2157 2019-09-25 14:39:35.000000 cvprac-1.4.0/docs/release-notes-0.8.0.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2384 2019-09-25 14:39:35.000000 cvprac-1.4.0/docs/release-notes-0.9.0.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3171 2019-09-25 14:39:35.000000 cvprac-1.4.0/docs/release-notes-1.0.0.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1759 2019-09-25 14:39:35.000000 cvprac-1.4.0/docs/release-notes-1.0.1.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3148 2020-02-04 01:24:48.000000 cvprac-1.4.0/docs/release-notes-1.0.2.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)      303 2020-06-04 16:29:41.000000 cvprac-1.4.0/docs/release-notes-1.0.3.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3328 2020-08-18 17:37:36.000000 cvprac-1.4.0/docs/release-notes-1.0.4.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1588 2021-05-17 20:03:41.000000 cvprac-1.4.0/docs/release-notes-1.0.5.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2154 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/release-notes-1.0.6.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1407 2022-05-20 17:35:24.000000 cvprac-1.4.0/docs/release-notes-1.0.7.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3350 2022-05-20 21:38:36.000000 cvprac-1.4.0/docs/release-notes-1.2.0.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1523 2022-10-10 14:46:28.000000 cvprac-1.4.0/docs/release-notes-1.2.2.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1716 2023-03-07 20:14:16.000000 cvprac-1.4.0/docs/release-notes-1.3.0.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)      206 2023-04-13 23:02:47.000000 cvprac-1.4.0/docs/release-notes-1.3.1.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1152 2023-12-14 23:59:12.000000 cvprac-1.4.0/docs/release-notes-1.3.2.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1173 2024-05-06 17:46:39.000000 cvprac-1.4.0/docs/release-notes-1.4.0.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)       40 2024-04-17 15:09:51.000000 cvprac-1.4.0/requirements.txt
+-rw-r--r--   0 mhartzel   (501) staff       (20)       38 2024-05-07 15:23:17.511877 cvprac-1.4.0/setup.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     4996 2024-04-17 15:09:51.000000 cvprac-1.4.0/setup.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.289446 cvprac-1.4.0/test/
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.479982 cvprac-1.4.0/test/fixtures/
+-rw-r--r--   0 mhartzel   (501) staff       (20)      495 2024-05-05 21:19:56.000000 cvprac-1.4.0/test/fixtures/cvp_nodes.yaml
+-rw-r--r--   0 mhartzel   (501) staff       (20)  3941571 2019-09-25 14:39:35.000000 cvprac-1.4.0/test/fixtures/image-file.swix
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.496203 cvprac-1.4.0/test/lib/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2633 2024-04-25 20:36:28.000000 cvprac-1.4.0/test/lib/systestlib.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.504908 cvprac-1.4.0/test/system/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     7006 2024-04-25 20:36:28.000000 cvprac-1.4.0/test/system/test_cvp_base.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)    34906 2024-04-25 20:36:28.000000 cvprac-1.4.0/test/system/test_cvp_change_control_api.py
+-rwxr-xr-x   0 mhartzel   (501) staff       (20)    20096 2024-04-25 20:36:28.000000 cvprac-1.4.0/test/system/test_cvp_client.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)   119716 2024-05-01 14:26:19.000000 cvprac-1.4.0/test/system/test_cvp_client_api.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2024-05-07 15:23:17.508735 cvprac-1.4.0/test/unit/
+-rw-r--r--   0 mhartzel   (501) staff       (20)    10956 2024-04-25 20:36:28.000000 cvprac-1.4.0/test/unit/test_api.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)    26721 2024-04-29 20:36:54.000000 cvprac-1.4.0/test/unit/test_client.py
```

### Comparing `cvprac-1.3.2/.pylintrc` & `cvprac-1.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/LICENSE` & `cvprac-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/Makefile` & `cvprac-1.4.0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 	find . -type f -regex ".*\.py[co]$$" -delete
 
 coverage_report:
 	$(COVERAGE) report -m
 
 pep8:
 	-pep8 -r --max-line-length=120 --ignore=$(PEP8_IGNORE) cvprac/
-	-pep8 -r --max-line-length=120 --ignore=$(PEP8_IGNORE),E402 test/
+	-pep8 -r --max-line-length=120 --ignore=$(PEP8_IGNORE),E402 test/lib/
+	-pep8 -r --max-line-length=120 --ignore=$(PEP8_IGNORE),E402 test/system/
+	-pep8 -r --ignore=$(PEP8_IGNORE),E402,E501 test/unit/
 
 pyflakes:
 	pyflakes cvprac/ test/
 
 pylint:
 	find ./cvprac ./test -name \*.py | xargs pylint --rcfile .pylintrc
```

### Comparing `cvprac-1.3.2/PKG-INFO` & `cvprac-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: cvprac
-Version: 1.3.2
+Version: 1.4.0
 Summary: Arista Cloudvision(R) Portal Rest API Client written in python
 Home-page: https://github.com/aristanetworks/cvprac
 Author: Arista Networks, Inc.
 Author-email: eosplus-dev@arista.com
 License: BSD-3
-Download-URL: https://github.com/aristanetworks/cvprac/tarball/1.3.2
+Download-URL: https://github.com/aristanetworks/cvprac/tarball/1.4.0
 Keywords: networking CloudVision development rest api
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Arista Cloudvision® Portal RESTful API Client
 
 [![pypi](https://img.shields.io/pypi/v/cvprac.svg)](https://pypi.python.org/pypi/cvprac)
```

### Comparing `cvprac-1.3.2/README.md` & `cvprac-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/cvprac/__init__.py` & `cvprac-1.4.0/cvprac/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,9 +28,9 @@
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 ''' RESTful API Client class for Cloudvision(R) Portal
 '''
 
-__version__ = '1.3.2'
+__version__ = '1.4.0'
 __author__ = 'Arista Networks, Inc.'
```

### Comparing `cvprac-1.3.2/cvprac/cvp_api.py` & `cvprac-1.4.0/cvprac/cvp_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=fixme,too-many-locals,redefined-builtin
 #
 # Copyright (c) 2017, Arista Networks, Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are
 # met:
@@ -31,15 +32,14 @@
 #
 ''' Class containing calls to CVP RESTful API.
 '''
 import operator
 import os
 import time
 # This import is for proper file IO handling support for both Python 2 and 3
-# pylint: disable=redefined-builtin
 from io import open
 from datetime import datetime
 from re import split
 
 from cvprac.cvp_client_errors import CvpApiError
 
 try:
@@ -52,15 +52,61 @@
     '<': operator.lt,
     '>=': operator.ge,
     '<=': operator.le,
     '==': operator.eq
 }
 
 
-class CvpApi(object):
+def sanitize_warnings(data):
+    ''' Sanitize the warnings returned after validation.
+
+        In some cases where the configlets have both errors
+        and warnings, CVP may split warnings that have
+        `,` across multiple strings.
+        This method concatenates the strings back into one string
+        per warning, and corrects the warningCount.
+
+        Args:
+            data (dict): A dict that contians the result
+                of the validation operation
+        Returns:
+            response (dict): A dict that contains the result of the
+                validation operation
+    '''
+    if "warnings" not in data:
+        # nothing to do here, we can return as is
+        return data
+    # Since there may be warnings incorrectly split on
+    # ', ' within the warning text by CVP, we join all the
+    # warnings together using ', ' into one large string
+    temp_warnings = ", ".join(data['warnings']).strip()
+
+    # To split the large string again we match on the
+    # 'at line XXX' that should indicate the end of the warning.
+    # We capture as well the remaining \\n or whitespace and include
+    # the extra ', ' added in the previous step in the matching criteria.
+    # The extra ', ' is not included in the strings of the new list
+    temp_warnings = split(
+        r'(.*?at line \d+.*?),\s+',
+        temp_warnings
+    )
+
+    # The behaviour of re.split will add empty strings
+    # if the regex matches on the begging or ending of the line.
+    # Refer to https://docs.python.org/3/library/re.html#re.split
+
+    # Use filter to remove any empty strings
+    # that re.split inserted
+    data['warnings'] = list(filter(None, temp_warnings))
+    # Update the count of warnings to the correct value
+    data['warningCount'] = len(data['warnings'])
+    return data
+
+
+class CvpApi():
     ''' CvpApi class contains calls to CVP RESTful API.  The RESTful API
         parameters are passed in as parameters to the method.  The results of
         the RESTful API call are converted from json to a dict and returned.
         Where needed minimal processing is performed on the results.
         Any method that does a cvprac get or post call could raise the
         following errors:
 
@@ -106,16 +152,15 @@
                     >= - Greater Than or Equal To
                     <= - Less Than or Equal To
                     == - Equal To
                 version (float): The float API Version number to compare the
                     running CVP version to.
         '''
         if opr not in OPERATOR_DICT:
-            self.log.error('%s is an invalid operation for version comparison'
-                           % opr)
+            self.log.error("%s is an invalid operation for version comparison", opr)
             return False
 
         # Since CVaaS is automatically the latest version of the API, if
         # operators > or >= are provided we can quickly check if we are running
         # on CVaaS and return True if found.
         if opr in ['>', '>='] and self.clnt.is_cvaas:
             return True
@@ -161,17 +206,17 @@
                 status (str): state of the user (Enabled/Disabled)
                 first_name (str): first name of the user
                 last_name (str): last name of the user
                 email (str): email address of the user
                 user_type (str): type of AAA (Local/TACACS/RADIUS)
         '''
         if status not in ['Enabled', 'Disabled']:
-            self.log.error('Invalid status %s.'
-                           ' Status must be Enabled or Disabled.'
-                           ' Defaulting to Disabled' % status)
+            self.log.error(f"Invalid status {status}."
+                           " Status must be Enabled or Disabled."
+                           " Defaulting to Disabled")
             status = 'Disabled'
         data = {"roles": [role],
                 "user": {"contactNumber": "",
                          "email": email,
                          "firstName": first_name,
                          "lastName": last_name,
                          "password": password,
@@ -194,37 +239,37 @@
                 status (str): state of the user (Enabled/Disabled)
                 first_name (str): first name of the user
                 last_name (str): last name of the user
                 email (str): email address of the user
                 user_type (str): type of AAA (Local/TACACS/RADIUS)
         '''
         if status not in ['Enabled', 'Disabled']:
-            self.log.error('Invalid status %s.'
-                           ' Status must be Enabled or Disabled.'
-                           ' Defaulting to Disabled' % status)
+            self.log.error(f"Invalid status {status}."
+                           f" Status must be Enabled or Disabled."
+                           f" Defaulting to Disabled")
             status = 'Disabled'
         data = {"roles": [role],
                 "user": {"contactNumber": "",
                          "email": email,
                          "firstName": first_name,
                          "lastName": last_name,
                          "password": password,
                          "userId": username,
                          "userStatus": status,
                          "userType": user_type}}
-        return self.clnt.post('/user/updateUser.do?userId={}'.format(username),
+        return self.clnt.post(f"/user/updateUser.do?userId={username}",
                               data=data, timeout=self.request_timeout)
 
     def get_user(self, username):
         ''' Returns specified user information
 
             Args:
                 username (str): username on CVP
         '''
-        return self.clnt.get('/user/getUser.do?userId={}'.format(username),
+        return self.clnt.get(f"/user/getUser.do?userId={qplus(username)}",
                              timeout=self.request_timeout)
 
     def get_users(self, query='', start=0, end=0):
         ''' Returns all users in CVP filtered by an optional query parameter
 
             Args:
                 query (str): Query parameter to filter users by.
@@ -244,18 +289,17 @@
                                 'lastAccessed': 1654555139700,
                                 'contactNumber': '',
                                 'userType': 'Local',
                                 'userStatus': 'Enabled',
                                 'currentStatus': 'Online',
                                 'addedByUser': 'cvp system'}]}
         '''
-        self.log.debug('get_users: query: %s' % query)
-        return self.clnt.get('/user/getUsers.do?'
-                             'queryparam=%s&startIndex=%d&endIndex=%d' %
-                             (qplus(query), start, end),
+        self.log.debug(f"get_users: query: {query}")
+        return self.clnt.get(f"/user/getUsers.do?"
+                             f"queryparam={qplus(query)}&startIndex={start}&endIndex={end}",
                              timeout=self.request_timeout)
 
     def delete_user(self, username):
         ''' Remove specified user from CVP
 
             Args:
                 username (str): username on CVP
@@ -271,20 +315,20 @@
             Args:
                 task_id (int): CVP task identifier
 
             Returns:
                 task (dict): The CVP task for the associated Id.  Returns None
                     if the task_id was invalid.
         '''
-        self.log.debug('get_task_by_id: task_id: %s' % task_id)
+        self.log.debug(f"get_task_by_id: task_id: {task_id}")
         try:
-            task = self.clnt.get('/task/getTaskById.do?taskId=%s' % task_id,
+            task = self.clnt.get(f"/task/getTaskById.do?taskId={task_id}",
                                  timeout=self.request_timeout)
         except CvpApiError as error:
-            self.log.debug('Caught error: %s attempting to get task.' % error)
+            self.log.debug(f"Caught error: {error} attempting to get task.")
             # Catch an invalid task_id error and return None
             return None
         return task
 
     def get_tasks_by_status(self, status, start=0, end=0):
         ''' Returns a list of tasks with the given status.
 
@@ -293,18 +337,18 @@
                 start (int): Start index for the pagination.  Default is 0.
                 end (int): End index for the pagination.  If end index is 0
                     then all the records will be returned.  Default is 0.
 
             Returns:
                 tasks (list): The list of tasks
         '''
-        self.log.debug('get_tasks_by_status: status: %s' % status)
+        self.log.debug(f"get_tasks_by_status: status: {status}")
         data = self.clnt.get(
-            '/task/getTasks.do?queryparam=%s&startIndex=%d&endIndex=%d' %
-            (status, start, end), timeout=self.request_timeout)
+            f"/task/getTasks.do?queryparam={status}&startIndex={start}&endIndex={end}",
+            timeout=self.request_timeout)
         return data['data']
 
     def get_tasks(self, start=0, end=0):
         ''' Returns a list of all the tasks.
 
             Args:
                 start (int): Start index for the pagination.  Default is 0.
@@ -312,17 +356,16 @@
                     then all the records will be returned.  Default is 0.
 
             Returns:
                 tasks (dict): The 'total' key contains the number of tasks,
                     the 'data' key contains a list of the tasks.
         '''
         self.log.debug('get_tasks:')
-        return self.clnt.get('/task/getTasks.do?queryparam=&startIndex=%d&'
-                             'endIndex=%d' % (start, end),
-                             timeout=self.request_timeout)
+        return self.clnt.get(f"/task/getTasks.do?queryparam=&startIndex={start}&"
+                             f"endIndex={end}", timeout=self.request_timeout)
 
     def get_logs_by_id(self, task_id, start=0, end=0):
         ''' Returns the log entries for the task with the specified TaskId.
 
             Args:
                 task_id (int): CVP task identifier
                 start (int): The first log entry to return.  Default is 0.
@@ -330,46 +373,44 @@
                     means to return all log entries.  Can be a large number to
                     indicate the last log entry.
 
             Returns:
                 task (dict): The CVP log for the associated Id.  Returns None
                     if the task_id was invalid.
         '''
-        self.log.debug('get_logs_by_id: task_id: %s' % task_id)
+        self.log.debug(f"get_logs_by_id: task_id: {task_id}")
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion < 5.0:
             self.log.debug('v1 - v4 /task/getLogsByID.do?')
-            resp = self.clnt.get('/task/getLogsById.do?id=%s&queryparam='
-                                 '&startIndex=%d&endIndex=%d' %
-                                 (task_id, start, end),
+            resp = self.clnt.get(f"/task/getLogsById.do?id={task_id}&queryparam="
+                                 f"&startIndex={start}&endIndex={end}",
                                  timeout=self.request_timeout)
         else:
             self.log.debug('v5 /audit/getLogs.do')
             task_info = self.get_task_by_id(task_id)
             stage_id = None
             if 'stageId' in task_info:
                 stage_id = task_info['stageId']
             else:
-                self.log.debug('No stage ID found for task %s' % task_id)
+                self.log.debug(f"No stage ID found for task {task_id}")
             if 'ccIdV2' in task_info:
                 cc_id = task_info['ccIdV2']
                 if cc_id == '':
-                    self.log.debug('No ccIdV2 for task %s.'
-                                   ' It was likely cancelled.'
-                                   ' Using old /task/getLogsByID.do?'
-                                   % task_id)
+                    self.log.debug(f"No ccIdV2 for task {task_id}."
+                                   f" It was likely cancelled."
+                                   f" Using old /task/getLogsByID.do?")
                     resp = self.clnt.get(
-                        '/task/getLogsById.do?id=%s&queryparam='
-                        '&startIndex=%d&endIndex=%d' % (task_id, start, end),
+                        f"/task/getLogsById.do?id={task_id}&queryparam="
+                        f"&startIndex={start}&endIndex={end}",
                         timeout=self.request_timeout)
                 else:
                     resp = self.get_audit_logs_by_id(cc_id, stage_id)
             else:
-                self.log.debug('No change ID found for task %s' % task_id)
+                self.log.debug(f"No change ID found for task {task_id}")
                 resp = None
         return resp
 
     def get_audit_logs_by_id(self, cc_id, stage_id=None, data_size=75):
         ''' Returns the audit logs of a particular ChangeControl.
 
             Args:
@@ -394,16 +435,15 @@
     def add_note_to_task(self, task_id, note):
         ''' Add notes to the task.
 
             Args:
                 task_id (str): Task ID
                 note (str): Note to add to the task
         '''
-        self.log.debug('add_note_to_task: task_id: %s note: %s' %
-                       (task_id, note))
+        self.log.debug(f"add_note_to_task: task_id: {task_id} note: {note}")
         data = {'workOrderId': task_id, 'note': note}
         self.clnt.post('/task/addNoteToTask.do', data=data,
                        timeout=self.request_timeout)
 
     def execute_task(self, task_id):
         ''' Execute the task.  Note that if the task has failed then inspect
             the task logs to determine why the task failed.  If you see:
@@ -412,149 +452,142 @@
 
             then it means that the netelement does not have the same user ID
             and/or password as the CVP user executing the task.
 
             Args:
                 task_id (str): Task ID
         '''
-        self.log.debug('execute_task: task_id: %s' % task_id)
+        self.log.debug(f"execute_task: task_id: {task_id}")
         data = {'data': [task_id]}
-        self.clnt.post('/task/executeTask.do', data=data,
-                       timeout=self.request_timeout)
+        self.clnt.post('/task/executeTask.do', data=data, timeout=self.request_timeout)
 
     def cancel_task(self, task_id):
         ''' Cancel the task
 
             Args:
                 task_id (str): Task ID
         '''
-        self.log.debug('cancel_task: task_id: %s' % task_id)
+        self.log.debug(f"cancel_task: task_id: {task_id}")
         data = {'data': [task_id]}
         return self.clnt.post('/task/cancelTask.do', data=data,
                               timeout=self.request_timeout)
 
     def get_configlets(self, start=0, end=0):
         ''' Returns a list of all defined configlets.
 
             Args:
                 start (int): Start index for the pagination. Default is 0.
                 end (int): End index for the pagination. If end index is 0
                     then all the records will be returned. Default is 0.
         '''
         if self.clnt.apiversion is None:
             self.get_cvp_info()
-        configlets = self.clnt.get('/configlet/getConfiglets.do?'
-                                   'startIndex=%d&endIndex=%d' % (start, end),
+        configlets = self.clnt.get(f"/configlet/getConfiglets.do?"
+                                   f"startIndex={start}&endIndex={end}",
                                    timeout=self.request_timeout)
         if self.clnt.apiversion == 1.0 or self.clnt.apiversion >= 4.0:
             self.log.debug('v1/v4+ Inventory API Call')
             return configlets
-        else:
-            self.log.debug('v2 Inventory API Call')
-            # New API getConfiglets does not return the actual configlet config
-            # Get the actual configlet config using getConfigletByName
-            if 'data' in configlets:
-                for configlet in configlets['data']:
-                    full_cfglt_data = self.get_configlet_by_name(
-                        configlet['name'])
-                    configlet['config'] = full_cfglt_data['config']
-            return configlets
+        self.log.debug('v2 Inventory API Call')
+        # New API getConfiglets does not return the actual configlet config
+        # Get the actual configlet config using getConfigletByName
+        if 'data' in configlets:
+            for configlet in configlets['data']:
+                full_cfglt_data = self.get_configlet_by_name(configlet['name'])
+                configlet['config'] = full_cfglt_data['config']
+        return configlets
 
     def get_configlets_and_mappers(self):
         ''' Returns a list of all defined configlets and associated mappers
         '''
         self.log.debug(
             'get_configlets_and_mappers: getConfigletsAndAssociatedMappers')
-        return self.clnt.get('/configlet/getConfigletsAndAssociatedMappers.do')
+        return self.clnt.get('/configlet/getConfigletsAndAssociatedMappers.do',
+                             timeout=self.request_timeout)
 
     def get_configlet_builder(self, c_id):
         ''' Returns the configlet builder data for the given configlet ID.
 
             Args:
                 c_id (str): The ID (key) for the configlet to be queried.
         '''
-        return self.clnt.get('/configlet/getConfigletBuilder.do?id=%s'
-                             % c_id, timeout=self.request_timeout)
+        return self.clnt.get(f"/configlet/getConfigletBuilder.do?id={c_id}",
+                             timeout=self.request_timeout)
 
     def search_configlets(self, query, start=0, end=0):
         ''' Returns a list of configlets that match a search query.
 
             Args:
                 query (str): A simple string of text to be matched against
                     the existing configlets. Not a regex.
                 start (int): Start index for the pagination. Default is 0.
                 end (int): End index for the pagination. If end index is 0
                     then all the records will be returned. Default is 0.
         '''
-        self.log.debug('search_configlets: query: %s' % query)
-        return self.clnt.get('/configlet/searchConfiglets.do?'
-                             'queryparam=%s&startIndex=%d&endIndex=%d' %
-                             (qplus(query), start, end),
+        self.log.debug(f"search_configlets: query: {query}")
+        return self.clnt.get(f"/configlet/searchConfiglets.do?"
+                             f"queryparam={qplus(query)}&startIndex={start}&endIndex={end}",
                              timeout=self.request_timeout)
 
     def get_configlet_by_name(self, name):
         ''' Returns the configlet with the specified name
 
             Args:
                 name (str): Name of the configlet.  Can contain spaces.
 
             Returns:
                 configlet (dict): The configlet dict.
         '''
-        self.log.debug('get_configlets_by_name: name: %s' % name)
-        return self.clnt.get('/configlet/getConfigletByName.do?name=%s'
-                             % qplus(name), timeout=self.request_timeout)
+        self.log.debug(f"get_configlets_by_name: name: {name}")
+        return self.clnt.get(f"/configlet/getConfigletByName.do?name={qplus(name)}",
+                             timeout=self.request_timeout)
 
     def get_configlets_by_container_id(self, c_id, start=0, end=0):
         ''' Returns a list of configlets applied to the given container.
 
             Args:
                 c_id (str): The container ID (key) to query.
                 start (int): Start index for the pagination. Default is 0.
                 end (int): End index for the pagination. If end index is 0
                     then all the records will be returned. Default is 0.
         '''
-        return self.clnt.get('/provisioning/getConfigletsByContainerId.do?'
-                             'containerId=%s&startIndex=%d&endIndex=%d'
-                             % (c_id, start, end),
+        return self.clnt.get(f"/provisioning/getConfigletsByContainerId.do?"
+                             f"containerId={c_id}&startIndex={start}&endIndex={end}",
                              timeout=self.request_timeout)
 
     def get_configlets_by_netelement_id(self, d_id, start=0, end=0):
         ''' Returns a list of configlets applied to the given device.
 
             Args:
                 d_id (str): The device ID (key) to query.
                 start (int): Start index for the pagination. Default is 0.
                 end (int): End index for the pagination. If end index is 0
                     then all the records will be returned. Default is 0.
         '''
-        return self.clnt.get('/provisioning/getConfigletsByNetElementId.do?'
-                             'netElementId=%s&startIndex=%d&endIndex=%d'
-                             % (d_id, start, end),
+        return self.clnt.get(f"/provisioning/getConfigletsByNetElementId.do?"
+                             f"netElementId={d_id}&startIndex={start}&endIndex={end}",
                              timeout=self.request_timeout)
 
     def get_image_bundle_by_container_id(self, container_id, start=0, end=0,
                                          scope='false'):
         ''' Returns a list of ImageBundles applied to the given container.
             Args:
                 container_id (str): The container ID (key) to query.
                 start (int): Start index for the pagination. Default is 0.
                 end (int): End index for the pagination. If end index is 0
                     then all the records will be returned. Default is 0.
                 scope (string) the session scope (true or false).
         '''
-        if scope != 'true' and scope != 'false':
-            self.log.error('scope value must be true or false.'
-                           ' %s is an invalid value.'
-                           ' Defaulting back to false' % scope)
+        if scope not in ('true', 'false'):
+            self.log.error("scope value must be true or false. %s is an invalid value."
+                           " Defaulting back to false", scope)
             scope = 'false'
-        return self.clnt.get('/provisioning/getImageBundleByContainerId.do?'
-                             'containerId=%s&startIndex=%d&endIndex=%d'
-                             '&sessionScope=%s'
-                             % (container_id, start, end, scope),
+        return self.clnt.get(f"/provisioning/getImageBundleByContainerId.do?"
+                             f"containerId={container_id}&startIndex={start}&endIndex={end}"
+                             f"&sessionScope={scope}",
                              timeout=self.request_timeout)
 
     def get_configlet_history(self, key, start=0, end=0):
         ''' Returns the configlet history.
 
             Args:
                 key (str): Key for the configlet.
@@ -563,18 +596,18 @@
                     which means to return all configlet entries.  Can be a
                     large number to indicate the last configlet entry.
 
             Returns:
                 history (dict): The configlet dict with the changes from
                     most recent to oldest.
         '''
-        self.log.debug('get_configlets_history: key: %s' % key)
-        return self.clnt.get('/configlet/getConfigletHistory.do?configletId='
-                             '%s&queryparam=&startIndex=%d&endIndex=%d' %
-                             (key, start, end), timeout=self.request_timeout)
+        self.log.debug(f"get_configlets_history: key: {key}")
+        return self.clnt.get(f"/configlet/getConfigletHistory.do?configletId="
+                             f"{key}&queryparam=&startIndex={start}&endIndex={end}",
+                             timeout=self.request_timeout)
 
     def get_inventory(self, start=0, end=0, query='', provisioned=True):
         ''' Returns the a dict of the net elements known to CVP.
 
             Args:
                 start (int): The first inventory entry to return.  Default is 0
                 end (int): The last inventory entry to return.  Default is 0
@@ -585,21 +618,20 @@
                     are running a specific version of EOS.
         '''
         self.log.debug('get_inventory: called')
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion == 1.0:
             self.log.debug('v1 Inventory API Call')
-            data = self.clnt.get('/inventory/getInventory.do?'
-                                 'queryparam=%s&startIndex=%d&endIndex=%d' %
-                                 (qplus(query), start, end),
+            data = self.clnt.get(f"/inventory/getInventory.do?"
+                                 f"queryparam={qplus(query)}&startIndex={start}&endIndex={end}",
                                  timeout=self.request_timeout)
             return data['netElementList']
         self.log.debug('v2 Inventory API Call')
-        data = self.clnt.get('/inventory/devices?provisioned=%s' % provisioned,
+        data = self.clnt.get(f"/inventory/devices?provisioned={provisioned}",
                              timeout=self.request_timeout)
         containers = self.get_containers()
         for dev in data:
             dev['key'] = dev['systemMacAddress']
             dev['deviceInfo'] = dev['deviceStatus'] = dev['status']
             dev['isMLAGEnabled'] = dev['mlagEnabled']
             dev['isDANZEnabled'] = dev['danzEnabled']
@@ -699,16 +731,15 @@
                         time.sleep(2)
                         inv = self.get_inventory()
 
                 if device_ips:
                     # If any devices did not appear, there is a problem
                     # Join the missing IPs into a string for output
                     missing_ips = ', '.join(device_ips)
-                    raise RuntimeError('Devices {} failed to appear '
-                                       'in inventory'.format(missing_ips))
+                    raise RuntimeError(f"Devices {missing_ips} failed to appear in inventory")
 
             # Move the devices to their specified containers
             for device in device_list:
                 devs = [dev for dev in inv if 'ipAddress' in dev and
                         device['device_ip'] in dev['ipAddress']]
                 dev = devs[0]
                 container = {'key': device['parent_key'],
@@ -729,88 +760,88 @@
         device = {
             'device_ip': device_ip,
             'parent_name': parent_name,
             'parent_key': parent_key
         }
         self.add_devices_to_inventory([device], wait=wait)
 
-    def retry_add_to_inventory(self, device_mac, device_ip, username,
+    def retry_add_to_inventory(self, dev_mac, device_ip, username,
                                password):
         '''Retry addition of device to Cvp inventory
 
             Args:
-                device_mac (str): MAC address of device
+                dev_mac (str): MAC address of device
                 device_ip (str): ip address assigned to device
                 username (str): username for device login
                 password (str): password for user
         '''
         self.log.debug('retry_add_to_inventory: called')
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion == 1.0:
             self.log.debug('v1 Inventory API Call')
-            data = {"key": device_mac,
+            data = {"key": dev_mac,
                     "ipAddress": device_ip,
                     "userName": username,
                     "password": password}
             self.clnt.post('/inventory/add/retryAddDeviceToInventory.do?'
                            'startIndex=0&endIndex=0',
                            data=data,
                            timeout=self.request_timeout)
         else:
             self.log.debug('v2 Inventory API Call')
             self.log.warning(
                 'retry_add_to_inventory: not implemented for v2 APIs')
 
-    def delete_device(self, device_mac):
+    def delete_device(self, dev_mac):
         '''Delete the device and its pending tasks from Cvp inventory
 
             Args:
-                device_mac (str): mac address of device we are deleting
+                dev_mac (str): mac address of device we are deleting
                                   For CVP 2020 this param is now required to
                                   be the device serial number instead of MAC
                                   address. This method will handle getting
                                   the device serial number via the provided
                                   MAC address.
             Returns:
                 data (dict): Contains success or failure message
         '''
         self.log.debug('delete_device: called')
-        return self.delete_devices([device_mac])
+        return self.delete_devices([dev_mac])
 
-    def delete_devices(self, device_macs):
+    def delete_devices(self, dev_macs):
         '''Delete the device and its pending tasks from Cvp inventory
 
             Args:
-                device_macs (list): list of mac address for
+                dev_macs (list): list of mac address for
                                     devices we're deleting
                                     For CVP 2020 this param is now required to
                                     be a list of device serial numbers instead
                                     of MAC addresses. This method will handle
                                     getting the device serial number via the
                                     provided MAC address.
             Returns:
                 data (dict): Contains success or failure message
         '''
         self.log.debug('delete_devices: called')
         resp = None
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion < 4.0:
-            data = {'data': device_macs}
+            data = {'data': dev_macs}
             resp = self.clnt.post('/inventory/deleteDevices.do?', data=data,
                                   timeout=self.request_timeout)
         else:
             self.log.warning('NOTE: The Delete Devices API has updated for'
                              ' CVP 2020.2 and it is not required to send the'
                              ' device serial number instead of mac address'
                              ' when deleting a device. Looking up each devices'
                              'serial num based on provided MAC addresses')
             devices = []
-            for dev_mac in device_macs:
+            for dev_mac in dev_macs:
                 device_info = self.get_device_by_mac(dev_mac)
                 if device_info is not None and 'serialNumber' in device_info:
                     devices.append(device_info)
             resp = self.delete_devices_by_serial(devices)
         return resp
 
     def delete_devices_by_serial(self, devices):
@@ -898,15 +929,15 @@
                     the fqdn string to match on the hostname portion
                     specifically which should be the first component
 
             Returns:
                 device (dict): The net element device dict for the device if
                     otherwise returns an empty hash.
         '''
-        self.log.debug('get_device_by_name: fqdn: %s' % fqdn)
+        self.log.debug(f"get_device_by_name: fqdn: {fqdn}")
         # data = self.get_inventory(start=0, end=0, query=fqdn)
         data = self.search_topology(fqdn)
         device = {}
         if 'netElementList' in data:
             for netelem in data['netElementList']:
                 if not search_by_hostname:
                     if netelem['fqdn'] == fqdn:
@@ -914,103 +945,100 @@
                         break
                 else:
                     if netelem['fqdn'].split('.')[0] == fqdn:
                         device = netelem
                         break
         return device
 
-    def get_device_by_mac(self, device_mac):
+    def get_device_by_mac(self, dev_mac):
         ''' Returns the net element device dict for the devices mac address.
 
             Args:
-                device_mac (str): MAC Address of the device.
+                dev_mac (str): MAC Address of the device.
 
             Returns:
                 device (dict): The net element device dict for the device if
                     otherwise returns an empty hash.
         '''
-        self.log.debug('get_device_by_mac: MAC address: %s' % device_mac)
-        # data = self.get_inventory(start=0, end=0, query=device_mac)
-        data = self.search_topology(device_mac)
+        self.log.debug(f"get_device_by_mac: MAC address: {dev_mac}")
+        # data = self.get_inventory(start=0, end=0, query=dev_mac)
+        data = self.search_topology(dev_mac)
         device = {}
         if 'netElementList' in data:
             for netelem in data['netElementList']:
-                if netelem['systemMacAddress'] == device_mac:
+                if netelem['systemMacAddress'] == dev_mac:
                     device = netelem
                     break
         return device
 
     def get_device_by_serial(self, device_serial):
         ''' Returns the net element device dict for the devices serial number.
 
             Args:
                 device_serial (str): Serial number of the device.
 
             Returns:
                 device (dict): The net element device dict for the device if
                     otherwise returns an empty hash.
         '''
-        self.log.debug('get_device_by_serial: Serial Number: %s'
-                       % device_serial)
+        self.log.debug(f"get_device_by_serial: Serial Number: {device_serial}")
         data = self.search_topology(device_serial)
         device = {}
         if 'netElementList' in data:
             for netelem in data['netElementList']:
                 if netelem['serialNumber'] == device_serial:
                     device = netelem
                     break
         return device
 
-    def get_device_configuration(self, device_mac):
+    def get_device_configuration(self, dev_mac):
         ''' Returns the running configuration for the device provided.
 
             Args:
-                device_mac (str): Mac address of the device to get the running
+                dev_mac (str): Mac address of the device to get the running
                     configuration for.
 
             Returns:
                 device (dict): The net element device dict for the device if
                     otherwise returns an empty hash.
         '''
-        self.log.debug('get_device_configuration: device_mac: %s' % device_mac)
+        self.log.debug(f"get_device_configuration: dev_mac: {dev_mac}")
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion < 4.0:
-            data = self.clnt.get('/inventory/getInventoryConfiguration.do?'
-                                 'netElementId=%s' % device_mac,
+            data = self.clnt.get(f"/inventory/getInventoryConfiguration.do?netElementId={dev_mac}",
                                  timeout=self.request_timeout)
         else:
-            data = self.clnt.get('/inventory/device/config?'
-                                 'netElementId=%s' % device_mac,
+            data = self.clnt.get(f"/inventory/device/config?netElementId={dev_mac}",
                                  timeout=self.request_timeout)
         running_config = ''
         if 'output' in data:
             running_config = data['output']
         return running_config
 
-    def get_device_image_info(self, device_mac):
+    def get_device_image_info(self, dev_mac):
         ''' Return a dict of info about a device in CVP.
 
             Args:
-                device_mac (str): Mac address of the device to get the running
+                dev_mac (str): Mac address of the device to get the running
                     configuration for.
 
             Returns:
                 device_image_info (dict): Dict of image info for the device
                     if found. Otherwise returns None.
         '''
-        self.log.debug('Attempt to get net element data for %s' % device_mac)
+        self.log.debug(f"Attempt to get net element data for {dev_mac}")
         try:
             device_image_info = self.clnt.get(
-                '/provisioning/getNetElementInfoById.do?netElementId=%s'
-                % qplus(device_mac), timeout=self.request_timeout)
+                f"/provisioning/getNetElementInfoById.do?netElementId={qplus(dev_mac)}",
+                timeout=self.request_timeout)
         except CvpApiError as error:
             # Catch error when device for provided MAC is not found
             if 'Invalid Netelement id' in str(error):
-                self.log.debug('Device with MAC %s not found' % device_mac)
+                self.log.debug(f"Device with MAC {dev_mac} not found")
                 return None
             raise error
         return device_image_info
 
     def get_containers(self, start=0, end=0):
         ''' Returns a list of all the containers.
 
@@ -1025,16 +1053,16 @@
                 with associated info.
         '''
         self.log.debug('Get list of containers')
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion == 1.0:
             self.log.debug('v1 Inventory API Call')
-            return self.clnt.get('/inventory/add/searchContainers.do?'
-                                 'startIndex=%d&endIndex=%d' % (start, end))
+            return self.clnt.get(f"/inventory/add/searchContainers.do?"
+                                 f"startIndex={start}&endIndex={end}")
         self.log.debug('v2 Inventory API Call')
         containers = self.clnt.get('/inventory/containers')
         for container in containers:
             container['name'] = container['Name']
             container['key'] = container['Key']
             full_cont_info = self.get_container_by_id(
                 container['Key'])
@@ -1042,17 +1070,16 @@
                     container['Key'] != 'root'):
                 container['parentName'] = full_cont_info['parentName']
                 for cont in containers:
                     if cont['Name'] == full_cont_info['parentName']:
                         container['parentId'] = cont['Key']
                         break
                 else:
-                    self.log.debug(
-                        'No container parentId found for parentName %s',
-                        full_cont_info['parentName'])
+                    self.log.debug(f"No container parentId found for"
+                                   f" parentName {full_cont_info['parentName']}")
                     container['parentId'] = None
             else:
                 container['parentName'] = None
                 container['parentId'] = None
             container['type'] = None
             container['id'] = 21
             container['factoryId'] = 1
@@ -1065,17 +1092,17 @@
 
             Args:
                 name (str): String to search for in container names.
 
             Returns:
                 container (dict): Container info in dictionary format or None
         '''
-        self.log.debug('Get info for container %s' % name)
-        conts = self.clnt.get('/provisioning/searchTopology.do?queryParam=%s'
-                              '&startIndex=0&endIndex=0' % qplus(name))
+        self.log.debug(f"Get info for container {name}")
+        conts = self.clnt.get(f"/provisioning/searchTopology.do?queryParam={qplus(name)}"
+                              f"&startIndex=0&endIndex=0")
         if conts['total'] > 0 and conts['containerList']:
             for cont in conts['containerList']:
                 if cont['name'] == name:
                     return cont
         return None
 
     def get_container_by_id(self, key):
@@ -1083,32 +1110,32 @@
 
             Args:
                 key (str): String ID for container to find.
 
             Returns:
                 container (dict): Container info in dictionary format or None
         '''
-        self.log.debug('Get info for container %s' % key)
-        return self.clnt.get('/provisioning/getContainerInfoById.do?'
-                             'containerId=%s' % qplus(key))
+        self.log.debug(f"Get info for container {key}")
+        return self.clnt.get(f"/provisioning/getContainerInfoById.do?"
+                             f"containerId={qplus(key)}")
 
     def get_configlets_by_device_id(self, mac, start=0, end=0):
         ''' Returns the list of configlets applied to a device.
 
             Args:
                 mac (str): Device mac address (i.e. device id)
                 start (int): The first configlet entry to return.  Default is 0
                 end (int): The last configlet entry to return.  Default is 0
                     which means to return all configlet entries.  Can be a
                     large number to indicate the last configlet entry.
 
             Returns:
                 configlets (list): The list of configlets applied to the device
         '''
-        self.log.debug('get_configlets_by_device: mac: %s' % mac)
+        self.log.debug(f"get_configlets_by_device: mac: {mac}")
         data = self.get_configlets_by_netelement_id(mac, start, end)
         return data['configletList']
 
     def add_configlet_builder(self, name, config, draft=False, form=None):
         ''' Add a confilget builder and return the key for the configlet builder.
 
             Args:
@@ -1138,59 +1165,56 @@
 
             Returns:
                 key (str): The key for the configlet
         '''
         if not form:
             form = []
 
-        self.log.debug('add_configlet_builder: name: %s config: %s form: %s'
-                       % (name, config, form))
+        self.log.debug(f"add_configlet_builder: name: {name} config: {config} form: {form}")
         data = {'name': name,
                 'data': {'formList': form,
                          'main_script': {'data': config}}}
         # Create the configlet builder
-        self.clnt.post('/configlet/addConfigletBuilder.do?isDraft=%s' % draft,
+        self.clnt.post(f"/configlet/addConfigletBuilder.do?isDraft={draft}",
                        data=data, timeout=self.request_timeout)
 
         # Get the key for the configlet
-        data = self.clnt.get(
-            '/configlet/getConfigletByName.do?name=%s' % qplus(name),
-            timeout=self.request_timeout)
+        data = self.clnt.get(f"/configlet/getConfigletByName.do?name={qplus(name)}",
+                             timeout=self.request_timeout)
         return data['key']
 
     def add_configlet(self, name, config):
         ''' Add a configlet and return the key for the configlet.
 
             Args:
                 name (str): Configlet name
                 config (str): Switch config statements
 
             Returns:
                 key (str): The key for the configlet
         '''
-        self.log.debug('add_configlet: name: %s config: %s' % (name, config))
+        self.log.debug(f"add_configlet: name: {name} config: {config}")
         body = {'name': name, 'config': config}
         # Create the configlet
         self.clnt.post('/configlet/addConfiglet.do', data=body,
                        timeout=self.request_timeout)
 
         # Get the key for the configlet
-        data = self.clnt.get('/configlet/getConfigletByName.do?name=%s'
-                             % qplus(name), timeout=self.request_timeout)
+        data = self.clnt.get(f"/configlet/getConfigletByName.do?name={qplus(name)}",
+                             timeout=self.request_timeout)
         return data['key']
 
-
     def delete_configlet(self, name, key):
         ''' Delete the configlet.
 
             Args:
                 name (str): Configlet name
                 key (str): Configlet key
         '''
-        self.log.debug('delete_configlet: name: %s key: %s' % (name, key))
+        self.log.debug(f"delete_configlet: name: {name} key: {key}")
         body = [{'name': name, 'key': key}]
         # Delete the configlet
         self.clnt.post('/configlet/deleteConfiglet.do', data=body,
                        timeout=self.request_timeout)
 
     def update_configlet(self, config, key, name, wait_task_ids=False):
         ''' Update a configlet.
@@ -1200,16 +1224,15 @@
                 key (str): Configlet key
                 name (str): Configlet name
                 wait_task_ids (boolean): Wait for task IDs to generate
 
             Returns:
                 data (dict): Contains success or failure message
         '''
-        self.log.debug('update_configlet: config: %s key: %s name: %s' %
-                       (config, key, name))
+        self.log.debug(f"update_configlet: config: {config} key: {key} name: {name}")
 
         # Update the configlet
         body = {'config': config, 'key': key, 'name': name,
                 'waitForTaskIds': wait_task_ids}
         return self.clnt.post('/configlet/updateConfiglet.do', data=body,
                               timeout=self.request_timeout)
 
@@ -1252,53 +1275,47 @@
             "data": {
                 "formList": form,
                 "main_script": {
                     "data": config
                 }
             }
         }
-        debug_str = 'update_configlet_builder:' \
-                    ' config: {} key: {} name: {} form: {}'
-        self.log.debug(debug_str.format(config, key, name, form))
+        self.log.debug(f"update_configlet_builder: config: {config}"
+                       f" key: {key} name: {name} form: {form}")
         # Update the configlet builder
-        url_string = '/configlet/updateConfigletBuilder.do?' \
-                     'isDraft={}&id={}&action=save'
-        return self.clnt.post(url_string.format(draft, key),
-                              data=data, timeout=self.request_timeout)
+        url_string = f"/configlet/updateConfigletBuilder.do?isDraft={draft}&id={key}&action=save"
+        return self.clnt.post(url_string, data=data, timeout=self.request_timeout)
 
-    def update_reconcile_configlet(self, device_mac, config, key, name,
+    def update_reconcile_configlet(self, dev_mac, config, key, name,
                                    reconciled=False):
         ''' Update the reconcile configlet.
 
             Args:
-                device_mac (str): Mac address/Key for device whose reconcile
+                dev_mac (str): Mac address/Key for device whose reconcile
                     configlet is being updated
                 config (str): Reconciled config statements
                 key (str): Reconcile Configlet key
                 name (str): Reconcile Configlet name
                 reconciled (boolean): Wait for task IDs to generate
 
             Returns:
                 data (dict): Contains success or failure message
         '''
-        log_str = ('update_reconcile_configlet:'
-                   ' device_mac: {} config: {} key: {} name: {}')
-        self.log.debug(log_str.format(device_mac, config, key, name))
+        self.log.debug(f"update_reconcile_configlet: dev_mac: {dev_mac}"
+                       f" config: {config} key: {key} name: {name}")
 
-        url_str = ('/provisioning/updateReconcileConfiglet.do?'
-                   'netElementId={}')
+        url_str = f"/provisioning/updateReconcileConfiglet.do?netElementId={dev_mac}"
         body = {
             'config': config,
             'key': key,
             'name': name,
             'reconciled': reconciled,
             'unCheckedLines': '',
         }
-        return self.clnt.post(url_str.format(device_mac), data=body,
-                              timeout=self.request_timeout)
+        return self.clnt.post(url_str, data=body, timeout=self.request_timeout)
 
     def add_note_to_configlet(self, key, note):
         ''' Add a note to a configlet.
 
             Args:
                 key (str): Configlet key
                 note (str): Note to be added to configlet.
@@ -1306,131 +1323,79 @@
         data = {
             'key': key,
             'note': note,
         }
         return self.clnt.post('/configlet/addNoteToConfiglet.do',
                               data=data, timeout=self.request_timeout)
 
-    def sanitize_warnings(self, data):
-        ''' Sanitize the warnings returned after validation.
-
-            In some cases where the configlets has both errors
-            and warnings, CVP may split any warnings that have
-            `,` across multiple strings.
-            This method concats the strings back into one string
-            per warning, and correct the warningCount.
-
-            Args:
-                data (dict): A dict that contians the result
-                    of the validation operation
-            Returns:
-                response (dict): A dict that contains the result of the
-                    validation operation
-        '''
-        if "warnings" not in data:
-            # nothing to do here, we can return as is
-            return data
-        # Since there may be warnings incorrectly split on
-        # ', ' within the warning text by CVP, we join all the
-        # warnings together using ', ' into one large string
-        temp_warnings = ", ".join(data['warnings']).strip()
-
-        # To split the large string again we match on the
-        # 'at line XXX' that should indicate the end of the warning.
-        # We capture as well the remaining \\n or whitespace and include
-        # the extra ', ' added in the previous step in the matching criteria.
-        # The extra ', ' is not included in the strings of the new list
-        temp_warnings = split(
-            r'(.*?at line \d+.*?),\s+',
-            temp_warnings
-        )
-
-        # The behaviour of re.split will add empty strings
-        # if the regex matches on the begging or ending of the line.
-        # Refer to https://docs.python.org/3/library/re.html#re.split
-
-        # Use filter to remove any empty strings
-        # that re.split inserted
-        data['warnings'] = list(filter(None, temp_warnings))
-        # Update the count of warnings to the correct value
-        data['warningCount'] = len(data['warnings'])
-        return data
-
-    def validate_config_for_device(self, device_mac, config):
+    def validate_config_for_device(self, dev_mac, config):
         ''' Validate a config against a device
 
             Args:
-                device_mac (str): Device MAC address
+                dev_mac (str): Device MAC address
                 config (str): Switch config statements
 
             Returns:
                 response (dict): A dict that contains the result of the
                     validation operation
         '''
-        self.log.debug('validate_config_for_device: device_mac: %s config: %s'
-                       % (device_mac, config))
-        body = {'netElementId': device_mac, 'config': config}
-        return self.sanitize_warnings(
+        self.log.debug(f"validate_config_for_device: dev_mac: {dev_mac} config: {config}")
+        body = {'netElementId': dev_mac, 'config': config}
+        return sanitize_warnings(
             self.clnt.post(
                 '/configlet/validateConfig.do',
                 data=body,
                 timeout=self.request_timeout
             )
         )
 
-    def validate_config(self, device_mac, config):
+    def validate_config(self, dev_mac, config):
         ''' Validate a config against a device and parse response to
             produce log messages are return a flag for the config validity.
 
             Args:
-                device_mac (str): Device MAC address
+                dev_mac (str): Device MAC address
                 config (str): Switch config statements
 
             Returns:
                 response (boolean): A flag signifying if the config is valid or
                     not.
         '''
-        self.log.debug('validate_config: device_mac: %s config: %s'
-                       % (device_mac, config))
-        result = self.validate_config_for_device(device_mac, config)
+        self.log.debug(f"validate_config: dev_mac: {dev_mac} config: {config}")
+        result = self.validate_config_for_device(dev_mac, config)
         validated = True
         if 'warningCount' in result and result['warnings']:
             for warning in result['warnings']:
-                self.log.warning('Validation of config produced warning - %s'
-                                 % warning)
+                self.log.warning(f"Validation of config produced warning - {warning}")
         if 'errorCount' in result:
-            self.log.error('Validation of config produced %s errors'
-                           % result['errorCount'])
+            self.log.error(f"Validation of config produced {result['errorCount']} errors")
             if 'errors' in result:
                 for error in result['errors']:
-                    self.log.error('Validation of config produced error - %s'
-                                   % error)
+                    self.log.error(f"Validation of config produced error - {error}")
             validated = False
         if 'result' in result:
             for item in result['result']:
                 if 'messages' in item:
                     for message in item['messages']:
-                        self.log.info('Validation of config returned'
-                                      ' message - %s' % message)
+                        self.log.info(f"Validation of config returned message - {message}")
         return validated
 
     def get_all_temp_actions(self, start=0, end=0):
         ''' Returns a list of existing temp actions.
 
             Args:
                 start (int): Start index for the pagination. Default is 0.
                 end (int): End index for the pagination. If end index is 0
                     then all the records will be returned. Default is 0.
 
             Returns:
                 response (dict): A dict that contains a list of the current
                     temp actions.
         '''
-        url = ('/provisioning/getAllTempActions.do?startIndex=%d&endIndex=%d'
-               % (start, end))
+        url = (f"/provisioning/getAllTempActions.do?startIndex={start}&endIndex={end}")
         data = self.clnt.get(url, timeout=self.request_timeout)
 
         return data
 
     def _add_temp_action(self, data):
         ''' Adds temp action that requires a saveTopology call to take effect.
 
@@ -1458,15 +1423,15 @@
                     task ids created (if any).
 
                     Ex: {u'data': {u'status': u'success', u'taskIds': []}}
         '''
         url = '/provisioning/v2/saveTopology.do'
         return self.clnt.post(url, data=data, timeout=self.request_timeout)
 
-    def apply_configlets_to_device(self, app_name, dev, new_configlets,
+    def apply_configlets_to_device(self, app_name, dev, new_configlets, # pylint: disable=too-many-locals
                                    create_task=True, reorder_configlets=False, validate=False):
         ''' Apply the configlets to the device.
 
             Args:
                 app_name (str): The application name to use in info field.
                 dev (dict): The switch device dict
                 new_configlets (list): List of configlet name and key pairs
@@ -1493,16 +1458,15 @@
 
             Returns:
                 response (dict): A dict that contains a status and a list of
                     task ids created (if any).
 
                     Ex: {u'data': {u'status': u'success', u'taskIds': [u'32']}}
         '''
-        self.log.debug('apply_configlets_to_device: dev: %s names: %s' %
-                       (dev, new_configlets))
+        self.log.debug(f"apply_configlets_to_device: dev: {dev} names: {new_configlets}")
         # Get a list of the names and keys of the configlets
         cnames = []
         ckeys = []
 
         if not reorder_configlets:
             # Get all the configlets assigned to the device.
             configlets = self.get_configlets_by_device_id(
@@ -1512,15 +1476,15 @@
                 ckeys.append(configlet['key'])
 
         # Add the new configlets to the end of the arrays
         for entry in new_configlets:
             cnames.append(entry['name'])
             ckeys.append(entry['key'])
 
-        info = '%s: Configlet Assign: to Device %s' % (app_name, dev['fqdn'])
+        info = f"{app_name}: Configlet Assign: to Device {dev['fqdn']}"
         info_preview = '<b>Configlet Assign:</b> to Device' + dev['fqdn']
         data = {'data': [{'info': info,
                           'infoPreview': info_preview,
                           'note': '',
                           'action': 'associate',
                           'nodeType': 'configlet',
                           'nodeId': '',
@@ -1540,24 +1504,25 @@
                           'toName': dev['fqdn'],
                           'nodeIpAddress': dev['ipAddress'],
                           'nodeTargetIpAddress': dev['ipAddress'],
                           'childTasks': [],
                           'parentTask': ''}]}
         if validate:
             validation_result = self.validate_configlets_for_device(dev['systemMacAddress'], ckeys)
-            data['data'][0].update({
-                "configCompareCount": {
-                    "mismatch": validation_result['mismatch'],
-                    "reconcile": validation_result['reconcile'],
-                    "new": validation_result['new']
+            data['data'][0].update(
+                {
+                    "configCompareCount":
+                    {
+                        "mismatch": validation_result['mismatch'],
+                        "reconcile": validation_result['reconcile'],
+                        "new": validation_result['new']
                     }
                 }
             )
-        self.log.debug('apply_configlets_to_device: saveTopology data:\n%s' %
-                       data['data'])
+        self.log.debug(f"apply_configlets_to_device: saveTopology data:\n{data['data']}")
         self._add_temp_action(data)
         if create_task:
             return self._save_topology_v2([])
         return None
 
     # pylint: disable=too-many-locals
     def remove_configlets_from_device(self, app_name, dev, del_configlets,
@@ -1579,16 +1544,15 @@
 
             Returns:
                 response (dict): A dict that contains a status and a list of
                     task ids created (if any).
 
                     Ex: {u'data': {u'status': u'success', u'taskIds': [u'35']}}
         '''
-        self.log.debug('remove_configlets_from_device: dev: %s names: %s' %
-                       (dev, del_configlets))
+        self.log.debug(f"remove_configlets_from_device: dev: {dev} names: {del_configlets}")
 
         # Get all the configlets assigned to the device.
         configlets = self.get_configlets_by_device_id(dev['systemMacAddress'])
 
         # Get a list of the names and keys of the configlets.  Do not add
         # configlets that are on the delete list.
         keep_names = []
@@ -1604,15 +1568,15 @@
         # list of the configlets to remove.
         del_names = []
         del_keys = []
         for entry in del_configlets:
             del_names.append(entry['name'])
             del_keys.append(entry['key'])
 
-        info = '%s Configlet Remove: from Device %s' % (app_name, dev['fqdn'])
+        info = f"{app_name} Configlet Remove: from Device {dev['fqdn']}"
         info_preview = '<b>Configlet Remove:</b> from Device' + dev['fqdn']
         data = {'data': [{'info': info,
                           'infoPreview': info_preview,
                           'note': '',
                           'action': 'associate',
                           'nodeType': 'configlet',
                           'nodeId': '',
@@ -1631,25 +1595,26 @@
                           'fromName': '',
                           'toName': dev['fqdn'],
                           'nodeIpAddress': dev['ipAddress'],
                           'nodeTargetIpAddress': dev['ipAddress'],
                           'childTasks': [],
                           'parentTask': ''}]}
         if validate:
-            validation_result = self.validate_configlets_for_device(dev['systemMacAddress'], keep_keys)
-            data['data'][0].update({
-                "configCompareCount": {
-                    "mismatch": validation_result['mismatch'],
-                    "reconcile": validation_result['reconcile'],
-                    "new": validation_result['new']
+            validation_result = self.validate_configlets_for_device(dev['systemMacAddress'],
+                                                                    keep_keys)
+            data['data'][0].update(
+                {
+                    "configCompareCount": {
+                        "mismatch": validation_result['mismatch'],
+                        "reconcile": validation_result['reconcile'],
+                        "new": validation_result['new']
                     }
                 }
             )
-        self.log.debug('remove_configlets_from_device: saveTopology data:\n%s'
-                       % data['data'])
+        self.log.debug(f"remove_configlets_from_device: saveTopology data:\n{data['data']}")
         self._add_temp_action(data)
         if create_task:
             return self._save_topology_v2([])
         return None
 
     def apply_configlets_to_container(self, app_name, container,
                                       new_configlets, create_task=True):
@@ -1664,17 +1629,16 @@
 
             Returns:
                 response (dict): A dict that contains a status and a list of
                     task ids created (if any).
 
                     Ex: {u'data': {u'status': u'success', u'taskIds': [u'32']}}
         '''
-        self.log.debug(
-            'apply_configlets_to_container: container: %s names: %s' %
-            (container, new_configlets))
+        self.log.debug(f"apply_configlets_to_container: container: {container}"
+                       f" names: {new_configlets}")
         # Get all the configlets assigned to the device.
         configlets = self.get_configlets_by_container_id(container['key'])
 
         # Get a list of the names and keys of the configlets
         # Static Configlets
         cnames = []
         ckeys = []
@@ -1691,16 +1655,15 @@
                     bkeys.append(configlet['key'])
 
                     # Add the new configlets to the end of the arrays
         for entry in new_configlets:
             cnames.append(entry['name'])
             ckeys.append(entry['key'])
 
-        info = '%s: Configlet Assign: to Container %s' % (app_name,
-                                                          container['name'])
+        info = f"{app_name}: Configlet Assign: to Container {container['name']}"
         info_preview = '<b>Configlet Assign:</b> to Container' + container[
             'name']
         data = {'data': [{'info': info,
                           'infoPreview': info_preview,
                           'note': '',
                           'action': 'associate',
                           'nodeType': 'configlet',
@@ -1719,17 +1682,15 @@
                           'nodeName': '',
                           'fromName': '',
                           'toName': container['name'],
                           'nodeIpAddress': '',
                           'nodeTargetIpAddress': '',
                           'childTasks': [],
                           'parentTask': ''}]}
-        self.log.debug(
-            'apply_configlets_to_container: saveTopology data:\n%s' %
-            data['data'])
+        self.log.debug(f"apply_configlets_to_container: saveTopology data:\n{data['data']}")
         self._add_temp_action(data)
         if create_task:
             return self._save_topology_v2([])
         return data
 
     # pylint: disable=too-many-locals
     # pylint: disable=invalid-name
@@ -1746,17 +1707,16 @@
 
             Returns:
                 response (dict): A dict that contains a status and a list of
                     task ids created (if any).
 
                     Ex: {u'data': {u'status': u'success', u'taskIds': [u'35']}}
         '''
-        self.log.debug(
-            'remove_configlets_from_container: container: %s names: %s' %
-            (container, del_configlets))
+        self.log.debug(f"remove_configlets_from_container: container: {container}"
+                       f" names: {del_configlets}")
 
         # Get all the configlets assigned to the device.
         configlets = self.get_configlets_by_container_id(container['key'])
 
         # Get a list of the names and keys of the configlets.  Do not add
         # configlets that are on the delete list.
         keep_names = []
@@ -1772,16 +1732,15 @@
         # list of the configlets to remove.
         del_names = []
         del_keys = []
         for entry in del_configlets:
             del_names.append(entry['name'])
             del_keys.append(entry['key'])
 
-        info = '%s Configlet Remove: from Container %s' % (app_name,
-                                                           container['name'])
+        info = f"{app_name} Configlet Remove: from Container {container['name']}"
         info_preview = '<b>Configlet Remove:</b> from Container' + container[
             'name']
         data = {'data': [{'info': info,
                           'infoPreview': info_preview,
                           'note': '',
                           'action': 'associate',
                           'nodeType': 'configlet',
@@ -1800,17 +1759,15 @@
                           'nodeName': '',
                           'fromName': '',
                           'toName': container['name'],
                           'nodeIpAddress': '',
                           'nodeTargetIpAddress': '',
                           'childTasks': [],
                           'parentTask': ''}]}
-        self.log.debug(
-            'remove_configlets_from_container: saveTopology data:\n%s'
-            % data['data'])
+        self.log.debug(f"remove_configlets_from_container: saveTopology data:\n{data['data']}")
         self._add_temp_action(data)
         if create_task:
             return self._save_topology_v2([])
         return data
 
     def validate_configlets_for_device(self, mac, configlet_keys,
                                        page_type='viewConfig'):
@@ -1835,17 +1792,16 @@
                          "mismatch": 0,
                          "warnings": [""],
                          "errors": [{"configletLineNo": 0,
                                      "error": "string",
                                      "configletId": "string"}, ...]
                         }
         '''
-        self.log.debug('validate_configlets_for_device: '
-                       'MAC: %s - conf keys: %s - page_type: %s' %
-                       (mac, configlet_keys, page_type))
+        self.log.debug(f"validate_configlets_for_device: "
+                       f"MAC: {mac} - conf keys: {configlet_keys} - page_type: {page_type}")
         data = {'configIdList': configlet_keys,
                 'netElementId': mac,
                 'pageType': page_type}
         return self.clnt.post(
             '/provisioning/v2/validateAndCompareConfiglets.do',
             data=data, timeout=self.request_timeout)
 
@@ -1854,32 +1810,30 @@
 
             Args:
                 configlet_name (str): The name of the configlet to be queried.
                 start (int): Start index for the pagination. Default is 0.
                 end (int): End index for the pagination. If end index is 0
                     then all the records will be returned. Default is 0.
         '''
-        return self.clnt.get('/configlet/getAppliedDevices.do?'
-                             'configletName=%s&startIndex=%d&endIndex=%d'
-                             % (configlet_name, start, end),
+        return self.clnt.get(f"/configlet/getAppliedDevices.do?"
+                             f"configletName={configlet_name}&startIndex={start}&endIndex={end}",
                              timeout=self.request_timeout)
 
     def get_applied_containers(self, configlet_name, start=0, end=0):
         ''' Returns a list of containers to which the named
             configlet is applied.
 
             Args:
                 configlet_name (str): The name of the configlet to be queried.
                 start (int): Start index for the pagination. Default is 0.
                 end (int): End index for the pagination. If end index is 0
                     then all the records will be returned. Default is 0.
         '''
-        return self.clnt.get('/configlet/getAppliedContainers.do?'
-                             'configletName=%s&startIndex=%d&endIndex=%d'
-                             % (configlet_name, start, end),
+        return self.clnt.get(f"/configlet/getAppliedContainers.do?"
+                             f"configletName={configlet_name}&startIndex={start}&endIndex={end}",
                              timeout=self.request_timeout)
 
     # pylint: disable=too-many-arguments
     def _container_op(self, container_name, container_key, parent_name,
                       parent_key, operation):
         ''' Perform the operation on the container.
 
@@ -1892,16 +1846,15 @@
 
             Returns:
                 response (dict): A dict that contains a status and a list of
                     task ids created (if any).
 
                     Ex: {u'data': {u'status': u'success', u'taskIds': []}}
         '''
-        msg = ('%s container %s under container %s' %
-               (operation, container_name, parent_name))
+        msg = (f"{operation} container {container_name} under container {parent_name}")
         data = {'data': [{'info': msg,
                           'infoPreview': msg,
                           'action': operation,
                           'nodeType': 'container',
                           'nodeId': container_key,
                           'toId': '',
                           'fromId': '',
@@ -1932,16 +1885,16 @@
 
             Returns:
                 response (dict): A dict that contains a status and a list of
                     task ids created (if any).
 
                     Ex: {u'data': {u'status': u'success', u'taskIds': []}}
         '''
-        self.log.debug('add_container: container: %s parent: %s parent_key: %s'
-                       % (container_name, parent_name, parent_key))
+        self.log.debug(f"add_container: container: {container_name}"
+                       f" parent: {parent_name} parent_key: {parent_key}")
         return self._container_op(container_name, 'new_container', parent_name,
                                   parent_key, 'add')
 
     def delete_container(self, container_name, container_key, parent_name,
                          parent_key):
         ''' Add the container to the specified parent.
 
@@ -1953,50 +1906,47 @@
 
             Returns:
                 response (dict): A dict that contains a status and a list of
                     task ids created (if any).
 
                     Ex: {u'data': {u'status': u'success', u'taskIds': []}}
         '''
-        self.log.debug('delete_container: container: %s container_key: %s '
-                       'parent: %s parent_key: %s' %
-                       (container_name, container_key, parent_name,
-                        parent_key))
+        self.log.debug(f"delete_container: container: {container_name}"
+                       f" container_key: {container_key} parent: {parent_name}"
+                       f" parent_key: {parent_key}")
         resp = self._container_op(container_name, container_key, parent_name,
                                   parent_key, 'delete')
         # As of CVP version 2020.1 the addTempAction.do API endpoint stopped
         # raising an Error when attempting to delete a container with children.
         # To account for this try to see if the container being deleted
         # still exists after the attempted delete. If it still exists
         # raise an error similar to how CVP behaved prior to CVP 2020.1
         try:
             still_exists = self.get_container_by_id(container_key)
         except CvpApiError as error:
             if 'Invalid Container id' in error.msg:
                 return resp
-            else:
-                raise
+            raise
         if still_exists is not None:
             raise CvpApiError('Container was not deleted. Check for children')
         return resp
 
-    def get_parent_container_for_device(self, device_mac):
+    def get_parent_container_for_device(self, dev_mac):
         ''' Add the container to the specified parent.
 
             Args:
-                device_mac (str): Device mac address
+                dev_mac (str): Device mac address
 
             Returns:
                 response (dict): A dict that contains the parent container info
         '''
-        self.log.debug('get_parent_container_for_device: called for %s'
-                       % device_mac)
-        data = self.clnt.get('/provisioning/searchTopology.do?'
-                             'queryParam=%s&startIndex=0&endIndex=0'
-                             % device_mac, timeout=self.request_timeout)
+        self.log.debug(f"get_parent_container_for_device: called for {dev_mac}")
+        data = self.clnt.get(f"/provisioning/searchTopology.do?"
+                             f"queryParam={dev_mac}&startIndex=0&endIndex=0",
+                             timeout=self.request_timeout)
         if data['total'] > 0:
             cont_name = data['netElementContainerList'][0]['containerName']
             return self.get_container_by_name(cont_name)
         return None
 
     def move_device_to_container(self, app_name, device, container,
                                  create_task=True):
@@ -2011,19 +1961,17 @@
 
             Returns:
                 response (dict): A dict that contains a status and a list of
                     task ids created (if any).
 
                     Ex: {u'data': {u'status': u'success', u'taskIds': []}}
         '''
-        info = 'Device Add {} to container {} by {}'.format(device['fqdn'],
-                                                            container['name'],
-                                                            app_name)
-        self.log.debug('Attempting to move device %s to container %s'
-                       % (device['fqdn'], container['name']))
+        info = f"Device Add {device['fqdn']} to container {container['name']} by {app_name}"
+        self.log.debug(f"Attempting to move device {device['fqdn']} to"
+                       f" container {container['name']}")
         if 'parentContainerId' in device:
             from_id = device['parentContainerId']
         else:
             parent_cont = self.get_parent_container_for_device(device['key'])
             from_id = parent_cont['key']
         data = {'data': [{'info': info,
                           'infoPreview': info,
@@ -2038,16 +1986,15 @@
                           'childTasks': [],
                           'parentTask': ''}]}
         try:
             self._add_temp_action(data)
         # pylint: disable=invalid-name
         except CvpApiError as e:
             if 'Data already exists' in str(e):
-                self.log.debug('Device %s already in container %s'
-                               % (device['fqdn'], container))
+                self.log.debug(f"Device {device['fqdn']} already in container {container}")
         if create_task:
             return self._save_topology_v2([])
         return None
 
     def search_topology(self, query, start=0, end=0):
         ''' Search the topology for items matching the query parameter.
 
@@ -2058,28 +2005,43 @@
                 end (int): End index for the pagination.  If end index is 0
                     then all the records will be returned.  Default is 0.
 
             Returns:
                 response (dict): A dict that contains the container and
                     netelement lists.
         '''
-        self.log.debug('search_topology: query: %s start: %d end: %d' %
-                       (query, start, end))
-        data = self.clnt.get('/provisioning/searchTopology.do?queryParam=%s&'
-                             'startIndex=%d&endIndex=%d'
-                             % (qplus(query), start, end),
-                             timeout=self.request_timeout)
+        self.log.debug(f"search_topology: query: {query} start: {start} end: {end}")
+        if self.clnt.apiversion is None:
+            self.get_cvp_info()
+        if self.clnt.apiversion <= 6.0:
+            # Original search topology endpoint
+            req_url = (f"/provisioning/searchTopology.do?queryParam={qplus(query)}&"
+                       f"startIndex={start}&endIndex={end}")
+        else:
+            # Newer CVP versions should use the V3 version of search topology endpoint
+            req_url = (f"/provisioning/v3/searchTopology.do?queryParam={qplus(query)}&"
+                       f"startIndex={start}&endIndex={end}")
+
+        data = self.clnt.get(req_url, timeout=self.request_timeout)
         if 'netElementList' in data:
             for device in data['netElementList']:
                 device['status'] = device['deviceStatus']
-                device['mlagEnabled'] = device['isMLAGEnabled']
-                device['danzEnabled'] = device['isDANZEnabled']
                 device['parentContainerKey'] = device['parentContainerId']
-                device['bootupTimestamp'] = device['bootupTimeStamp']
-                device['internalBuild'] = device['internalBuildId']
+                if 'isMLAGEnabled' in device:
+                    # original key was mlagEnabled but it changed to isMLAGEnabled
+                    device['mlagEnabled'] = device['isMLAGEnabled']
+                elif 'mlagEnabled' in device:
+                    # Key for V3 search topology changes back to mlagEnabled again
+                    device['isMLAGEnabled'] = device['mlagEnabled']
+                # Key isDANZEnabled for V3 search topology is no longer in return data.
+                device['danzEnabled'] = device.get('isDANZEnabled', '')
+                # Key bootupTimeStamp for V3 search topology is no longer in return data.
+                device['bootupTimestamp'] = device.get('bootupTimeStamp', '')
+                # Key internalBuildId for V3 search topology is no longer in return data.
+                device['internalBuild'] = device.get('internalBuildId', '')
         return data
 
     def filter_topology(self, node_id='root', fmt='topology',
                         start=0, end=0):
         ''' Filter the CVP topology for container and device information.
 
             Args:
@@ -2087,17 +2049,16 @@
                     Default is 'root', for the Tenant container.
                 fmt (str): The type of filter to return. Must be either
                     'topology' or 'list'. Default is 'topology'.
                 start (int): Start index for the pagination. Default is 0.
                 end (int): End index for the pagination. If end index is 0
                     then all the records will be returned. Default is 0.
         '''
-        url = ('/provisioning/filterTopology.do?nodeId=%s&'
-               'format=%s&startIndex=%d&endIndex=%d'
-               % (node_id, fmt, start, end))
+        url = (f"/provisioning/filterTopology.do?nodeId={node_id}&"
+               f"format={fmt}&startIndex={start}&endIndex={end}")
         return self.clnt.get(url, timeout=self.request_timeout)
 
     def check_compliance(self, node_key, node_type):
         ''' Check that a device is in compliance, that is the configlets
             applied to the device match the devices running configuration.
 
             Args:
@@ -2106,33 +2067,32 @@
                 node_type (str): The device type. This is either 'netelement'
                     or 'container'
 
             Returns:
                 response (dict): A dict that contains the results of the
                     compliance check.
         '''
-        self.log.debug('check_compliance: node_key: %s node_type: %s' %
-                       (node_key, node_type))
+        self.log.debug(f"check_compliance: node_key: {node_key} node_type: {node_type}")
         data = {'nodeId': node_key, 'nodeType': node_type}
         resp = self.clnt.post('/provisioning/checkCompliance.do', data=data,
                               timeout=self.request_timeout)
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion >= 2.0:
-            if resp['complianceIndication'] == u'':
+            if resp['complianceIndication'] == '':
                 resp['complianceIndication'] = 'NONE'
         return resp
 
     def get_event_by_id(self, e_id):
         ''' Return information on the requested event ID.
 
             Args:
                 e_id (str): The event id to be queried.
         '''
-        return self.clnt.get('/event/getEventById.do?eventId=%s' % e_id,
+        return self.clnt.get(f"/event/getEventById.do?eventId={e_id}",
                              timeout=self.request_timeout)
 
     def get_default_snapshot_template(self):
         ''' Return the default snapshot template.
 
         '''
         if self.clnt.apiversion is None:
@@ -2179,17 +2139,17 @@
                 filepath (str): Local path to the image to upload.
 
             Returns:
                 data (dict): Dictionary of image add data.
         '''
         # Get the absolute file path to be uploaded
         image_path = os.path.abspath(filepath)
-        image_data = open(image_path, 'rb')
-        response = self.clnt.post('/image/addImage.do',
-                                  files={'file': image_data})
+        with open(image_path, 'rb') as image_data:
+            response = self.clnt.post('/image/addImage.do',
+                                      files={'file': image_data})
         return response
 
     def cancel_image(self, image_name):
         ''' Discard/cancel the uploaded image/image bundle before save.
 
             Args:
                 image_name (string): Name of image to cancel/discard.
@@ -2210,17 +2170,16 @@
                     then all the records will be returned.  Default is 0.
 
             Returns:
                 images (dict): The 'total' key contains the number of images,
                     the 'data' key contains a list of images and their info.
         '''
         self.log.debug('Get info about images')
-        return self.clnt.get('/image/getImages.do?queryparam=&startIndex=%d&'
-                             'endIndex=%d' % (start, end),
-                             timeout=self.request_timeout)
+        return self.clnt.get(f"/image/getImages.do?queryparam=&startIndex={start}&"
+                             f"endIndex={end}", timeout=self.request_timeout)
 
     def get_image_bundles(self, start=0, end=0):
         ''' Return a list of all image bundles.
 
             Args:
                 start (int): Start index for the pagination.  Default is 0.
                 end (int): End index for the pagination.  If end index is 0
@@ -2229,36 +2188,36 @@
             Returns:
                 image bundles (dict): The 'total' key contains the number of
                     image bundles, the 'data' key contains a list of image
                     bundles and their info.
         '''
         self.log.debug('Get image bundles that can be applied to devices or'
                        ' containers')
-        return self.clnt.get('/image/getImageBundles.do?queryparam=&'
-                             'startIndex=%d&endIndex=%d' % (start, end),
+        return self.clnt.get(f"/image/getImageBundles.do?queryparam=&"
+                             f"startIndex={start}&endIndex={end}",
                              timeout=self.request_timeout)
 
     def get_image_bundle_by_name(self, name):
         ''' Return a dict of info about an image bundle.
 
             Args:
                 name (str): Name of image bundle to return info about.
 
             Returns:
                 image bundle (dict): Dict of info specific to the image bundle
                     requested or None if the name requested doesn't exist.
         '''
-        self.log.debug('Attempt to get image bundle %s' % name)
+        self.log.debug(f"Attempt to get image bundle {name}")
         try:
-            image = self.clnt.get('/image/getImageBundleByName.do?name=%s'
-                                  % qplus(name), timeout=self.request_timeout)
+            image = self.clnt.get(f"/image/getImageBundleByName.do?name={qplus(name)}",
+                                  timeout=self.request_timeout)
         except CvpApiError as error:
             # Catch an invalid task_id error and return None
             if 'Entity does not exist' in str(error):
-                self.log.debug('Bundle with name %s does not exist' % name)
+                self.log.debug(f"Bundle with name {name} does not exist")
                 return None
             raise error
         return image
 
     def delete_image_bundle(self, image_key, image_name):
         ''' Delete image bundle
 
@@ -2358,32 +2317,30 @@
             Returns:
                 response (dict): A dict that contains a status and a list of
                     task ids created (if any). Image updates will not run until
                     task or tasks are executed.
 
                     Ex: {u'data': {u'status': u'success', u'taskIds': [u'32']}}
         '''
-        self.log.debug('Attempt to apply %s to %s %s' % (image['name'],
-                                                         id_type, name))
-        info = 'Apply image: %s to %s %s' % (image['name'], id_type, name)
+        self.log.debug(f"Attempt to apply {image['name']} to {id_type} {name}")
+        info = f"Apply image: {image['name']} to {id_type} {name}"
         node_id = ''
         if 'imageBundleKeys' in image:
             if image['imageBundleKeys']:
                 node_id = image['imageBundleKeys'][0]
-            self.log.info('Provided image is an image object.'
-                          ' Using first value from imageBundleKeys - %s'
-                          % node_id)
+            self.log.info(f"Provided image is an image object."
+                          f" Using first value from imageBundleKeys - {node_id}")
         if 'id' in image:
             node_id = image['id']
-            self.log.info('Provided image is an image bundle object.'
-                          ' Found v1 API id field - %s' % node_id)
+            self.log.info(f"Provided image is an image bundle object."
+                          f" Found v1 API id field - {node_id}")
         elif 'key' in image:
             node_id = image['key']
-            self.log.info('Provided image is an image bundle object.'
-                          ' Found v2 API key field - %s' % node_id)
+            self.log.info(f"Provided image is an image bundle object."
+                          f" Found v2 API key field - {node_id}")
         data = {'data': [{'info': info,
                           'infoPreview': info,
                           'note': '',
                           'action': 'associate',
                           'nodeType': 'imagebundle',
                           'nodeId': node_id,
                           'toId': element['key'],
@@ -2442,31 +2399,30 @@
 
             Returns:
                 response (dict): A dict that contains a status and a list of
                     task ids created (if any).
 
                     Ex: {u'data': {u'status': u'success', u'taskIds': [u'32']}}
         '''
-        self.log.debug('Attempt to remove %s from %s' % (image['name'], name))
-        info = 'Remove image: %s from %s' % (image['name'], name)
+        self.log.debug(f"Attempt to remove {image['name']} from {name}")
+        info = f"Remove image: {image['name']} from {name}"
         node_id = ''
         if 'imageBundleKeys' in image:
             if image['imageBundleKeys']:
                 node_id = image['imageBundleKeys'][0]
-            self.log.info('Provided image is an image object.'
-                          ' Using first value from imageBundleKeys - %s'
-                          % node_id)
+            self.log.info(f"Provided image is an image object."
+                          f" Using first value from imageBundleKeys - {node_id}")
         if 'id' in image:
             node_id = image['id']
-            self.log.info('Provided image is an image bundle object.'
-                          ' Found v1 API id field - %s' % node_id)
+            self.log.info(f"Provided image is an image bundle object."
+                          f" Found v1 API id field - {node_id}")
         elif 'key' in image:
             node_id = image['key']
-            self.log.info('Provided image is an image bundle object.'
-                          ' Found v2 API key field - %s' % node_id)
+            self.log.info(f"Provided image is an image bundle object."
+                          f" Found v2 API key field - {node_id}")
         data = {'data': [{'info': info,
                           'infoPreview': info,
                           'note': '',
                           'action': 'associate',
                           'nodeType': 'imagebundle',
                           'nodeId': '',
                           'toId': element['key'],
@@ -2490,27 +2446,27 @@
                 start (int): Start index for the pagination.  Default is 0.
                 end (int): End index for the pagination.  If end index is 0
                     then all the records will be returned.  Default is 0.
 
             Returns:
                 change controls (list): The list of change controls
         '''
-        self.log.debug('get_change_controls: query: %s' % query)
+        self.log.debug(f"get_change_controls: query: {query}")
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion >= 3.0:
             self.log.debug('v3/v4/v5 getChangeControls API Call')
             self.log.warning(
                 'get_change_controls: change control APIs moved for v3/v4/v5')
             return None
 
         self.log.debug('v2 getChangeControls API Call')
         data = self.clnt.get(
-            '/changeControl/getChangeControls.do?searchText=%s'
-            '&startIndex=%d&endIndex=%d' % (qplus(query), start, end),
+            f"/changeControl/getChangeControls.do?searchText={qplus(query)}"
+            f"&startIndex={start}&endIndex={end}",
             timeout=self.request_timeout)
         if 'data' not in data:
             return None
         return data['data']
 
     def change_control_available_tasks(self, query='', start=0, end=0):
         ''' Returns a list of tasks that are available for a change control.
@@ -2520,26 +2476,26 @@
                 start (int): Start index for the pagination.  Default is 0.
                 end (int): End index for the pagination.  If end index is 0
                     then all the records will be returned.  Default is 0.
 
             Returns:
                 tasks (list): The list of available tasks
         '''
-        self.log.debug('change_control_available_tasks: query: %s' % query)
+        self.log.debug(f"change_control_available_tasks: query: {query}")
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion >= 3.0:
             self.log.debug(
                 'v3/v4/v5 uses existing get_task_by_status API Call')
             return self.get_tasks_by_status('PENDING')
 
         self.log.debug('v2 getTasksByStatus API Call')
         data = self.clnt.get(
-            '/changeControl/getTasksByStatus.do?searchText=%s'
-            '&startIndex=%d&endIndex=%d' % (qplus(query), start, end),
+            f"/changeControl/getTasksByStatus.do?searchText={qplus(query)}"
+            f"&startIndex={start}&endIndex={end}",
             timeout=self.request_timeout)
         if 'data' not in data:
             return None
         return data['data']
 
     def create_change_control(self, name, change_control_tasks, timezone,
                               country_id, date_time, snapshot_template_key='',
@@ -2640,40 +2596,39 @@
                 Ex: [{u'id': u'cc_id',
                       u'update_timestamp': u'...'}]
         '''
         self.log.debug('create_change_control_v3')
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion < 3.0:
-            self.log.debug('Wrong method for API version %s.'
-                           ' Use create_change_control method',
-                           self.clnt.apiversion)
+            self.log.debug(f"Wrong method for API version {self.clnt.apiversion}."
+                           f" Use create_change_control method")
             self.log.warning('create_change_control_v3:'
                              ' Use old change control APIs for old versions')
             return None
 
         self.log.debug('v3 Update change control API Call')
         stages = []
         if sequential:
             for index, task in enumerate(tasks):
-                stage_id = 'stage%d' % index
+                stage_id = f"stage{index}"
                 stage = {'stage': [{
                     'id': stage_id,
                     'action': {
                         'name': 'task',
                         'args': {
                             'TaskID': task,
                         }
                     }
                 }]}
                 stages.append(stage)
         else:
             stage_rows = []
             for index, task in enumerate(tasks):
-                stage_id = 'stage%d' % index
+                stage_id = f"stage{index}"
                 stage_row = {
                     'id': stage_id,
                     'action': {
                         'name': 'task',
                         'args': {
                             'TaskID': task,
                         }
@@ -2700,16 +2655,15 @@
                 notes (string): The notes to add to the change control.
 
             Returns:
                 response (dict): A dict that contains...
 
                 Ex: {"data": "success"}
         '''
-        self.log.debug('add_notes_to_change_control: cc_id %s, notes %s'
-                       % (cc_id, notes))
+        self.log.debug(f"add_notes_to_change_control: cc_id {cc_id}, notes {notes}")
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion >= 3.0:
             self.log.debug(
                 'v3/v4/v5 addNotesToChangeControl API Call deprecated')
             self.log.warning('add_notes_to_change_control:'
                              ' change control APIs not supported for v3/v4/v5')
@@ -2756,17 +2710,16 @@
         '''
         if not timestamp:
             timestamp = datetime.utcnow().isoformat() + 'Z'
         self.log.debug('approve_change_control')
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion < 3.0:
-            self.log.debug('Approval methods not valid for API version %s.'
-                           ' Functionality did not exist',
-                           self.clnt.apiversion)
+            self.log.debug(f"Approval methods not valid for API version {self.clnt.apiversion}."
+                           f" Functionality did not exist")
             return None
 
         self.log.debug('v3 Approve change control API Call')
         data = {'cc_id': cc_id, 'cc_timestamp': timestamp}
         return self.clnt.post(
             '/api/v3/services/ccapi.ChangeControl/AddApproval',
             data=data, timeout=self.request_timeout)
@@ -2777,17 +2730,16 @@
             Args:
                 cc_id (string): The change control IDs to be approved.
         '''
         self.log.debug('delete_change_control_approval')
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion < 3.0:
-            self.log.debug('Approval methods not valid for API version %s.'
-                           ' Functionality did not exist',
-                           self.clnt.apiversion)
+            self.log.debug(f"Approval methods not valid for API version {self.clnt.apiversion}."
+                           f" Functionality did not exist")
             return None
 
         self.log.debug('v3 Delete Approval for change control API Call')
         data = {'cc_id': cc_id}
         return self.clnt.post(
             '/api/v3/services/ccapi.ChangeControl/DeleteApproval',
             data=data, timeout=self.request_timeout)
@@ -2892,30 +2844,30 @@
                      'stopOnError': False,
                      'taskCount': 1,
                      'taskEndTime': 0,
                      'taskStartTime': 0,
                      'timeZone': '',
                      'type': 'Custom'}
         '''
-        self.log.debug('get_change_control_info: %s', cc_id)
+        self.log.debug(f"get_change_control_info: {cc_id}")
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion >= 3.0:
             self.log.debug('get_change_control_info method deprecated for'
                            ' v3/v4/v5. Moved to get_change_control_status')
             self.log.warning('get_change_control_info:'
                              ' info change control API moved for v3/v4/v5 to'
                              ' status')
             return None
 
         self.log.debug('v2 getChangeControlInformation.do API Call')
         try:
             resp = self.clnt.get(
-                '/changeControl/getChangeControlInformation.do?'
-                'startIndex=0&endIndex=0&ccId=%s' % cc_id,
+                f"/changeControl/getChangeControlInformation.do?"
+                f"startIndex=0&endIndex=0&ccId={cc_id}",
                 timeout=self.request_timeout)
         except CvpApiError as error:
             if 'No data found' in error.msg:
                 return None
             raise
         return resp
 
@@ -2936,22 +2888,21 @@
                                               u'state': u'Completed'},
                                           u'Task_0_1': {
                                               u'error': u'',
                                               u'state': u'Completed'}
                                          },
                               u'state': u'Completed'}}]
         '''
-        self.log.debug('get_change_control_status: %s', cc_id)
+        self.log.debug(f"get_change_control_status: {cc_id}")
         if self.clnt.apiversion is None:
             self.get_cvp_info()
         if self.clnt.apiversion < 3.0:
-            self.log.debug('get_change_control_status method not supported'
-                           ' for API version %s. Use old'
-                           ' get_change_control_info method'
-                           % self.clnt.apiversion)
+            self.log.debug(f"get_change_control_status method not supported"
+                           f" for API version {self.clnt.apiversion}. Use old"
+                           f" get_change_control_info method")
             return None
 
         self.log.debug(
             'v3 /api/v3/services/ccapi.ChangeControl/GetStatus API Call')
         data = {'cc_id': cc_id}
         return self.clnt.post(
             '/api/v3/services/ccapi.ChangeControl/GetStatus',
@@ -2968,16 +2919,15 @@
 
             Returns:
                 response (dict): A dict that contains a status and a list of
                     task ids created (if any).
 
                     Ex: {u'data': {u'status': u'success', u'taskIds': []}}
         '''
-        info = ('App %s resetting device %s and moving it to Undefined'
-                % (app_name, device['fqdn']))
+        info = (f"App {app_name} resetting device {device['fqdn']} and moving it to Undefined")
         self.log.debug(info)
 
         if 'parentContainerId' in device:
             from_id = device['parentContainerId']
         else:
             parent_cont = self.get_parent_container_for_device(device['key'])
             if parent_cont and 'key' in parent_cont:
@@ -2997,16 +2947,15 @@
                           'toIdType': 'container',
                           'childTasks': [],
                           'parentTask': ''}]}
         try:
             self._add_temp_action(data)
         except CvpApiError as error:
             if 'Data already exists' in str(error):
-                self.log.debug('Device %s already in container Undefined'
-                               % device['fqdn'])
+                self.log.debug(f"Device {device['fqdn']} already in container Undefined")
         if create_task:
             return self._save_topology_v2([])
         return None
 
     def deploy_device(self, device, container, configlets=None,
                       image_bundle=None, create_task=True,
                       app_name='Deploy_device'):
@@ -3024,25 +2973,25 @@
 
             Returns:
                 response (dict): A dict that contains a status and a list of
                     task ids created (if any).
 
                     Ex: {u'data': {u'status': u'success', u'taskIds': [u'32']}}
         '''
-        info = 'Deploy device %s to container %s' % (device['fqdn'], container)
+        info = f"Deploy device {device['fqdn']} to container {container}"
         self.log.debug(info)
         container_info = self.get_container_by_name(container)
         # Add action for moving device to specified container
         self.move_device_to_container(app_name, device, container_info,
                                       create_task=False)
 
         # Get proposed configlets device will inherit from container it is
         # being moved to.
-        prop_conf = self.clnt.get('/provisioning/getTempConfigsByNetElementId.'
-                                  'do?netElementId=%s' % device['key'])
+        prop_conf = self.clnt.get(f"/provisioning/getTempConfigsByNetElementId."
+                                  f"do?netElementId={device['key']}")
         new_configlets = prop_conf['proposedConfiglets']
         if configlets:
             new_configlets.extend(configlets)
         self.apply_configlets_to_device('deploy_device', device,
                                         new_configlets, create_task=False)
         # Apply image to the device
         if image_bundle:
@@ -3057,48 +3006,49 @@
         ''' Create TerminAttr enrollment token for device authentication
             via certificates.
 
             Args:
                devices (list): list of device Serial Numbers for which the
                    token should be generated. The default is all devices.
                duration (string): the token's validity time (max 1 month),
-                  accepted formats are: "24h", "86400s", "60m"
+                  accepted formats for the legacy endpoint: "24h", "86400s", "60m"
+                  accepted format for the new endpoint: "86400s" (only seconds)
             Returns:
                 response (list) on CVaaS: A list that contains the generated
                     enrollment token.
 
                     Ex: [{'enrollmentToken':{'token': <token>, 'groups': [],
                     'reenrollDevices': <devices list>,
-                    'validFor': <duration e.g 24h>, 'field_mask': None}}]
+                    'validFor': <duration e.g 86400s>, 'field_mask': None}}]
                 response (dict) on CV on-prem: A dictionary that contains the
                     generated enrollment token.
 
                     Ex: {'data': <token>}
         '''
+        endpoint_legacy = '/cvpservice/enroll/createToken'
+        endpoint = '/api/resources/admin.Enrollment/AddEnrollmentToken'
         if not devices:
             devices = ["*"]
         # For on-prem check the version as it is only supported from 2021.2.0+
         if not self.clnt.is_cvaas:
             if self.clnt.apiversion is None:
                 self.get_cvp_info()
+            # TODO: update this check when 2024.2.0 is released
             if self.clnt.apiversion >= 6.0:
                 self.log.debug('v6 /cvpservice/enroll/createToken')
                 data = {"reenrollDevices": devices, "duration": duration}
-                return self.clnt.post('/cvpservice/enroll/createToken',
-                                      data=data, timeout=self.request_timeout)
+                return self.clnt.post(endpoint_legacy, data=data, timeout=self.request_timeout)
             self.log.warning(
                 'Enrollment Tokens only supported on CVP 2021.2.0+')
             return None
         data = {
             "enrollmentToken": {"reenrollDevices": devices,
                                 "validFor": duration}
         }
-        return self.clnt.post(
-            '/api/v3/services/admin.Enrollment/AddEnrollmentToken',
-            data=data, timeout=self.request_timeout)
+        return self.clnt.post(endpoint, data=data, timeout=self.request_timeout)
 
     def get_all_tags(self, element_type='ELEMENT_TYPE_UNSPECIFIED', workspace_id=''):
         ''' Get all device and/or interface tags from the mainline workspace or all other workspaces
             Args:
                element_type (str): Can be ELEMENT_TYPE_DEVICE, ELEMENT_TYPE_INTERFACE and
                   ELEMENT_TYPE_UNSPECIFIED
                   set to ELEMENT_TYPE_UNSPECIFIED by default which fetches all tags
@@ -3117,16 +3067,17 @@
                         "key": {
                             "elementType": element_type,
                             "workspaceId": workspace_id
                         }
                     }
                 ]
             }
-            self.log.debug('v6 {}'.format(tag_url))
+            self.log.debug(f"v6 {tag_url}")
             return self.clnt.post(tag_url, data=payload)
+        return None
 
     def get_tag_edits(self, workspace_id):
         ''' Show all tags edits in a workspace
 
             Args:
                 workspace_id: The ID of the workspace
 
@@ -3147,14 +3098,15 @@
                             "workspace_id": workspace_id
                         }
                     }
                 ]
             }
             self.log.debug('v6 ' + tag_url + ' ' + str(payload))
             return self.clnt.post(tag_url, data=payload)
+        return None
 
     def get_tag_assignment_edits(self, workspace_id):
         ''' Show all tags assignment edits in a workspace
 
             Args:
                 workspace_id: The ID of the workspace
 
@@ -3175,14 +3127,15 @@
                             "workspace_id": workspace_id
                         }
                     }
                 ]
             }
             self.log.debug('v6 ' + tag_url + ' ' + str(payload))
             return self.clnt.post(tag_url, data=payload)
+        return None
 
     def tag_config(self, element_type, workspace_id, tag_label, tag_value, remove=False):
         ''' Create/Delete device or interface tags.
             Tag creation with the tag.v2 resource API has to be done within a workspace.
 
             Args:
                element_type (str): Can be ELEMENT_TYPE_DEVICE or ELEMENT_TYPE_INTERFACE to
@@ -3209,16 +3162,17 @@
                     "elementType": element_type,
                     "workspaceId": workspace_id,
                     "label": tag_label,
                     "value": tag_value
                 },
                 "remove": remove
             }
-            self.log.debug('v6 {} '.format(tag_url) + str(payload))
+            self.log.debug(f"v6 {tag_url} " + str(payload))
             return self.clnt.post(tag_url, data=payload)
+        return None
 
     def tag_assignment_config(self, element_type, workspace_id, tag_label,
                               tag_value, device_id, interface_id, remove=False):
         ''' Assign/Unassign device or interface tags.
             Tag assignment with the tag.v2 resource API has to be done within a workspace.
 
             Args:
@@ -3253,44 +3207,46 @@
                     "label": tag_label,
                     "value": tag_value,
                     "deviceId": device_id,
                     "interfaceId": interface_id
                 },
                 "remove": remove
             }
-            self.log.debug('v6 {} '.format(tag_url) + str(payload))
+            self.log.debug(f"v6 {tag_url} " + str(payload))
             return self.clnt.post(tag_url, data=payload)
+        return None
 
     def get_all_workspaces(self):
         ''' Get state information for all workspaces
 
             Returns:
                response (dict): A dict that contains a list of key-values for workspaces
         '''
         msg = 'Workspace Resource APIs are supported from 2021.2.0 or newer.'
         # For on-prem check the version as it is only supported from 2021.2.0+
         if self.cvp_version_compare('>=', 6.0, msg):
             workspace_url = '/api/resources/workspace/v1/Workspace/all'
             payload = {}
-            self.log.debug('v6 {}'.format(workspace_url))
+            self.log.debug(f"v6 {workspace_url}")
             return self.clnt.post(workspace_url, data=payload)
+        return None
 
     def get_workspace(self, workspace_id):
         ''' Get state information for all workspaces
 
             Returns:
                response (dict): A dict that contains a list of key-values for workspaces
         '''
         msg = 'Workspace Resource APIs are supported from 2021.2.0 or newer.'
         # For on-prem check the version as it is only supported from 2021.2.0+
         if self.cvp_version_compare('>=', 6.0, msg):
-            workspace_url = '/api/resources/workspace/v1/Workspace?key.workspaceId={}'.format(
-                workspace_id)
-            self.log.debug('v6 {}'.format(workspace_url))
+            workspace_url = f"/api/resources/workspace/v1/Workspace?key.workspaceId={workspace_id}"
+            self.log.debug(f"v6 {workspace_url}")
             return self.clnt.get(workspace_url)
+        return None
 
     def workspace_config(self, workspace_id, display_name,
                          description='', request='REQUEST_UNSPECIFIED',
                          request_id=''):
         ''' Create, Build and Submit workspaces.
 
             Args:
@@ -3329,14 +3285,15 @@
                 "request": request,
                 "requestParams": {
                     "requestId": request_id
                 }
             }
             self.log.debug('v6 ' + str(workspace_url) + ' ' + str(payload))
             return self.clnt.post(workspace_url, data=payload)
+        return None
 
     def workspace_build_status(self, workspace_id, build_id):
         ''' Verify the state of the workspace build process.
 
             Args:
                 workspace_id (str): The (unique) name of the workspace.
                 build_id (str): The buildId of the workspace for which the
@@ -3345,18 +3302,19 @@
                 response (dict): A dict that contains...
                     Ex: {'value': {'key': {'workspaceId': 'string', 'buildId': 'string'},
                          'state': 'BUILD_STATE_SUCCESS', 'buildResults': {'values': ...
         '''
         msg = 'Workspace Resource APIs are supported from 2021.2.0 or newer.'
         # For on-prem check the version as it is only supported from 2021.2.0+
         if self.cvp_version_compare('>=', 6.0, msg):
-            params = 'key.workspaceId={}&key.buildId={}'.format(workspace_id, build_id)
+            params = f"key.workspaceId={workspace_id}&key.buildId={build_id}"
             workspace_url = '/api/resources/workspace/v1/WorkspaceBuild?' + params
-            self.log.debug('v6 {}'.format(workspace_url + params))
+            self.log.debug(f"v6 {workspace_url + params}")
             return self.clnt.get(workspace_url, timeout=self.request_timeout)
+        return None
 
     def change_control_get_one(self, cc_id, cc_time=None):
         ''' Get the configuration and status of a change control using Resource APIs.
             Supported versions: CVP 2021.2.0 or newer and CVaaS.
 
             Args:
                cc_id (str): The ID of the change control.
@@ -3376,40 +3334,42 @@
                        "approve":{"value":true, "time":"2021-12-13T21:11:26.788753264Z",
                        "user":"cvpadmin"}}, "time":"2021-12-13T21:11:26.788753264Z"}%
         '''
         msg = 'Change Control Resource APIs are supported from 2021.2.0 or newer.'
         # For on-prem check the version as it is only supported from 2021.2.0+
         if self.cvp_version_compare('>=', 6.0, msg):
             if cc_time is None:
-                params = 'key.id={}'.format(cc_id)
+                params = f"key.id={cc_id}"
             else:
-                params = 'key.id={}&time={}'.format(cc_id, cc_time)
+                params = f"key.id={cc_id}&time={cc_time}"
             cc_url = '/api/resources/changecontrol/v1/ChangeControl?' + params
-            self.log.debug('v6 {}'.format(cc_url))
+            self.log.debug(f"v6 {cc_url}")
             try:
                 response = self.clnt.get(cc_url, timeout=self.request_timeout)
             except Exception as error:
                 if 'resource not found' in str(error):
                     return None
                 raise error
             return response
+        return None
 
     def change_control_get_all(self):
         ''' Get the configuration and status of all Change Controls using Resource APIs.
             Supported versions: CVP 2021.2.0 or newer and CVaaS.
 
             Returns:
                response (dict): A dict that contains a list of all Change Controls.
         '''
         msg = 'Change Control Resource APIs are supported from 2021.2.0 or newer.'
         # For on-prem check the version as it is only supported from 2021.2.0+
         if self.cvp_version_compare('>=', 6.0, msg):
             cc_url = '/api/resources/changecontrol/v1/ChangeControl/all'
-            self.log.debug('v6 {}'.format(cc_url))
+            self.log.debug(f"v6 {cc_url}")
             return self.clnt.get(cc_url, timeout=self.request_timeout)
+        return None
 
     def change_control_approval_get_one(self, cc_id, cc_time=None):
         ''' Get the state of a specific Change Control's approve config using Resource APIs.
             Supported versions: CVP 2021.2.0 or newer and CVaaS.
 
             Args:
                cc_id (str): The ID of the change control.
@@ -3422,41 +3382,43 @@
                          'version': '2021-12-13T21:05:58.813750128Z'},
                          'time': '2021-12-13T21:11:26.788753264Z'}
         '''
         msg = 'Change Control Resource APIs are supported from 2021.2.0 or newer.'
         # For on-prem check the version as it is only supported from 2021.2.0+
         if self.cvp_version_compare('>=', 6.0, msg):
             if cc_time is None:
-                params = 'key.id={}'.format(cc_id)
+                params = f"key.id={cc_id}"
             else:
-                params = 'key.id={}&time={}'.format(cc_id, cc_time)
+                params = f"key.id={cc_id}&time={cc_time}"
             cc_url = '/api/resources/changecontrol/v1/ApproveConfig?' + params
             cc_status = self.change_control_get_one(cc_id)
             if cc_status is None:
                 return None
             if 'value' in cc_status and 'approve' not in cc_status['value']:
                 self.log.warning("The change has not been approved yet."
                                  " A change has to be approved at least once for the 'approve'"
                                  " state to be populated.")
                 return None
             return self.clnt.get(cc_url, timeout=self.request_timeout)
+        return None
 
     def change_control_approval_get_all(self):
         ''' Get state information for all Change Control Approvals using Resource APIs.
             Supported versions: CVP 2021.2.0 or newer and CVaaS.
 
             Returns:
                response (dict): A dict that contains a list of all Change Control Approval Configs.
         '''
         msg = 'Change Control Resource APIs are supported from 2021.2.0 or newer.'
         # For on-prem check the version as it is only supported from 2021.2.0+
         if self.cvp_version_compare('>=', 6.0, msg):
             cc_url = '/api/resources/changecontrol/v1/ApproveConfig/all'
-            self.log.debug('v6 {}'.format(cc_url))
+            self.log.debug(f"v6 {cc_url}")
             return self.clnt.get(cc_url, timeout=self.request_timeout)
+        return None
 
     def change_control_approve(self, cc_id, notes="", approve=True):
         ''' Approve/Unapprove a change control using Resource APIs.
             Supported versions: CVP 2021.2.0 or newer and CVaaS.
 
             Args:
               cc_id (str): The ID of the change control.
@@ -3494,18 +3456,19 @@
 
             Args:
               cc_id (str): The ID of the change control.
         '''
         msg = 'Change Control Resource APIs are supported from 2021.2.0 or newer.'
         # For on-prem check the version as it is only supported from 2021.2.0+
         if self.cvp_version_compare('>=', 6.0, msg):
-            params = 'key.id={}'.format(cc_id)
+            params = f"key.id={cc_id}"
             cc_url = '/api/resources/changecontrol/v1/ChangeControlConfig?' + params
-            self.log.debug('v6 {}'.format(cc_url))
+            self.log.debug(f"v6 {cc_url}")
             return self.clnt.delete(cc_url, timeout=self.request_timeout)
+        return None
 
     def change_control_create_with_custom_stages(self, custom_cc=None):
         ''' Create a Change Control with custom stage hierarchy using Resource APIs.
             Supported versions: CVP 2021.2.0 or newer and CVaaS.
 
             Args:
                 custom_cc (dict): A dictionary with the entire stage hierarchy.
@@ -3632,14 +3595,15 @@
         msg = 'Change Control Resource APIs are supported from 2021.2.0 or newer.'
         # For on-prem check the version as it is only supported from 2021.2.0+
         if self.cvp_version_compare('>=', 6.0, msg):
             payload = custom_cc
             cc_url = '/api/resources/changecontrol/v1/ChangeControlConfig'
             self.log.debug('v6 ' + str(cc_url) + ' ' + str(payload))
             return self.clnt.post(cc_url, data=payload)
+        return None
 
     def change_control_create_for_tasks(self, cc_id, name, tasks, series=True):
         ''' Create a simple Change Control for tasks using Resource APIs.
             Supported versions: CVP 2021.2.0 or newer and CVaaS.
 
             This function will create a change with either all Task actions in series or parallel.
             For custom stage hierarchy the change_control_create_with_custom_stages()
@@ -3655,15 +3619,15 @@
                 response (dict): A dict that contains...
                 Ex: {'value': {'key': {'id':cc_id,
                       'time': '...'}
         '''
         stages = {'values': {'root': {'name': 'root', 'rows': {'values': []}}}}
         if series:
             for index, task in enumerate(tasks):
-                stage_id = 'stage%d' % index
+                stage_id = f"stage{index}"
                 stages['values']['root']['rows']['values'].append({'values': [stage_id]})
                 stages['values'][stage_id] = {
                     'action': {
                         'args': {
                             'values': {
                                 'TaskID': task,
                             },
@@ -3672,15 +3636,15 @@
                         'timeout': 3000,
                     },
                     'name': stage_id,
                 }
         else:
             stages['values']['root']['rows']['values'].append({'values': []})
             for index, task in enumerate(tasks):
-                stage_id = 'stage%d' % index
+                stage_id = f"stage{index}"
                 stages['values']['root']['rows']['values'][0]['values'].append(stage_id)
                 stages['values'][stage_id] = {
                     'action': {
                         'args': {
                             'values': {
                                 'TaskID': task,
                             },
@@ -3703,14 +3667,15 @@
                     'notes': 'randomString',
                     'stages': stages
                 }
             }
             cc_url = '/api/resources/changecontrol/v1/ChangeControlConfig'
             self.log.debug('v6 ' + str(cc_url) + ' ' + str(payload))
             return self.clnt.post(cc_url, data=payload, timeout=self.request_timeout)
+        return None
 
     def change_control_start(self, cc_id, notes=""):
         ''' Start a Change Control using Resource APIs.
             Supported versions: CVP 2021.2.0 or newer and CVaaS.
             Args:
                 cc_id (string): The ID for the new change control.
                 notes (string): An optional note.
@@ -3730,14 +3695,15 @@
                     "value": True,
                     "notes": notes
                 }
             }
             cc_url = '/api/resources/changecontrol/v1/ChangeControlConfig'
             self.log.debug('v6 ' + str(cc_url) + ' ' + str(payload))
             return self.clnt.post(cc_url, data=payload, timeout=self.request_timeout)
+        return None
 
     def change_control_stop(self, cc_id, notes=""):
         ''' Stop a Change Control using Resource APIs.
             Supported versions: CVP 2021.2.0 or newer and CVaaS.
 
             Args:
                 cc_id (string): The ID for the new change control.
@@ -3758,14 +3724,15 @@
                     "value": False,
                     "notes": notes
                 }
             }
             cc_url = '/api/resources/changecontrol/v1/ChangeControlConfig'
             self.log.debug('v6 ' + str(cc_url) + ' ' + str(payload))
             return self.clnt.post(cc_url, data=payload, timeout=self.request_timeout)
+        return None
 
     def change_control_schedule(self, cc_id, schedule_time, notes=""):
         ''' Schedule a Change Control using Resource APIs.
             Supported versions: CVP 2022.1.0 or newer and CVaaS.
 
             Args:
                 cc_id (string): The ID for the new change control.
@@ -3789,24 +3756,25 @@
                     "value": schedule_time,
                     "notes": notes
                 }
             }
             cc_url = '/api/resources/changecontrol/v1/ChangeControlConfig'
             self.log.debug('v8 ' + str(cc_url) + ' ' + str(payload))
             return self.clnt.post(cc_url, data=payload, timeout=self.request_timeout)
+        return None
 
     def device_decommissioning(self, device_id, request_id):
         ''' Decommission a device using Resource APIs.
             Supported versions: CVP 2021.3.0 or newer and CVaaS.
             Args:
                 device_id (string): Serial Number of the device.
                 request_id (string): Key identifies the request to decommission the device.
                     Recommended to generate uuid with str(uuid.uuid4()).
             Returns:
-                response (dict): Returns None if the device is not found else returns A dict that contains...
+                response (dict): Returns None if device is not found else return dict that contains
                 Ex: {'value': {'key': {'requestId': '4a4ba5a2-9886-4cd5-84d6-bdaf85a9f091'},
                      'deviceId': 'BAD032986065E8DC14CBB6472EC314A6'},
                      'time': '2022-02-12T02:58:30.765459650Z'}
         '''
         device_exists = False
         inventory = self.get_inventory(provisioned=False)
         for device in inventory:
@@ -3823,18 +3791,17 @@
                     },
                     "device_id": device_id
                 }
                 url = '/api/resources/inventory/v1/DeviceDecommissioningConfig'
                 self.log.debug('v7 ' + str(url) + ' ' + str(payload))
                 return self.clnt.post(url, data=payload, timeout=self.request_timeout)
         else:
-            self.log.warning(
-                'Device with %s serial number does not exist (or is not registered) to decommission'
-                % device_id)
-            return None
+            self.log.warning("Device with %s serial number does not exist (or is not registered)"
+                             " to decommission", device_id)
+        return None
 
     def device_decommissioning_status_get_one(self, request_id):
         ''' Get the decommission status of a device using Resource APIs.
             Supported versions: CVP 2021.3.0 or newer and CVaaS.
             Args:
                 request_id (string): key identifies the request to decommission the device
             Returns:
@@ -3843,18 +3810,19 @@
                   "status":"DECOMMISSIONING_STATUS_IN_PROGRESS",
                   "statusMessage":"Disabled TerminAttr, waiting for device to be marked inactive"},
                   "time":"2022-02-04T19:41:46.376310308Z","type":"INITIAL"}}
         '''
         msg = 'Decommissioning via Resource APIs are supported from 2021.3.0 or newer.'
         # For on-prem check the version as it is only supported from 2021.3.0+
         if self.cvp_version_compare('>=', 7.0, msg):
-            params = 'key.requestId={}'.format(request_id)
+            params = f"key.requestId={request_id}"
             url = '/api/resources/inventory/v1/DeviceDecommissioning?' + params
             self.log.debug('v7 ' + str(url))
             return self.clnt.get(url, timeout=self.request_timeout)
+        return None
 
     def device_decommissioning_status_get_all(self, status="DECOMMISSIONING_STATUS_UNSPECIFIED"):
         ''' Get the decommissioning status of all devices using Resource APIs.
             Supported versions: CVP 2021.3.0 or newer and CVaaS.
             Args:
                 status (enum): By default it will get the decommissioning status for all devices.
                     Possible values:
@@ -3878,14 +3846,15 @@
                         "status": status,
                     }
                 ]
             }
             url = '/api/resources/inventory/v1/DeviceDecommissioning/all'
             self.log.debug('v7 ' + str(url))
             return self.clnt.post(url, data=payload, timeout=self.request_timeout)
+        return None
 
     def add_role(self, name, description, moduleList):
         ''' Add new local role to the CVP UI.
             Args:
                 name (str): local role name on CVP
                 description (str): role description
                 moduleList (list): list of modules (name (str) and mode (str))
@@ -3914,17 +3883,18 @@
 
     def get_role(self, rolekey):
         ''' Returns specified role information.
             Args:
                 rolekey (str): role key on CVP
             Returns:
                response (dict): Returns a dict that contains the role.
-               Ex: {'name': 'Test Role', 'key': 'role_1599019487020581247', 'description': 'Test'...}
+               Ex: {'name': 'Test Role', 'key': 'role_1599019487020581247',
+                    'description': 'Test'...}
         '''
-        return self.clnt.get('/role/getRole.do?roleId={}'.format(rolekey),
+        return self.clnt.get(f"/role/getRole.do?roleId={rolekey}",
                              timeout=self.request_timeout)
 
     def get_roles(self):
         ''' Get all the user roles in CloudVision.
             Returns:
                response (dict): Returns a dict that contains all the user role states..
                Ex: {'total': 7, 'roles': [{'name': 'Test Role', 'key': 'role_1599019487020581247',
@@ -3958,16 +3928,17 @@
                       'description': 'string','valid_until': '2022-11-02T06:58:53Z',
                       'created_by': 'string', 'last_used': None},
                       'time': '2022-05-03T15:38:53.725014447Z', 'type': 'INITIAL'}, ...]
         '''
         msg = 'Service Account Resource APIs are supported from 2021.3.0+.'
         if self.cvp_version_compare('>=', 7.0, msg):
             url = '/api/v3/services/arista.serviceaccount.v1.TokenService/GetAll'
-            self.log.debug('v7 {}'.format(url))
+            self.log.debug(f"v7 {url}")
             return self.clnt.post(url)
+        return None
 
     def svc_account_token_get_one(self, token_id):
         ''' Get a service account token's state using Resource APIs
             Supported versions: CVP 2021.3.0 or newer and CVaaS.
             Returns:
                 response (list): Returns a list of dict that contains...
                 Ex: [{'value': {'key': {'id': 'randomId'}, 'user': 'string',
@@ -3975,16 +3946,17 @@
                       'created_by': 'cvpadmin', 'last_used': None},
                       'time': '2022-05-03T15:38:53.725014447Z', 'type': 'INITIAL'}]
         '''
         msg = 'Service Account Resource APIs are supported from 2021.3.0+.'
         if self.cvp_version_compare('>=', 7.0, msg):
             payload = {"key": {"id": token_id}}
             url = '/api/v3/services/arista.serviceaccount.v1.TokenService/GetOne'
-            self.log.debug('v7 {} {}'.format(url, payload))
+            self.log.debug(f"v7 {url} {payload}")
             return self.clnt.post(url, data=payload)
+        return None
 
     def svc_account_token_delete(self, token_id):
         ''' Delete a service account token using Resource APIs.
             Supported versions: CVP 2021.3.0 or newer and CVaaS.
             Args:
                 token_id (string): The id of the service account token.
             Returns:
@@ -3992,16 +3964,17 @@
                 Ex: [{'key': {'id': '<token_id>'},
                       'time': '2022-07-26T15:29:03.687167871Z'}]
         '''
         msg = 'Service Account Resource APIs are supported from 2021.3.0+.'
         if self.cvp_version_compare('>=', 7.0, msg):
             payload = {"key": {"id": token_id}}
             url = '/api/v3/services/arista.serviceaccount.v1.TokenConfigService/Delete'
-            self.log.debug('v7 {} {}'.format(url, payload))
+            self.log.debug(f"v7 {url} {payload}")
             return self.clnt.post(url, data=payload)
+        return None
 
     def svc_account_token_set(self, username, duration, description):
         ''' Create a service account token using Resource APIs.
             Supported versions: CVP 2021.3.0 or newer and CVaaS.
             Args:
                 username (string): The service account username for which the token will be
                     generated.
@@ -4016,32 +3989,34 @@
         '''
         payload = {'value': {'description': description,
                              'user': username,
                              'valid_for': duration}}
         msg = 'Service Account Resource APIs are supported from 2021.3.0+.'
         if self.cvp_version_compare('>=', 7.0, msg):
             url = '/api/v3/services/arista.serviceaccount.v1.TokenConfigService/Set'
-            self.log.debug('v7 {} {}'.format(url, payload))
+            self.log.debug(f"v7 {url} {payload}")
             return self.clnt.post(url, data=payload)
+        return None
 
     def svc_account_get_all(self):
         ''' Get all service account states using Resource APIs.
             Supported versions: CVP 2021.3.0 or newer and CVaaS.
             Returns:
                 response (list): Returns a list of dictionaries that contains...
                 Ex: [{'value': {'key': {'name': 'ansible'}, 'status': 'ACCOUNT_STATUS_ENABLED',
                       'description': 'lab-tests', 'groups': {'values': ['network-admin']}},
                       'time': '2022-02-10T04:28:14.251684869Z', 'type': 'INITIAL'}, ...]
 
         '''
         msg = 'Service Account Resource APIs are supported from 2021.3.0+.'
         if self.cvp_version_compare('>=', 7.0, msg):
             url = '/api/v3/services/arista.serviceaccount.v1.AccountService/GetAll'
-            self.log.debug('v7 {} '.format(url))
+            self.log.debug(f"v7 {url}")
             return self.clnt.post(url)
+        return None
 
     def svc_account_get_one(self, username):
         ''' Get a service account's state using Resource APIs
             Supported versions: CVP 2021.3.0 or newer and CVaaS.
             Args:
                 username (string): The service account username.
             Returns:
@@ -4050,16 +4025,17 @@
                       'description': 'lab-tests', 'groups': {'values': ['network-admin']}},
                       'time': '2022-02-10T04:28:14.251684869Z'}]
         '''
         msg = 'Service Account Resource APIs are supported from 2021.3.0+.'
         if self.cvp_version_compare('>=', 7.0, msg):
             payload = {"key": {"name": username}}
             url = '/api/v3/services/arista.serviceaccount.v1.AccountService/GetOne'
-            self.log.debug('v7 {} {}'.format(url, payload))
+            self.log.debug(f"v7 {url} {payload}")
             return self.clnt.post(url, data=payload)
+        return None
 
     def svc_account_set(self, username, description, roles, status):
         ''' Create a service account using Resource APIs.
             Supported versions: CVP 2021.3.0 or newer and CVaaS.
             Args:
                 username (string): The service account username.
                 description (string): The description of the service account.
@@ -4083,24 +4059,25 @@
         if self.cvp_version_compare('>=', 7.0, msg):
             role_ids = []
             all_roles = self.get_roles()
             for role in all_roles['roles']:
                 if role['key'] in roles or role['name'] in roles:
                     role_ids.append(role['key'])
             if len(roles) != len(role_ids):
-                self.log.warning('Not all provided roles {} are valid. '
-                                 'Only using the found valid roles {}'.format(roles, role_ids))
+                self.log.warning(f"Not all provided roles {roles} are valid. "
+                                 f"Only using the found valid roles {role_ids}")
 
             payload = {'value': {'description': description,
                                  'groups': {'values': role_ids},
                                  'key': {'name': username},
                                  'status': status}}
             url = '/api/v3/services/arista.serviceaccount.v1.AccountConfigService/Set'
-            self.log.debug('v7 {} {}'.format(url, payload))
+            self.log.debug(f"v7 {url} {payload}")
             return self.clnt.post(url, data=payload)
+        return None
 
     def svc_account_delete(self, username):
         ''' Delete a service account using Resource APIs.
             Supported versions: CVP 2021.3.0 or newer and CVaaS.
             Args:
                 username (string): The service account username.
             Returns:
@@ -4108,16 +4085,17 @@
                 Ex: [{'key': {'name': 'cvprac2'},
                       'time': '2022-07-26T18:26:53.637425846Z'}]
         '''
         msg = 'Service Account Resource APIs are supported from 2021.3.0+.'
         if self.cvp_version_compare('>=', 7.0, msg):
             payload = {"key": {"name": username}}
             url = '/api/v3/services/arista.serviceaccount.v1.AccountConfigService/Delete'
-            self.log.debug('v7 {} {}'.format(url, payload))
+            self.log.debug(f"v7 {url} {payload}")
             return self.clnt.post(url, data=payload)
+        return None
 
     def svc_account_delete_expired_tokens(self):
         ''' Delete all service account tokens using Resource APIs.
             Supported versions: CVP 2021.3.0 or newer and CVaaS.
             Returns:
                 response (list): Returns a list of dict that contains the list of tokens
                 that were deleted:
```

### Comparing `cvprac-1.3.2/cvprac/cvp_client.py` & `cvprac-1.4.0/cvprac/cvp_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
+
+# pylint: disable=too-many-branches,too-many-statements,too-many-locals,too-many-lines
+
 ''' RESTful API Client class for Cloudvision(R) Portal
 
 This module provides a RESTful API client for Cloudvision(R) Portal (CVP)
 which can be used for building applications that work with Arista CVP.
 
 When the class is instantiated the logging is configured.  Either syslog,
 file logging, both, or none can be enabled.  If neither syslog nor filename is
@@ -92,26 +95,32 @@
 
 import os
 import re
 import json
 import logging
 from logging.handlers import SysLogHandler
 from itertools import cycle
-from pkg_resources import parse_version
+from packaging.version import parse
 
 import requests
-from requests.exceptions import ConnectionError, HTTPError, Timeout, \
-    ReadTimeout, TooManyRedirects, JSONDecodeError
+from requests.exceptions import ( # pylint: disable=redefined-builtin
+    ConnectionError,
+    HTTPError,
+    Timeout,
+    ReadTimeout,
+    TooManyRedirects,
+    JSONDecodeError
+)
 
 from cvprac.cvp_api import CvpApi
 from cvprac.cvp_client_errors import CvpApiError, CvpLoginError, \
     CvpRequestError, CvpSessionLogOutError
 
 
-class CvpClient(object):
+class CvpClient():
     ''' Use this class to create a persistent connection to CVP.
     '''
     # pylint: disable=too-many-instance-attributes
     # Maximum number of times to retry a get or post to the same
     # CVP node.
     NUM_RETRY_REQUESTS = 3
     LATEST_API_VERSION = 9.0
@@ -229,36 +238,45 @@
             version_components = version.split(".")
             if len(version_components) < 3:
                 version_components.append("0")
                 self.log.info('Version found with less than 3 components.'
                               ' Appending 0. Updated Version String - %s',
                               ".".join(version_components))
             full_version = ".".join(version_components)
-            if parse_version(full_version) >= parse_version('2023.1.0'):
+            if parse(full_version) >= parse('2024.1.0'):
+                self.log.info('Setting API version to v12')
+                self.apiversion = 12.0
+            elif parse(full_version) >= parse('2023.3.0'):
+                self.log.info('Setting API version to v11')
+                self.apiversion = 11.0
+            elif parse(full_version) >= parse('2023.2.0'):
+                self.log.info('Setting API version to v10')
+                self.apiversion = 10.0
+            elif parse(full_version) >= parse('2023.1.0'):
                 self.log.info('Setting API version to v9')
                 self.apiversion = 9.0
-            elif parse_version(full_version) >= parse_version('2022.1.0'):
+            elif parse(full_version) >= parse('2022.1.0'):
                 self.log.info('Setting API version to v8')
                 self.apiversion = 8.0
-            elif parse_version(full_version) >= parse_version('2021.3.0'):
+            elif parse(full_version) >= parse('2021.3.0'):
                 self.log.info('Setting API version to v7')
                 self.apiversion = 7.0
-            elif parse_version(full_version) >= parse_version('2021.2.0'):
+            elif parse(full_version) >= parse('2021.2.0'):
                 self.log.info('Setting API version to v6')
                 self.apiversion = 6.0
-            elif parse_version(full_version) >= parse_version('2020.2.4'):
+            elif parse(full_version) >= parse('2020.2.4'):
                 self.log.info('Setting API version to v5')
                 self.apiversion = 5.0
-            elif parse_version(full_version) >= parse_version('2020.1.1'):
+            elif parse(full_version) >= parse('2020.1.1'):
                 self.log.info('Setting API version to v4')
                 self.apiversion = 4.0
-            elif parse_version(full_version) >= parse_version('2019.0.0'):
+            elif parse(full_version) >= parse('2019.0.0'):
                 self.log.info('Setting API version to v3')
                 self.apiversion = 3.0
-            elif parse_version(full_version) >= parse_version('2018.2.0'):
+            elif parse(full_version) >= parse('2018.2.0'):
                 self.log.info('Setting API version to v2')
                 self.apiversion = 2.0
             else:
                 self.log.info('Setting API version to v1')
                 self.apiversion = 1.0
 
     def connect(self, nodes, username, password, connect_timeout=10,
@@ -374,21 +392,20 @@
         num_nodes = self.node_cnt
         if not all_nodes and num_nodes > 1:
             num_nodes -= 1
 
         self.error_msg = '\n'
         for _ in range(0, num_nodes):
             host = next(self.node_pool)
-            self.url_prefix = ('https://%s:%d/web' % (host, self.port or 443))
-            self.url_prefix_short = ('https://%s:%d'
-                                     % (host, self.port or 443))
+            self.url_prefix = f"https://{host}:{self.port or 443}/web"
+            self.url_prefix_short = f"https://{host}:{self.port or 443}"
             error = self._reset_session()
             if error is None:
                 break
-            self.error_msg += '%s: %s\n' % (host, error)
+            self.error_msg += f"{host}: {error}\n"
 
     def _reset_session(self):
         ''' Get a new request session and try logging into the current
             CVP node. If the login succeeded None will be returned and
             self.session will be valid. If the login failed then an
             exception error will be returned and self.session will
             be set to None.
@@ -424,31 +441,28 @@
                 CvpSessionLogOutError: A CvpSessionLogOutError is raised if
                     response from server indicates session was logged out.
         '''
         if not response.ok:
             if 'Unauthorized' in response.reason:
                 # Check for 'Unauthorized' User error because this is how
                 # CVP responds to a logged out users requests in 2018.x.
-                msg = '%s: Request Error: %s' % (prefix, response.reason)
+                msg = f"{prefix}: Request Error: {response.reason}"
                 self.log.error(msg)
                 raise CvpApiError(msg)
             if 'User is unauthorized' in response.text:
                 # Check for 'User is unauthorized' response text because this
                 # is how CVP responds to a logged out users requests in 2019.x.
-                msg = '%s: Request Error: User is unauthorized' % prefix
+                msg = f"{prefix}: Request Error: User is unauthorized"
                 self.log.error(msg)
                 raise CvpApiError(msg)
-            else:
-                msg = '%s: Request Error: %s - %s' % (prefix, response.reason,
-                                                      response.text)
-                self.log.error(msg)
-                raise CvpRequestError(msg)
+            msg = f"{prefix}: Request Error: {response.reason} - {response.text}"
+            raise CvpRequestError(msg)
 
         if 'LOG OUT MESSAGE' in response.text:
-            msg = ('%s: Request Error: session logged out' % prefix)
+            msg = f"{prefix}: Request Error: session logged out"
             raise CvpSessionLogOutError(msg)
 
         joutput = json_decoder(response.text)
         err_code_val = self._finditem(joutput, 'errorCode')
         if err_code_val:
             if 'errorMessage' in joutput:
                 err_msg = joutput['errorMessage']
@@ -456,33 +470,32 @@
                 if 'errors' in joutput:
                     error_list = joutput['errors']
                 else:
                     error_list = [joutput['errorCode']]
                 # Build the error message from all the errors.
                 err_msg = error_list[0]
                 for idx in range(1, len(error_list)):
-                    err_msg = '%s\n%s' % (err_msg, error_list[idx])
+                    err_msg = f"{err_msg}\n{error_list[idx]}"
 
-            msg = ('%s: Request Error: %s' % (prefix, err_msg))
+            msg = f"{prefix}: Request Error: {err_msg}"
             self.log.error(msg)
             raise CvpApiError(msg)
 
     def _check_response_status(self, response, prefix):
         ''' Check for status OK in a response from a GET or POST request.
             The response argument contains a response object from a GET or POST
             request.  The prefix argument contains the prefix to put into the
             error message.
 
             Raises:
                 CvpRequestError: A CvpRequestError is raised if request
                 response status is not OK.
         '''
         if not response.ok:
-            msg = '%s: Request Error: %s - %s' % (prefix, response.reason,
-                                                  response.text)
+            msg = f"{prefix}: Request Error: {response.reason} - {response.text}"
             self.log.error(msg)
             raise CvpRequestError(msg)
 
     def _login(self):
         ''' Make a POST request to CVP login authentication.
             An error can be raised from the post method call or the
             _is_good_response method call.  Any errors raised would be a good
@@ -508,15 +521,15 @@
                     request failed and no session could be established to a
                     CVP node.  Destroy the class and re-instantiate.
         '''
         # Remove any previous session id from the headers
         self.headers.pop('APP_SESSION_ID', None)
         if self.api_token is not None:
             return self._set_headers_api_token()
-        elif self.is_cvaas:
+        if self.is_cvaas:
             raise CvpLoginError('CVaaS only supports API token authentication.'
                                 ' Please create an API token and provide it'
                                 ' via the api_token parameter in combination'
                                 ' with the is_cvaas parameter')
         return self._login_on_prem()
 
     def _login_on_prem(self):
@@ -547,48 +560,50 @@
         '''
         url = self.url_prefix + '/login/authenticate.do'
         response = self.session.post(url,
                                      data=json.dumps(self.authdata),
                                      headers=self.headers,
                                      timeout=self.connect_timeout,
                                      verify=self.cert)
-        self._is_good_response(response, 'Authenticate: %s' % url)
+        self._is_good_response(response, f"Authenticate: {url}")
 
         self.cookies = response.cookies
         self.headers['APP_SESSION_ID'] = response.json()['sessionId']
 
     def _set_headers_api_token(self):
         ''' Sets headers with API token instead of making a call to login API.
         '''
         # If using an API token there is no need to run a Login API.
         # Simply add the token into the headers or cookies
-        self.headers['Authorization'] = 'Bearer %s' % self.api_token
+        self.headers['Authorization'] = f"Bearer {self.api_token}"
         # Alternative to adding token to headers it can be added to
         # cookies as shown below.
         # self.cookies = {'access_token': self.api_token}
         url = self.url_prefix_short + '/api/v1/rest/'
-        response = self.session.get(url,
-                            cookies=self.cookies,
-                            headers=self.headers,
-                            timeout=self.connect_timeout,
-                            verify=self.cert)
+        response = self.session.get(
+            url,
+            cookies=self.cookies,
+            headers=self.headers,
+            timeout=self.connect_timeout,
+            verify=self.cert
+        )
         # Verify that the generic request was successful
-        self._is_good_response(response, 'Authenticate: %s' % url)
+        self._is_good_response(response, f"Authenticate: {url}")
 
     def logout(self):
         '''
 
         :return:
         '''
         response = self.post('/login/logout.do')
         if response['data'] == 'success':
             self.log.info('User logged out.')
             self.session = None
         else:
-            err = 'Error trying to logout %s' % response
+            err = f"Error trying to logout {response}"
             self.log.error(err)
 
     def _make_request(self, req_type, url, timeout, data=None,
                       files=None):
         ''' Make a GET, POST or DELETE request to CVP.  If the request call raises a
             timeout or CvpSessionLogOutError then the request will be retried
             on the same CVP node.  Otherwise the request will be tried on the
@@ -696,16 +711,16 @@
         # service account APIs being a special case /services/ API that
         # returns a null string for no objects instead of an empty string.
         if not response.content or response.content == b'null':
             return {'data': []}
 
         try:
             resp_data = response.json()
-            if (resp_data is not None and 'result' in resp_data
-                    and '/resources/' in full_url):
+            if (resp_data is not None and 'result' in resp_data and
+                    '/resources/' in full_url):
                 # Resource APIs use JSON streaming and will return
                 # multiple JSON objects during GetAll type API
                 # calls. We are wrapping the multiple objects into
                 # a key "data" and we also return a dictionary with
                 # key "data" as an empty dict for no data. This
                 # checks and keeps consistent the "data" key wrapper
                 # for a Resource API GetAll that returns a single
@@ -721,18 +736,16 @@
             self.log.debug('Error trying to decode request response - %s',
                            err_str)
             if 'Extra data' in str(error):
                 self.log.debug('Found multiple objects or NO objects in'
                                ' response data. Attempt to decode')
                 decoded_data = json_decoder(response.text)
                 return {'data': decoded_data}
-            else:
-                self.log.error('Unknown format for JSONDecodeError - %s',
-                               err_str)
-                raise error
+            self.log.error("Unknown format for JSONDecodeError - %s", err_str)
+            raise error
 
     def _send_request(self, req_type, full_url, timeout, data=None,
                       files=None):
         ''' Make a GET, POST or DELETE request to CVP.  If the request call
             raises a timeout or CvpSessionLogOutError then the request will be
             retried on the same CVP node.  Otherwise the request will be tried
             on the next CVP node.
@@ -791,15 +804,15 @@
                         response = self.session.post(full_url,
                                                      cookies=self.cookies,
                                                      data=json.dumps(data),
                                                      headers=self.headers,
                                                      timeout=timeout,
                                                      verify=self.cert)
                     else:
-                        fhs = dict()
+                        fhs = {}
                         fhs['Accept'] = self.headers['Accept']
                         if 'APP_SESSION_ID' in self.headers:
                             fhs['APP_SESSION_ID'] = self.headers[
                                 'APP_SESSION_ID']
                         if 'Authorization' in self.headers:
                             fhs['Authorization'] = self.headers[
                                 'Authorization']
@@ -826,51 +839,47 @@
                 # retry this request to the same node. If this is the final
                 # try raise the error so another CVP node can be tried
                 if req_try + 1 == self.NUM_RETRY_REQUESTS:
                     raise error
                 continue
 
             try:
-                self._is_good_response(response, '%s: %s ' %
-                                       (req_type, full_url))
+                self._is_good_response(response, f"{req_type}: {full_url} ")
             except CvpSessionLogOutError as error:
                 self.log.debug(error)
                 # Retry the request to the same node if there was a CVP session
                 # logout. Reset the session which will login. If a valid
                 # session comes back then clear the error so this request will
                 # be retried on the same node.
                 if req_try + 1 == self.NUM_RETRY_REQUESTS:
                     raise error
-                else:
-                    self._reset_session()
-                    if not self.session:
-                        raise error
-                    continue
+                self._reset_session()
+                if not self.session:
+                    raise error
+                continue
             except CvpApiError as error:
                 self.log.debug(error)
                 if ('Unauthorized' in error.msg or
                         'User is unauthorized' in error.msg):
                     # Retry the request to the same node if there was an
                     # Unauthorized User error because this is how CVP responds
                     # to a logged out users requests in 2017.1.
                     # Check for 'User is unauthorized' in error because this is
                     # how CVP responds to a logged out user requests in 2019.x.
                     # Reset the session which will login. If a valid
                     # session comes back then clear the error so this request
                     # will be retried on the same node.
                     if req_try + 1 == self.NUM_RETRY_REQUESTS:
                         raise error
-                    else:
-                        self._reset_session()
-                        if not self.session:
-                            raise error
-                        continue
-                else:
-                    # pylint: disable=raising-bad-type
-                    raise error
+                    self._reset_session()
+                    if not self.session:
+                        raise error
+                    continue
+                # pylint: disable=raising-bad-type
+                raise error
             return response
 
     def get(self, url, timeout=30):
         ''' Make a GET request to CVP.  If the request call raises an error
             or if the JSON response contains a CVP session related error then
             retry the request on another CVP node.
```

### Comparing `cvprac-1.3.2/cvprac/cvp_client_errors.py` & `cvprac-1.4.0/cvprac/cvp_client_errors.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/cvprac.egg-info/PKG-INFO` & `cvprac-1.4.0/cvprac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: cvprac
-Version: 1.3.2
+Version: 1.4.0
 Summary: Arista Cloudvision(R) Portal Rest API Client written in python
 Home-page: https://github.com/aristanetworks/cvprac
 Author: Arista Networks, Inc.
 Author-email: eosplus-dev@arista.com
 License: BSD-3
-Download-URL: https://github.com/aristanetworks/cvprac/tarball/1.3.2
+Download-URL: https://github.com/aristanetworks/cvprac/tarball/1.4.0
 Keywords: networking CloudVision development rest api
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Arista Cloudvision® Portal RESTful API Client
 
 [![pypi](https://img.shields.io/pypi/v/cvprac.svg)](https://pypi.python.org/pypi/cvprac)
```

### Comparing `cvprac-1.3.2/cvprac.egg-info/SOURCES.txt` & `cvprac-1.4.0/cvprac.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 docs/release-notes-1.0.6.rst
 docs/release-notes-1.0.7.rst
 docs/release-notes-1.2.0.rst
 docs/release-notes-1.2.2.rst
 docs/release-notes-1.3.0.rst
 docs/release-notes-1.3.1.rst
 docs/release-notes-1.3.2.rst
+docs/release-notes-1.4.0.rst
 docs/labs/README.md
 docs/labs/lab01-cvp-info/get_cvp_info.py
 docs/labs/lab02-inventory-operations/compliance_check.py
 docs/labs/lab02-inventory-operations/get_running_configs.py
 docs/labs/lab02-inventory-operations/get_running_configs_by_time.py
 docs/labs/lab02-inventory-operations/remove_all_devices_legacy.py
 docs/labs/lab02-inventory-operations/remove_and_decommission_device.py
```

### Comparing `cvprac-1.3.2/cvprac.spec` & `cvprac-1.4.0/cvprac.spec`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/README.md` & `cvprac-1.4.0/docs/labs/README.md`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab01-cvp-info/get_cvp_info.py` & `cvprac-1.4.0/docs/labs/lab01-cvp-info/get_cvp_info.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab02-inventory-operations/compliance_check.py` & `cvprac-1.4.0/docs/labs/lab02-inventory-operations/compliance_check.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab02-inventory-operations/get_running_configs.py` & `cvprac-1.4.0/docs/labs/lab02-inventory-operations/get_running_configs.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab02-inventory-operations/get_running_configs_by_time.py` & `cvprac-1.4.0/docs/labs/lab02-inventory-operations/get_running_configs_by_time.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab02-inventory-operations/remove_all_devices_legacy.py` & `cvprac-1.4.0/docs/labs/lab02-inventory-operations/remove_all_devices_legacy.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab02-inventory-operations/remove_and_decommission_device.py` & `cvprac-1.4.0/docs/labs/lab02-inventory-operations/remove_and_decommission_device.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab02-inventory-operations/remove_devices_from_container_legacy.py` & `cvprac-1.4.0/docs/labs/lab02-inventory-operations/remove_devices_from_container_legacy.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab02-inventory-operations/remove_devices_legacy.py` & `cvprac-1.4.0/docs/labs/lab02-inventory-operations/remove_devices_legacy.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab03-configlet-management/assign_configlet_to_device.py` & `cvprac-1.4.0/docs/labs/lab03-configlet-management/assign_configlet_to_device.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab03-configlet-management/backup_configlets.py` & `cvprac-1.4.0/docs/labs/lab03-configlet-management/backup_configlets.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab03-configlet-management/backup_configletsV2.py` & `cvprac-1.4.0/docs/labs/lab03-configlet-management/backup_configletsV2.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab03-configlet-management/config_search.py` & `cvprac-1.4.0/docs/labs/lab03-configlet-management/config_search.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab03-configlet-management/create_configlet.py` & `cvprac-1.4.0/docs/labs/lab03-configlet-management/create_configlet.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab03-configlet-management/create_configlet_from_file.py` & `cvprac-1.4.0/docs/labs/lab03-configlet-management/create_configlet_from_file.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab03-configlet-management/get_applied_netelements.py` & `cvprac-1.4.0/docs/labs/lab03-configlet-management/get_applied_netelements.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab03-configlet-management/get_configlets.py` & `cvprac-1.4.0/docs/labs/lab03-configlet-management/get_configlets.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab03-configlet-management/reorder_configlet_on_device.py` & `cvprac-1.4.0/docs/labs/lab03-configlet-management/reorder_configlet_on_device.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab03-configlet-management/update_configlet.py` & `cvprac-1.4.0/docs/labs/lab03-configlet-management/update_configlet.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab04-container-management/add_image_to_container.py` & `cvprac-1.4.0/docs/labs/lab04-container-management/add_image_to_container.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab04-container-management/assign_configlet_to_container.py` & `cvprac-1.4.0/docs/labs/lab04-container-management/assign_configlet_to_container.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab04-container-management/create_container.py` & `cvprac-1.4.0/docs/labs/lab04-container-management/create_container.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab04-container-management/remove_image_from_container.py` & `cvprac-1.4.0/docs/labs/lab04-container-management/remove_image_from_container.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab04-container-management/rename_container.py` & `cvprac-1.4.0/docs/labs/lab04-container-management/rename_container.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab05-device-management/add_image_to_devices.py` & `cvprac-1.4.0/docs/labs/lab05-device-management/add_image_to_devices.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab05-device-management/add_image_wo_tempaction.py` & `cvprac-1.4.0/docs/labs/lab05-device-management/add_image_wo_tempaction.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab05-device-management/remove_image_from_device.py` & `cvprac-1.4.0/docs/labs/lab05-device-management/remove_image_from_device.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab05-device-management/set_mgmt_ip.py` & `cvprac-1.4.0/docs/labs/lab05-device-management/set_mgmt_ip.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/atd_e2e_provisioning_workflow.py` & `cvprac-1.4.0/docs/labs/lab06-provisioning/atd_e2e_provisioning_workflow.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/auto_reconcile_on_rc_change.py` & `cvprac-1.4.0/docs/labs/lab06-provisioning/auto_reconcile_on_rc_change.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/change_control_custom_rapi.py` & `cvprac-1.4.0/docs/labs/lab06-provisioning/change_control_custom_rapi.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/change_control_workflow.py` & `cvprac-1.4.0/docs/labs/lab06-provisioning/change_control_workflow.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/change_control_workflow_rapi.py` & `cvprac-1.4.0/docs/labs/lab06-provisioning/change_control_workflow_rapi.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/configlets/AVD_leaf1.cfg` & `cvprac-1.4.0/docs/labs/lab06-provisioning/configlets/AVD_leaf1.cfg`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/configlets/AVD_leaf2.cfg` & `cvprac-1.4.0/docs/labs/lab06-provisioning/configlets/AVD_leaf2.cfg`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/configlets/AVD_leaf3.cfg` & `cvprac-1.4.0/docs/labs/lab06-provisioning/configlets/AVD_leaf3.cfg`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/configlets/AVD_leaf4.cfg` & `cvprac-1.4.0/docs/labs/lab06-provisioning/configlets/AVD_leaf4.cfg`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/configlets/AVD_spine1.cfg` & `cvprac-1.4.0/docs/labs/lab06-provisioning/configlets/AVD_spine1.cfg`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/configlets/AVD_spine2.cfg` & `cvprac-1.4.0/docs/labs/lab06-provisioning/configlets/AVD_spine2.cfg`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/gen_builder.py` & `cvprac-1.4.0/docs/labs/lab06-provisioning/gen_builder.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/mlag_issu.py` & `cvprac-1.4.0/docs/labs/lab06-provisioning/mlag_issu.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/move_device.py` & `cvprac-1.4.0/docs/labs/lab06-provisioning/move_device.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab06-provisioning/vc_task_retrigger.py` & `cvprac-1.4.0/docs/labs/lab06-provisioning/vc_task_retrigger.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # that can be found in the COPYING file.
 
 # Example on how to re-trigger task creation if a config push task was previously
 # cancelled and the device is still config out of sync
 import argparse
 import ssl
 import sys
-from pkg_resources import parse_version
+from packaging.version import parse
 from getpass import getpass
 from cvprac.cvp_client import CvpClient
 import requests.packages.urllib3
 requests.packages.urllib3.disable_warnings()
 
 
 if ((sys.version_info.major == 3) or
@@ -52,15 +52,15 @@
         try:
             clnt.connect(nodes=[cvpserver], username=args.username, password=args.password)
         except Exception as e:
             print("Unable to connect to CVP: %s" % str(e))
 
         # Get the current CVP version
         cvp_release = clnt.api.get_cvp_info()['version']
-        if parse_version(cvp_release) < parse_version('2020.3.0'):
+        if parse(cvp_release) < parse('2020.3.0'):
             # For older CVP, we manually trigger a compliance check
             try:
                 clnt.api.check_compliance('root', 'container')
             except:
                 # Bad practice, but the check compliance applied to a container can't actually work
                 # since the complianceIndication  key doesn't exist on the container level
                 pass
```

### Comparing `cvprac-1.3.2/docs/labs/lab07-aaa/add_new_user_cvaas.py` & `cvprac-1.4.0/docs/labs/lab07-aaa/add_new_user_cvaas.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab07-aaa/add_new_user_onprem.py` & `cvprac-1.4.0/docs/labs/lab07-aaa/add_new_user_onprem.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab07-aaa/add_users_from_csv_cvaas.py` & `cvprac-1.4.0/docs/labs/lab07-aaa/add_users_from_csv_cvaas.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab07-aaa/create_svc_account.py` & `cvprac-1.4.0/docs/labs/lab07-aaa/create_svc_account.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab07-aaa/create_svc_account_token.py` & `cvprac-1.4.0/docs/labs/lab07-aaa/create_svc_account_token.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab07-aaa/create_terminattr_tokens.py` & `cvprac-1.4.0/docs/labs/lab07-aaa/create_terminattr_tokens.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab07-aaa/delete_all_expired_svc_account_tokens.py` & `cvprac-1.4.0/docs/labs/lab07-aaa/delete_all_expired_svc_account_tokens.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab07-aaa/delete_svc_account.py` & `cvprac-1.4.0/docs/labs/lab07-aaa/delete_svc_account.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab07-aaa/delete_svc_account_created_by_user.py` & `cvprac-1.4.0/docs/labs/lab07-aaa/delete_svc_account_created_by_user.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab07-aaa/get_user_info.py` & `cvprac-1.4.0/docs/labs/lab07-aaa/get_user_info.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab07-aaa/svc_account_misc.py` & `cvprac-1.4.0/docs/labs/lab07-aaa/svc_account_misc.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab08-resource-apis/resource_cvprac.py` & `cvprac-1.4.0/docs/labs/lab08-resource-apis/resource_cvprac.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/lab08-resource-apis/topology_tag_assignment.py` & `cvprac-1.4.0/docs/labs/lab08-resource-apis/topology_tag_assignment.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/static/serviceaccount1.png` & `cvprac-1.4.0/docs/labs/static/serviceaccount1.png`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/static/serviceaccount2.png` & `cvprac-1.4.0/docs/labs/static/serviceaccount2.png`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/labs/static/serviceaccount3.png` & `cvprac-1.4.0/docs/labs/static/serviceaccount3.png`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-0.7.0.rst` & `cvprac-1.4.0/docs/release-notes-0.7.0.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-0.8.0.rst` & `cvprac-1.4.0/docs/release-notes-0.8.0.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-0.9.0.rst` & `cvprac-1.4.0/docs/release-notes-0.9.0.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-1.0.0.rst` & `cvprac-1.4.0/docs/release-notes-1.0.0.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-1.0.1.rst` & `cvprac-1.4.0/docs/release-notes-1.0.1.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-1.0.2.rst` & `cvprac-1.4.0/docs/release-notes-1.0.2.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-1.0.4.rst` & `cvprac-1.4.0/docs/release-notes-1.0.4.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-1.0.5.rst` & `cvprac-1.4.0/docs/release-notes-1.0.5.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-1.0.6.rst` & `cvprac-1.4.0/docs/release-notes-1.0.6.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-1.0.7.rst` & `cvprac-1.4.0/docs/release-notes-1.0.7.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-1.2.0.rst` & `cvprac-1.4.0/docs/release-notes-1.2.0.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-1.2.2.rst` & `cvprac-1.4.0/docs/release-notes-1.2.2.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-1.3.0.rst` & `cvprac-1.4.0/docs/release-notes-1.3.0.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/docs/release-notes-1.3.2.rst` & `cvprac-1.4.0/docs/release-notes-1.3.2.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/setup.py` & `cvprac-1.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,26 +96,31 @@
         'Topic :: System :: Networking',
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: BSD License',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 
     # What does your project relate to?
     keywords='networking CloudVision development rest api',
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['requests[socks]>=2.27.0'],
+    install_requires=['requests[socks]>=2.27.0', 'packaging>=23.2'],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev]
     extras_require={
         'dev': ['check-manifest', 'pep8', 'pyflakes', 'pylint', 'coverage',
```

### Comparing `cvprac-1.3.2/test/fixtures/image-file.swix` & `cvprac-1.4.0/test/fixtures/image-file.swix`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.2/test/lib/systestlib.py` & `cvprac-1.4.0/test/lib/systestlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,22 +51,22 @@
     return os.path.join(get_fixtures_path(), filename)
 
 
 class DutSystemTest(unittest.TestCase):
     ''' DutSystemTest class that provides information about the DUTs used.
     '''
     def __init__(self, *args, **kwargs):
-        super(DutSystemTest, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     @classmethod
     def setUpClass(cls):
         ''' Read in the list of CVP node names or IP addresses to use
             for testing.
 
             Format for duts list of dicts:
             { node: nodename, user: username, password: password }
         '''
         cls.duts = {}
         filename = get_fixture('cvp_nodes.yaml')
-        with open(filename, 'r') as stream:
+        with open(filename, 'r', encoding="utf-8") as stream:
             cls.duts = yaml.safe_load(stream)
             stream.close()
```

### Comparing `cvprac-1.3.2/test/system/test_cvp_base.py` & `cvprac-1.4.0/test/system/test_cvp_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,26 @@
+# pylint: disable=wrong-import-position
+
 ''' Base class for TestCvpClient and TestCvpClientCC class.
 '''
 from pprint import pprint
 import os
 import sys
 import re
 import time
 import uuid
 import urllib3
-from cvprac.cvp_client import CvpClient
 
 sys.path.append(os.path.join(os.path.dirname(__file__), '../lib'))
 from systestlib import DutSystemTest
-
+from cvprac.cvp_client import CvpClient
 
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-#
-# sys.path.append(os.path.join(os.path.dirname(__file__), '../lib'))
-# from systestlib import DutSystemTest
-
 
 class TestCvpClientBase(DutSystemTest):
     ''' Base class for TestCvpClient and TestCvpClientCC class.
     '''
     # pylint: disable=too-many-public-methods
     # pylint: disable=invalid-name
     @classmethod
@@ -57,16 +54,16 @@
         # Verify that there is at least one device in the inventory
         err_msg = 'CVP node must contain at least one device'
         result = cls.api.get_inventory()
         assert result is not None
         if len(result) < 1:
             raise AssertionError(err_msg)
         assert len(result) >= 1
-        device = [res for res in result if res['hostname']
-                  == dut.get("device", "")]
+        device = [res for res in result if res['hostname'] ==
+                  dut.get("device", "")]
         cls.device = device[0]
         # Get the container for the device on the list and
         # use that container as the parent container.
         result = cls.api.search_topology(cls.device['fqdn'])
         assert result is not None
         dev_container = result['netElementContainerList']
         assert len(dev_container) >= 1
@@ -139,15 +136,15 @@
         ''' Create a task by making a simple change to a configlet assigned
             to the device.
 
             Returns:
                 (task_id, config)
                 task_id (str): Task ID
                 config (str): Previous configlets contents
-        '''
+        ''' # pylint: disable=duplicate-code
         task_id = self._get_next_task_id()
         # Update the lldp time in the first configlet in the list.
         configlet = None
         for conf in self.dev_configlets:
             if conf['netElementCount'] == 1:
                 configlet = conf
                 break
@@ -184,7 +181,17 @@
             if result is not None:
                 break
             cnt -= 1
         err_msg = f'Timeout waiting for task id {task_id} to be created'
         self.assertGreater(cnt, 0, msg=err_msg)
         self.task_id = task_id
         return task_id, org_config
+
+    def delete_change_control(self, cc_id):
+        """ Delete change control
+        """
+        pprint('DELETING CHANGE CONTROL...')
+        delete_chg_ctrl = self.api.change_control_delete(
+            cc_id)
+        assert delete_chg_ctrl is not None
+        assert delete_chg_ctrl['key']['id'] == self.cc_id
+        return delete_chg_ctrl
```

### Comparing `cvprac-1.3.2/test/system/test_cvp_change_control_api.py` & `cvprac-1.4.0/test/system/test_cvp_change_control_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=too-many-public-methods
 '''
     Tests for change control apis
 '''
 from pprint import pprint
 import time
 import unittest
 from test_cvp_base import TestCvpClientBase
@@ -157,24 +158,14 @@
             self.cc_id, notes=STOP_NOTE)
         assert stop_chg_ctrl is not None
         assert stop_chg_ctrl['value']['start']['value'] is False
         assert stop_chg_ctrl['value']['start']['notes'] == STOP_NOTE
         assert stop_chg_ctrl['value']['key']['id'] == self.cc_id
         return stop_chg_ctrl
 
-    def delete_change_control(self, cc_id):
-        """ Delete change control
-        """
-        pprint('DELETING CHANGE CONTROL...')
-        delete_chg_ctrl = self.api.change_control_delete(
-            cc_id)
-        assert delete_chg_ctrl is not None
-        assert delete_chg_ctrl['key']['id'] == self.cc_id
-        return delete_chg_ctrl
-
     def change_control_get_one(self, cc_id):
         """ Change control get one
         """
         chg_ctrl_get_one = self.api.change_control_get_one(
             cc_id)
         return chg_ctrl_get_one
 
@@ -344,16 +335,15 @@
         # Set client apiversion if it is not already set
         pprint(
             "test_api_change_control_create_for_none_task_id_in_list")
         if self.get_version():
             pprint(
                 'CREATE CHANGE CONTROL FOR LIST OF NONE TASK IDs...')
             with self.assertRaises(CvpRequestError):
-                self.create_change_control_for_task([
-                                                     None])
+                self.create_change_control_for_task([None])
 
     def test_api_change_control_create_for_none_task_ids_not_list(self):
         """ Verify change_control_create_for_tasks for none task ids list
         """
         # Set client apiversion if it is not already set
         pprint(
             "test_api_change_control_create_for_none_task_ids_not_list")
@@ -427,15 +417,16 @@
             #                                     ' does not exist"}'
             # if self.clnt.apiversion < 8.0:
             #     # CVP 2021.X.X format
             #     pprint('USING ERROR MESSAGE FORMAT FOR CVP 2021.X.X')
             #     err_msg = "POST: https://" + node + "/api/resources/changecontrol/v1/" \
             #                                         "ChangeControlConfig : Request Error: " \
             #                                         "Bad Request -" \
-            #                                         " {\"code\":9,[ ]?\"message\":\"not approved\"}"
+            #                                         " {\"code\":9,[ ]?
+            #                                            \"message\":\"not approved\"}"
             # with self.assertRaisesRegex(CvpRequestError, err_msg):
             with self.assertRaises(CvpRequestError):
                 self.start_change_control(CHANGE_CONTROL_ID_INVALID)
 
     def test_api_change_control_delete_invalid_cc(self):
         """ Verify test_api_change_control_delete_invalid_cc
                  """
@@ -462,25 +453,25 @@
             pprint("CHANGE CONTROL GET ONE...")
             # chg_ctrl_get_one = self.api.change_control_get_one(self.cc_id)
             chg_ctrl_get_one = self.change_control_get_one(
                 self.cc_id)
             assert chg_ctrl_get_one is not None
             assert chg_ctrl_get_one['value']['key']['id'] == self.cc_id
             assert chg_ctrl_get_one['value']['change']['name'] == self.cc_name
-            assert chg_ctrl_get_one['value']['change']['stages']['values']['stage0'] \
-                ['action']['args']['values']['TaskID'] == task_id
+            assert chg_ctrl_get_one['value']['change']['stages']['values']['stage0'][
+                'action']['args']['values']['TaskID'] == task_id
             # verify with actual api output
             response = self.get_cc_status(
                 self.cc_id)
             assert chg_ctrl_get_one['value']['key']['id'] == response['value']['key']['id']
             assert chg_ctrl_get_one['value']['change']['name'] == response['value']['change'][
                 'name']
-            assert chg_ctrl_get_one['value']['change']['stages']['values']['stage0']['action'] \
-                ['args']['values']['TaskID'] == response['value']['change']['stages']['values'] \
-                ['stage0']['action']['args']['values']['TaskID']
+            assert chg_ctrl_get_one['value']['change']['stages']['values']['stage0']['action'][
+                'args']['values']['TaskID'] == response['value']['change']['stages']['values'][
+                    'stage0']['action']['args']['values']['TaskID']
 
             # Delete CC
             self.delete_change_control(self.cc_id)
 
             # Cancel Task
             self.cancel_task(task_id)
 
@@ -490,15 +481,15 @@
         pprint(
             "test_api_change_control_get_one_without_ccid")
         if self.get_version():
             pprint(
                 "CHANGE CONTROL GET ONE WITHOUT CC_ID...")
             err_msg = "change_control_get_one() missing 1 required positional argument: 'cc_id'"
             with self.assertRaises(TypeError) as ex:
-                self.change_control_get_one()
+                self.change_control_get_one() # pylint: disable=no-value-for-parameter
                 self.assertEqual(
                     err_msg, ex.exception)
 
     def test_api_change_control_get_one_with_none_ccid(self):
         """ Verify change_control_get_one_with_none_ccid
          """
         pprint(
@@ -657,35 +648,45 @@
                                                    }
                                           },
                                   '2': {'name': 'stage 2ab',
                                         'rows': {'values': [{'values': ['2a', '2b']}]
                                                  }
                                         },
                                   '1a': {'action': {'args': {'values': {'DeviceID': device_id_1,
-                                                                    'TemplateID': template_id[0]}},
+                                                                        'TemplateID': template_id[0]
+                                                                        }
+                                                             },
                                                     'name': 'snapshot',
                                                     'timeout': 3000},
                                          'name': 'stage 1a'},
                                   '1b': {'action': {'args': {'values': {'DeviceID': device_id_1,
-                                                                    'TemplateID': template_id[0]}},
+                                                                        'TemplateID': template_id[0]
+                                                                        }
+                                                             },
                                                     'name': 'snapshot',
                                                     'timeout': 3000},
                                          'name': 'stage 1b'},
                                   '2a': {'action': {'args': {'values': {'DeviceID': device_id_1,
-                                                                    'TemplateID': template_id[0]}},
+                                                                        'TemplateID': template_id[0]
+                                                                        }
+                                                             },
                                                     'name': 'snapshot',
                                                     'timeout': 3000},
                                          'name': 'stage 2a'},
                                   '2b': {'action': {'args': {'values': {'DeviceID': device_id_2,
-                                                                    'TemplateID': template_id[1]}},
+                                                                        'TemplateID': template_id[1]
+                                                                        }
+                                                             },
                                                     'name': 'snapshot',
                                                     'timeout': 3000},
                                          'name': 'stage 2a'},
                                   '3': {'action': {'args': {'values': {'DeviceID': device_id_2,
-                                                                    'TemplateID': template_id[1]}},
+                                                                       'TemplateID': template_id[1]
+                                                                       }
+                                                            },
                                                    'name': 'snapshot',
                                                    'timeout': 3000},
                                         'name': 'stage 3'},
                                   }}}}
 
         if self.get_version():
             pprint(
```

### Comparing `cvprac-1.3.2/test/system/test_cvp_client.py` & `cvprac-1.4.0/test/system/test_cvp_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,22 +60,22 @@
     # pylint: disable=invalid-name
     NEW_PASSWORD = 'ChangeMe'
 
     def setUp(self):
         ''' Instantiate the CvpClient class.
             Log messages to the /tmp/TestCvpClient.log
         '''
-        super(TestCvpClient, self).setUp()
+        super().setUp()
         self.clnt = CvpClient(filename='/tmp/TestCvpClient.log')
         self.assertIsNotNone(self.clnt)
 
     def tearDown(self):
         ''' Destroy the CvpClient class.
         '''
-        super(TestCvpClient, self).tearDown()
+        super().tearDown()
         self.clnt = None
 
     def _change_passwd(self, nodes, username, old_password, new_password):
         ''' Helper method to change the user password on CVP.
         '''
         # Create a new connection to handle the request.
         clnt = CvpClient(filename='/tmp/TestCvpClient.log')
@@ -154,15 +154,16 @@
     def test_connect_token_good(self):
         ''' Verify https connection succeeds to a single CVP node
             Uses https protocol and port with a valid token.
         '''
         dut = self.duts[0]
         if 'api_token' not in dut:
             raise unittest.SkipTest('No API token found for DUT. Skipping test.')
-        self.clnt.connect([dut['node']], dut['username'], dut['password'], api_token=dut['api_token'])
+        self.clnt.connect([dut['node']], dut['username'], dut['password'],
+                          api_token=dut['api_token'])
 
     def test_connect_set_request_timeout(self):
         ''' Verify API request timeout is set when provided to
             client connect method.
         '''
         dut = self.duts[0]
         self.clnt.connect([dut['node']], dut['username'], dut['password'],
@@ -193,15 +194,16 @@
     def test_connect_token_expired(self):
         ''' Verify connect fails with an expired token.
         '''
         dut = self.duts[0]
         if 'expired_api_token' not in dut:
             raise unittest.SkipTest('No Expired token given. Skipping test.')
         with self.assertRaises(CvpLoginError):
-            self.clnt.connect([dut['node']], dut['username'], 'password', api_token=dut['api_token_expired'])
+            self.clnt.connect([dut['node']], dut['username'], 'password',
+                              api_token=dut['api_token_expired'])
 
     def test_connect_node_bad(self):
         ''' Verify connection fails to a single bogus CVP node
         '''
         with self.assertRaises(CvpLoginError):
             self.clnt.connect(['bogus'], 'username', 'password',
                               connect_timeout=1)
```

### Comparing `cvprac-1.3.2/test/system/test_cvp_client_api.py` & `cvprac-1.4.0/test/system/test_cvp_client_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# pylint: disable=wrong-import-position
-# pylint: disable=too-many-lines
+# pylint: disable=wrong-import-position,too-many-lines
+# pylint: disable=consider-using-f-string,fixme
+# pylint: disable=too-many-branches,too-many-statements,too-many-locals
 #
 # Copyright (c) 2017, Arista Networks, Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are
 # met:
@@ -46,20 +47,19 @@
 
        and in the test log is the error:
 
          Failure response received from the netElement : ' Unauthorized User '
 '''
 import os
 import shutil
-import sys
 import time
 import unittest
 import uuid
-from pkg_resources import parse_version
 from pprint import pprint
+from packaging.version import parse
 import urllib3
 from test_cvp_base import TestCvpClientBase
 from requests.exceptions import Timeout
 from cvprac.cvp_client_errors import CvpApiError, CvpRequestError
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
@@ -712,26 +712,30 @@
         # that this error message changes. So this is version comparision and
         # parsing is repetitive.
         if not self.clnt.apiversion:
             self.api.get_cvp_info()
         version_components = self.clnt.version.split(".")
         if len(version_components) < 3:
             version_components.append("0")
-            self.log.info('Version found with less than 3 components.'
-                          ' Appending 0. Updated Version String - %s',
-                          ".".join(version_components))
+            full_version = ".".join(version_components)
+            pprint(f"Version found with less than 3 components."
+                   f" Appending 0. Updated Version String - {full_version}")
         full_version = ".".join(version_components)
 
-        config = 'interface ethernet1\n description test\nspanning-tree portfast\n!\nruter bgp something'
+        config = ("interface ethernet1\n description test\nspanning-tree"
+                  " portfast\n!\nruter bgp something")
         result = self.api.validate_config_for_device(self.device['key'], config)
-        expected_warning = "! portfast should only be enabled on ports connected to a single host. Connecting hubs, concentrators, switches, bridges, etc. to this interface when portfast is enabled can cause temporary bridging loops. Use with CAUTION. at line 3"
+        expected_warning = ("! portfast should only be enabled on ports connected to a single host."
+                            " Connecting hubs, concentrators, switches, bridges, etc. to this"
+                            " interface when portfast is enabled can cause temporary bridging"
+                            " loops. Use with CAUTION. at line 3")
         self.assertTrue(expected_warning in result["warnings"][0])
         expected_error = "> ruter bgp something% Invalid input "
         # Error message format changes as of 2021.1.0 or 2021.1.1
-        if parse_version(full_version) >= parse_version("2021.1.0"):
+        if parse(full_version) >= parse("2021.1.0"):
             expected_error += "(at token 0: 'ruter') "
         expected_error += "at line 5"
         self.assertEqual(result['errors'][0]["error"], expected_error)
         self.assertEqual(result['warningCount'], 1)
 
     def test_api_get_task_by_id_bad(self):
         ''' Verify get_task_by_id with bad task id
@@ -825,15 +829,15 @@
                 'formList': list,
                 'main_script': dict,
             }
             for key in list(exp_data.keys()):
                 self.assertIn(key, result['data'])
                 self.assertIsInstance(result['data'][key], exp_data[key])
         else:
-            print('No Base Configlet Builder SYS_TelemetryBuilerV* found. Skipping')
+            pprint('No Base Configlet Builder SYS_TelemetryBuilerV* found. Skipping')
             time.sleep(1)
 
     def test_api_get_configlet_by_name(self):
         ''' Verify get_configlet_by_name
         '''
         configlet = None
         for conf in self.dev_configlets:
@@ -923,14 +927,17 @@
         self.assertIsNotNone(result)
 
     def test_api_get_device_by_name(self):
         ''' Verify get_device_by_name
         '''
         result = self.api.get_device_by_name(self.device['fqdn'])
         self.assertIsNotNone(result)
+        # Remove hasZTR key as it is not in inventory data. This key was added
+        # in searchTopology V3 API return data.
+        result.pop('hasZTR', '')
         for key in result:
             self.assertIn(key, self.device)
             # Some differences in result values between inventory
             # and searchTopology. For example "no" vs "False" or
             # "false" vs "False"
             # self.assertEqual(result[key], self.device[key])
 
@@ -1907,32 +1914,31 @@
         for image in images:
             for key in remove_keys:
                 image.pop(key, None)
 
         # Create a new bundle with the same images
         original_name = f'test_image_bundle_{time.time()}'
         result = self.api.save_image_bundle(original_name, images)
-        expected = r'Bundle\s*:\s+%s successfully created' % original_name
-        self.assertRegexpMatches(result['data'], expected)
+        expected = r"Bundle\s*:\s+%s successfully created" % original_name
+        self.assertRegex(result['data'], expected)
 
         # Assert bundle added
         new_bundles = self.api.get_image_bundles()
         new_total = new_bundles['total']
         self.assertEqual(total + 1, new_total)
 
         # Get the bundle ID from the new bundle
         bundle = self.api.get_image_bundle_by_name(original_name)
         bundle_id = bundle['id']
 
         # Update the name of the bundle and mark it as uncertified
         updated_name = original_name + "_updated"
         result = self.api.update_image_bundle(bundle_id, updated_name, images,
                                               certified=False)
-        self.assertRegexpMatches(result['data'],
-                                 'Image bundle updated successfully')
+        self.assertRegex(result['data'], 'Image bundle updated successfully')
 
         # Verify the updated bundle name has the correct bundle ID
         # and is not a certified image bundle
         bundle = self.api.get_image_bundle_by_name(updated_name)
         bundle_id = bundle['id']
         bundle_name = bundle['name']
         self.assertEqual(bundle['id'], bundle_id)
@@ -2124,16 +2130,15 @@
         self.assertEqual(re_added_dev['systemMacAddress'],
                          test_dev['systemMacAddress'])
         # apply original configlets back to device
         results = self.api.apply_configlets_to_device("test_api_inventory",
                                                       test_dev, orig_configlets,
                                                       create_task=True)
         # execute returned task and wait for it to complete
-        task_res = self.api.execute_task(results['data']['taskIds'][0])
-        self.assertEqual(task_res, None)
+        self.api.execute_task(results['data']['taskIds'][0])
         task_status = self.api.get_task_by_id(results['data']['taskIds'][0])
         while task_status['taskStatus'] != 'COMPLETED':
             task_status = self.api.get_task_by_id(
                 results['data']['taskIds'][0])
             time.sleep(1)
         if self.clnt.apiversion >= 6.0:
             self.api.request_timeout = orig_timeout
@@ -2206,28 +2211,28 @@
     #         (task_id, _) = self._create_task()
     #         chg_ctrl = self.api.create_change_control_v3(
     #             chg_ctrl_name, chg_ctrl_name, [task_id], True)
     #         cc_id = ''
     #         if len(chg_ctrl) > 0:
     #             if 'id' in chg_ctrl[0]:
     #                 cc_id = chg_ctrl[0]['id']
-    #         print('')
-    #         print(chg_ctrl)
-    #         print(cc_id)
-    #         print('')
+    #         pprint('')
+    #         pprint(chg_ctrl)
+    #         pprint(cc_id)
+    #         pprint('')
     #
     #         if cc_id != '':
     #             # Verify the pending change control information
     #             status_url = '/cvpservice/changeControl/' \
     #                          'getChangeControlInformation.do?' \
     #                          'startIndex=0&endIndex=0&ccId={}'.format(cc_id)
     #             chg_ctrl_pending = self.clnt.get(status_url)
-    #             print('')
-    #             print(chg_ctrl_pending)
-    #             print('')
+    #             pprint('')
+    #             pprint(chg_ctrl_pending)
+    #             pprint('')
     #     else:
     #         pprint('SKIPPING TEST FOR API - {0}'.format(
     #             self.clnt.apiversion))
     #         time.sleep(1)
 
     def test_api_cancel_change_control(self):
         ''' Verify cancel_change_control.
@@ -2584,18 +2589,17 @@
                     if self.clnt.apiversion > 7.0:
                         self.assertIn('needsBuild', result['value'])
                         if not result['value']['needsBuild']:
                             # expect needsBuild to be set to True after a build
                             # once this is found we can break
                             self.assertEqual(result['value']['needsBuild'], False)
                             break
-                        else:
-                            # needsBuild has not yet been updated. Read workspace
-                            # data again.
-                            time.sleep(1)
+                        # needsBuild has not yet been updated. Read workspace
+                        # data again.
+                        time.sleep(1)
                     else:
                         # if no needsBuild parameter no need to repeat call to
                         # check it.
                         break
 
             # Test Submit Workspace
             new_submit_id = new_workspace_id + '_SUBMIT_' + str(new_uuid)
```

### Comparing `cvprac-1.3.2/test/unit/test_api.py` & `cvprac-1.4.0/test/unit/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=wrong-import-position
+# pylint: disable=wrong-import-position,line-too-long
 #
 # Copyright (c) 2017, Arista Networks, Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are
 # met:
@@ -32,15 +32,15 @@
 #
 
 """ Unit tests for the CvpAPI class
 """
 import unittest
 from itertools import cycle
 from cvprac.cvp_client import CvpClient
-from cvprac.cvp_api import CvpApi
+from cvprac.cvp_api import CvpApi, sanitize_warnings
 
 
 class TestAPI(unittest.TestCase):
     """Unit test cases for CvpAPI"""
 
     # pylint: disable=protected-access
     # pylint: disable=invalid-name
@@ -53,15 +53,15 @@
         self.clnt.nodes = nodes
         self.clnt.node_cnt = len(nodes)
         self.clnt.node_pool = cycle(nodes)
         self.api = CvpApi(self.clnt)
 
     def test_sanitize_warnings(self):
         """Test sanitization if warnings are split"""
-        input = {
+        test_input = {
             "warnings": [
                 "! Change will take effect only after switch reboot at line 11\\n\\n",
                 "! \\nWARNING!\\nChanging TCAM profile will cause forwarding agent(s) to exit and restart.\\nAll traffic through the forwarding chip managed by the restarting\\nforwarding agent will be dropped.\\n at line 392",
                 "! portfast should only be enabled on ports connected to a single host. Connecting hubs",
                 "concentrators",
                 "switches",
                 "bridges",
@@ -100,19 +100,19 @@
                 {
                     "lineNo": " 6",
                     "error": "> ruter bgp 1512% Invalid input (at token 0: 'ruter') at line 6",
                 }
             ],
             "errorCount": 1,
         }
-        assert self.api.sanitize_warnings(input) == expected
+        self.assertEqual(sanitize_warnings(test_input), expected)
 
     def test_sanitize_warnings_skip(self):
         """Test sanitization if no warnings need changing"""
-        input = {
+        test_input = {
             "result": [
                 {
                     "output": "enter input line by line; when done enter one or more control-d\n\n> spanning-tree portfast\n! portfast should only be enabled on ports connected to a single host. Connecting hubs, concentrators, switches, bridges, etc. to this interface when portfast is enabled can cause temporary bridging loops. Use with CAUTION. at line 2\nCopy completed successfully.\n",
                     "messages": ["Copy completed successfully."],
                 },
                 {
                     "output": "! Command: show session-configuration named capiVerify-2002-f8a137cac96e11ed89be020000000000\n! device: tp-avd-leaf2 (vEOS-lab, EOS-4.29.1F)\n!\n! boot system flash:/vEOS-lab-4.29.1F.swi\n!\nno aaa root\n!\ntransceiver qsfp default-mode 4x10G\n!\nservice routing protocols model ribd\n!\nspanning-tree mode mstp\n!\ninterface Ethernet1\n   spanning-tree portfast\n!\ninterface Ethernet2\n!\ninterface Ethernet3\n!\ninterface Ethernet4\n!\ninterface Ethernet5\n!\ninterface Management1\n!\nno ip routing\n!\nend\n"
@@ -122,8 +122,8 @@
                 "! portfast should only be enabled on ports connected to a single host. Connecting hubs, concentrators, switches, bridges, etc. to this interface when portfast is enabled can cause temporary bridging loops. Use with CAUTION. at line 2"
             ],
             "id": "Arista-3-4826123409839743",
             "warningCount": 1,
             "jsonrpc": "2.0",
         }
         # The result should not change
-        assert self.api.sanitize_warnings(input) == input
+        self.assertEqual(sanitize_warnings(test_input), test_input)
```

### Comparing `cvprac-1.3.2/test/unit/test_client.py` & `cvprac-1.4.0/test/unit/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 #
 
 ''' Unit tests for the CvpClient class
 '''
 import json
 import unittest
 from itertools import cycle
-from mock import Mock
+from unittest.mock import Mock
 from requests.exceptions import HTTPError, ReadTimeout, JSONDecodeError
 from cvprac.cvp_client import CvpClient
 from cvprac.cvp_client_errors import CvpApiError, CvpSessionLogOutError
 
 
 class TestClient(unittest.TestCase):
     """ Unit test cases for CvpClient
```

