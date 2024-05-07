# Comparing `tmp/accelbyte-py-sdk-service-inventory-0.4.0.tar.gz` & `tmp/accelbyte_py_sdk_service_inventory-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-inventory-0.4.0.tar", last modified: Tue Feb 27 05:38:41 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_inventory-0.5.0.tar", last modified: Tue May  7 06:28:17 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-inventory-0.4.0.tar` & `accelbyte_py_sdk_service_inventory-0.5.0.tar`

### file list

```diff
@@ -1,125 +1,142 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.886497 accelbyte-py-sdk-service-inventory-0.4.0/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-02-27 05:38:41.886497 accelbyte-py-sdk-service-inventory-0.4.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      876 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.878497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.878497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.878497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/
--rw-rw-r--   0 root         (0) root         (0)     4079 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.882497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/
--rw-rw-r--   0 root         (0) root         (0)     3254 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8049 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_admin_update_item_req.py
--rw-rw-r--   0 root         (0) root         (0)     5708 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_req.py
--rw-rw-r--   0 root         (0) root         (0)     6566 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5781 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item.py
--rw-rw-r--   0 root         (0) root         (0)     5104 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item_req.py
--rw-rw-r--   0 root         (0) root         (0)     8033 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_configuration_req.py
--rw-rw-r--   0 root         (0) root         (0)     4996 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_req.py
--rw-rw-r--   0 root         (0) root         (0)    11998 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item.py
--rw-rw-r--   0 root         (0) root         (0)     3774 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_req.py
--rw-rw-r--   0 root         (0) root         (0)     5155 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_resp.py
--rw-rw-r--   0 root         (0) root         (0)     4683 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_req.py
--rw-rw-r--   0 root         (0) root         (0)     6082 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_resp.py
--rw-rw-r--   0 root         (0) root         (0)     3844 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_delete_inventory_req.py
--rw-rw-r--   0 root         (0) root         (0)     4591 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_error_response.py
--rw-rw-r--   0 root         (0) root         (0)     7908 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_req.py
--rw-rw-r--   0 root         (0) root         (0)    11465 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_resp.py
--rw-rw-r--   0 root         (0) root         (0)    10855 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_resp.py
--rw-rw-r--   0 root         (0) root         (0)    13579 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_item_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5384 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_configurations_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5037 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_resp.py
--rw-rw-r--   0 root         (0) root         (0)     4928 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5113 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_types_resp.py
--rw-rw-r--   0 root         (0) root         (0)     4964 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_tags_resp.py
--rw-rw-r--   0 root         (0) root         (0)     4887 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_req.py
--rw-rw-r--   0 root         (0) root         (0)     7114 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_resp.py
--rw-rw-r--   0 root         (0) root         (0)     8219 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_operation.py
--rw-rw-r--   0 root         (0) root         (0)     5424 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_paging.py
--rw-rw-r--   0 root         (0) root         (0)     4655 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_inventory_item_req.py
--rw-rw-r--   0 root         (0) root         (0)     5208 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_item.py
--rw-rw-r--   0 root         (0) root         (0)    10269 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_req.py
--rw-rw-r--   0 root         (0) root         (0)     9350 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_to_inventory_req.py
--rw-rw-r--   0 root         (0) root         (0)     5021 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item.py
--rw-rw-r--   0 root         (0) root         (0)     5091 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item_resp.py
--rw-rw-r--   0 root         (0) root         (0)     3946 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_inventory_req.py
--rw-rw-r--   0 root         (0) root         (0)     8612 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item.py
--rw-rw-r--   0 root         (0) root         (0)     6193 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_req.py
--rw-rw-r--   0 root         (0) root         (0)     6400 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_resp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.882497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/
--rw-rw-r--   0 root         (0) root         (0)      437 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.882497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/
--rw-rw-r--   0 root         (0) root         (0)      544 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8964 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/admin_create_chaining_o_8801c9.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.882497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/
--rw-rw-r--   0 root         (0) root         (0)      828 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7660 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_create_inventory.py
--rw-rw-r--   0 root         (0) root         (0)     7309 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_get_inventory.py
--rw-rw-r--   0 root         (0) root         (0)    12144 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_list_inventories.py
--rw-rw-r--   0 root         (0) root         (0)     8690 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_update_inventory.py
--rw-rw-r--   0 root         (0) root         (0)     8365 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/delete_inventory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.882497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/
--rw-rw-r--   0 root         (0) root         (0)      966 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8009 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_create_inventory__71b514.py
--rw-rw-r--   0 root         (0) root         (0)     7874 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_delete_inventory__38371e.py
--rw-rw-r--   0 root         (0) root         (0)     7967 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_get_inventory_con_709281.py
--rw-rw-r--   0 root         (0) root         (0)    10735 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_list_inventory_co_67d862.py
--rw-rw-r--   0 root         (0) root         (0)     9497 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_update_inventory__e10746.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.882497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/
--rw-rw-r--   0 root         (0) root         (0)      723 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7751 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_create_item_type.py
--rw-rw-r--   0 root         (0) root         (0)     7120 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_delete_item_type.py
--rw-rw-r--   0 root         (0) root         (0)     9484 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_list_item_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.882497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/
--rw-rw-r--   0 root         (0) root         (0)      942 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9477 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_remove_items.py
--rw-rw-r--   0 root         (0) root         (0)     9495 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_update_my_items.py
--rw-rw-r--   0 root         (0) root         (0)     9237 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_consume_user_item.py
--rw-rw-r--   0 root         (0) root         (0)     9068 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_get_inventory_item.py
--rw-rw-r--   0 root         (0) root         (0)    12997 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_list_items.py
--rw-rw-r--   0 root         (0) root         (0)     8258 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item.py
--rw-rw-r--   0 root         (0) root         (0)     9398 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item_to_inventory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.882497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/
--rw-rw-r--   0 root         (0) root         (0)      679 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7609 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_create_tag.py
--rw-rw-r--   0 root         (0) root         (0)     6882 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_delete_tag.py
--rw-rw-r--   0 root         (0) root         (0)    10131 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_list_tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.886497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/
--rw-rw-r--   0 root         (0) root         (0)      621 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10858 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/public_list_inventories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.886497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/
--rw-rw-r--   0 root         (0) root         (0)      659 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10573 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/public_list_inventory_c_d1722b.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.886497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/
--rw-rw-r--   0 root         (0) root         (0)      615 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9332 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/public_list_item_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.886497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/
--rw-rw-r--   0 root         (0) root         (0)      878 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8559 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_remove_my_items.py
--rw-rw-r--   0 root         (0) root         (0)     8449 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_update_my_items.py
--rw-rw-r--   0 root         (0) root         (0)     8260 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_consume_my_item.py
--rw-rw-r--   0 root         (0) root         (0)     8854 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_get_item.py
--rw-rw-r--   0 root         (0) root         (0)    12843 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_list_items.py
--rw-rw-r--   0 root         (0) root         (0)     8108 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_move_my_items.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.886497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_tags/
--rw-rw-r--   0 root         (0) root         (0)      593 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_tags/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9239 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_tags/public_list_tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.886497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     4500 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6055 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_chaining_operations.py
--rw-rw-r--   0 root         (0) root         (0)    18905 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventories.py
--rw-rw-r--   0 root         (0) root         (0)    19912 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventory_configurations.py
--rw-rw-r--   0 root         (0) root         (0)    11247 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_item_types.py
--rw-rw-r--   0 root         (0) root         (0)    27479 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_items.py
--rw-rw-r--   0 root         (0) root         (0)    11013 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_tags.py
--rw-rw-r--   0 root         (0) root         (0)     4934 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventories.py
--rw-rw-r--   0 root         (0) root         (0)     4985 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventory_configurations.py
--rw-rw-r--   0 root         (0) root         (0)     4468 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_public_item_types.py
--rw-rw-r--   0 root         (0) root         (0)    20466 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_public_items.py
--rw-rw-r--   0 root         (0) root         (0)     4333 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_public_tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:41.886497 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk_service_inventory.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-02-27 05:38:41.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk_service_inventory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7509 2024-02-27 05:38:41.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk_service_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 05:38:41.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk_service_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-27 05:38:41.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk_service_inventory.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-27 05:38:41.000000 accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk_service_inventory.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      363 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-inventory-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 05:38:41.886497 accelbyte-py-sdk-service-inventory-0.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.389219 accelbyte_py_sdk_service_inventory-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-07 06:28:17.389219 accelbyte_py_sdk_service_inventory-0.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      876 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.377220 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.377220 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.377220 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/
+-rw-rw-r--   0 root         (0) root         (0)     4833 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/
+-rw-rw-r--   0 root         (0) root         (0)     4392 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8049 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_admin_update_item_req.py
+-rw-rw-r--   0 root         (0) root         (0)     5708 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_req.py
+-rw-rw-r--   0 root         (0) root         (0)     6566 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5781 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item.py
+-rw-rw-r--   0 root         (0) root         (0)     5104 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item_req.py
+-rw-rw-r--   0 root         (0) root         (0)     5967 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_integration_configuration_req.py
+-rw-rw-r--   0 root         (0) root         (0)     8033 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_configuration_req.py
+-rw-rw-r--   0 root         (0) root         (0)     4996 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_req.py
+-rw-rw-r--   0 root         (0) root         (0)    11998 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item.py
+-rw-rw-r--   0 root         (0) root         (0)     3774 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_req.py
+-rw-rw-r--   0 root         (0) root         (0)     5155 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     4683 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_req.py
+-rw-rw-r--   0 root         (0) root         (0)     6082 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     3844 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_delete_inventory_req.py
+-rw-rw-r--   0 root         (0) root         (0)     4591 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_error_response.py
+-rw-rw-r--   0 root         (0) root         (0)     9060 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_integration_configuration_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     3910 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7908 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_req.py
+-rw-rw-r--   0 root         (0) root         (0)    11465 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_resp.py
+-rw-rw-r--   0 root         (0) root         (0)    10855 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_resp.py
+-rw-rw-r--   0 root         (0) root         (0)    14498 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_item_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5422 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_integration_configurations_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5384 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_configurations_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5037 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5113 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_types_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     4964 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_tags_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     4887 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_req.py
+-rw-rw-r--   0 root         (0) root         (0)     7114 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     8219 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_operation.py
+-rw-rw-r--   0 root         (0) root         (0)     5424 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_paging.py
+-rw-rw-r--   0 root         (0) root         (0)     8658 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_purchase_validation_item_req.py
+-rw-rw-r--   0 root         (0) root         (0)     9837 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_purchase_validation_req.py
+-rw-rw-r--   0 root         (0) root         (0)     4655 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_inventory_item_req.py
+-rw-rw-r--   0 root         (0) root         (0)     5208 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_item.py
+-rw-rw-r--   0 root         (0) root         (0)    11261 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_req.py
+-rw-rw-r--   0 root         (0) root         (0)    10367 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_to_inventory_req.py
+-rw-rw-r--   0 root         (0) root         (0)     5021 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item.py
+-rw-rw-r--   0 root         (0) root         (0)     5091 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5967 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_integration_configuration_req.py
+-rw-rw-r--   0 root         (0) root         (0)     3946 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_inventory_req.py
+-rw-rw-r--   0 root         (0) root         (0)     8612 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item.py
+-rw-rw-r--   0 root         (0) root         (0)     6193 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_req.py
+-rw-rw-r--   0 root         (0) root         (0)     6400 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     4446 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_status_integration_configuration_req.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/
+-rw-rw-r--   0 root         (0) root         (0)      437 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/
+-rw-rw-r--   0 root         (0) root         (0)      544 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9263 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/admin_create_chaining_o_8801c9.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/
+-rw-rw-r--   0 root         (0) root         (0)      907 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8368 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_create_integratio_c6b1bd.py
+-rw-rw-r--   0 root         (0) root         (0)     9942 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_list_integration__420e8d.py
+-rw-rw-r--   0 root         (0) root         (0)    10071 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_update_integratio_fe692f.py
+-rw-rw-r--   0 root         (0) root         (0)    10290 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_update_status_int_703321.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/
+-rw-rw-r--   0 root         (0) root         (0)      876 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7952 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_create_inventory.py
+-rw-rw-r--   0 root         (0) root         (0)     7615 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_get_inventory.py
+-rw-rw-r--   0 root         (0) root         (0)    12436 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_list_inventories.py
+-rw-rw-r--   0 root         (0) root         (0)     8825 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_purchasable.py
+-rw-rw-r--   0 root         (0) root         (0)     8996 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_update_inventory.py
+-rw-rw-r--   0 root         (0) root         (0)     8671 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/delete_inventory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/
+-rw-rw-r--   0 root         (0) root         (0)      966 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8313 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_create_inventory__71b514.py
+-rw-rw-r--   0 root         (0) root         (0)     8205 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_delete_inventory__38371e.py
+-rw-rw-r--   0 root         (0) root         (0)     8298 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_get_inventory_con_709281.py
+-rw-rw-r--   0 root         (0) root         (0)    11039 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_list_inventory_co_67d862.py
+-rw-rw-r--   0 root         (0) root         (0)     9828 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_update_inventory__e10746.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/
+-rw-rw-r--   0 root         (0) root         (0)      723 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8041 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_create_item_type.py
+-rw-rw-r--   0 root         (0) root         (0)     7425 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_delete_item_type.py
+-rw-rw-r--   0 root         (0) root         (0)     9774 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_list_item_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/
+-rw-rw-r--   0 root         (0) root         (0)     1010 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9804 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_remove_items.py
+-rw-rw-r--   0 root         (0) root         (0)     9822 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_update_my_items.py
+-rw-rw-r--   0 root         (0) root         (0)     9566 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_consume_user_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9416 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_get_inventory_item.py
+-rw-rw-r--   0 root         (0) root         (0)    13325 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_list_items.py
+-rw-rw-r--   0 root         (0) root         (0)     8703 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9725 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item_to_inventory.py
+-rw-rw-r--   0 root         (0) root         (0)     7889 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_sync_user_entitlements.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/
+-rw-rw-r--   0 root         (0) root         (0)      679 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7894 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_create_tag.py
+-rw-rw-r--   0 root         (0) root         (0)     7177 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_delete_tag.py
+-rw-rw-r--   0 root         (0) root         (0)    10416 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_list_tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/
+-rw-rw-r--   0 root         (0) root         (0)      621 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11160 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/public_list_inventories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/
+-rw-rw-r--   0 root         (0) root         (0)      659 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10878 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/public_list_inventory_c_d1722b.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/
+-rw-rw-r--   0 root         (0) root         (0)      615 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9623 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/public_list_item_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/
+-rw-rw-r--   0 root         (0) root         (0)      878 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8881 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_remove_my_items.py
+-rw-rw-r--   0 root         (0) root         (0)     8771 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_update_my_items.py
+-rw-rw-r--   0 root         (0) root         (0)     8584 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_consume_my_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9212 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_get_item.py
+-rw-rw-r--   0 root         (0) root         (0)    13165 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_list_items.py
+-rw-rw-r--   0 root         (0) root         (0)     8439 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_move_my_items.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_tags/
+-rw-rw-r--   0 root         (0) root         (0)      593 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_tags/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9525 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_tags/public_list_tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     5492 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6055 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_chaining_operations.py
+-rw-rw-r--   0 root         (0) root         (0)    17453 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_integration_configurations.py
+-rw-rw-r--   0 root         (0) root         (0)    22341 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventories.py
+-rw-rw-r--   0 root         (0) root         (0)    19912 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventory_configurations.py
+-rw-rw-r--   0 root         (0) root         (0)    11247 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_item_types.py
+-rw-rw-r--   0 root         (0) root         (0)    31125 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_items.py
+-rw-rw-r--   0 root         (0) root         (0)    11013 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_tags.py
+-rw-rw-r--   0 root         (0) root         (0)     4934 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventories.py
+-rw-rw-r--   0 root         (0) root         (0)     4985 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventory_configurations.py
+-rw-rw-r--   0 root         (0) root         (0)     4468 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_item_types.py
+-rw-rw-r--   0 root         (0) root         (0)    20466 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_items.py
+-rw-rw-r--   0 root         (0) root         (0)     4333 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-07 06:28:17.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8940 2024-05-07 06:28:17.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:28:17.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:28:17.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:28:17.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      363 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:28:17.389219 accelbyte_py_sdk_service_inventory-0.5.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/PKG-INFO` & `accelbyte_py_sdk_service_inventory-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-inventory
-Version: 0.4.0
+Version: 0.5.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Inventory Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Inventory Service
-* Version: 0.1.0
+* Version: 0.1.3
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/README.md` & `accelbyte_py_sdk_service_inventory-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Inventory Service
-* Version: 0.1.0
+* Version: 0.1.3
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,31 +4,43 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # admin_chaining_operations
 from .wrappers import admin_create_chaining_operations
 from .wrappers import admin_create_chaining_operations_async
 
+# admin_integration_configurations
+from .wrappers import admin_create_integration_configuration
+from .wrappers import admin_create_integration_configuration_async
+from .wrappers import admin_list_integration_configurations
+from .wrappers import admin_list_integration_configurations_async
+from .wrappers import admin_update_integration_configuration
+from .wrappers import admin_update_integration_configuration_async
+from .wrappers import admin_update_status_integration_configuration
+from .wrappers import admin_update_status_integration_configuration_async
+
 # admin_inventories
 from .wrappers import admin_create_inventory
 from .wrappers import admin_create_inventory_async
 from .wrappers import admin_get_inventory
 from .wrappers import admin_get_inventory_async
 from .wrappers import admin_list_inventories
 from .wrappers import admin_list_inventories_async
+from .wrappers import admin_purchasable
+from .wrappers import admin_purchasable_async
 from .wrappers import admin_update_inventory
 from .wrappers import admin_update_inventory_async
 from .wrappers import delete_inventory
 from .wrappers import delete_inventory_async
 
 # admin_inventory_configurations
 from .wrappers import admin_create_inventory_configuration
@@ -61,14 +73,16 @@
 from .wrappers import admin_get_inventory_item_async
 from .wrappers import admin_list_items
 from .wrappers import admin_list_items_async
 from .wrappers import admin_save_item
 from .wrappers import admin_save_item_async
 from .wrappers import admin_save_item_to_inventory
 from .wrappers import admin_save_item_to_inventory_async
+from .wrappers import admin_sync_user_entitlements
+from .wrappers import admin_sync_user_entitlements_async
 
 # admin_tags
 from .wrappers import admin_create_tag
 from .wrappers import admin_create_tag_async
 from .wrappers import admin_delete_tag
 from .wrappers import admin_delete_tag_async
 from .wrappers import admin_list_tags
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,59 +4,84 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .apimodels_admin_update_item_req import ApimodelsAdminUpdateItemReq
 from .apimodels_chaining_operation_req import ApimodelsChainingOperationReq
 from .apimodels_chaining_operation_resp import ApimodelsChainingOperationResp
 from .apimodels_consume_item import ApimodelsConsumeItem
 from .apimodels_consume_item_req import ApimodelsConsumeItemReq
+from .apimodels_create_integration_configuration_req import (
+    ApimodelsCreateIntegrationConfigurationReq,
+)
 from .apimodels_create_inventory_configuration_req import (
     ApimodelsCreateInventoryConfigurationReq,
 )
 from .apimodels_create_inventory_req import ApimodelsCreateInventoryReq
 from .apimodels_create_item import ApimodelsCreateItem
 from .apimodels_create_item_type_req import ApimodelsCreateItemTypeReq
 from .apimodels_create_item_type_resp import ApimodelsCreateItemTypeResp
 from .apimodels_create_tag_req import ApimodelsCreateTagReq
 from .apimodels_create_tag_req import OwnerEnum as ApimodelsCreateTagReqOwnerEnum
 from .apimodels_create_tag_resp import ApimodelsCreateTagResp
 from .apimodels_create_tag_resp import OwnerEnum as ApimodelsCreateTagRespOwnerEnum
 from .apimodels_delete_inventory_req import ApimodelsDeleteInventoryReq
 from .apimodels_error_response import ApimodelsErrorResponse
+from .apimodels_integration_configuration_resp import (
+    ApimodelsIntegrationConfigurationResp,
+)
+from .apimodels_inventory_config import ApimodelsInventoryConfig
 from .apimodels_inventory_configuration_req import ApimodelsInventoryConfigurationReq
 from .apimodels_inventory_configuration_resp import ApimodelsInventoryConfigurationResp
 from .apimodels_inventory_configuration_resp import (
     StatusEnum as ApimodelsInventoryConfigurationRespStatusEnum,
 )
 from .apimodels_inventory_resp import ApimodelsInventoryResp
 from .apimodels_item_resp import ApimodelsItemResp
+from .apimodels_list_integration_configurations_resp import (
+    ApimodelsListIntegrationConfigurationsResp,
+)
 from .apimodels_list_inventory_configurations_resp import (
     ApimodelsListInventoryConfigurationsResp,
 )
 from .apimodels_list_inventory_resp import ApimodelsListInventoryResp
 from .apimodels_list_item_resp import ApimodelsListItemResp
 from .apimodels_list_item_types_resp import ApimodelsListItemTypesResp
 from .apimodels_list_tags_resp import ApimodelsListTagsResp
 from .apimodels_move_items_req import ApimodelsMoveItemsReq
 from .apimodels_move_items_resp import ApimodelsMoveItemsResp
 from .apimodels_operation import ApimodelsOperation
 from .apimodels_paging import ApimodelsPaging
+from .apimodels_purchase_validation_item_req import ApimodelsPurchaseValidationItemReq
+from .apimodels_purchase_validation_req import ApimodelsPurchaseValidationReq
 from .apimodels_remove_inventory_item_req import ApimodelsRemoveInventoryItemReq
 from .apimodels_remove_item import ApimodelsRemoveItem
 from .apimodels_save_item_req import ApimodelsSaveItemReq
+from .apimodels_save_item_req import SourceEnum as ApimodelsSaveItemReqSourceEnum
 from .apimodels_save_item_to_inventory_req import ApimodelsSaveItemToInventoryReq
+from .apimodels_save_item_to_inventory_req import (
+    SourceEnum as ApimodelsSaveItemToInventoryReqSourceEnum,
+)
 from .apimodels_trade_item import ApimodelsTradeItem
 from .apimodels_trade_item_resp import ApimodelsTradeItemResp
+from .apimodels_update_integration_configuration_req import (
+    ApimodelsUpdateIntegrationConfigurationReq,
+)
 from .apimodels_update_inventory_req import ApimodelsUpdateInventoryReq
 from .apimodels_update_item import ApimodelsUpdateItem
 from .apimodels_update_item_req import ApimodelsUpdateItemReq
 from .apimodels_update_item_resp import ApimodelsUpdateItemResp
+from .apimodels_update_status_integration_configuration_req import (
+    ApimodelsUpdateStatusIntegrationConfigurationReq,
+)
+from .apimodels_update_status_integration_configuration_req import (
+    StatusEnum as ApimodelsUpdateStatusIntegrationConfigurationReqStatusEnum,
+)
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_admin_update_item_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_admin_update_item_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_configuration_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_configuration_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_delete_inventory_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_delete_inventory_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_error_response.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_error_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_item_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_item_resp.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,16 @@
         tags: (tags) REQUIRED List[str]
 
         type_: (type) REQUIRED str
 
         updated_at: (updatedAt) REQUIRED str
 
         user_id: (userId) REQUIRED str
+
+        platform_available: (platformAvailable) OPTIONAL bool
     """
 
     # region fields
 
     created_at: str  # REQUIRED
     custom_attributes: Dict[str, Any]  # REQUIRED
     id_: str  # REQUIRED
@@ -76,14 +78,15 @@
     slot_used: int  # REQUIRED
     source: str  # REQUIRED
     source_item_id: str  # REQUIRED
     tags: List[str]  # REQUIRED
     type_: str  # REQUIRED
     updated_at: str  # REQUIRED
     user_id: str  # REQUIRED
+    platform_available: bool  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_created_at(self, value: str) -> ApimodelsItemResp:
         self.created_at = value
@@ -141,14 +144,18 @@
         self.updated_at = value
         return self
 
     def with_user_id(self, value: str) -> ApimodelsItemResp:
         self.user_id = value
         return self
 
+    def with_platform_available(self, value: bool) -> ApimodelsItemResp:
+        self.platform_available = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "created_at"):
@@ -211,14 +218,18 @@
             result["updatedAt"] = str(self.updated_at)
         elif include_empty:
             result["updatedAt"] = ""
         if hasattr(self, "user_id"):
             result["userId"] = str(self.user_id)
         elif include_empty:
             result["userId"] = ""
+        if hasattr(self, "platform_available"):
+            result["platformAvailable"] = bool(self.platform_available)
+        elif include_empty:
+            result["platformAvailable"] = False
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
@@ -235,14 +246,15 @@
         slot_used: int,
         source: str,
         source_item_id: str,
         tags: List[str],
         type_: str,
         updated_at: str,
         user_id: str,
+        platform_available: Optional[bool] = None,
         **kwargs,
     ) -> ApimodelsItemResp:
         instance = cls()
         instance.created_at = created_at
         instance.custom_attributes = custom_attributes
         instance.id_ = id_
         instance.inventory_id = inventory_id
@@ -253,14 +265,16 @@
         instance.slot_used = slot_used
         instance.source = source
         instance.source_item_id = source_item_id
         instance.tags = tags
         instance.type_ = type_
         instance.updated_at = updated_at
         instance.user_id = user_id
+        if platform_available is not None:
+            instance.platform_available = platform_available
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ApimodelsItemResp:
         instance = cls()
@@ -329,14 +343,18 @@
             instance.updated_at = str(dict_["updatedAt"])
         elif include_empty:
             instance.updated_at = ""
         if "userId" in dict_ and dict_["userId"] is not None:
             instance.user_id = str(dict_["userId"])
         elif include_empty:
             instance.user_id = ""
+        if "platformAvailable" in dict_ and dict_["platformAvailable"] is not None:
+            instance.platform_available = bool(dict_["platformAvailable"])
+        elif include_empty:
+            instance.platform_available = False
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ApimodelsItemResp]:
         return (
@@ -385,14 +403,15 @@
             "slotUsed": "slot_used",
             "source": "source",
             "sourceItemId": "source_item_id",
             "tags": "tags",
             "type": "type_",
             "updatedAt": "updated_at",
             "userId": "user_id",
+            "platformAvailable": "platform_available",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "createdAt": True,
             "customAttributes": True,
@@ -405,10 +424,11 @@
             "slotUsed": True,
             "source": True,
             "sourceItemId": True,
             "tags": True,
             "type": True,
             "updatedAt": True,
             "userId": True,
+            "platformAvailable": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_configurations_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_configurations_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_types_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_types_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_tags_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_tags_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_operation.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_operation.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_paging.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_paging.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_inventory_item_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_inventory_item_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_item.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_req.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
+from accelbyte_py_sdk.core import StrEnum
+
+
+class SourceEnum(StrEnum):
+    ECOMMERCE = "ECOMMERCE"
+    OTHER = "OTHER"
 
 
 class ApimodelsSaveItemReq(Model):
     """Apimodels save item req (apimodels.SaveItemReq)
 
     Properties:
         custom_attributes: (customAttributes) REQUIRED Dict[str, Any]
@@ -40,14 +46,16 @@
 
         server_custom_attributes: (serverCustomAttributes) REQUIRED Dict[str, Any]
 
         slot_id: (slotId) REQUIRED str
 
         slot_used: (slotUsed) REQUIRED int
 
+        source: (source) REQUIRED Union[str, SourceEnum]
+
         source_item_id: (sourceItemId) REQUIRED str
 
         tags: (tags) REQUIRED List[str]
 
         type_: (type) REQUIRED str
     """
 
@@ -55,14 +63,15 @@
 
     custom_attributes: Dict[str, Any]  # REQUIRED
     inventory_configuration_code: str  # REQUIRED
     qty: int  # REQUIRED
     server_custom_attributes: Dict[str, Any]  # REQUIRED
     slot_id: str  # REQUIRED
     slot_used: int  # REQUIRED
+    source: Union[str, SourceEnum]  # REQUIRED
     source_item_id: str  # REQUIRED
     tags: List[str]  # REQUIRED
     type_: str  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
@@ -89,14 +98,18 @@
         self.slot_id = value
         return self
 
     def with_slot_used(self, value: int) -> ApimodelsSaveItemReq:
         self.slot_used = value
         return self
 
+    def with_source(self, value: Union[str, SourceEnum]) -> ApimodelsSaveItemReq:
+        self.source = value
+        return self
+
     def with_source_item_id(self, value: str) -> ApimodelsSaveItemReq:
         self.source_item_id = value
         return self
 
     def with_tags(self, value: List[str]) -> ApimodelsSaveItemReq:
         self.tags = value
         return self
@@ -137,14 +150,18 @@
             result["slotId"] = str(self.slot_id)
         elif include_empty:
             result["slotId"] = ""
         if hasattr(self, "slot_used"):
             result["slotUsed"] = int(self.slot_used)
         elif include_empty:
             result["slotUsed"] = 0
+        if hasattr(self, "source"):
+            result["source"] = str(self.source)
+        elif include_empty:
+            result["source"] = Union[str, SourceEnum]()
         if hasattr(self, "source_item_id"):
             result["sourceItemId"] = str(self.source_item_id)
         elif include_empty:
             result["sourceItemId"] = ""
         if hasattr(self, "tags"):
             result["tags"] = [str(i0) for i0 in self.tags]
         elif include_empty:
@@ -164,26 +181,28 @@
         cls,
         custom_attributes: Dict[str, Any],
         inventory_configuration_code: str,
         qty: int,
         server_custom_attributes: Dict[str, Any],
         slot_id: str,
         slot_used: int,
+        source: Union[str, SourceEnum],
         source_item_id: str,
         tags: List[str],
         type_: str,
         **kwargs,
     ) -> ApimodelsSaveItemReq:
         instance = cls()
         instance.custom_attributes = custom_attributes
         instance.inventory_configuration_code = inventory_configuration_code
         instance.qty = qty
         instance.server_custom_attributes = server_custom_attributes
         instance.slot_id = slot_id
         instance.slot_used = slot_used
+        instance.source = source
         instance.source_item_id = source_item_id
         instance.tags = tags
         instance.type_ = type_
         return instance
 
     @classmethod
     def create_from_dict(
@@ -224,14 +243,18 @@
             instance.slot_id = str(dict_["slotId"])
         elif include_empty:
             instance.slot_id = ""
         if "slotUsed" in dict_ and dict_["slotUsed"] is not None:
             instance.slot_used = int(dict_["slotUsed"])
         elif include_empty:
             instance.slot_used = 0
+        if "source" in dict_ and dict_["source"] is not None:
+            instance.source = str(dict_["source"])
+        elif include_empty:
+            instance.source = Union[str, SourceEnum]()
         if "sourceItemId" in dict_ and dict_["sourceItemId"] is not None:
             instance.source_item_id = str(dict_["sourceItemId"])
         elif include_empty:
             instance.source_item_id = ""
         if "tags" in dict_ and dict_["tags"] is not None:
             instance.tags = [str(i0) for i0 in dict_["tags"]]
         elif include_empty:
@@ -285,27 +308,35 @@
         return {
             "customAttributes": "custom_attributes",
             "inventoryConfigurationCode": "inventory_configuration_code",
             "qty": "qty",
             "serverCustomAttributes": "server_custom_attributes",
             "slotId": "slot_id",
             "slotUsed": "slot_used",
+            "source": "source",
             "sourceItemId": "source_item_id",
             "tags": "tags",
             "type": "type_",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "customAttributes": True,
             "inventoryConfigurationCode": True,
             "qty": True,
             "serverCustomAttributes": True,
             "slotId": True,
             "slotUsed": True,
+            "source": True,
             "sourceItemId": True,
             "tags": True,
             "type": True,
         }
 
+    @staticmethod
+    def get_enum_map() -> Dict[str, List[Any]]:
+        return {
+            "source": ["ECOMMERCE", "OTHER"],
+        }
+
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_to_inventory_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_to_inventory_req.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
+from accelbyte_py_sdk.core import StrEnum
+
+
+class SourceEnum(StrEnum):
+    ECOMMERCE = "ECOMMERCE"
+    OTHER = "OTHER"
 
 
 class ApimodelsSaveItemToInventoryReq(Model):
     """Apimodels save item to inventory req (apimodels.SaveItemToInventoryReq)
 
     Properties:
         custom_attributes: (customAttributes) REQUIRED Dict[str, Any]
@@ -38,28 +44,31 @@
 
         server_custom_attributes: (serverCustomAttributes) REQUIRED Dict[str, Any]
 
         slot_id: (slotId) REQUIRED str
 
         slot_used: (slotUsed) REQUIRED int
 
+        source: (source) REQUIRED Union[str, SourceEnum]
+
         source_item_id: (sourceItemId) REQUIRED str
 
         tags: (tags) REQUIRED List[str]
 
         type_: (type) REQUIRED str
     """
 
     # region fields
 
     custom_attributes: Dict[str, Any]  # REQUIRED
     qty: int  # REQUIRED
     server_custom_attributes: Dict[str, Any]  # REQUIRED
     slot_id: str  # REQUIRED
     slot_used: int  # REQUIRED
+    source: Union[str, SourceEnum]  # REQUIRED
     source_item_id: str  # REQUIRED
     tags: List[str]  # REQUIRED
     type_: str  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
@@ -84,14 +93,20 @@
         self.slot_id = value
         return self
 
     def with_slot_used(self, value: int) -> ApimodelsSaveItemToInventoryReq:
         self.slot_used = value
         return self
 
+    def with_source(
+        self, value: Union[str, SourceEnum]
+    ) -> ApimodelsSaveItemToInventoryReq:
+        self.source = value
+        return self
+
     def with_source_item_id(self, value: str) -> ApimodelsSaveItemToInventoryReq:
         self.source_item_id = value
         return self
 
     def with_tags(self, value: List[str]) -> ApimodelsSaveItemToInventoryReq:
         self.tags = value
         return self
@@ -126,14 +141,18 @@
             result["slotId"] = str(self.slot_id)
         elif include_empty:
             result["slotId"] = ""
         if hasattr(self, "slot_used"):
             result["slotUsed"] = int(self.slot_used)
         elif include_empty:
             result["slotUsed"] = 0
+        if hasattr(self, "source"):
+            result["source"] = str(self.source)
+        elif include_empty:
+            result["source"] = Union[str, SourceEnum]()
         if hasattr(self, "source_item_id"):
             result["sourceItemId"] = str(self.source_item_id)
         elif include_empty:
             result["sourceItemId"] = ""
         if hasattr(self, "tags"):
             result["tags"] = [str(i0) for i0 in self.tags]
         elif include_empty:
@@ -152,25 +171,27 @@
     def create(
         cls,
         custom_attributes: Dict[str, Any],
         qty: int,
         server_custom_attributes: Dict[str, Any],
         slot_id: str,
         slot_used: int,
+        source: Union[str, SourceEnum],
         source_item_id: str,
         tags: List[str],
         type_: str,
         **kwargs,
     ) -> ApimodelsSaveItemToInventoryReq:
         instance = cls()
         instance.custom_attributes = custom_attributes
         instance.qty = qty
         instance.server_custom_attributes = server_custom_attributes
         instance.slot_id = slot_id
         instance.slot_used = slot_used
+        instance.source = source
         instance.source_item_id = source_item_id
         instance.tags = tags
         instance.type_ = type_
         return instance
 
     @classmethod
     def create_from_dict(
@@ -202,14 +223,18 @@
             instance.slot_id = str(dict_["slotId"])
         elif include_empty:
             instance.slot_id = ""
         if "slotUsed" in dict_ and dict_["slotUsed"] is not None:
             instance.slot_used = int(dict_["slotUsed"])
         elif include_empty:
             instance.slot_used = 0
+        if "source" in dict_ and dict_["source"] is not None:
+            instance.source = str(dict_["source"])
+        elif include_empty:
+            instance.source = Union[str, SourceEnum]()
         if "sourceItemId" in dict_ and dict_["sourceItemId"] is not None:
             instance.source_item_id = str(dict_["sourceItemId"])
         elif include_empty:
             instance.source_item_id = ""
         if "tags" in dict_ and dict_["tags"] is not None:
             instance.tags = [str(i0) for i0 in dict_["tags"]]
         elif include_empty:
@@ -262,26 +287,34 @@
     def get_field_info() -> Dict[str, str]:
         return {
             "customAttributes": "custom_attributes",
             "qty": "qty",
             "serverCustomAttributes": "server_custom_attributes",
             "slotId": "slot_id",
             "slotUsed": "slot_used",
+            "source": "source",
             "sourceItemId": "source_item_id",
             "tags": "tags",
             "type": "type_",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "customAttributes": True,
             "qty": True,
             "serverCustomAttributes": True,
             "slotId": True,
             "slotUsed": True,
+            "source": True,
             "sourceItemId": True,
             "tags": True,
             "type": True,
         }
 
+    @staticmethod
+    def get_enum_map() -> Dict[str, List[Any]]:
+        return {
+            "source": ["ECOMMERCE", "OTHER"],
+        }
+
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_inventory_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_inventory_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_req.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_resp.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_chaining_o_8801c9 import AdminCreateChainingOperations
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/admin_create_chaining_o_8801c9.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/admin_create_chaining_o_8801c9.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,32 +85,44 @@
 
         500: Internal Server Error - ApimodelsChainingOperationResp (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/chainingOperations"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/chainingOperations"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     body: ApimodelsChainingOperationReq  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_inventory import AdminCreateInventory
 from .admin_get_inventory import AdminGetInventory
 from .admin_list_inventories import AdminListInventories
 from .admin_list_inventories import (
     SortByEnum as AdminListInventoriesSortByEnum,
 )
+from .admin_purchasable import AdminPurchasable
 from .admin_update_inventory import AdminUpdateInventory
 from .delete_inventory import DeleteInventory
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_create_inventory.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_create_inventory.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,32 +71,44 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/inventories"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/inventories"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     body: ApimodelsCreateInventoryReq  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_get_inventory.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_get_inventory.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,32 +69,44 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/inventories/{inventoryId}"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/inventories/{inventoryId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_list_inventories.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_list_inventories.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,20 +89,24 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/inventories"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/inventories"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     namespace: str  # REQUIRED in [path]
     inventory_configuration_code: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     sort_by: Union[str, SortByEnum]  # OPTIONAL in [query]
     user_id: str  # OPTIONAL in [query]
 
@@ -111,14 +115,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_update_inventory.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/delete_inventory.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,83 +25,92 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
+from ...models import ApimodelsDeleteInventoryReq
 from ...models import ApimodelsErrorResponse
-from ...models import ApimodelsInventoryResp
-from ...models import ApimodelsUpdateInventoryReq
 
 
-class AdminUpdateInventory(Operation):
-    """To update inventory (AdminUpdateInventory)
+class DeleteInventory(Operation):
+    """To delete inventory (deleteInventory)
 
-    Updating an inventory.
-    Positive value will increase MaxSlots from existing value
-    Negative value will decrease MaxSlots from existing value
-    Limited slots can not be changed to unlimited, vice versa
+    Deleting an inventory.
+    If an inventory still has items, it cannot be deleted.
 
-    Permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY [UPDATE]
+    ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY [DELETE]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY [UPDATE]
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY [DELETE]
 
     Properties:
         url: /inventory/v1/admin/namespaces/{namespace}/inventories/{inventoryId}
 
-        method: PUT
+        method: DELETE
 
         tags: ["Admin Inventories"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ApimodelsUpdateInventoryReq in body
+        body: (body) REQUIRED ApimodelsDeleteInventoryReq in body
 
         inventory_id: (inventoryId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ApimodelsInventoryResp (OK)
+        204: No Content - (No Content)
 
         400: Bad Request - ApimodelsErrorResponse (Bad Request)
 
         404: Not Found - ApimodelsErrorResponse (Not Found)
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/inventories/{inventoryId}"
-    _method: str = "PUT"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/inventories/{inventoryId}"
+    _base_path: str = ""
+    _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ApimodelsUpdateInventoryReq  # REQUIRED in [body]
+    service_name: Optional[str] = "inventory"
+
+    body: ApimodelsDeleteInventoryReq  # REQUIRED in [body]
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -148,36 +157,36 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ApimodelsUpdateInventoryReq) -> AdminUpdateInventory:
+    def with_body(self, value: ApimodelsDeleteInventoryReq) -> DeleteInventory:
         self.body = value
         return self
 
-    def with_inventory_id(self, value: str) -> AdminUpdateInventory:
+    def with_inventory_id(self, value: str) -> DeleteInventory:
         self.inventory_id = value
         return self
 
-    def with_namespace(self, value: str) -> AdminUpdateInventory:
+    def with_namespace(self, value: str) -> DeleteInventory:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ApimodelsUpdateInventoryReq()
+            result["body"] = ApimodelsDeleteInventoryReq()
         if hasattr(self, "inventory_id") and self.inventory_id:
             result["inventoryId"] = str(self.inventory_id)
         elif include_empty:
             result["inventoryId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
@@ -187,21 +196,18 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, ApimodelsInventoryResp],
-        Union[None, ApimodelsErrorResponse, HttpResponse],
-    ]:
+    ) -> Tuple[None, Union[None, ApimodelsErrorResponse, HttpResponse]]:
         """Parse the given response.
 
-        200: OK - ApimodelsInventoryResp (OK)
+        204: No Content - (No Content)
 
         400: Bad Request - ApimodelsErrorResponse (Bad Request)
 
         404: Not Found - ApimodelsErrorResponse (Not Found)
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
 
@@ -214,16 +220,16 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return ApimodelsInventoryResp.create_from_dict(content), None
+        if code == 204:
+            return None, None
         if code == 400:
             return None, ApimodelsErrorResponse.create_from_dict(content)
         if code == 404:
             return None, ApimodelsErrorResponse.create_from_dict(content)
         if code == 500:
             return None, ApimodelsErrorResponse.create_from_dict(content)
 
@@ -234,38 +240,38 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: ApimodelsUpdateInventoryReq,
+        body: ApimodelsDeleteInventoryReq,
         inventory_id: str,
         namespace: str,
         **kwargs,
-    ) -> AdminUpdateInventory:
+    ) -> DeleteInventory:
         instance = cls()
         instance.body = body
         instance.inventory_id = inventory_id
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminUpdateInventory:
+    ) -> DeleteInventory:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ApimodelsUpdateInventoryReq.create_from_dict(
+            instance.body = ApimodelsDeleteInventoryReq.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ApimodelsUpdateInventoryReq()
+            instance.body = ApimodelsDeleteInventoryReq()
         if "inventoryId" in dict_ and dict_["inventoryId"] is not None:
             instance.inventory_id = str(dict_["inventoryId"])
         elif include_empty:
             instance.inventory_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/delete_inventory.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_update_my_items.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,80 +25,96 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ApimodelsDeleteInventoryReq
+from ...models import ApimodelsAdminUpdateItemReq
 from ...models import ApimodelsErrorResponse
+from ...models import ApimodelsUpdateItemResp
 
 
-class DeleteInventory(Operation):
-    """To delete inventory (deleteInventory)
+class AdminBulkUpdateMyItems(Operation):
+    """To bulk update items (AdminBulkUpdateMyItems)
 
-    Deleting an inventory.
-    If an inventory still has items, it cannot be deleted.
+    Bulk Updating user's own items.
+    Tags will be auto-created.
 
-    ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY [DELETE]
+    Permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [UPDATE]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY [DELETE]
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [UPDATE]
 
     Properties:
-        url: /inventory/v1/admin/namespaces/{namespace}/inventories/{inventoryId}
+        url: /inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/items
 
-        method: DELETE
+        method: PUT
 
-        tags: ["Admin Inventories"]
+        tags: ["Admin Items"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ApimodelsDeleteInventoryReq in body
+        body: (body) REQUIRED List[ApimodelsAdminUpdateItemReq] in body
 
         inventory_id: (inventoryId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
+        user_id: (userId) REQUIRED str in path
+
     Responses:
-        204: No Content - (No Content)
+        200: OK - List[ApimodelsUpdateItemResp] (OK)
 
         400: Bad Request - ApimodelsErrorResponse (Bad Request)
 
         404: Not Found - ApimodelsErrorResponse (Not Found)
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/inventory/v1/admin/namespaces/{namespace}/inventories/{inventoryId}"
-    _method: str = "DELETE"
+    _url: str = "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/items"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/items"
+    _base_path: str = ""
+    _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ApimodelsDeleteInventoryReq  # REQUIRED in [body]
+    service_name: Optional[str] = "inventory"
+
+    body: List[ApimodelsAdminUpdateItemReq]  # REQUIRED in [body]
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
+    user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -127,75 +143,92 @@
             "body": self.get_body_params(),
             "path": self.get_path_params(),
         }
 
     def get_body_params(self) -> Any:
         if not hasattr(self, "body") or self.body is None:
             return None
-        return self.body.to_dict()
+        return [i.to_dict() for i in self.body]
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "inventory_id"):
             result["inventoryId"] = self.inventory_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
+        if hasattr(self, "user_id"):
+            result["userId"] = self.user_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ApimodelsDeleteInventoryReq) -> DeleteInventory:
+    def with_body(
+        self, value: List[ApimodelsAdminUpdateItemReq]
+    ) -> AdminBulkUpdateMyItems:
         self.body = value
         return self
 
-    def with_inventory_id(self, value: str) -> DeleteInventory:
+    def with_inventory_id(self, value: str) -> AdminBulkUpdateMyItems:
         self.inventory_id = value
         return self
 
-    def with_namespace(self, value: str) -> DeleteInventory:
+    def with_namespace(self, value: str) -> AdminBulkUpdateMyItems:
         self.namespace = value
         return self
 
+    def with_user_id(self, value: str) -> AdminBulkUpdateMyItems:
+        self.user_id = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
-            result["body"] = self.body.to_dict(include_empty=include_empty)
+            result["body"] = [
+                i0.to_dict(include_empty=include_empty) for i0 in self.body
+            ]
         elif include_empty:
-            result["body"] = ApimodelsDeleteInventoryReq()
+            result["body"] = []
         if hasattr(self, "inventory_id") and self.inventory_id:
             result["inventoryId"] = str(self.inventory_id)
         elif include_empty:
             result["inventoryId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
+        if hasattr(self, "user_id") and self.user_id:
+            result["userId"] = str(self.user_id)
+        elif include_empty:
+            result["userId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, ApimodelsErrorResponse, HttpResponse]]:
+    ) -> Tuple[
+        Union[None, List[ApimodelsUpdateItemResp]],
+        Union[None, ApimodelsErrorResponse, HttpResponse],
+    ]:
         """Parse the given response.
 
-        204: No Content - (No Content)
+        200: OK - List[ApimodelsUpdateItemResp] (OK)
 
         400: Bad Request - ApimodelsErrorResponse (Bad Request)
 
         404: Not Found - ApimodelsErrorResponse (Not Found)
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
 
@@ -208,16 +241,16 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 204:
-            return None, None
+        if code == 200:
+            return [ApimodelsUpdateItemResp.create_from_dict(i) for i in content], None
         if code == 400:
             return None, ApimodelsErrorResponse.create_from_dict(content)
         if code == 404:
             return None, ApimodelsErrorResponse.create_from_dict(content)
         if code == 500:
             return None, ApimodelsErrorResponse.create_from_dict(content)
 
@@ -228,58 +261,69 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: ApimodelsDeleteInventoryReq,
+        body: List[ApimodelsAdminUpdateItemReq],
         inventory_id: str,
         namespace: str,
+        user_id: str,
         **kwargs,
-    ) -> DeleteInventory:
+    ) -> AdminBulkUpdateMyItems:
         instance = cls()
         instance.body = body
         instance.inventory_id = inventory_id
         instance.namespace = namespace
+        instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> DeleteInventory:
+    ) -> AdminBulkUpdateMyItems:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ApimodelsDeleteInventoryReq.create_from_dict(
-                dict_["body"], include_empty=include_empty
-            )
+            instance.body = [
+                ApimodelsAdminUpdateItemReq.create_from_dict(
+                    i0, include_empty=include_empty
+                )
+                for i0 in dict_["body"]
+            ]
         elif include_empty:
-            instance.body = ApimodelsDeleteInventoryReq()
+            instance.body = []
         if "inventoryId" in dict_ and dict_["inventoryId"] is not None:
             instance.inventory_id = str(dict_["inventoryId"])
         elif include_empty:
             instance.inventory_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
+        if "userId" in dict_ and dict_["userId"] is not None:
+            instance.user_id = str(dict_["userId"])
+        elif include_empty:
+            instance.user_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "body": "body",
             "inventoryId": "inventory_id",
             "namespace": "namespace",
+            "userId": "user_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "body": True,
             "inventoryId": True,
             "namespace": True,
+            "userId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_inventory__71b514 import AdminCreateInventoryConfiguration
 from .admin_delete_inventory__38371e import AdminDeleteInventoryConfiguration
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_create_inventory__71b514.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_create_inventory__71b514.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,32 +71,44 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/inventoryConfigurations"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/inventoryConfigurations"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     body: ApimodelsCreateInventoryConfigurationReq  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_delete_inventory__38371e.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_delete_inventory__38371e.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,32 +69,44 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/inventoryConfigurations/{inventoryConfigurationId}"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/inventoryConfigurations/{inventoryConfigurationId}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     inventory_configuration_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_get_inventory_con_709281.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_get_inventory_con_709281.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,32 +69,44 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/inventoryConfigurations/{inventoryConfigurationId}"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/inventoryConfigurations/{inventoryConfigurationId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     inventory_configuration_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_list_inventory_co_67d862.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_list_inventory_co_67d862.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,20 +87,24 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/inventoryConfigurations"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/inventoryConfigurations"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     namespace: str  # REQUIRED in [path]
     code: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     sort_by: Union[str, SortByEnum]  # OPTIONAL in [query]
 
     # endregion fields
@@ -108,14 +112,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_update_inventory__e10746.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_update_inventory__e10746.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,33 +75,45 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/inventoryConfigurations/{inventoryConfigurationId}"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/inventoryConfigurations/{inventoryConfigurationId}"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     body: ApimodelsInventoryConfigurationReq  # REQUIRED in [body]
     inventory_configuration_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_item_type import AdminCreateItemType
 from .admin_delete_item_type import AdminDeleteItemType
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_create_item_type.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_create_item_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,32 +72,44 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/itemtypes"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/itemtypes"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     body: ApimodelsCreateItemTypeReq  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_delete_item_type.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_delete_item_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,32 +67,44 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/itemtypes/{itemTypeName}"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/itemtypes/{itemTypeName}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     item_type_name: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_list_item_types.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/public_list_item_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,31 +39,26 @@
     CREATEDAT_ASC = "createdAt:asc"
     CREATEDAT_DESC = "createdAt:desc"
     NAME = "name"
     NAME_ASC = "name:asc"
     NAME_DESC = "name:desc"
 
 
-class AdminListItemTypes(Operation):
-    """To list itemtypes (AdminListItemTypes)
+class PublicListItemTypes(Operation):
+    """To list item types (PublicListItemTypes)
 
     This endpoint will list all item types in a namespace.
     The response body will be in the form of standard pagination.
 
-    Permission: ADMIN:NAMESPACE:{namespace}:INVENTORY:ITEMTYPE [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INVENTORY:ITEMTYPE [READ]
-
     Properties:
-        url: /inventory/v1/admin/namespaces/{namespace}/itemtypes
+        url: /inventory/v1/public/namespaces/{namespace}/itemtypes
 
         method: GET
 
-        tags: ["Admin Item Types"]
+        tags: ["Public Item Types"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -81,35 +76,47 @@
         400: Bad Request - ApimodelsErrorResponse (Bad Request)
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/inventory/v1/admin/namespaces/{namespace}/itemtypes"
+    _url: str = "/inventory/v1/public/namespaces/{namespace}/itemtypes"
+    _path: str = "/inventory/v1/public/namespaces/{namespace}/itemtypes"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     sort_by: Union[str, SortByEnum]  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -159,27 +166,27 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> AdminListItemTypes:
+    def with_namespace(self, value: str) -> PublicListItemTypes:
         self.namespace = value
         return self
 
-    def with_limit(self, value: int) -> AdminListItemTypes:
+    def with_limit(self, value: int) -> PublicListItemTypes:
         self.limit = value
         return self
 
-    def with_offset(self, value: int) -> AdminListItemTypes:
+    def with_offset(self, value: int) -> PublicListItemTypes:
         self.offset = value
         return self
 
-    def with_sort_by(self, value: Union[str, SortByEnum]) -> AdminListItemTypes:
+    def with_sort_by(self, value: Union[str, SortByEnum]) -> PublicListItemTypes:
         self.sort_by = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -254,15 +261,15 @@
     def create(
         cls,
         namespace: str,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         sort_by: Optional[Union[str, SortByEnum]] = None,
         **kwargs,
-    ) -> AdminListItemTypes:
+    ) -> PublicListItemTypes:
         instance = cls()
         instance.namespace = namespace
         if limit is not None:
             instance.limit = limit
         if offset is not None:
             instance.offset = offset
         if sort_by is not None:
@@ -270,15 +277,15 @@
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminListItemTypes:
+    ) -> PublicListItemTypes:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "limit" in dict_ and dict_["limit"] is not None:
             instance.limit = int(dict_["limit"])
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_bulk_remove_items import AdminBulkRemoveItems
 from .admin_bulk_update_my_items import AdminBulkUpdateMyItems
@@ -20,7 +20,8 @@
 from .admin_get_inventory_item import AdminGetInventoryItem
 from .admin_list_items import AdminListItems
 from .admin_list_items import (
     SortByEnum as AdminListItemsSortByEnum,
 )
 from .admin_save_item import AdminSaveItem
 from .admin_save_item_to_inventory import AdminSaveItemToInventory
+from .admin_sync_user_entitlements import AdminSyncUserEntitlements
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_remove_items.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_remove_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,34 +74,46 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/items"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/items"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     body: List[ApimodelsRemoveInventoryItemReq]  # REQUIRED in [body]
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_update_my_items.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_consume_user_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,84 +25,95 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ApimodelsAdminUpdateItemReq
+from ...models import ApimodelsConsumeItemReq
 from ...models import ApimodelsErrorResponse
-from ...models import ApimodelsUpdateItemResp
+from ...models import ApimodelsItemResp
 
 
-class AdminBulkUpdateMyItems(Operation):
-    """To bulk update items (AdminBulkUpdateMyItems)
+class AdminConsumeUserItem(Operation):
+    """To consume item (AdminConsumeUserItem)
 
-    Bulk Updating user's own items.
-    Tags will be auto-created.
+    Consume user's own item
 
     Permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [UPDATE]
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [UPDATE]
 
     Properties:
-        url: /inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/items
+        url: /inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/consume
 
-        method: PUT
+        method: POST
 
         tags: ["Admin Items"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED List[ApimodelsAdminUpdateItemReq] in body
+        body: (body) REQUIRED ApimodelsConsumeItemReq in body
 
         inventory_id: (inventoryId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        200: OK - List[ApimodelsUpdateItemResp] (OK)
+        200: OK - ApimodelsItemResp (OK)
 
         400: Bad Request - ApimodelsErrorResponse (Bad Request)
 
         404: Not Found - ApimodelsErrorResponse (Not Found)
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/items"
-    _method: str = "PUT"
+    _url: str = "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/consume"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/consume"
+    _base_path: str = ""
+    _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: List[ApimodelsAdminUpdateItemReq]  # REQUIRED in [body]
+    service_name: Optional[str] = "inventory"
+
+    body: ApimodelsConsumeItemReq  # REQUIRED in [body]
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -131,15 +142,15 @@
             "body": self.get_body_params(),
             "path": self.get_path_params(),
         }
 
     def get_body_params(self) -> Any:
         if not hasattr(self, "body") or self.body is None:
             return None
-        return [i.to_dict() for i in self.body]
+        return self.body.to_dict()
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "inventory_id"):
             result["inventoryId"] = self.inventory_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
@@ -151,44 +162,40 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(
-        self, value: List[ApimodelsAdminUpdateItemReq]
-    ) -> AdminBulkUpdateMyItems:
+    def with_body(self, value: ApimodelsConsumeItemReq) -> AdminConsumeUserItem:
         self.body = value
         return self
 
-    def with_inventory_id(self, value: str) -> AdminBulkUpdateMyItems:
+    def with_inventory_id(self, value: str) -> AdminConsumeUserItem:
         self.inventory_id = value
         return self
 
-    def with_namespace(self, value: str) -> AdminBulkUpdateMyItems:
+    def with_namespace(self, value: str) -> AdminConsumeUserItem:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> AdminBulkUpdateMyItems:
+    def with_user_id(self, value: str) -> AdminConsumeUserItem:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
-            result["body"] = [
-                i0.to_dict(include_empty=include_empty) for i0 in self.body
-            ]
+            result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = []
+            result["body"] = ApimodelsConsumeItemReq()
         if hasattr(self, "inventory_id") and self.inventory_id:
             result["inventoryId"] = str(self.inventory_id)
         elif include_empty:
             result["inventoryId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
@@ -203,20 +210,20 @@
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, List[ApimodelsUpdateItemResp]],
+        Union[None, ApimodelsItemResp],
         Union[None, ApimodelsErrorResponse, HttpResponse],
     ]:
         """Parse the given response.
 
-        200: OK - List[ApimodelsUpdateItemResp] (OK)
+        200: OK - ApimodelsItemResp (OK)
 
         400: Bad Request - ApimodelsErrorResponse (Bad Request)
 
         404: Not Found - ApimodelsErrorResponse (Not Found)
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
 
@@ -230,15 +237,15 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return [ApimodelsUpdateItemResp.create_from_dict(i) for i in content], None
+            return ApimodelsItemResp.create_from_dict(content), None
         if code == 400:
             return None, ApimodelsErrorResponse.create_from_dict(content)
         if code == 404:
             return None, ApimodelsErrorResponse.create_from_dict(content)
         if code == 500:
             return None, ApimodelsErrorResponse.create_from_dict(content)
 
@@ -249,43 +256,40 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: List[ApimodelsAdminUpdateItemReq],
+        body: ApimodelsConsumeItemReq,
         inventory_id: str,
         namespace: str,
         user_id: str,
         **kwargs,
-    ) -> AdminBulkUpdateMyItems:
+    ) -> AdminConsumeUserItem:
         instance = cls()
         instance.body = body
         instance.inventory_id = inventory_id
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminBulkUpdateMyItems:
+    ) -> AdminConsumeUserItem:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = [
-                ApimodelsAdminUpdateItemReq.create_from_dict(
-                    i0, include_empty=include_empty
-                )
-                for i0 in dict_["body"]
-            ]
+            instance.body = ApimodelsConsumeItemReq.create_from_dict(
+                dict_["body"], include_empty=include_empty
+            )
         elif include_empty:
-            instance.body = []
+            instance.body = ApimodelsConsumeItemReq()
         if "inventoryId" in dict_ and dict_["inventoryId"] is not None:
             instance.inventory_id = str(dict_["inventoryId"])
         elif include_empty:
             instance.inventory_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_consume_user_item.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_purchasable.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,83 +25,95 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ApimodelsConsumeItemReq
 from ...models import ApimodelsErrorResponse
-from ...models import ApimodelsItemResp
+from ...models import ApimodelsPurchaseValidationReq
 
 
-class AdminConsumeUserItem(Operation):
-    """To consume item (AdminConsumeUserItem)
+class AdminPurchasable(Operation):
+    """To validate user inventory capacity when purchase ecommerce item (AdminPurchasable)
 
-    Consume user's own item
+    Validate purchase ecommerce item.
 
-    Permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [UPDATE]
+    Permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY [UPDATE]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [UPDATE]
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY [UPDATE]
 
     Properties:
-        url: /inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/consume
+        url: /inventory/v1/admin/namespaces/{namespace}/users/{userId}/purchaseable
 
         method: POST
 
-        tags: ["Admin Items"]
+        tags: ["Admin Inventories"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ApimodelsConsumeItemReq in body
-
-        inventory_id: (inventoryId) REQUIRED str in path
+        body: (body) REQUIRED ApimodelsPurchaseValidationReq in body
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        200: OK - ApimodelsItemResp (OK)
+        204: No Content - (No Content)
 
         400: Bad Request - ApimodelsErrorResponse (Bad Request)
 
         404: Not Found - ApimodelsErrorResponse (Not Found)
 
+        409: Conflict - ApimodelsErrorResponse (Conflict)
+
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/consume"
+    _url: str = "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/purchaseable"
+    _path: str = (
+        "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/purchaseable"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ApimodelsConsumeItemReq  # REQUIRED in [body]
-    inventory_id: str  # REQUIRED in [path]
+    service_name: Optional[str] = "inventory"
+
+    body: ApimodelsPurchaseValidationReq  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -134,60 +146,50 @@
     def get_body_params(self) -> Any:
         if not hasattr(self, "body") or self.body is None:
             return None
         return self.body.to_dict()
 
     def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "inventory_id"):
-            result["inventoryId"] = self.inventory_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         if hasattr(self, "user_id"):
             result["userId"] = self.user_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ApimodelsConsumeItemReq) -> AdminConsumeUserItem:
+    def with_body(self, value: ApimodelsPurchaseValidationReq) -> AdminPurchasable:
         self.body = value
         return self
 
-    def with_inventory_id(self, value: str) -> AdminConsumeUserItem:
-        self.inventory_id = value
-        return self
-
-    def with_namespace(self, value: str) -> AdminConsumeUserItem:
+    def with_namespace(self, value: str) -> AdminPurchasable:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> AdminConsumeUserItem:
+    def with_user_id(self, value: str) -> AdminPurchasable:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ApimodelsConsumeItemReq()
-        if hasattr(self, "inventory_id") and self.inventory_id:
-            result["inventoryId"] = str(self.inventory_id)
-        elif include_empty:
-            result["inventoryId"] = ""
+            result["body"] = ApimodelsPurchaseValidationReq()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         if hasattr(self, "user_id") and self.user_id:
             result["userId"] = str(self.user_id)
         elif include_empty:
@@ -197,26 +199,25 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, ApimodelsItemResp],
-        Union[None, ApimodelsErrorResponse, HttpResponse],
-    ]:
+    ) -> Tuple[None, Union[None, ApimodelsErrorResponse, HttpResponse]]:
         """Parse the given response.
 
-        200: OK - ApimodelsItemResp (OK)
+        204: No Content - (No Content)
 
         400: Bad Request - ApimodelsErrorResponse (Bad Request)
 
         404: Not Found - ApimodelsErrorResponse (Not Found)
 
+        409: Conflict - ApimodelsErrorResponse (Conflict)
+
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
@@ -224,86 +225,80 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return ApimodelsItemResp.create_from_dict(content), None
+        if code == 204:
+            return None, None
         if code == 400:
             return None, ApimodelsErrorResponse.create_from_dict(content)
         if code == 404:
             return None, ApimodelsErrorResponse.create_from_dict(content)
+        if code == 409:
+            return None, ApimodelsErrorResponse.create_from_dict(content)
         if code == 500:
             return None, ApimodelsErrorResponse.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: ApimodelsConsumeItemReq,
-        inventory_id: str,
+        body: ApimodelsPurchaseValidationReq,
         namespace: str,
         user_id: str,
         **kwargs,
-    ) -> AdminConsumeUserItem:
+    ) -> AdminPurchasable:
         instance = cls()
         instance.body = body
-        instance.inventory_id = inventory_id
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminConsumeUserItem:
+    ) -> AdminPurchasable:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ApimodelsConsumeItemReq.create_from_dict(
+            instance.body = ApimodelsPurchaseValidationReq.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ApimodelsConsumeItemReq()
-        if "inventoryId" in dict_ and dict_["inventoryId"] is not None:
-            instance.inventory_id = str(dict_["inventoryId"])
-        elif include_empty:
-            instance.inventory_id = ""
+            instance.body = ApimodelsPurchaseValidationReq()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "userId" in dict_ and dict_["userId"] is not None:
             instance.user_id = str(dict_["userId"])
         elif include_empty:
             instance.user_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "body": "body",
-            "inventoryId": "inventory_id",
             "namespace": "namespace",
             "userId": "user_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "body": True,
-            "inventoryId": True,
             "namespace": True,
             "userId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_get_inventory_item.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_get_inventory_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,34 +73,46 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/inventories/{inventoryId}/slots/{slotId}/sourceItems/{sourceItemId}"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/inventories/{inventoryId}/slots/{slotId}/sourceItems/{sourceItemId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     slot_id: str  # REQUIRED in [path]
     source_item_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_list_items.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_list_items.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,20 +95,26 @@
     """
 
     # region fields
 
     _url: str = (
         "/inventory/v1/admin/namespaces/{namespace}/inventories/{inventoryId}/items"
     )
+    _path: str = (
+        "/inventory/v1/admin/namespaces/{namespace}/inventories/{inventoryId}/items"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     qty_gte: int  # OPTIONAL in [query]
     sort_by: Union[str, SortByEnum]  # OPTIONAL in [query]
     source_item_id: str  # OPTIONAL in [query]
@@ -119,14 +125,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 
     If the item already exists, its qty will be increased,
     so no new item with same sourceItemId will be created
 
     Tags will be auto-created.
     ItemType will be auto-created.
 
+    For Ecommerce item, this fields will be override by ecommerce configuration
+    (slotUsed, serverCustomAttributes, customAttributes, type)
+
     Permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [CREATE]
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [CREATE]
 
     Properties:
         url: /inventory/v1/admin/namespaces/{namespace}/users/{userId}/items
@@ -78,33 +81,45 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/items"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/items"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     body: ApimodelsSaveItemReq  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item_to_inventory.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item_to_inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,34 +79,46 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/items"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/users/{userId}/inventories/{inventoryId}/items"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     body: ApimodelsSaveItemToInventoryReq  # REQUIRED in [body]
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_tag import AdminCreateTag
 from .admin_delete_tag import AdminDeleteTag
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_create_tag.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_create_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,32 +72,44 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/tags"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/tags"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     body: ApimodelsCreateTagReq  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_delete_tag.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_delete_tag.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,32 +67,44 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/tags/{tagName}"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/tags/{tagName}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     namespace: str  # REQUIRED in [path]
     tag_name: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_list_tags.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_list_tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,20 +84,24 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/admin/namespaces/{namespace}/tags"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/tags"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     owner: str  # OPTIONAL in [query]
     sort_by: Union[str, SortByEnum]  # OPTIONAL in [query]
 
     # endregion fields
@@ -105,14 +109,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_list_inventories import PublicListInventories
 from .public_list_inventories import (
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/public_list_inventories.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/public_list_inventories.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,20 +79,24 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories"
+    _path: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     namespace: str  # REQUIRED in [path]
     inventory_configuration_code: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     sort_by: Union[str, SortByEnum]  # OPTIONAL in [query]
 
     # endregion fields
@@ -100,14 +104,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_list_inventory_c_d1722b import PublicListInventoryConfigurations
 from .public_list_inventory_c_d1722b import (
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/public_list_inventory_c_d1722b.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/public_list_inventory_c_d1722b.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,20 +82,24 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/public/namespaces/{namespace}/inventoryConfigurations"
+    _path: str = "/inventory/v1/public/namespaces/{namespace}/inventoryConfigurations"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     namespace: str  # REQUIRED in [path]
     code: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     sort_by: Union[str, SortByEnum]  # OPTIONAL in [query]
 
     # endregion fields
@@ -103,14 +107,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_list_item_types import PublicListItemTypes
 from .public_list_item_types import (
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/public_list_item_types.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_list_item_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,26 +39,31 @@
     CREATEDAT_ASC = "createdAt:asc"
     CREATEDAT_DESC = "createdAt:desc"
     NAME = "name"
     NAME_ASC = "name:asc"
     NAME_DESC = "name:desc"
 
 
-class PublicListItemTypes(Operation):
-    """To list item types (PublicListItemTypes)
+class AdminListItemTypes(Operation):
+    """To list itemtypes (AdminListItemTypes)
 
     This endpoint will list all item types in a namespace.
     The response body will be in the form of standard pagination.
 
+    Permission: ADMIN:NAMESPACE:{namespace}:INVENTORY:ITEMTYPE [READ]
+
+    Required Permission(s):
+        - ADMIN:NAMESPACE:{namespace}:INVENTORY:ITEMTYPE [READ]
+
     Properties:
-        url: /inventory/v1/public/namespaces/{namespace}/itemtypes
+        url: /inventory/v1/admin/namespaces/{namespace}/itemtypes
 
         method: GET
 
-        tags: ["Public Item Types"]
+        tags: ["Admin Item Types"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -76,35 +81,47 @@
         400: Bad Request - ApimodelsErrorResponse (Bad Request)
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/inventory/v1/public/namespaces/{namespace}/itemtypes"
+    _url: str = "/inventory/v1/admin/namespaces/{namespace}/itemtypes"
+    _path: str = "/inventory/v1/admin/namespaces/{namespace}/itemtypes"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     sort_by: Union[str, SortByEnum]  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -154,27 +171,27 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> PublicListItemTypes:
+    def with_namespace(self, value: str) -> AdminListItemTypes:
         self.namespace = value
         return self
 
-    def with_limit(self, value: int) -> PublicListItemTypes:
+    def with_limit(self, value: int) -> AdminListItemTypes:
         self.limit = value
         return self
 
-    def with_offset(self, value: int) -> PublicListItemTypes:
+    def with_offset(self, value: int) -> AdminListItemTypes:
         self.offset = value
         return self
 
-    def with_sort_by(self, value: Union[str, SortByEnum]) -> PublicListItemTypes:
+    def with_sort_by(self, value: Union[str, SortByEnum]) -> AdminListItemTypes:
         self.sort_by = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -249,15 +266,15 @@
     def create(
         cls,
         namespace: str,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         sort_by: Optional[Union[str, SortByEnum]] = None,
         **kwargs,
-    ) -> PublicListItemTypes:
+    ) -> AdminListItemTypes:
         instance = cls()
         instance.namespace = namespace
         if limit is not None:
             instance.limit = limit
         if offset is not None:
             instance.offset = offset
         if sort_by is not None:
@@ -265,15 +282,15 @@
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublicListItemTypes:
+    ) -> AdminListItemTypes:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "limit" in dict_ and dict_["limit"] is not None:
             instance.limit = int(dict_["limit"])
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_bulk_remove_my_items import PublicBulkRemoveMyItems
 from .public_bulk_update_my_items import PublicBulkUpdateMyItems
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_remove_my_items.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_remove_my_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,33 +67,45 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories/{inventoryId}/items"
+    _path: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories/{inventoryId}/items"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     body: List[ApimodelsRemoveInventoryItemReq]  # REQUIRED in [body]
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_update_my_items.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_update_my_items.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,33 +67,45 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories/{inventoryId}/items"
+    _path: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories/{inventoryId}/items"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     body: List[ApimodelsUpdateItemReq]  # REQUIRED in [body]
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_consume_my_item.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_consume_my_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,33 +67,45 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories/{inventoryId}/consume"
+    _path: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories/{inventoryId}/consume"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     body: ApimodelsConsumeItemReq  # REQUIRED in [body]
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_get_item.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_get_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,34 +68,46 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories/{inventoryId}/slots/{slotId}/sourceItems/{sourceItemId}"
+    _path: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories/{inventoryId}/slots/{slotId}/sourceItems/{sourceItemId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     slot_id: str  # REQUIRED in [path]
     source_item_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_list_items.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_list_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,20 +88,24 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories/{inventoryId}/items"
+    _path: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories/{inventoryId}/items"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     qty_gte: int  # OPTIONAL in [query]
     sort_by: Union[str, SortByEnum]  # OPTIONAL in [query]
     source_item_id: str  # OPTIONAL in [query]
@@ -112,14 +116,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_move_my_items.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_move_my_items.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,33 +65,45 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories/{inventoryId}/items/movement"
+    _path: str = "/inventory/v1/public/namespaces/{namespace}/users/me/inventories/{inventoryId}/items/movement"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     body: ApimodelsMoveItemsReq  # REQUIRED in [body]
     inventory_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_tags/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_tags/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_list_tags import PublicListTags
 from .public_list_tags import (
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/operations/public_tags/public_list_tags.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_tags/public_list_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,34 +77,46 @@
 
         500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/inventory/v1/public/namespaces/{namespace}/tags"
+    _path: str = "/inventory/v1/public/namespaces/{namespace}/tags"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "inventory"
+
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     sort_by: Union[str, SortByEnum]  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/__init__.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,29 +4,50 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._admin_chaining_operations import admin_create_chaining_operations
 from ._admin_chaining_operations import admin_create_chaining_operations_async
 
+from ._admin_integration_configurations import admin_create_integration_configuration
+from ._admin_integration_configurations import (
+    admin_create_integration_configuration_async,
+)
+from ._admin_integration_configurations import admin_list_integration_configurations
+from ._admin_integration_configurations import (
+    admin_list_integration_configurations_async,
+)
+from ._admin_integration_configurations import admin_update_integration_configuration
+from ._admin_integration_configurations import (
+    admin_update_integration_configuration_async,
+)
+from ._admin_integration_configurations import (
+    admin_update_status_integration_configuration,
+)
+from ._admin_integration_configurations import (
+    admin_update_status_integration_configuration_async,
+)
+
 from ._admin_inventories import admin_create_inventory
 from ._admin_inventories import admin_create_inventory_async
 from ._admin_inventories import admin_get_inventory
 from ._admin_inventories import admin_get_inventory_async
 from ._admin_inventories import admin_list_inventories
 from ._admin_inventories import admin_list_inventories_async
+from ._admin_inventories import admin_purchasable
+from ._admin_inventories import admin_purchasable_async
 from ._admin_inventories import admin_update_inventory
 from ._admin_inventories import admin_update_inventory_async
 from ._admin_inventories import delete_inventory
 from ._admin_inventories import delete_inventory_async
 
 from ._admin_inventory_configurations import admin_create_inventory_configuration
 from ._admin_inventory_configurations import admin_create_inventory_configuration_async
@@ -56,14 +77,16 @@
 from ._admin_items import admin_get_inventory_item_async
 from ._admin_items import admin_list_items
 from ._admin_items import admin_list_items_async
 from ._admin_items import admin_save_item
 from ._admin_items import admin_save_item_async
 from ._admin_items import admin_save_item_to_inventory
 from ._admin_items import admin_save_item_to_inventory_async
+from ._admin_items import admin_sync_user_entitlements
+from ._admin_items import admin_sync_user_entitlements_async
 
 from ._admin_tags import admin_create_tag
 from ._admin_tags import admin_create_tag_async
 from ._admin_tags import admin_delete_tag
 from ._admin_tags import admin_delete_tag_async
 from ._admin_tags import admin_list_tags
 from ._admin_tags import admin_list_tags_async
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_chaining_operations.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_chaining_operations.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventories.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventories.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,22 +30,24 @@
 from accelbyte_py_sdk.core import same_doc_as
 
 from ..models import ApimodelsCreateInventoryReq
 from ..models import ApimodelsDeleteInventoryReq
 from ..models import ApimodelsErrorResponse
 from ..models import ApimodelsInventoryResp
 from ..models import ApimodelsListInventoryResp
+from ..models import ApimodelsPurchaseValidationReq
 from ..models import ApimodelsUpdateInventoryReq
 
 from ..operations.admin_inventories import AdminCreateInventory
 from ..operations.admin_inventories import AdminGetInventory
 from ..operations.admin_inventories import AdminListInventories
 from ..operations.admin_inventories import (
     AdminListInventoriesSortByEnum,
 )
+from ..operations.admin_inventories import AdminPurchasable
 from ..operations.admin_inventories import AdminUpdateInventory
 from ..operations.admin_inventories import DeleteInventory
 
 
 @same_doc_as(AdminCreateInventory)
 def admin_create_inventory(
     body: ApimodelsCreateInventoryReq,
@@ -397,14 +399,134 @@
         user_id=user_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
+
+@same_doc_as(AdminPurchasable)
+def admin_purchasable(
+    body: ApimodelsPurchaseValidationReq,
+    user_id: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """To validate user inventory capacity when purchase ecommerce item (AdminPurchasable)
+
+    Validate purchase ecommerce item.
+
+    Permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY [UPDATE]
+
+    Required Permission(s):
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY [UPDATE]
+
+    Properties:
+        url: /inventory/v1/admin/namespaces/{namespace}/users/{userId}/purchaseable
+
+        method: POST
+
+        tags: ["Admin Inventories"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        body: (body) REQUIRED ApimodelsPurchaseValidationReq in body
+
+        namespace: (namespace) REQUIRED str in path
+
+        user_id: (userId) REQUIRED str in path
+
+    Responses:
+        204: No Content - (No Content)
+
+        400: Bad Request - ApimodelsErrorResponse (Bad Request)
+
+        404: Not Found - ApimodelsErrorResponse (Not Found)
+
+        409: Conflict - ApimodelsErrorResponse (Conflict)
+
+        500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminPurchasable.create(
+        body=body,
+        user_id=user_id,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(AdminPurchasable)
+async def admin_purchasable_async(
+    body: ApimodelsPurchaseValidationReq,
+    user_id: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """To validate user inventory capacity when purchase ecommerce item (AdminPurchasable)
+
+    Validate purchase ecommerce item.
+
+    Permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY [UPDATE]
+
+    Required Permission(s):
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY [UPDATE]
+
+    Properties:
+        url: /inventory/v1/admin/namespaces/{namespace}/users/{userId}/purchaseable
+
+        method: POST
+
+        tags: ["Admin Inventories"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        body: (body) REQUIRED ApimodelsPurchaseValidationReq in body
+
+        namespace: (namespace) REQUIRED str in path
+
+        user_id: (userId) REQUIRED str in path
+
+    Responses:
+        204: No Content - (No Content)
+
+        400: Bad Request - ApimodelsErrorResponse (Bad Request)
+
+        404: Not Found - ApimodelsErrorResponse (Not Found)
+
+        409: Conflict - ApimodelsErrorResponse (Conflict)
+
+        500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminPurchasable.create(
+        body=body,
+        user_id=user_id,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
 
 @same_doc_as(AdminUpdateInventory)
 def admin_update_inventory(
     body: ApimodelsUpdateInventoryReq,
     inventory_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventory_configurations.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventory_configurations.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_item_types.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_item_types.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_items.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_items.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,14 +45,17 @@
 from ..operations.admin_items import AdminGetInventoryItem
 from ..operations.admin_items import AdminListItems
 from ..operations.admin_items import (
     AdminListItemsSortByEnum,
 )
 from ..operations.admin_items import AdminSaveItem
 from ..operations.admin_items import AdminSaveItemToInventory
+from ..operations.admin_items import AdminSyncUserEntitlements
+from ..models import ApimodelsSaveItemReqSourceEnum
+from ..models import ApimodelsSaveItemToInventoryReqSourceEnum
 
 
 @same_doc_as(AdminBulkRemoveItems)
 def admin_bulk_remove_items(
     body: List[ApimodelsRemoveInventoryItemReq],
     inventory_id: str,
     user_id: str,
@@ -719,14 +722,17 @@
 
     If the item already exists, its qty will be increased,
     so no new item with same sourceItemId will be created
 
     Tags will be auto-created.
     ItemType will be auto-created.
 
+    For Ecommerce item, this fields will be override by ecommerce configuration
+    (slotUsed, serverCustomAttributes, customAttributes, type)
+
     Permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [CREATE]
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [CREATE]
 
     Properties:
         url: /inventory/v1/admin/namespaces/{namespace}/users/{userId}/items
@@ -782,14 +788,17 @@
 
     If the item already exists, its qty will be increased,
     so no new item with same sourceItemId will be created
 
     Tags will be auto-created.
     ItemType will be auto-created.
 
+    For Ecommerce item, this fields will be override by ecommerce configuration
+    (slotUsed, serverCustomAttributes, customAttributes, type)
+
     Permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [CREATE]
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [CREATE]
 
     Properties:
         url: /inventory/v1/admin/namespaces/{namespace}/users/{userId}/items
@@ -959,7 +968,119 @@
         inventory_id=inventory_id,
         user_id=user_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
+
+
+@same_doc_as(AdminSyncUserEntitlements)
+def admin_sync_user_entitlements(
+    user_id: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """To sync user's entitlements to e-commerce (AdminSyncUserEntitlements)
+
+    Permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [UPDATE]
+
+    Required Permission(s):
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [UPDATE]
+
+    Properties:
+        url: /inventory/v1/admin/namespaces/{namespace}/users/{userId}/items/entitlements/sync
+
+        method: PUT
+
+        tags: ["Admin Items"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+        user_id: (userId) REQUIRED str in path
+
+    Responses:
+        204: No Content - (No Content)
+
+        400: Bad Request - ApimodelsErrorResponse (Bad Request)
+
+        401: Unauthorized - ApimodelsErrorResponse (Unauthorized)
+
+        403: Forbidden - ApimodelsErrorResponse (Forbidden)
+
+        404: Not Found - ApimodelsErrorResponse (Not Found)
+
+        500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminSyncUserEntitlements.create(
+        user_id=user_id,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(AdminSyncUserEntitlements)
+async def admin_sync_user_entitlements_async(
+    user_id: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """To sync user's entitlements to e-commerce (AdminSyncUserEntitlements)
+
+    Permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [UPDATE]
+
+    Required Permission(s):
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:INVENTORY:ITEM [UPDATE]
+
+    Properties:
+        url: /inventory/v1/admin/namespaces/{namespace}/users/{userId}/items/entitlements/sync
+
+        method: PUT
+
+        tags: ["Admin Items"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+        user_id: (userId) REQUIRED str in path
+
+    Responses:
+        204: No Content - (No Content)
+
+        400: Bad Request - ApimodelsErrorResponse (Bad Request)
+
+        401: Unauthorized - ApimodelsErrorResponse (Unauthorized)
+
+        403: Forbidden - ApimodelsErrorResponse (Forbidden)
+
+        404: Not Found - ApimodelsErrorResponse (Not Found)
+
+        500: Internal Server Error - ApimodelsErrorResponse (Internal Server Error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminSyncUserEntitlements.create(
+        user_id=user_id,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_tags.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_tags.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventories.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventories.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventory_configurations.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventory_configurations.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_public_item_types.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_item_types.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_public_items.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk/api/inventory/wrappers/_public_tags.py` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_tags.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk_service_inventory.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-inventory
-Version: 0.4.0
+Version: 0.5.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Inventory Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Inventory Service
-* Version: 0.1.0
+* Version: 0.1.3
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-inventory-0.4.0/accelbyte_py_sdk_service_inventory.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,53 +3,67 @@
 accelbyte_py_sdk/api/inventory/__init__.py
 accelbyte_py_sdk/api/inventory/models/__init__.py
 accelbyte_py_sdk/api/inventory/models/apimodels_admin_update_item_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_resp.py
 accelbyte_py_sdk/api/inventory/models/apimodels_consume_item.py
 accelbyte_py_sdk/api/inventory/models/apimodels_consume_item_req.py
+accelbyte_py_sdk/api/inventory/models/apimodels_create_integration_configuration_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_configuration_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_create_item.py
 accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_resp.py
 accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_resp.py
 accelbyte_py_sdk/api/inventory/models/apimodels_delete_inventory_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_error_response.py
+accelbyte_py_sdk/api/inventory/models/apimodels_integration_configuration_resp.py
+accelbyte_py_sdk/api/inventory/models/apimodels_inventory_config.py
 accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_resp.py
 accelbyte_py_sdk/api/inventory/models/apimodels_inventory_resp.py
 accelbyte_py_sdk/api/inventory/models/apimodels_item_resp.py
+accelbyte_py_sdk/api/inventory/models/apimodels_list_integration_configurations_resp.py
 accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_configurations_resp.py
 accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_resp.py
 accelbyte_py_sdk/api/inventory/models/apimodels_list_item_resp.py
 accelbyte_py_sdk/api/inventory/models/apimodels_list_item_types_resp.py
 accelbyte_py_sdk/api/inventory/models/apimodels_list_tags_resp.py
 accelbyte_py_sdk/api/inventory/models/apimodels_move_items_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_move_items_resp.py
 accelbyte_py_sdk/api/inventory/models/apimodels_operation.py
 accelbyte_py_sdk/api/inventory/models/apimodels_paging.py
+accelbyte_py_sdk/api/inventory/models/apimodels_purchase_validation_item_req.py
+accelbyte_py_sdk/api/inventory/models/apimodels_purchase_validation_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_remove_inventory_item_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_remove_item.py
 accelbyte_py_sdk/api/inventory/models/apimodels_save_item_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_save_item_to_inventory_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_trade_item.py
 accelbyte_py_sdk/api/inventory/models/apimodels_trade_item_resp.py
+accelbyte_py_sdk/api/inventory/models/apimodels_update_integration_configuration_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_update_inventory_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_update_item.py
 accelbyte_py_sdk/api/inventory/models/apimodels_update_item_req.py
 accelbyte_py_sdk/api/inventory/models/apimodels_update_item_resp.py
+accelbyte_py_sdk/api/inventory/models/apimodels_update_status_integration_configuration_req.py
 accelbyte_py_sdk/api/inventory/operations/__init__.py
 accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/__init__.py
 accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/admin_create_chaining_o_8801c9.py
+accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/__init__.py
+accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_create_integratio_c6b1bd.py
+accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_list_integration__420e8d.py
+accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_update_integratio_fe692f.py
+accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_update_status_int_703321.py
 accelbyte_py_sdk/api/inventory/operations/admin_inventories/__init__.py
 accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_create_inventory.py
 accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_get_inventory.py
 accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_list_inventories.py
+accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_purchasable.py
 accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_update_inventory.py
 accelbyte_py_sdk/api/inventory/operations/admin_inventories/delete_inventory.py
 accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/__init__.py
 accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_create_inventory__71b514.py
 accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_delete_inventory__38371e.py
 accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_get_inventory_con_709281.py
 accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_list_inventory_co_67d862.py
@@ -62,14 +76,15 @@
 accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_remove_items.py
 accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_update_my_items.py
 accelbyte_py_sdk/api/inventory/operations/admin_items/admin_consume_user_item.py
 accelbyte_py_sdk/api/inventory/operations/admin_items/admin_get_inventory_item.py
 accelbyte_py_sdk/api/inventory/operations/admin_items/admin_list_items.py
 accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item.py
 accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item_to_inventory.py
+accelbyte_py_sdk/api/inventory/operations/admin_items/admin_sync_user_entitlements.py
 accelbyte_py_sdk/api/inventory/operations/admin_tags/__init__.py
 accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_create_tag.py
 accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_delete_tag.py
 accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_list_tags.py
 accelbyte_py_sdk/api/inventory/operations/public_inventories/__init__.py
 accelbyte_py_sdk/api/inventory/operations/public_inventories/public_list_inventories.py
 accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/__init__.py
@@ -83,14 +98,15 @@
 accelbyte_py_sdk/api/inventory/operations/public_items/public_get_item.py
 accelbyte_py_sdk/api/inventory/operations/public_items/public_list_items.py
 accelbyte_py_sdk/api/inventory/operations/public_items/public_move_my_items.py
 accelbyte_py_sdk/api/inventory/operations/public_tags/__init__.py
 accelbyte_py_sdk/api/inventory/operations/public_tags/public_list_tags.py
 accelbyte_py_sdk/api/inventory/wrappers/__init__.py
 accelbyte_py_sdk/api/inventory/wrappers/_admin_chaining_operations.py
+accelbyte_py_sdk/api/inventory/wrappers/_admin_integration_configurations.py
 accelbyte_py_sdk/api/inventory/wrappers/_admin_inventories.py
 accelbyte_py_sdk/api/inventory/wrappers/_admin_inventory_configurations.py
 accelbyte_py_sdk/api/inventory/wrappers/_admin_item_types.py
 accelbyte_py_sdk/api/inventory/wrappers/_admin_items.py
 accelbyte_py_sdk/api/inventory/wrappers/_admin_tags.py
 accelbyte_py_sdk/api/inventory/wrappers/_public_inventories.py
 accelbyte_py_sdk/api/inventory/wrappers/_public_inventory_configurations.py
```

