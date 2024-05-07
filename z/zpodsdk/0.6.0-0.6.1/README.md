# Comparing `tmp/zpodsdk-0.6.0.tar.gz` & `tmp/zpodsdk-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpodsdk-0.6.0.tar", max compression
+gzip compressed data, was "zpodsdk-0.6.1.tar", max compression
```

## Comparing `zpodsdk-0.6.0.tar` & `zpodsdk-0.6.1.tar`

### file list

```diff
@@ -1,147 +1,147 @@
--rw-r--r--   0        0        0     3656 2024-03-15 19:13:51.369008 zpodsdk-0.6.0/README.md
--rw-r--r--   0        0        0      497 2024-04-30 17:04:45.121879 zpodsdk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      174 2024-04-30 17:04:45.121879 zpodsdk-0.6.0/src/zpodsdk/__init__.py
--rw-r--r--   0        0        0       45 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 19:02:54.428741 zpodsdk-0.6.0/src/zpodsdk/api/components/__init__.py
--rw-r--r--   0        0        0     4427 2024-03-27 19:02:54.792771 zpodsdk-0.6.0/src/zpodsdk/api/components/components_disable.py
--rw-r--r--   0        0        0     4421 2024-03-27 19:02:54.792771 zpodsdk-0.6.0/src/zpodsdk/api/components/components_enable.py
--rw-r--r--   0        0        0     4394 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/components/components_get.py
--rw-r--r--   0        0        0     4277 2024-03-27 19:02:54.792771 zpodsdk-0.6.0/src/zpodsdk/api/components/components_get_all.py
--rw-r--r--   0        0        0        0 2024-03-27 19:02:54.436742 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/__init__.py
--rw-r--r--   0        0        0     4784 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_create.py
--rw-r--r--   0        0        0     4194 2024-03-27 19:02:54.784771 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_delete.py
--rw-r--r--   0        0        0     4944 2024-03-27 19:02:54.784771 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_enet_create.py
--rw-r--r--   0        0        0     4544 2024-03-27 19:02:54.780771 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_enet_delete.py
--rw-r--r--   0        0        0     4729 2024-03-27 19:02:54.780771 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_enet_get.py
--rw-r--r--   0        0        0     4716 2024-03-27 19:02:54.780771 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_enet_get_all.py
--rw-r--r--   0        0        0     4379 2024-03-27 19:02:54.780771 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_get.py
--rw-r--r--   0        0        0     4262 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_get_all.py
--rw-r--r--   0        0        0     4910 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_permissions_get_all.py
--rw-r--r--   0        0        0     6168 2024-03-27 19:02:54.780771 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_permissions_groups_add.py
--rw-r--r--   0        0        0     5789 2024-03-27 19:02:54.780771 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_permissions_groups_remove.py
--rw-r--r--   0        0        0     6151 2024-03-27 19:02:54.780771 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_permissions_users_add.py
--rw-r--r--   0        0        0     5772 2024-03-27 19:02:54.780771 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_permissions_users_remove.py
--rw-r--r--   0        0        0     5088 2024-03-27 19:02:54.784771 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_update.py
--rw-r--r--   0        0        0     4189 2024-03-27 19:02:54.784771 zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_verify.py
--rw-r--r--   0        0        0        0 2024-03-27 19:02:54.456744 zpodsdk-0.6.0/src/zpodsdk/api/libraries/__init__.py
--rw-r--r--   0        0        0     4707 2024-03-27 19:02:54.784771 zpodsdk-0.6.0/src/zpodsdk/api/libraries/libraries_create.py
--rw-r--r--   0        0        0     4194 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/libraries/libraries_delete.py
--rw-r--r--   0        0        0     4313 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/libraries/libraries_get.py
--rw-r--r--   0        0        0     4196 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/libraries/libraries_get_all.py
--rw-r--r--   0        0        0     4338 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/libraries/libraries_resync.py
--rw-r--r--   0        0        0     5011 2024-03-27 19:02:54.784771 zpodsdk-0.6.0/src/zpodsdk/api/libraries/libraries_update.py
--rw-r--r--   0        0        0        0 2024-03-27 19:02:54.460744 zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/__init__.py
--rw-r--r--   0        0        0     4916 2024-03-27 19:02:54.796772 zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_create.py
--rw-r--r--   0        0        0     4209 2024-03-27 19:02:54.796772 zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_delete.py
--rw-r--r--   0        0        0     4433 2024-03-27 19:02:54.808773 zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_get.py
--rw-r--r--   0        0        0     4354 2024-03-27 19:02:54.792771 zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_get_all.py
--rw-r--r--   0        0        0     4973 2024-03-27 19:02:54.820774 zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_update.py
--rw-r--r--   0        0        0     5460 2024-03-27 19:02:54.796772 zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_users_add.py
--rw-r--r--   0        0        0     4689 2024-03-27 19:02:54.808773 zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_users_delete.py
--rw-r--r--   0        0        0     4696 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_users_get_all.py
--rw-r--r--   0        0        0        0 2024-03-27 19:02:54.472745 zpodsdk-0.6.0/src/zpodsdk/api/profiles/__init__.py
--rw-r--r--   0        0        0     5377 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/api/profiles/profiles_create.py
--rw-r--r--   0        0        0     4192 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/api/profiles/profiles_delete.py
--rw-r--r--   0        0        0     4311 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/api/profiles/profiles_get.py
--rw-r--r--   0        0        0     4194 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/api/profiles/profiles_get_all.py
--rw-r--r--   0        0        0     5009 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/api/profiles/profiles_update.py
--rw-r--r--   0        0        0        0 2024-03-27 19:02:54.388738 zpodsdk-0.6.0/src/zpodsdk/api/root/__init__.py
--rw-r--r--   0        0        0     3728 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/api/root/root_root.py
--rw-r--r--   0        0        0        0 2024-03-27 19:02:54.480746 zpodsdk-0.6.0/src/zpodsdk/api/settings/__init__.py
--rw-r--r--   0        0        0     4705 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/settings/settings_create.py
--rw-r--r--   0        0        0     4192 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/settings/settings_delete.py
--rw-r--r--   0        0        0     4311 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/settings/settings_get.py
--rw-r--r--   0        0        0     4194 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/settings/settings_get_all.py
--rw-r--r--   0        0        0     5009 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/settings/settings_update.py
--rw-r--r--   0        0        0        0 2024-03-27 19:02:54.488746 zpodsdk-0.6.0/src/zpodsdk/api/users/__init__.py
--rw-r--r--   0        0        0     4733 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/users/users_create.py
--rw-r--r--   0        0        0     4355 2024-03-27 19:02:54.792771 zpodsdk-0.6.0/src/zpodsdk/api/users/users_disable.py
--rw-r--r--   0        0        0     4348 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/users/users_enable.py
--rw-r--r--   0        0        0     4319 2024-03-27 19:02:54.792771 zpodsdk-0.6.0/src/zpodsdk/api/users/users_get.py
--rw-r--r--   0        0        0     5108 2024-03-27 19:02:54.792771 zpodsdk-0.6.0/src/zpodsdk/api/users/users_get_all.py
--rw-r--r--   0        0        0     3911 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/users/users_get_me.py
--rw-r--r--   0        0        0     4453 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/api/users/users_reset_api_token.py
--rw-r--r--   0        0        0     5421 2024-03-27 19:02:54.792771 zpodsdk-0.6.0/src/zpodsdk/api/users/users_update.py
--rw-r--r--   0        0        0        0 2024-03-27 19:02:54.496747 zpodsdk-0.6.0/src/zpodsdk/api/zpods/__init__.py
--rw-r--r--   0        0        0     4984 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_components_add.py
--rw-r--r--   0        0        0     4946 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_components_get.py
--rw-r--r--   0        0        0     4773 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_components_get_all.py
--rw-r--r--   0        0        0     4748 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_components_remove.py
--rw-r--r--   0        0        0     4627 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_create.py
--rw-r--r--   0        0        0     4186 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_delete.py
--rw-r--r--   0        0        0     4735 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_features_get_all.py
--rw-r--r--   0        0        0     4266 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_get.py
--rw-r--r--   0        0        0     4149 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_get_all.py
--rw-r--r--   0        0        0     4735 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_networks_get_all.py
--rw-r--r--   0        0        0     4792 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_permissions_get_all.py
--rw-r--r--   0        0        0     6122 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_permissions_groups_add.py
--rw-r--r--   0        0        0     5747 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_permissions_groups_remove.py
--rw-r--r--   0        0        0     6105 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_permissions_users_add.py
--rw-r--r--   0        0        0     5730 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_permissions_users_remove.py
--rw-r--r--   0        0        0     4931 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_update.py
--rw-r--r--   0        0        0    12209 2024-03-27 19:02:54.804772 zpodsdk-0.6.0/src/zpodsdk/client.py
--rw-r--r--   0        0        0      546 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/errors.py
--rw-r--r--   0        0        0     4426 2024-04-15 14:23:40.295079 zpodsdk-0.6.0/src/zpodsdk/models/__init__.py
--rw-r--r--   0        0        0     1739 2024-03-27 19:02:54.796772 zpodsdk-0.6.0/src/zpodsdk/models/component_view.py
--rw-r--r--   0        0        0     3350 2024-03-27 19:02:54.804772 zpodsdk-0.6.0/src/zpodsdk/models/component_view_full.py
--rw-r--r--   0        0        0     2717 2024-04-15 14:23:40.295079 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_compute_create.py
--rw-r--r--   0        0        0     1965 2024-03-27 19:02:54.796772 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_compute_update.py
--rw-r--r--   0        0        0     3263 2024-04-15 14:23:40.295079 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_compute_view.py
--rw-r--r--   0        0        0     1326 2024-04-15 14:23:40.295079 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_create.py
--rw-r--r--   0        0        0      719 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_enet_create.py
--rw-r--r--   0        0        0      914 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_enet_view.py
--rw-r--r--   0        0        0     2190 2024-04-15 14:23:40.295079 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_network_create.py
--rw-r--r--   0        0        0      181 2024-04-15 14:23:40.295079 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_network_drivers.py
--rw-r--r--   0        0        0     1965 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_network_update.py
--rw-r--r--   0        0        0     2736 2024-04-15 14:23:40.295079 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_network_view.py
--rw-r--r--   0        0        0     2029 2024-03-27 19:02:54.804772 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_permission_group_add_remove.py
--rw-r--r--   0        0        0     1993 2024-03-27 19:02:54.808773 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_permission_user_add_remove.py
--rw-r--r--   0        0        0     2963 2024-03-27 19:02:54.788771 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_permission_view.py
--rw-r--r--   0        0        0      165 2024-04-15 14:23:40.295079 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_status.py
--rw-r--r--   0        0        0     3308 2024-04-15 14:23:40.295079 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_update.py
--rw-r--r--   0        0        0     1289 2024-04-15 14:23:40.295079 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_view.py
--rw-r--r--   0        0        0     1705 2024-04-15 14:23:40.295079 zpodsdk-0.6.0/src/zpodsdk/models/endpoint_view_full.py
--rw-r--r--   0        0        0     1398 2024-03-27 19:02:54.808773 zpodsdk-0.6.0/src/zpodsdk/models/endpoints_create.py
--rw-r--r--   0        0        0     3316 2024-04-15 14:23:40.295079 zpodsdk-0.6.0/src/zpodsdk/models/endpoints_update.py
--rw-r--r--   0        0        0     1362 2024-03-27 19:02:54.796772 zpodsdk-0.6.0/src/zpodsdk/models/endpoints_view.py
--rw-r--r--   0        0        0     2193 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/models/http_validation_error.py
--rw-r--r--   0        0        0     1083 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/models/library_create.py
--rw-r--r--   0        0        0     1968 2024-03-27 19:02:54.808773 zpodsdk-0.6.0/src/zpodsdk/models/library_update.py
--rw-r--r--   0        0        0     3131 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/models/library_view.py
--rw-r--r--   0        0        0      731 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/models/permission_group_create.py
--rw-r--r--   0        0        0      731 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/models/permission_group_update.py
--rw-r--r--   0        0        0      767 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/models/permission_group_user_add.py
--rw-r--r--   0        0        0     1440 2024-03-27 19:02:54.804772 zpodsdk-0.6.0/src/zpodsdk/models/permission_group_view.py
--rw-r--r--   0        0        0     2942 2024-03-27 19:02:54.804772 zpodsdk-0.6.0/src/zpodsdk/models/profile_create.py
--rw-r--r--   0        0        0     4482 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/models/profile_item_create.py
--rw-r--r--   0        0        0     4482 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/models/profile_item_update.py
--rw-r--r--   0        0        0     4474 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/models/profile_item_view.py
--rw-r--r--   0        0        0     5406 2024-03-27 19:02:54.796772 zpodsdk-0.6.0/src/zpodsdk/models/profile_update.py
--rw-r--r--   0        0        0     3696 2024-03-27 19:02:54.804772 zpodsdk-0.6.0/src/zpodsdk/models/profile_view.py
--rw-r--r--   0        0        0     1063 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/models/setting_create.py
--rw-r--r--   0        0        0     1931 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/models/setting_update.py
--rw-r--r--   0        0        0     1178 2024-03-27 19:02:54.796772 zpodsdk-0.6.0/src/zpodsdk/models/setting_view.py
--rw-r--r--   0        0        0     1808 2024-03-27 19:02:54.800772 zpodsdk-0.6.0/src/zpodsdk/models/user_create.py
--rw-r--r--   0        0        0     1951 2024-03-27 19:02:54.784771 zpodsdk-0.6.0/src/zpodsdk/models/user_update.py
--rw-r--r--   0        0        0     2692 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/models/user_update_admin.py
--rw-r--r--   0        0        0      993 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/models/user_view.py
--rw-r--r--   0        0        0     3423 2024-03-27 19:02:54.804772 zpodsdk-0.6.0/src/zpodsdk/models/user_view_full.py
--rw-r--r--   0        0        0     3634 2024-03-27 19:02:54.804772 zpodsdk-0.6.0/src/zpodsdk/models/user_view_full_plus.py
--rw-r--r--   0        0        0     2153 2024-03-27 19:02:54.804772 zpodsdk-0.6.0/src/zpodsdk/models/validation_error.py
--rw-r--r--   0        0        0     3444 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/models/zpod_component_create.py
--rw-r--r--   0        0        0     4385 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/models/zpod_component_view.py
--rw-r--r--   0        0        0     2385 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/models/zpod_create.py
--rw-r--r--   0        0        0     1081 2024-03-27 19:02:54.804772 zpodsdk-0.6.0/src/zpodsdk/models/zpod_feature_view.py
--rw-r--r--   0        0        0     1226 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/models/zpod_feature_view_data.py
--rw-r--r--   0        0        0      830 2024-03-27 19:02:54.808773 zpodsdk-0.6.0/src/zpodsdk/models/zpod_network_view.py
--rw-r--r--   0        0        0      177 2024-03-27 19:02:54.624758 zpodsdk-0.6.0/src/zpodsdk/models/zpod_permission.py
--rw-r--r--   0        0        0     2013 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/models/zpod_permission_group_add_remove.py
--rw-r--r--   0        0        0     1977 2024-03-27 19:02:54.772770 zpodsdk-0.6.0/src/zpodsdk/models/zpod_permission_user_add_remove.py
--rw-r--r--   0        0        0     3010 2024-03-27 19:02:54.804772 zpodsdk-0.6.0/src/zpodsdk/models/zpod_permission_view.py
--rw-r--r--   0        0        0      311 2024-03-27 19:02:54.656760 zpodsdk-0.6.0/src/zpodsdk/models/zpod_status.py
--rw-r--r--   0        0        0     1285 2024-03-27 19:02:54.804772 zpodsdk-0.6.0/src/zpodsdk/models/zpod_update.py
--rw-r--r--   0        0        0     6572 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/models/zpod_view.py
--rw-r--r--   0        0        0       25 2024-03-27 19:02:54.168720 zpodsdk-0.6.0/src/zpodsdk/py.typed
--rw-r--r--   0        0        0     1018 2024-03-27 19:02:54.776770 zpodsdk-0.6.0/src/zpodsdk/types.py
--rw-r--r--   0        0        0    14381 2024-03-27 19:02:54.784771 zpodsdk-0.6.0/src/zpodsdk/zpod_client.py
--rw-r--r--   0        0        0     4192 1970-01-01 00:00:00.000000 zpodsdk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3656 2023-07-18 08:54:27.717596 zpodsdk-0.6.1/README.md
+-rw-r--r--   0        0        0      497 2024-05-07 14:59:28.105945 zpodsdk-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      174 2024-05-07 14:59:28.101945 zpodsdk-0.6.1/src/zpodsdk/__init__.py
+-rw-r--r--   0        0        0       45 2024-03-21 09:35:36.949672 zpodsdk-0.6.1/src/zpodsdk/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 09:35:36.949672 zpodsdk-0.6.1/src/zpodsdk/api/components/__init__.py
+-rw-r--r--   0        0        0     4427 2024-03-21 09:35:36.949672 zpodsdk-0.6.1/src/zpodsdk/api/components/components_disable.py
+-rw-r--r--   0        0        0     4421 2024-03-21 09:35:36.949672 zpodsdk-0.6.1/src/zpodsdk/api/components/components_enable.py
+-rw-r--r--   0        0        0     4394 2024-03-21 09:35:36.949672 zpodsdk-0.6.1/src/zpodsdk/api/components/components_get.py
+-rw-r--r--   0        0        0     4277 2024-03-21 09:35:36.949672 zpodsdk-0.6.1/src/zpodsdk/api/components/components_get_all.py
+-rw-r--r--   0        0        0        0 2024-03-21 09:35:36.949672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/__init__.py
+-rw-r--r--   0        0        0     4784 2024-03-21 09:35:36.949672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_create.py
+-rw-r--r--   0        0        0     4194 2024-03-21 09:35:36.949672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_delete.py
+-rw-r--r--   0        0        0     4944 2024-03-21 09:35:36.949672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_enet_create.py
+-rw-r--r--   0        0        0     4544 2024-03-21 09:35:36.949672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_enet_delete.py
+-rw-r--r--   0        0        0     4729 2024-03-21 09:35:36.949672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_enet_get.py
+-rw-r--r--   0        0        0     4716 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_enet_get_all.py
+-rw-r--r--   0        0        0     4379 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_get.py
+-rw-r--r--   0        0        0     4262 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_get_all.py
+-rw-r--r--   0        0        0     4910 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_permissions_get_all.py
+-rw-r--r--   0        0        0     6168 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_permissions_groups_add.py
+-rw-r--r--   0        0        0     5789 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_permissions_groups_remove.py
+-rw-r--r--   0        0        0     6151 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_permissions_users_add.py
+-rw-r--r--   0        0        0     5772 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_permissions_users_remove.py
+-rw-r--r--   0        0        0     5088 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_update.py
+-rw-r--r--   0        0        0     4189 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_verify.py
+-rw-r--r--   0        0        0        0 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/libraries/__init__.py
+-rw-r--r--   0        0        0     4707 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/libraries/libraries_create.py
+-rw-r--r--   0        0        0     4194 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/libraries/libraries_delete.py
+-rw-r--r--   0        0        0     4313 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/libraries/libraries_get.py
+-rw-r--r--   0        0        0     4196 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/libraries/libraries_get_all.py
+-rw-r--r--   0        0        0     4338 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/libraries/libraries_resync.py
+-rw-r--r--   0        0        0     5011 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/libraries/libraries_update.py
+-rw-r--r--   0        0        0        0 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/__init__.py
+-rw-r--r--   0        0        0     4916 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_create.py
+-rw-r--r--   0        0        0     4209 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_delete.py
+-rw-r--r--   0        0        0     4433 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_get.py
+-rw-r--r--   0        0        0     4354 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_get_all.py
+-rw-r--r--   0        0        0     4973 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_update.py
+-rw-r--r--   0        0        0     5460 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_users_add.py
+-rw-r--r--   0        0        0     4689 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_users_delete.py
+-rw-r--r--   0        0        0     4696 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_users_get_all.py
+-rw-r--r--   0        0        0        0 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/profiles/__init__.py
+-rw-r--r--   0        0        0     5377 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/profiles/profiles_create.py
+-rw-r--r--   0        0        0     4192 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/profiles/profiles_delete.py
+-rw-r--r--   0        0        0     4311 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/profiles/profiles_get.py
+-rw-r--r--   0        0        0     4194 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/profiles/profiles_get_all.py
+-rw-r--r--   0        0        0     5009 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/profiles/profiles_update.py
+-rw-r--r--   0        0        0        0 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/root/__init__.py
+-rw-r--r--   0        0        0     3728 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/root/root_root.py
+-rw-r--r--   0        0        0        0 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/settings/__init__.py
+-rw-r--r--   0        0        0     4705 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/settings/settings_create.py
+-rw-r--r--   0        0        0     4192 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/settings/settings_delete.py
+-rw-r--r--   0        0        0     4311 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/settings/settings_get.py
+-rw-r--r--   0        0        0     4194 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/settings/settings_get_all.py
+-rw-r--r--   0        0        0     5009 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/settings/settings_update.py
+-rw-r--r--   0        0        0        0 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/users/__init__.py
+-rw-r--r--   0        0        0     4733 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/users/users_create.py
+-rw-r--r--   0        0        0     4355 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/users/users_disable.py
+-rw-r--r--   0        0        0     4348 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/users/users_enable.py
+-rw-r--r--   0        0        0     4319 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/users/users_get.py
+-rw-r--r--   0        0        0     5108 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/users/users_get_all.py
+-rw-r--r--   0        0        0     3911 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/users/users_get_me.py
+-rw-r--r--   0        0        0     4453 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/users/users_reset_api_token.py
+-rw-r--r--   0        0        0     5421 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/users/users_update.py
+-rw-r--r--   0        0        0        0 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/__init__.py
+-rw-r--r--   0        0        0     4984 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_components_add.py
+-rw-r--r--   0        0        0     4946 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_components_get.py
+-rw-r--r--   0        0        0     4773 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_components_get_all.py
+-rw-r--r--   0        0        0     4748 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_components_remove.py
+-rw-r--r--   0        0        0     4627 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_create.py
+-rw-r--r--   0        0        0     4186 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_delete.py
+-rw-r--r--   0        0        0     4735 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_features_get_all.py
+-rw-r--r--   0        0        0     4266 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_get.py
+-rw-r--r--   0        0        0     4149 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_get_all.py
+-rw-r--r--   0        0        0     4735 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_networks_get_all.py
+-rw-r--r--   0        0        0     4792 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_permissions_get_all.py
+-rw-r--r--   0        0        0     6122 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_permissions_groups_add.py
+-rw-r--r--   0        0        0     5747 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_permissions_groups_remove.py
+-rw-r--r--   0        0        0     6105 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_permissions_users_add.py
+-rw-r--r--   0        0        0     5730 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_permissions_users_remove.py
+-rw-r--r--   0        0        0     4931 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_update.py
+-rw-r--r--   0        0        0    12209 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/client.py
+-rw-r--r--   0        0        0      546 2024-03-25 18:36:05.588859 zpodsdk-0.6.1/src/zpodsdk/errors.py
+-rw-r--r--   0        0        0     4426 2024-04-15 14:55:56.813893 zpodsdk-0.6.1/src/zpodsdk/models/__init__.py
+-rw-r--r--   0        0        0     1739 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/models/component_view.py
+-rw-r--r--   0        0        0     3350 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/models/component_view_full.py
+-rw-r--r--   0        0        0     2717 2024-04-15 14:55:56.813893 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_compute_create.py
+-rw-r--r--   0        0        0     1965 2024-03-21 09:35:36.953672 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_compute_update.py
+-rw-r--r--   0        0        0     3263 2024-04-15 14:55:56.813893 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_compute_view.py
+-rw-r--r--   0        0        0     1326 2024-04-15 14:55:56.813893 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_create.py
+-rw-r--r--   0        0        0      719 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_enet_create.py
+-rw-r--r--   0        0        0      914 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_enet_view.py
+-rw-r--r--   0        0        0     2190 2024-04-15 14:55:56.813893 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_network_create.py
+-rw-r--r--   0        0        0      181 2024-04-15 14:55:56.813893 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_network_drivers.py
+-rw-r--r--   0        0        0     1965 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_network_update.py
+-rw-r--r--   0        0        0     2736 2024-04-15 14:55:56.813893 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_network_view.py
+-rw-r--r--   0        0        0     2029 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_permission_group_add_remove.py
+-rw-r--r--   0        0        0     1993 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_permission_user_add_remove.py
+-rw-r--r--   0        0        0     2963 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_permission_view.py
+-rw-r--r--   0        0        0      165 2024-04-15 14:55:56.813893 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_status.py
+-rw-r--r--   0        0        0     3308 2024-04-15 14:55:56.813893 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_update.py
+-rw-r--r--   0        0        0     1289 2024-04-15 14:55:56.813893 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_view.py
+-rw-r--r--   0        0        0     1705 2024-04-15 14:55:56.813893 zpodsdk-0.6.1/src/zpodsdk/models/endpoint_view_full.py
+-rw-r--r--   0        0        0     1398 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/endpoints_create.py
+-rw-r--r--   0        0        0     3316 2024-04-15 14:55:56.813893 zpodsdk-0.6.1/src/zpodsdk/models/endpoints_update.py
+-rw-r--r--   0        0        0     1362 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/endpoints_view.py
+-rw-r--r--   0        0        0     2193 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/http_validation_error.py
+-rw-r--r--   0        0        0     1083 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/library_create.py
+-rw-r--r--   0        0        0     1968 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/library_update.py
+-rw-r--r--   0        0        0     3131 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/library_view.py
+-rw-r--r--   0        0        0      731 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/permission_group_create.py
+-rw-r--r--   0        0        0      731 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/permission_group_update.py
+-rw-r--r--   0        0        0      767 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/permission_group_user_add.py
+-rw-r--r--   0        0        0     1440 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/permission_group_view.py
+-rw-r--r--   0        0        0     2942 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/profile_create.py
+-rw-r--r--   0        0        0     4482 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/profile_item_create.py
+-rw-r--r--   0        0        0     4482 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/profile_item_update.py
+-rw-r--r--   0        0        0     4474 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/profile_item_view.py
+-rw-r--r--   0        0        0     5406 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/profile_update.py
+-rw-r--r--   0        0        0     3696 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/profile_view.py
+-rw-r--r--   0        0        0     1063 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/setting_create.py
+-rw-r--r--   0        0        0     1931 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/setting_update.py
+-rw-r--r--   0        0        0     1178 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/setting_view.py
+-rw-r--r--   0        0        0     1808 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/user_create.py
+-rw-r--r--   0        0        0     1951 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/user_update.py
+-rw-r--r--   0        0        0     2692 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/user_update_admin.py
+-rw-r--r--   0        0        0      993 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/user_view.py
+-rw-r--r--   0        0        0     3423 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/user_view_full.py
+-rw-r--r--   0        0        0     3634 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/user_view_full_plus.py
+-rw-r--r--   0        0        0     2153 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/validation_error.py
+-rw-r--r--   0        0        0     3444 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/zpod_component_create.py
+-rw-r--r--   0        0        0     4385 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/zpod_component_view.py
+-rw-r--r--   0        0        0     2385 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/zpod_create.py
+-rw-r--r--   0        0        0     1081 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/zpod_feature_view.py
+-rw-r--r--   0        0        0     1226 2024-03-25 18:36:05.588859 zpodsdk-0.6.1/src/zpodsdk/models/zpod_feature_view_data.py
+-rw-r--r--   0        0        0      830 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/zpod_network_view.py
+-rw-r--r--   0        0        0      177 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/zpod_permission.py
+-rw-r--r--   0        0        0     2013 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/zpod_permission_group_add_remove.py
+-rw-r--r--   0        0        0     1977 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/zpod_permission_user_add_remove.py
+-rw-r--r--   0        0        0     3010 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/zpod_permission_view.py
+-rw-r--r--   0        0        0      311 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/zpod_status.py
+-rw-r--r--   0        0        0     1285 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/zpod_update.py
+-rw-r--r--   0        0        0     6572 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/models/zpod_view.py
+-rw-r--r--   0        0        0       25 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/py.typed
+-rw-r--r--   0        0        0     1018 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/types.py
+-rw-r--r--   0        0        0    14381 2024-03-21 09:35:36.957673 zpodsdk-0.6.1/src/zpodsdk/zpod_client.py
+-rw-r--r--   0        0        0     4192 1970-01-01 00:00:00.000000 zpodsdk-0.6.1/PKG-INFO
```

### Comparing `zpodsdk-0.6.0/README.md` & `zpodsdk-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/components/components_disable.py` & `zpodsdk-0.6.1/src/zpodsdk/api/components/components_disable.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/components/components_enable.py` & `zpodsdk-0.6.1/src/zpodsdk/api/components/components_enable.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/components/components_get.py` & `zpodsdk-0.6.1/src/zpodsdk/api/components/components_get.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/components/components_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/components/components_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_create.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_delete.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_delete.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_enet_create.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_enet_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_enet_delete.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_enet_delete.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_enet_get.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_enet_get.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_enet_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_enet_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_get.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_get.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_permissions_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_permissions_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_permissions_groups_add.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_permissions_groups_add.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_permissions_groups_remove.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_permissions_groups_remove.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_permissions_users_add.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_permissions_users_add.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_permissions_users_remove.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_permissions_users_remove.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_update.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/endpoints/endpoints_verify.py` & `zpodsdk-0.6.1/src/zpodsdk/api/endpoints/endpoints_verify.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/libraries/libraries_create.py` & `zpodsdk-0.6.1/src/zpodsdk/api/libraries/libraries_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/libraries/libraries_delete.py` & `zpodsdk-0.6.1/src/zpodsdk/api/libraries/libraries_delete.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/libraries/libraries_get.py` & `zpodsdk-0.6.1/src/zpodsdk/api/libraries/libraries_get.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/libraries/libraries_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/libraries/libraries_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/libraries/libraries_resync.py` & `zpodsdk-0.6.1/src/zpodsdk/api/libraries/libraries_resync.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/libraries/libraries_update.py` & `zpodsdk-0.6.1/src/zpodsdk/api/libraries/libraries_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_create.py` & `zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_delete.py` & `zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_delete.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_get.py` & `zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_get.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_update.py` & `zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_users_add.py` & `zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_users_add.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_users_delete.py` & `zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_users_delete.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/permission_groups/permission_groups_users_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/permission_groups/permission_groups_users_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/profiles/profiles_create.py` & `zpodsdk-0.6.1/src/zpodsdk/api/profiles/profiles_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/profiles/profiles_delete.py` & `zpodsdk-0.6.1/src/zpodsdk/api/profiles/profiles_delete.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/profiles/profiles_get.py` & `zpodsdk-0.6.1/src/zpodsdk/api/profiles/profiles_get.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/profiles/profiles_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/profiles/profiles_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/profiles/profiles_update.py` & `zpodsdk-0.6.1/src/zpodsdk/api/profiles/profiles_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/root/root_root.py` & `zpodsdk-0.6.1/src/zpodsdk/api/root/root_root.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/settings/settings_create.py` & `zpodsdk-0.6.1/src/zpodsdk/api/settings/settings_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/settings/settings_delete.py` & `zpodsdk-0.6.1/src/zpodsdk/api/settings/settings_delete.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/settings/settings_get.py` & `zpodsdk-0.6.1/src/zpodsdk/api/settings/settings_get.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/settings/settings_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/settings/settings_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/settings/settings_update.py` & `zpodsdk-0.6.1/src/zpodsdk/api/settings/settings_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/users/users_create.py` & `zpodsdk-0.6.1/src/zpodsdk/api/users/users_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/users/users_disable.py` & `zpodsdk-0.6.1/src/zpodsdk/api/users/users_disable.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/users/users_enable.py` & `zpodsdk-0.6.1/src/zpodsdk/api/users/users_enable.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/users/users_get.py` & `zpodsdk-0.6.1/src/zpodsdk/api/users/users_get.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/users/users_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/users/users_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/users/users_get_me.py` & `zpodsdk-0.6.1/src/zpodsdk/api/users/users_get_me.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/users/users_reset_api_token.py` & `zpodsdk-0.6.1/src/zpodsdk/api/users/users_reset_api_token.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/users/users_update.py` & `zpodsdk-0.6.1/src/zpodsdk/api/users/users_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_components_add.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_components_add.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_components_get.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_components_get.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_components_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_components_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_components_remove.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_components_remove.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_create.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_delete.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_delete.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_features_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_features_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_get.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_get.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_networks_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_networks_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_permissions_get_all.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_permissions_get_all.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_permissions_groups_add.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_permissions_groups_add.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_permissions_groups_remove.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_permissions_groups_remove.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_permissions_users_add.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_permissions_users_add.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_permissions_users_remove.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_permissions_users_remove.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/api/zpods/zpods_update.py` & `zpodsdk-0.6.1/src/zpodsdk/api/zpods/zpods_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/client.py` & `zpodsdk-0.6.1/src/zpodsdk/client.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/errors.py` & `zpodsdk-0.6.1/src/zpodsdk/errors.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/__init__.py` & `zpodsdk-0.6.1/src/zpodsdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/component_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/component_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/component_view_full.py` & `zpodsdk-0.6.1/src/zpodsdk/models/component_view_full.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_compute_create.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_compute_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_compute_update.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_compute_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_compute_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_compute_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_create.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_enet_create.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_enet_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_enet_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_enet_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_network_create.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_network_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_network_update.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_network_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_network_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_network_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_permission_group_add_remove.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_permission_group_add_remove.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_permission_user_add_remove.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_permission_user_add_remove.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_permission_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_permission_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_update.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoint_view_full.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoint_view_full.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoints_create.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoints_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoints_update.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoints_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/endpoints_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/endpoints_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/http_validation_error.py` & `zpodsdk-0.6.1/src/zpodsdk/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/library_create.py` & `zpodsdk-0.6.1/src/zpodsdk/models/library_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/library_update.py` & `zpodsdk-0.6.1/src/zpodsdk/models/library_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/library_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/library_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/permission_group_create.py` & `zpodsdk-0.6.1/src/zpodsdk/models/permission_group_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/permission_group_update.py` & `zpodsdk-0.6.1/src/zpodsdk/models/permission_group_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/permission_group_user_add.py` & `zpodsdk-0.6.1/src/zpodsdk/models/permission_group_user_add.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/permission_group_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/permission_group_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/profile_create.py` & `zpodsdk-0.6.1/src/zpodsdk/models/profile_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/profile_item_create.py` & `zpodsdk-0.6.1/src/zpodsdk/models/profile_item_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/profile_item_update.py` & `zpodsdk-0.6.1/src/zpodsdk/models/profile_item_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/profile_item_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/profile_item_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/profile_update.py` & `zpodsdk-0.6.1/src/zpodsdk/models/profile_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/profile_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/profile_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/setting_create.py` & `zpodsdk-0.6.1/src/zpodsdk/models/setting_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/setting_update.py` & `zpodsdk-0.6.1/src/zpodsdk/models/setting_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/setting_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/setting_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/user_create.py` & `zpodsdk-0.6.1/src/zpodsdk/models/user_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/user_update.py` & `zpodsdk-0.6.1/src/zpodsdk/models/user_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/user_update_admin.py` & `zpodsdk-0.6.1/src/zpodsdk/models/user_update_admin.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/user_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/user_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/user_view_full.py` & `zpodsdk-0.6.1/src/zpodsdk/models/user_view_full.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/user_view_full_plus.py` & `zpodsdk-0.6.1/src/zpodsdk/models/user_view_full_plus.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/validation_error.py` & `zpodsdk-0.6.1/src/zpodsdk/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/zpod_component_create.py` & `zpodsdk-0.6.1/src/zpodsdk/models/zpod_component_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/zpod_component_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/zpod_component_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/zpod_create.py` & `zpodsdk-0.6.1/src/zpodsdk/models/zpod_create.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/zpod_feature_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/zpod_feature_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/zpod_feature_view_data.py` & `zpodsdk-0.6.1/src/zpodsdk/models/zpod_feature_view_data.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/zpod_network_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/zpod_network_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/zpod_permission_group_add_remove.py` & `zpodsdk-0.6.1/src/zpodsdk/models/zpod_permission_group_add_remove.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/zpod_permission_user_add_remove.py` & `zpodsdk-0.6.1/src/zpodsdk/models/zpod_permission_user_add_remove.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/zpod_permission_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/zpod_permission_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/zpod_update.py` & `zpodsdk-0.6.1/src/zpodsdk/models/zpod_update.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/models/zpod_view.py` & `zpodsdk-0.6.1/src/zpodsdk/models/zpod_view.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/types.py` & `zpodsdk-0.6.1/src/zpodsdk/types.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/src/zpodsdk/zpod_client.py` & `zpodsdk-0.6.1/src/zpodsdk/zpod_client.py`

 * *Files identical despite different names*

### Comparing `zpodsdk-0.6.0/PKG-INFO` & `zpodsdk-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpodsdk
-Version: 0.6.0
+Version: 0.6.1
 Summary: A client library for accessing zPod API
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

