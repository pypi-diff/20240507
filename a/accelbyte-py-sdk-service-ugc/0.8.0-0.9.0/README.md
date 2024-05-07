# Comparing `tmp/accelbyte-py-sdk-service-ugc-0.8.0.tar.gz` & `tmp/accelbyte-py-sdk-service-ugc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-ugc-0.8.0.tar", last modified: Tue Feb 27 05:43:03 2024, max compression
+gzip compressed data, was "accelbyte-py-sdk-service-ugc-0.9.0.tar", last modified: Wed Mar 13 06:15:13 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-ugc-0.8.0.tar` & `accelbyte-py-sdk-service-ugc-0.9.0.tar`

### file list

```diff
@@ -1,321 +1,321 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.246808 accelbyte-py-sdk-service-ugc-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1109 2024-02-27 05:43:03.246808 accelbyte-py-sdk-service-ugc-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      865 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.218808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.218808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.218808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/
--rw-rw-r--   0 root         (0) root         (0)    17282 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.226808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/
--rw-rw-r--   0 root         (0) root         (0)     6729 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3924 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_add_download_count_response.py
--rw-rw-r--   0 root         (0) root         (0)     9294 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_admin_content_request_v2.py
--rw-rw-r--   0 root         (0) root         (0)     4035 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_admin_get_content_bulk_request.py
--rw-rw-r--   0 root         (0) root         (0)    12487 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_admin_update_content_request.py
--rw-rw-r--   0 root         (0) root         (0)     7818 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_admin_update_content_request_v2.py
--rw-rw-r--   0 root         (0) root         (0)     4592 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_approve_staging_content_request.py
--rw-rw-r--   0 root         (0) root         (0)     4300 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_channel_request.py
--rw-rw-r--   0 root         (0) root         (0)     6456 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_channel_response.py
--rw-rw-r--   0 root         (0) root         (0)     4944 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_config_response.py
--rw-rw-r--   0 root         (0) root         (0)    23046 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_download_response.py
--rw-rw-r--   0 root         (0) root         (0)    20806 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_download_response_v2.py
--rw-rw-r--   0 root         (0) root         (0)     6141 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_downloader_response.py
--rw-rw-r--   0 root         (0) root         (0)     3889 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_like_request.py
--rw-rw-r--   0 root         (0) root         (0)     4596 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_like_response.py
--rw-rw-r--   0 root         (0) root         (0)     5944 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_likers_response.py
--rw-rw-r--   0 root         (0) root         (0)     8445 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_request_v2.py
--rw-rw-r--   0 root         (0) root         (0)     5029 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_snapshot.py
--rw-rw-r--   0 root         (0) root         (0)     6088 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_version_response.py
--rw-rw-r--   0 root         (0) root         (0)     9251 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_content_request.py
--rw-rw-r--   0 root         (0) root         (0)    11023 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_content_request_s3.py
--rw-rw-r--   0 root         (0) root         (0)    20160 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_content_response.py
--rw-rw-r--   0 root         (0) root         (0)    18653 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_content_response_v2.py
--rw-rw-r--   0 root         (0) root         (0)     4462 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_group_request.py
--rw-rw-r--   0 root         (0) root         (0)     7856 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_group_response.py
--rw-rw-r--   0 root         (0) root         (0)     4467 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_screenshot_request.py
--rw-rw-r--   0 root         (0) root         (0)     6055 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_screenshot_request_item.py
--rw-rw-r--   0 root         (0) root         (0)     4404 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_screenshot_response.py
--rw-rw-r--   0 root         (0) root         (0)     3703 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_tag_request.py
--rw-rw-r--   0 root         (0) root         (0)     4935 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_tag_response.py
--rw-rw-r--   0 root         (0) root         (0)     4441 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_type_request.py
--rw-rw-r--   0 root         (0) root         (0)     6512 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_type_response.py
--rw-rw-r--   0 root         (0) root         (0)     4398 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_creator_follow_state.py
--rw-rw-r--   0 root         (0) root         (0)     7686 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_creator_overview_response.py
--rw-rw-r--   0 root         (0) root         (0)     8815 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_creator_response.py
--rw-rw-r--   0 root         (0) root         (0)     4975 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_generate_content_upload_url_request.py
--rw-rw-r--   0 root         (0) root         (0)     6321 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_generate_content_upload_url_response.py
--rw-rw-r--   0 root         (0) root         (0)     4128 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_get_content_bulk_by_share_codes_request.py
--rw-rw-r--   0 root         (0) root         (0)     4940 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_get_content_preview_response.py
--rw-rw-r--   0 root         (0) root         (0)     3849 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_hide_content_request.py
--rw-rw-r--   0 root         (0) root         (0)     4258 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_like_state.py
--rw-rw-r--   0 root         (0) root         (0)     4327 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_list_content_versions_response.py
--rw-rw-r--   0 root         (0) root         (0)     5331 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_download_response.py
--rw-rw-r--   0 root         (0) root         (0)     5371 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_download_response_v2.py
--rw-rw-r--   0 root         (0) root         (0)     5369 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_downloader_response.py
--rw-rw-r--   0 root         (0) root         (0)     5293 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_likers_response.py
--rw-rw-r--   0 root         (0) root         (0)     5331 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_creator_overview_response.py
--rw-rw-r--   0 root         (0) root         (0)     5151 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_channel_response.py
--rw-rw-r--   0 root         (0) root         (0)     5144 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_configs_response.py
--rw-rw-r--   0 root         (0) root         (0)     5142 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_tag_response.py
--rw-rw-r--   0 root         (0) root         (0)     5161 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_type_response.py
--rw-rw-r--   0 root         (0) root         (0)     5143 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_group_response.py
--rw-rw-r--   0 root         (0) root         (0)     5361 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_list_staging_content_response.py
--rw-rw-r--   0 root         (0) root         (0)     5475 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paging_cursor.py
--rw-rw-r--   0 root         (0) root         (0)     4206 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_payload_url.py
--rw-rw-r--   0 root         (0) root         (0)     4975 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_preview_metadata.py
--rw-rw-r--   0 root         (0) root         (0)     4323 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_preview_url.py
--rw-rw-r--   0 root         (0) root         (0)     3767 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_public_channel_request.py
--rw-rw-r--   0 root         (0) root         (0)    10388 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_public_create_content_request_s3.py
--rw-rw-r--   0 root         (0) root         (0)     4046 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_public_get_content_bulk_request.py
--rw-rw-r--   0 root         (0) root         (0)     7395 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_screenshot_response.py
--rw-rw-r--   0 root         (0) root         (0)    15478 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_staging_content_response.py
--rw-rw-r--   0 root         (0) root         (0)     3767 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_channel_request.py
--rw-rw-r--   0 root         (0) root         (0)     3776 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_config_request.py
--rw-rw-r--   0 root         (0) root         (0)    11628 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_content_request.py
--rw-rw-r--   0 root         (0) root         (0)     6987 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_content_request_v2.py
--rw-rw-r--   0 root         (0) root         (0)    18653 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_content_response_v2.py
--rw-rw-r--   0 root         (0) root         (0)     3980 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_content_share_code_request.py
--rw-rw-r--   0 root         (0) root         (0)     4838 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_file_location_request.py
--rw-rw-r--   0 root         (0) root         (0)     4615 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_screenshot.py
--rw-rw-r--   0 root         (0) root         (0)     4341 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_screenshot_request.py
--rw-rw-r--   0 root         (0) root         (0)     4352 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_screenshot_response.py
--rw-rw-r--   0 root         (0) root         (0)     4862 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_staging_content_request.py
--rw-rw-r--   0 root         (0) root         (0)     3918 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_user_follow_request.py
--rw-rw-r--   0 root         (0) root         (0)     4564 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_user_follow_response.py
--rw-rw-r--   0 root         (0) root         (0)     4431 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/response_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.226808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/
--rw-rw-r--   0 root         (0) root         (0)      432 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.226808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/
--rw-rw-r--   0 root         (0) root         (0)      863 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7767 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_create_channel.py
--rw-rw-r--   0 root         (0) root         (0)     7843 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_delete_channel.py
--rw-rw-r--   0 root         (0) root         (0)     9613 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_get_channel.py
--rw-rw-r--   0 root         (0) root         (0)     9396 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_update_channel.py
--rw-rw-r--   0 root         (0) root         (0)     7102 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/single_admin_delete_channel.py
--rw-rw-r--   0 root         (0) root         (0)     8163 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/single_admin_get_channel.py
--rw-rw-r--   0 root         (0) root         (0)     8620 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/single_admin_update_channel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.226808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_config/
--rw-rw-r--   0 root         (0) root         (0)      563 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8320 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_config/admin_get_configs.py
--rw-rw-r--   0 root         (0) root         (0)     8378 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_config/admin_update_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.230808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/
--rw-rw-r--   0 root         (0) root         (0)     2083 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8853 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_delete_content.py
--rw-rw-r--   0 root         (0) root         (0)     8758 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_delete_content_sc_eeb785.py
--rw-rw-r--   0 root         (0) root         (0)     7463 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_download_content_preview.py
--rw-rw-r--   0 root         (0) root         (0)     9169 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_content.py
--rw-rw-r--   0 root         (0) root         (0)     8183 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_content_bulk.py
--rw-rw-r--   0 root         (0) root         (0)     8369 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_content_bulk__102504.py
--rw-rw-r--   0 root         (0) root         (0)     7502 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_specific_content.py
--rw-rw-r--   0 root         (0) root         (0)     7505 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_user_content__d4dc92.py
--rw-rw-r--   0 root         (0) root         (0)     9919 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_hide_user_content.py
--rw-rw-r--   0 root         (0) root         (0)    18427 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_search_channel_sp_40f87c.py
--rw-rw-r--   0 root         (0) root         (0)    17222 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_search_content.py
--rw-rw-r--   0 root         (0) root         (0)    10954 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_content_direct.py
--rw-rw-r--   0 root         (0) root         (0)    11720 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_content_s3.py
--rw-rw-r--   0 root         (0) root         (0)    12033 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_content_s3_bb64ed.py
--rw-rw-r--   0 root         (0) root         (0)     9139 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_screenshots.py
--rw-rw-r--   0 root         (0) root         (0)     9421 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_upload_content_direct.py
--rw-rw-r--   0 root         (0) root         (0)    10067 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_upload_content_s3.py
--rw-rw-r--   0 root         (0) root         (0)     9659 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_upload_content_sc_b38ae0.py
--rw-rw-r--   0 root         (0) root         (0)     8963 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/delete_content_by_share_code.py
--rw-rw-r--   0 root         (0) root         (0)     7498 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/list_content_versions.py
--rw-rw-r--   0 root         (0) root         (0)     8816 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/rollback_content_version.py
--rw-rw-r--   0 root         (0) root         (0)     8150 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_delete_content.py
--rw-rw-r--   0 root         (0) root         (0)     8445 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_get_content.py
--rw-rw-r--   0 root         (0) root         (0)    10105 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_update_con_1f2ab1.py
--rw-rw-r--   0 root         (0) root         (0)    11175 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_update_content_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.230808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/
--rw-rw-r--   0 root         (0) root         (0)     2190 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8388 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_bulk_get_content__b85ce3.py
--rw-rw-r--   0 root         (0) root         (0)     9601 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_create_content_v2.py
--rw-rw-r--   0 root         (0) root         (0)     8996 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_content_by_cd2201.py
--rw-rw-r--   0 root         (0) root         (0)     8775 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_content_sc_bf1900.py
--rw-rw-r--   0 root         (0) root         (0)     8208 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_official_c_0e2f56.py
--rw-rw-r--   0 root         (0) root         (0)     8919 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_user_content_v2.py
--rw-rw-r--   0 root         (0) root         (0)    10173 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_generate_official_791850.py
--rw-rw-r--   0 root         (0) root         (0)    10915 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_generate_user_con_cdad13.py
--rw-rw-r--   0 root         (0) root         (0)     8394 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_bulk__b58c74.py
--rw-rw-r--   0 root         (0) root         (0)    10810 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_ch_c1fd57.py
--rw-rw-r--   0 root         (0) root         (0)     7661 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_co_c26e1e.py
--rw-rw-r--   0 root         (0) root         (0)     7680 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_sh_03305f.py
--rw-rw-r--   0 root         (0) root         (0)    10200 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_user_idv2.py
--rw-rw-r--   0 root         (0) root         (0)    14035 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_list_content_v2.py
--rw-rw-r--   0 root         (0) root         (0)    11347 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_content_by_e139ff.py
--rw-rw-r--   0 root         (0) root         (0)    10115 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_content_hi_72a875.py
--rw-rw-r--   0 root         (0) root         (0)    10334 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_official_c_348c5f.py
--rw-rw-r--   0 root         (0) root         (0)    10149 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_official_c_e7d890.py
--rw-rw-r--   0 root         (0) root         (0)     9322 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_screenshots_v2.py
--rw-rw-r--   0 root         (0) root         (0)    11098 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_user_conte_8a8bc8.py
--rw-rw-r--   0 root         (0) root         (0)    10864 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_user_content_v2.py
--rw-rw-r--   0 root         (0) root         (0)     9674 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_upload_content_sc_3461bc.py
--rw-rw-r--   0 root         (0) root         (0)     7515 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/list_content_versions_v2.py
--rw-rw-r--   0 root         (0) root         (0)     8833 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/rollback_content_version_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.234808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/
--rw-rw-r--   0 root         (0) root         (0)     1232 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7559 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_create_group.py
--rw-rw-r--   0 root         (0) root         (0)     7747 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_delete_group.py
--rw-rw-r--   0 root         (0) root         (0)     8890 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_all_groups.py
--rw-rw-r--   0 root         (0) root         (0)     7919 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_group.py
--rw-rw-r--   0 root         (0) root         (0)    10388 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_group_contents.py
--rw-rw-r--   0 root         (0) root         (0)     9819 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_official_grou_23b467.py
--rw-rw-r--   0 root         (0) root         (0)    10581 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_user_group_co_73e55d.py
--rw-rw-r--   0 root         (0) root         (0)     9389 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_update_group.py
--rw-rw-r--   0 root         (0) root         (0)     7010 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_delete_group.py
--rw-rw-r--   0 root         (0) root         (0)     8162 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_get_all_groups.py
--rw-rw-r--   0 root         (0) root         (0)     7175 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_get_group.py
--rw-rw-r--   0 root         (0) root         (0)     9650 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_get_group__c6800e.py
--rw-rw-r--   0 root         (0) root         (0)     8631 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_update_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.234808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/
--rw-rw-r--   0 root         (0) root         (0)      745 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9260 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_approve_staging_content.py
--rw-rw-r--   0 root         (0) root         (0)     7690 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_get_staging_conte_7fe68e.py
--rw-rw-r--   0 root         (0) root         (0)    10254 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_list_staging_contents.py
--rw-rw-r--   0 root         (0) root         (0)    11074 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_list_user_staging_d2fe4e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.234808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/
--rw-rw-r--   0 root         (0) root         (0)      639 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7748 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_create_tag.py
--rw-rw-r--   0 root         (0) root         (0)     6857 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_delete_tag.py
--rw-rw-r--   0 root         (0) root         (0)     8007 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_get_tag.py
--rw-rw-r--   0 root         (0) root         (0)     8649 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_update_tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.234808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_type/
--rw-rw-r--   0 root         (0) root         (0)      647 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_type/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7788 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_create_type.py
--rw-rw-r--   0 root         (0) root         (0)     6899 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_delete_type.py
--rw-rw-r--   0 root         (0) root         (0)     8013 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_get_type.py
--rw-rw-r--   0 root         (0) root         (0)     8721 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_update_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.234808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/
--rw-rw-r--   0 root         (0) root         (0)      967 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7057 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_channels.py
--rw-rw-r--   0 root         (0) root         (0)     7086 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_contents.py
--rw-rw-r--   0 root         (0) root         (0)     7035 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_group.py
--rw-rw-r--   0 root         (0) root         (0)     7189 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_states.py
--rw-rw-r--   0 root         (0) root         (0)     7053 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_channel.py
--rw-rw-r--   0 root         (0) root         (0)     7142 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_contents.py
--rw-rw-r--   0 root         (0) root         (0)     7051 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_group.py
--rw-rw-r--   0 root         (0) root         (0)     7210 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_states.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.234808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_channel/
--rw-rw-r--   0 root         (0) root         (0)      642 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_channel/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7855 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_channel/delete_channel.py
--rw-rw-r--   0 root         (0) root         (0)     9658 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_channel/get_channels.py
--rw-rw-r--   0 root         (0) root         (0)     8345 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_channel/public_create_channel.py
--rw-rw-r--   0 root         (0) root         (0)     9403 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_channel/update_channel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.238808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/
--rw-rw-r--   0 root         (0) root         (0)     1647 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10012 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/create_content_direct.py
--rw-rw-r--   0 root         (0) root         (0)    10670 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/create_content_s3.py
--rw-rw-r--   0 root         (0) root         (0)     8869 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/delete_content.py
--rw-rw-r--   0 root         (0) root         (0)     9545 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/delete_content_screenshot.py
--rw-rw-r--   0 root         (0) root         (0)     9041 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_delete_content_b_e67ae8.py
--rw-rw-r--   0 root         (0) root         (0)     7511 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_download_content_2d5c80.py
--rw-rw-r--   0 root         (0) root         (0)     7404 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_download_content_32df1f.py
--rw-rw-r--   0 root         (0) root         (0)     7550 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_download_content_511956.py
--rw-rw-r--   0 root         (0) root         (0)     7953 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_get_content_bulk.py
--rw-rw-r--   0 root         (0) root         (0)     8293 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_get_content_bulk_382fb9.py
--rw-rw-r--   0 root         (0) root         (0)     9325 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_get_user_content.py
--rw-rw-r--   0 root         (0) root         (0)    17221 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_search_content.py
--rw-rw-r--   0 root         (0) root         (0)    11873 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_update_content_b_7f10f2.py
--rw-rw-r--   0 root         (0) root         (0)    18243 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/search_channel_specific_10d5e8.py
--rw-rw-r--   0 root         (0) root         (0)    10813 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_content_direct.py
--rw-rw-r--   0 root         (0) root         (0)    11521 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_content_s3.py
--rw-rw-r--   0 root         (0) root         (0)    11357 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_content_share_code.py
--rw-rw-r--   0 root         (0) root         (0)     9928 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_screenshots.py
--rw-rw-r--   0 root         (0) root         (0)    10452 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/upload_content_screenshot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.238808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/
--rw-rw-r--   0 root         (0) root         (0)     1698 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9707 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/delete_content_screenshot_v2.py
--rw-rw-r--   0 root         (0) root         (0)     7993 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_bulk_get_content_a86be5.py
--rw-rw-r--   0 root         (0) root         (0)     9960 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_create_content_v2.py
--rw-rw-r--   0 root         (0) root         (0)     9051 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_delete_content_b_4792d8.py
--rw-rw-r--   0 root         (0) root         (0)     8927 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_delete_content_v2.py
--rw-rw-r--   0 root         (0) root         (0)    11187 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_generate_content_ffec28.py
--rw-rw-r--   0 root         (0) root         (0)     8325 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_bulk_503347.py
--rw-rw-r--   0 root         (0) root         (0)    10789 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_c_87966e.py
--rw-rw-r--   0 root         (0) root         (0)     7610 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_idv2.py
--rw-rw-r--   0 root         (0) root         (0)     7497 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_s_4f7083.py
--rw-rw-r--   0 root         (0) root         (0)    10295 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_u_635e0b.py
--rw-rw-r--   0 root         (0) root         (0)    13948 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_list_content_v2.py
--rw-rw-r--   0 root         (0) root         (0)    11130 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_update_content_b_0c4d9c.py
--rw-rw-r--   0 root         (0) root         (0)    11340 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_update_content_f_55e48b.py
--rw-rw-r--   0 root         (0) root         (0)    10719 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_update_content_v2.py
--rw-rw-r--   0 root         (0) root         (0)    11598 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/update_content_share_code_v2.py
--rw-rw-r--   0 root         (0) root         (0)     9938 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/update_screenshots_v2.py
--rw-rw-r--   0 root         (0) root         (0)    10237 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/upload_content_screenshot_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.238808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_creator/
--rw-rw-r--   0 root         (0) root         (0)      569 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_creator/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7183 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_creator/public_get_creator.py
--rw-rw-r--   0 root         (0) root         (0)    10034 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_creator/public_search_creator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.238808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_legacy/
--rw-rw-r--   0 root         (0) root         (0)      514 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_legacy/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7385 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_legacy/add_download_count.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.238808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/
--rw-rw-r--   0 root         (0) root         (0)      606 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7744 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/public_add_download_count_v2.py
--rw-rw-r--   0 root         (0) root         (0)    11051 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/public_list_content_dow_d23b3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.238808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_follow/
--rw-rw-r--   0 root         (0) root         (0)      735 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_follow/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8462 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_followed_content.py
--rw-rw-r--   0 root         (0) root         (0)     8180 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_followed_users.py
--rw-rw-r--   0 root         (0) root         (0)     8923 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_public_followers.py
--rw-rw-r--   0 root         (0) root         (0)     8923 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_public_following.py
--rw-rw-r--   0 root         (0) root         (0)     8330 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_follow/update_user_follow_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.242808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/
--rw-rw-r--   0 root         (0) root         (0)      759 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8314 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/create_group.py
--rw-rw-r--   0 root         (0) root         (0)     7745 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/delete_group.py
--rw-rw-r--   0 root         (0) root         (0)     7883 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/get_group.py
--rw-rw-r--   0 root         (0) root         (0)    10383 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/get_group_content.py
--rw-rw-r--   0 root         (0) root         (0)     8857 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/get_groups.py
--rw-rw-r--   0 root         (0) root         (0)    10599 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/public_get_group_contents_v2.py
--rw-rw-r--   0 root         (0) root         (0)     9381 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/update_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.242808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/
--rw-rw-r--   0 root         (0) root         (0)      576 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14636 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/get_liked_content.py
--rw-rw-r--   0 root         (0) root         (0)     9295 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/update_content_like_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.242808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/
--rw-rw-r--   0 root         (0) root         (0)      599 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9951 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/public_list_content_like_v2.py
--rw-rw-r--   0 root         (0) root         (0)     9458 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/update_content_like_status_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.242808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/
--rw-rw-r--   0 root         (0) root         (0)      729 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8271 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/delete_user_staging_con_254bae.py
--rw-rw-r--   0 root         (0) root         (0)     8504 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/get_user_staging_content_by_id.py
--rw-rw-r--   0 root         (0) root         (0)    11071 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/list_user_staging_contents.py
--rw-rw-r--   0 root         (0) root         (0)    10053 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/update_staging_content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.242808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_tag/
--rw-rw-r--   0 root         (0) root         (0)      493 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_tag/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7898 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_tag/get_tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.242808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_type/
--rw-rw-r--   0 root         (0) root         (0)      495 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_type/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7914 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_type/get_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.246808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/
--rw-rw-r--   0 root         (0) root         (0)    19490 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    24014 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_channel.py
--rw-rw-r--   0 root         (0) root         (0)     7790 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_config.py
--rw-rw-r--   0 root         (0) root         (0)   109090 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_content.py
--rw-rw-r--   0 root         (0) root         (0)    99701 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_content_v2.py
--rw-rw-r--   0 root         (0) root         (0)    46273 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_group.py
--rw-rw-r--   0 root         (0) root         (0)    16655 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_staging_content.py
--rw-rw-r--   0 root         (0) root         (0)    13331 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_tag.py
--rw-rw-r--   0 root         (0) root         (0)    13498 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_type.py
--rw-rw-r--   0 root         (0) root         (0)    25221 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_anonymization.py
--rw-rw-r--   0 root         (0) root         (0)    14678 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_channel.py
--rw-rw-r--   0 root         (0) root         (0)    85702 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_content_legacy.py
--rw-rw-r--   0 root         (0) root         (0)    76348 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_content_v2.py
--rw-rw-r--   0 root         (0) root         (0)     7874 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_creator.py
--rw-rw-r--   0 root         (0) root         (0)     4137 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_download_count_legacy.py
--rw-rw-r--   0 root         (0) root         (0)     8625 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_download_count_v2.py
--rw-rw-r--   0 root         (0) root         (0)    16831 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_follow.py
--rw-rw-r--   0 root         (0) root         (0)    25897 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_group.py
--rw-rw-r--   0 root         (0) root         (0)    11025 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_like_legacy.py
--rw-rw-r--   0 root         (0) root         (0)     8979 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_like_v2.py
--rw-rw-r--   0 root         (0) root         (0)    16698 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_staging_content.py
--rw-rw-r--   0 root         (0) root         (0)     3900 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_tag.py
--rw-rw-r--   0 root         (0) root         (0)     3925 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:43:03.246808 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk_service_ugc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1109 2024-02-27 05:43:03.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk_service_ugc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20884 2024-02-27 05:43:03.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk_service_ugc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 05:43:03.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk_service_ugc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-27 05:43:03.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk_service_ugc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-27 05:43:03.000000 accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk_service_ugc.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      351 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-ugc-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 05:43:03.246808 accelbyte-py-sdk-service-ugc-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.671698 accelbyte-py-sdk-service-ugc-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-03-13 06:15:13.671698 accelbyte-py-sdk-service-ugc-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      865 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.643698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.643698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.647698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/
+-rw-rw-r--   0 root         (0) root         (0)    17282 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.651698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/
+-rw-rw-r--   0 root         (0) root         (0)     6729 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3924 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_add_download_count_response.py
+-rw-rw-r--   0 root         (0) root         (0)     9294 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_admin_content_request_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     4035 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_admin_get_content_bulk_request.py
+-rw-rw-r--   0 root         (0) root         (0)    12487 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_admin_update_content_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7818 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_admin_update_content_request_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     4592 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_approve_staging_content_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4300 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_channel_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6456 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_channel_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4944 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_config_response.py
+-rw-rw-r--   0 root         (0) root         (0)    23046 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_download_response.py
+-rw-rw-r--   0 root         (0) root         (0)    20806 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_download_response_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     6141 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_downloader_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3889 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_like_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4596 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_like_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5944 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_likers_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8445 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_request_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     5029 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_snapshot.py
+-rw-rw-r--   0 root         (0) root         (0)     6088 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_version_response.py
+-rw-rw-r--   0 root         (0) root         (0)     9251 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_content_request.py
+-rw-rw-r--   0 root         (0) root         (0)    11023 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_content_request_s3.py
+-rw-rw-r--   0 root         (0) root         (0)    20160 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_content_response.py
+-rw-rw-r--   0 root         (0) root         (0)    18653 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_content_response_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     4462 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_group_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7856 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_group_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4467 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_screenshot_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6114 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_screenshot_request_item.py
+-rw-rw-r--   0 root         (0) root         (0)     4404 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_screenshot_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3703 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_tag_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4935 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_tag_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4441 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_type_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6512 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_type_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4398 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_creator_follow_state.py
+-rw-rw-r--   0 root         (0) root         (0)     7686 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_creator_overview_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8815 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_creator_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4975 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_generate_content_upload_url_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6321 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_generate_content_upload_url_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4128 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_get_content_bulk_by_share_codes_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4940 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_get_content_preview_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3849 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_hide_content_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4258 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_like_state.py
+-rw-rw-r--   0 root         (0) root         (0)     4327 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_list_content_versions_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5331 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_download_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5371 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_download_response_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     5369 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_downloader_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5293 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_likers_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5331 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_creator_overview_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5151 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_channel_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5144 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_configs_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5142 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_tag_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5161 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_type_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5143 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_group_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5361 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_list_staging_content_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5475 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paging_cursor.py
+-rw-rw-r--   0 root         (0) root         (0)     4206 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_payload_url.py
+-rw-rw-r--   0 root         (0) root         (0)     4975 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_preview_metadata.py
+-rw-rw-r--   0 root         (0) root         (0)     4323 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_preview_url.py
+-rw-rw-r--   0 root         (0) root         (0)     3767 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_public_channel_request.py
+-rw-rw-r--   0 root         (0) root         (0)    10388 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_public_create_content_request_s3.py
+-rw-rw-r--   0 root         (0) root         (0)     4046 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_public_get_content_bulk_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7395 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_screenshot_response.py
+-rw-rw-r--   0 root         (0) root         (0)    15478 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_staging_content_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3767 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_channel_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3776 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)    11628 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_content_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6987 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_content_request_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    18653 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_content_response_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     3980 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_content_share_code_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4838 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_file_location_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4615 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_screenshot.py
+-rw-rw-r--   0 root         (0) root         (0)     4341 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_screenshot_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4352 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_screenshot_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4862 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_staging_content_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3918 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_user_follow_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4564 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_user_follow_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4431 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/response_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.651698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/
+-rw-rw-r--   0 root         (0) root         (0)      432 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.651698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/
+-rw-rw-r--   0 root         (0) root         (0)      863 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7614 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_create_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     7686 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_delete_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     9467 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_get_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     9239 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_update_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     6949 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/single_admin_delete_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     8021 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/single_admin_get_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     8467 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/single_admin_update_channel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.655698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_config/
+-rw-rw-r--   0 root         (0) root         (0)      563 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8192 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_config/admin_get_configs.py
+-rw-rw-r--   0 root         (0) root         (0)     8237 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_config/admin_update_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.655698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/
+-rw-rw-r--   0 root         (0) root         (0)     2083 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8853 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_delete_content.py
+-rw-rw-r--   0 root         (0) root         (0)     8623 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_delete_content_sc_eeb785.py
+-rw-rw-r--   0 root         (0) root         (0)     7463 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_download_content_preview.py
+-rw-rw-r--   0 root         (0) root         (0)     9169 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_content.py
+-rw-rw-r--   0 root         (0) root         (0)     8183 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_content_bulk.py
+-rw-rw-r--   0 root         (0) root         (0)     8369 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_content_bulk__102504.py
+-rw-rw-r--   0 root         (0) root         (0)     7502 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_specific_content.py
+-rw-rw-r--   0 root         (0) root         (0)     7505 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_user_content__d4dc92.py
+-rw-rw-r--   0 root         (0) root         (0)     9919 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_hide_user_content.py
+-rw-rw-r--   0 root         (0) root         (0)    18427 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_search_channel_sp_40f87c.py
+-rw-rw-r--   0 root         (0) root         (0)    17222 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_search_content.py
+-rw-rw-r--   0 root         (0) root         (0)    10954 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_content_direct.py
+-rw-rw-r--   0 root         (0) root         (0)    11720 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_content_s3.py
+-rw-rw-r--   0 root         (0) root         (0)    12033 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_content_s3_bb64ed.py
+-rw-rw-r--   0 root         (0) root         (0)     8956 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_screenshots.py
+-rw-rw-r--   0 root         (0) root         (0)     9421 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_upload_content_direct.py
+-rw-rw-r--   0 root         (0) root         (0)    10067 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_upload_content_s3.py
+-rw-rw-r--   0 root         (0) root         (0)     9505 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_upload_content_sc_b38ae0.py
+-rw-rw-r--   0 root         (0) root         (0)     8963 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/delete_content_by_share_code.py
+-rw-rw-r--   0 root         (0) root         (0)     7498 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/list_content_versions.py
+-rw-rw-r--   0 root         (0) root         (0)     8816 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/rollback_content_version.py
+-rw-rw-r--   0 root         (0) root         (0)     8150 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_delete_content.py
+-rw-rw-r--   0 root         (0) root         (0)     8445 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_get_content.py
+-rw-rw-r--   0 root         (0) root         (0)    10105 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_update_con_1f2ab1.py
+-rw-rw-r--   0 root         (0) root         (0)    11175 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_update_content_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.659698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/
+-rw-rw-r--   0 root         (0) root         (0)     2190 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8224 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_bulk_get_content__b85ce3.py
+-rw-rw-r--   0 root         (0) root         (0)     9447 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_create_content_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     8847 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_content_by_cd2201.py
+-rw-rw-r--   0 root         (0) root         (0)     8630 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_content_sc_bf1900.py
+-rw-rw-r--   0 root         (0) root         (0)     8063 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_official_c_0e2f56.py
+-rw-rw-r--   0 root         (0) root         (0)     8775 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_user_content_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    10032 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_generate_official_791850.py
+-rw-rw-r--   0 root         (0) root         (0)    10770 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_generate_user_con_cdad13.py
+-rw-rw-r--   0 root         (0) root         (0)     8230 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_bulk__b58c74.py
+-rw-rw-r--   0 root         (0) root         (0)    10671 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_ch_c1fd57.py
+-rw-rw-r--   0 root         (0) root         (0)     7527 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_co_c26e1e.py
+-rw-rw-r--   0 root         (0) root         (0)     7546 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_sh_03305f.py
+-rw-rw-r--   0 root         (0) root         (0)    10042 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_user_idv2.py
+-rw-rw-r--   0 root         (0) root         (0)    13867 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_list_content_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    11166 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_content_by_e139ff.py
+-rw-rw-r--   0 root         (0) root         (0)     9975 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_content_hi_72a875.py
+-rw-rw-r--   0 root         (0) root         (0)    10151 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_official_c_348c5f.py
+-rw-rw-r--   0 root         (0) root         (0)    10004 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_official_c_e7d890.py
+-rw-rw-r--   0 root         (0) root         (0)     9139 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_screenshots_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    10915 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_user_conte_8a8bc8.py
+-rw-rw-r--   0 root         (0) root         (0)    10715 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_user_content_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     9384 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_upload_content_sc_3461bc.py
+-rw-rw-r--   0 root         (0) root         (0)     7337 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/list_content_versions_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     8650 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/rollback_content_version_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.659698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/
+-rw-rw-r--   0 root         (0) root         (0)     1232 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7385 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_create_group.py
+-rw-rw-r--   0 root         (0) root         (0)     7573 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_delete_group.py
+-rw-rw-r--   0 root         (0) root         (0)     8731 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_all_groups.py
+-rw-rw-r--   0 root         (0) root         (0)     7762 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_group.py
+-rw-rw-r--   0 root         (0) root         (0)    10244 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_group_contents.py
+-rw-rw-r--   0 root         (0) root         (0)     9676 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_official_grou_23b467.py
+-rw-rw-r--   0 root         (0) root         (0)    10438 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_user_group_co_73e55d.py
+-rw-rw-r--   0 root         (0) root         (0)     9198 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_update_group.py
+-rw-rw-r--   0 root         (0) root         (0)     6848 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_delete_group.py
+-rw-rw-r--   0 root         (0) root         (0)     8003 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_get_all_groups.py
+-rw-rw-r--   0 root         (0) root         (0)     7018 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_get_group.py
+-rw-rw-r--   0 root         (0) root         (0)     9506 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_get_group__c6800e.py
+-rw-rw-r--   0 root         (0) root         (0)     8440 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_update_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.659698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/
+-rw-rw-r--   0 root         (0) root         (0)      745 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9214 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_approve_staging_content.py
+-rw-rw-r--   0 root         (0) root         (0)     7542 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_get_staging_conte_7fe68e.py
+-rw-rw-r--   0 root         (0) root         (0)    10120 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_list_staging_contents.py
+-rw-rw-r--   0 root         (0) root         (0)    10945 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_list_user_staging_d2fe4e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.659698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/
+-rw-rw-r--   0 root         (0) root         (0)      639 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7591 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_create_tag.py
+-rw-rw-r--   0 root         (0) root         (0)     6724 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_delete_tag.py
+-rw-rw-r--   0 root         (0) root         (0)     7887 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_get_tag.py
+-rw-rw-r--   0 root         (0) root         (0)     8498 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_update_tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.659698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_type/
+-rw-rw-r--   0 root         (0) root         (0)      647 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_type/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7631 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_create_type.py
+-rw-rw-r--   0 root         (0) root         (0)     6766 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_delete_type.py
+-rw-rw-r--   0 root         (0) root         (0)     7894 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_get_type.py
+-rw-rw-r--   0 root         (0) root         (0)     8564 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_update_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.659698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/
+-rw-rw-r--   0 root         (0) root         (0)      967 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6904 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_channels.py
+-rw-rw-r--   0 root         (0) root         (0)     7086 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_contents.py
+-rw-rw-r--   0 root         (0) root         (0)     6870 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_group.py
+-rw-rw-r--   0 root         (0) root         (0)     7189 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_states.py
+-rw-rw-r--   0 root         (0) root         (0)     6912 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     7142 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_contents.py
+-rw-rw-r--   0 root         (0) root         (0)     6898 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_group.py
+-rw-rw-r--   0 root         (0) root         (0)     7210 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_states.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.663698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_channel/
+-rw-rw-r--   0 root         (0) root         (0)      642 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_channel/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7710 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_channel/delete_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     9524 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_channel/get_channels.py
+-rw-rw-r--   0 root         (0) root         (0)     8200 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_channel/public_create_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     9258 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_channel/update_channel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.663698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/
+-rw-rw-r--   0 root         (0) root         (0)     1647 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10012 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/create_content_direct.py
+-rw-rw-r--   0 root         (0) root         (0)    10670 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/create_content_s3.py
+-rw-rw-r--   0 root         (0) root         (0)     8869 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/delete_content.py
+-rw-rw-r--   0 root         (0) root         (0)     9422 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/delete_content_screenshot.py
+-rw-rw-r--   0 root         (0) root         (0)     9041 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_delete_content_b_e67ae8.py
+-rw-rw-r--   0 root         (0) root         (0)     7511 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_download_content_2d5c80.py
+-rw-rw-r--   0 root         (0) root         (0)     7404 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_download_content_32df1f.py
+-rw-rw-r--   0 root         (0) root         (0)     7550 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_download_content_511956.py
+-rw-rw-r--   0 root         (0) root         (0)     7953 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_get_content_bulk.py
+-rw-rw-r--   0 root         (0) root         (0)     8293 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_get_content_bulk_382fb9.py
+-rw-rw-r--   0 root         (0) root         (0)     9325 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_get_user_content.py
+-rw-rw-r--   0 root         (0) root         (0)    17221 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_search_content.py
+-rw-rw-r--   0 root         (0) root         (0)    11873 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_update_content_b_7f10f2.py
+-rw-rw-r--   0 root         (0) root         (0)    18243 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/search_channel_specific_10d5e8.py
+-rw-rw-r--   0 root         (0) root         (0)    10813 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_content_direct.py
+-rw-rw-r--   0 root         (0) root         (0)    11521 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_content_s3.py
+-rw-rw-r--   0 root         (0) root         (0)    11357 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_content_share_code.py
+-rw-rw-r--   0 root         (0) root         (0)     9757 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_screenshots.py
+-rw-rw-r--   0 root         (0) root         (0)    10301 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/upload_content_screenshot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.663698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/
+-rw-rw-r--   0 root         (0) root         (0)     1698 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9574 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/delete_content_screenshot_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     7993 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_bulk_get_content_a86be5.py
+-rw-rw-r--   0 root         (0) root         (0)     9815 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_create_content_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     8923 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_delete_content_b_4792d8.py
+-rw-rw-r--   0 root         (0) root         (0)     8785 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_delete_content_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    11049 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_generate_content_ffec28.py
+-rw-rw-r--   0 root         (0) root         (0)     8325 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_bulk_503347.py
+-rw-rw-r--   0 root         (0) root         (0)    10789 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_c_87966e.py
+-rw-rw-r--   0 root         (0) root         (0)     7610 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_idv2.py
+-rw-rw-r--   0 root         (0) root         (0)     7497 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_s_4f7083.py
+-rw-rw-r--   0 root         (0) root         (0)    10295 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_u_635e0b.py
+-rw-rw-r--   0 root         (0) root         (0)    13943 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_list_content_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    10993 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_update_content_b_0c4d9c.py
+-rw-rw-r--   0 root         (0) root         (0)    11169 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_update_content_f_55e48b.py
+-rw-rw-r--   0 root         (0) root         (0)    10577 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_update_content_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    11407 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/update_content_share_code_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     9767 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/update_screenshots_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     9959 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/upload_content_screenshot_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.667698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_creator/
+-rw-rw-r--   0 root         (0) root         (0)      569 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_creator/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7183 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_creator/public_get_creator.py
+-rw-rw-r--   0 root         (0) root         (0)    10034 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_creator/public_search_creator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.667698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_legacy/
+-rw-rw-r--   0 root         (0) root         (0)      514 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_legacy/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7422 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_legacy/add_download_count.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.667698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/
+-rw-rw-r--   0 root         (0) root         (0)      606 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7781 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/public_add_download_count_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    11051 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/public_list_content_dow_d23b3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.667698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_follow/
+-rw-rw-r--   0 root         (0) root         (0)      735 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_follow/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8462 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_followed_content.py
+-rw-rw-r--   0 root         (0) root         (0)     8180 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_followed_users.py
+-rw-rw-r--   0 root         (0) root         (0)     8923 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_public_followers.py
+-rw-rw-r--   0 root         (0) root         (0)     8923 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_public_following.py
+-rw-rw-r--   0 root         (0) root         (0)     8330 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_follow/update_user_follow_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.667698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/
+-rw-rw-r--   0 root         (0) root         (0)      759 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8152 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/create_group.py
+-rw-rw-r--   0 root         (0) root         (0)     7600 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/delete_group.py
+-rw-rw-r--   0 root         (0) root         (0)     7739 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/get_group.py
+-rw-rw-r--   0 root         (0) root         (0)    10256 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/get_group_content.py
+-rw-rw-r--   0 root         (0) root         (0)     8711 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/get_groups.py
+-rw-rw-r--   0 root         (0) root         (0)    10467 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/public_get_group_contents_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     9202 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/update_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.667698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/
+-rw-rw-r--   0 root         (0) root         (0)      576 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14594 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/get_liked_content.py
+-rw-rw-r--   0 root         (0) root         (0)     9328 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/update_content_like_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.667698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/
+-rw-rw-r--   0 root         (0) root         (0)      599 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9951 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/public_list_content_like_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     9491 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/update_content_like_status_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.667698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/
+-rw-rw-r--   0 root         (0) root         (0)      729 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8139 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/delete_user_staging_con_254bae.py
+-rw-rw-r--   0 root         (0) root         (0)     8373 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/get_user_staging_content_by_id.py
+-rw-rw-r--   0 root         (0) root         (0)    10936 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/list_user_staging_contents.py
+-rw-rw-r--   0 root         (0) root         (0)     9910 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/update_staging_content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.667698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_tag/
+-rw-rw-r--   0 root         (0) root         (0)      493 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_tag/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7907 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_tag/get_tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.667698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_type/
+-rw-rw-r--   0 root         (0) root         (0)      495 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_type/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7918 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_type/get_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.671698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)    19490 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    21892 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     7252 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_config.py
+-rw-rw-r--   0 root         (0) root         (0)   108146 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_content.py
+-rw-rw-r--   0 root         (0) root         (0)    91903 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_content_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    42077 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_group.py
+-rw-rw-r--   0 root         (0) root         (0)    15741 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_staging_content.py
+-rw-rw-r--   0 root         (0) root         (0)    12209 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_tag.py
+-rw-rw-r--   0 root         (0) root         (0)    12366 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_type.py
+-rw-rw-r--   0 root         (0) root         (0)    23997 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_anonymization.py
+-rw-rw-r--   0 root         (0) root         (0)    13540 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_channel.py
+-rw-rw-r--   0 root         (0) root         (0)    84812 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_content_legacy.py
+-rw-rw-r--   0 root         (0) root         (0)    72786 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_content_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     7874 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_creator.py
+-rw-rw-r--   0 root         (0) root         (0)     4211 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_download_count_legacy.py
+-rw-rw-r--   0 root         (0) root         (0)     8699 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_download_count_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    16831 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_follow.py
+-rw-rw-r--   0 root         (0) root         (0)    23827 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_group.py
+-rw-rw-r--   0 root         (0) root         (0)    11007 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_like_legacy.py
+-rw-rw-r--   0 root         (0) root         (0)     9045 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_like_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    15616 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_staging_content.py
+-rw-rw-r--   0 root         (0) root         (0)     3918 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_tag.py
+-rw-rw-r--   0 root         (0) root         (0)     3933 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:13.671698 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk_service_ugc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-03-13 06:15:13.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk_service_ugc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20884 2024-03-13 06:15:13.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk_service_ugc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 06:15:13.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk_service_ugc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 06:15:13.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk_service_ugc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-13 06:15:13.000000 accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk_service_ugc.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      351 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-ugc-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 06:15:13.671698 accelbyte-py-sdk-service-ugc-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/PKG-INFO` & `accelbyte-py-sdk-service-ugc-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-ugc
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Ugc Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Ugc Service
-* Version: 2.19.6
+* Version: 2.19.7
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/README.md` & `accelbyte-py-sdk-service-ugc-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Ugc Service
-* Version: 2.19.6
+* Version: 2.19.7
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # admin_channel
 from .wrappers import admin_create_channel
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .models_add_download_count_response import ModelsAddDownloadCountResponse
 from .models_admin_content_request_v2 import ModelsAdminContentRequestV2
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_add_download_count_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_add_download_count_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_admin_content_request_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_admin_content_request_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_admin_get_content_bulk_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_admin_get_content_bulk_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_admin_update_content_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_admin_update_content_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_admin_update_content_request_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_admin_update_content_request_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_approve_staging_content_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_approve_staging_content_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_channel_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_channel_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_channel_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_channel_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_config_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_config_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_download_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_download_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_download_response_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_download_response_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_downloader_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_downloader_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_like_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_like_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_like_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_like_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_likers_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_likers_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_request_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_request_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_snapshot.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_snapshot.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_content_version_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_content_version_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_content_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_content_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_content_request_s3.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_content_request_s3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_content_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_content_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_content_response_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_content_response_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_group_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_group_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_group_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_group_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_screenshot_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_screenshot_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_screenshot_request_item.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_screenshot_request_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,102 +38,103 @@
     PNG = "png"
 
 
 class ModelsCreateScreenshotRequestItem(Model):
     """Models create screenshot request item (models.createScreenshotRequestItem)
 
     Properties:
-        content_type: (contentType) REQUIRED str
-
         description: (description) REQUIRED str
 
         file_extension: (fileExtension) REQUIRED Union[str, FileExtensionEnum]
+
+        content_type: (contentType) OPTIONAL str
     """
 
     # region fields
 
-    content_type: str  # REQUIRED
     description: str  # REQUIRED
     file_extension: Union[str, FileExtensionEnum]  # REQUIRED
+    content_type: str  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
-    def with_content_type(self, value: str) -> ModelsCreateScreenshotRequestItem:
-        self.content_type = value
-        return self
-
     def with_description(self, value: str) -> ModelsCreateScreenshotRequestItem:
         self.description = value
         return self
 
     def with_file_extension(
         self, value: Union[str, FileExtensionEnum]
     ) -> ModelsCreateScreenshotRequestItem:
         self.file_extension = value
         return self
 
+    def with_content_type(self, value: str) -> ModelsCreateScreenshotRequestItem:
+        self.content_type = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "content_type"):
-            result["contentType"] = str(self.content_type)
-        elif include_empty:
-            result["contentType"] = ""
         if hasattr(self, "description"):
             result["description"] = str(self.description)
         elif include_empty:
             result["description"] = ""
         if hasattr(self, "file_extension"):
             result["fileExtension"] = str(self.file_extension)
         elif include_empty:
             result["fileExtension"] = Union[str, FileExtensionEnum]()
+        if hasattr(self, "content_type"):
+            result["contentType"] = str(self.content_type)
+        elif include_empty:
+            result["contentType"] = ""
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        content_type: str,
         description: str,
         file_extension: Union[str, FileExtensionEnum],
+        content_type: Optional[str] = None,
         **kwargs,
     ) -> ModelsCreateScreenshotRequestItem:
         instance = cls()
-        instance.content_type = content_type
         instance.description = description
         instance.file_extension = file_extension
+        if content_type is not None:
+            instance.content_type = content_type
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsCreateScreenshotRequestItem:
         instance = cls()
         if not dict_:
             return instance
-        if "contentType" in dict_ and dict_["contentType"] is not None:
-            instance.content_type = str(dict_["contentType"])
-        elif include_empty:
-            instance.content_type = ""
         if "description" in dict_ and dict_["description"] is not None:
             instance.description = str(dict_["description"])
         elif include_empty:
             instance.description = ""
         if "fileExtension" in dict_ and dict_["fileExtension"] is not None:
             instance.file_extension = str(dict_["fileExtension"])
         elif include_empty:
             instance.file_extension = Union[str, FileExtensionEnum]()
+        if "contentType" in dict_ and dict_["contentType"] is not None:
+            instance.content_type = str(dict_["contentType"])
+        elif include_empty:
+            instance.content_type = ""
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsCreateScreenshotRequestItem]:
         return (
@@ -169,25 +170,25 @@
                 raise ValueError()
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "contentType": "content_type",
             "description": "description",
             "fileExtension": "file_extension",
+            "contentType": "content_type",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "contentType": True,
             "description": True,
             "fileExtension": True,
+            "contentType": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "fileExtension": ["bmp", "jfif", "jpeg", "jpg", "pjp", "png"],
         }
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_screenshot_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_screenshot_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_tag_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_tag_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_tag_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_tag_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_type_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_type_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_create_type_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_create_type_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_creator_follow_state.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_creator_follow_state.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_creator_overview_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_creator_overview_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_creator_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_creator_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_generate_content_upload_url_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_generate_content_upload_url_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_generate_content_upload_url_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_generate_content_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_get_content_bulk_by_share_codes_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_get_content_bulk_by_share_codes_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_get_content_preview_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_get_content_preview_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_hide_content_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_hide_content_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_like_state.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_like_state.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_list_content_versions_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_list_content_versions_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_download_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_download_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_download_response_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_download_response_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_downloader_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_downloader_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_likers_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_content_likers_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_creator_overview_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_creator_overview_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_channel_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_channel_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_configs_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_configs_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_tag_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_tag_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_type_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_get_type_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_group_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_group_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paginated_list_staging_content_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paginated_list_staging_content_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_paging_cursor.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_paging_cursor.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_payload_url.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_payload_url.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_preview_metadata.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_preview_metadata.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_preview_url.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_preview_url.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_public_channel_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_public_channel_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_public_create_content_request_s3.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_public_create_content_request_s3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_public_get_content_bulk_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_public_get_content_bulk_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_screenshot_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_screenshot_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_staging_content_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_staging_content_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_channel_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_channel_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_config_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_content_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_content_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_content_request_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_content_request_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_content_response_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_content_response_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_content_share_code_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_content_share_code_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_file_location_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_file_location_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_screenshot.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_screenshot.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_screenshot_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_screenshot_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_screenshot_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_screenshot_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_update_staging_content_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_update_staging_content_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_user_follow_request.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_user_follow_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/models_user_follow_response.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/models_user_follow_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/models/response_error.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_channel import AdminCreateChannel
 from .admin_delete_channel import AdminDeleteChannel
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_create_channel.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_content_bulk.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,66 +25,67 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsChannelRequest
-from ...models import ModelsChannelResponse
+from ...models import ModelsAdminGetContentBulkRequest
+from ...models import ModelsContentDownloadResponse
 from ...models import ResponseError
 
 
-class AdminCreateChannel(Operation):
-    """Create Channel (AdminCreateChannel)
+class AdminGetContentBulk(Operation):
+    """Bulk get content by content IDs (AdminGetContentBulk)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [CREATE]
+    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
+    Maximum contentId per request 100
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [CREATE]
+        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/channels
+        url: /ugc/v1/admin/namespaces/{namespace}/contents/bulk
 
         method: POST
 
-        tags: ["Admin Channel"]
+        tags: ["Admin Content"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsChannelRequest in body
+        body: (body) REQUIRED ModelsAdminGetContentBulkRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        201: Created - ModelsChannelResponse (Channel created)
+        200: OK - List[ModelsContentDownloadResponse] (Bulk get content by content IDs)
 
-        400: Bad Request - ResponseError (770503: Invalid channel {ID}: should uuid without hypen)
+        400: Bad Request - ResponseError (773900: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        409: Conflict - ResponseError (770504: Channel already exist)
+        403: Forbidden - ResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ResponseError (770502: Unable to save channel)
+        500: Internal Server Error - ResponseError (773901: Unable to get ugc content: database/Unable to get creator | 773902: Failed generate download URL)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/admin/namespaces/{namespace}/channels"
+    _url: str = "/ugc/v1/admin/namespaces/{namespace}/contents/bulk"
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsChannelRequest  # REQUIRED in [body]
+    body: ModelsAdminGetContentBulkRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
@@ -140,114 +141,117 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsChannelRequest) -> AdminCreateChannel:
+    def with_body(self, value: ModelsAdminGetContentBulkRequest) -> AdminGetContentBulk:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> AdminCreateChannel:
+    def with_namespace(self, value: str) -> AdminGetContentBulk:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsChannelRequest()
+            result["body"] = ModelsAdminGetContentBulkRequest()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsChannelResponse], Union[None, HttpResponse, ResponseError]
+        Union[None, List[ModelsContentDownloadResponse]],
+        Union[None, HttpResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        201: Created - ModelsChannelResponse (Channel created)
+        200: OK - List[ModelsContentDownloadResponse] (Bulk get content by content IDs)
 
-        400: Bad Request - ResponseError (770503: Invalid channel {ID}: should uuid without hypen)
+        400: Bad Request - ResponseError (773900: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        409: Conflict - ResponseError (770504: Channel already exist)
+        403: Forbidden - ResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ResponseError (770502: Unable to save channel)
+        500: Internal Server Error - ResponseError (773901: Unable to get ugc content: database/Unable to get creator | 773902: Failed generate download URL)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 201:
-            return ModelsChannelResponse.create_from_dict(content), None
+        if code == 200:
+            return [
+                ModelsContentDownloadResponse.create_from_dict(i) for i in content
+            ], None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
-        if code == 409:
+        if code == 403:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, body: ModelsChannelRequest, namespace: str, **kwargs
-    ) -> AdminCreateChannel:
+        cls, body: ModelsAdminGetContentBulkRequest, namespace: str, **kwargs
+    ) -> AdminGetContentBulk:
         instance = cls()
         instance.body = body
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminCreateChannel:
+    ) -> AdminGetContentBulk:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsChannelRequest.create_from_dict(
+            instance.body = ModelsAdminGetContentBulkRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsChannelRequest()
+            instance.body = ModelsAdminGetContentBulkRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_delete_channel.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_delete_channel.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class AdminDeleteChannel(Operation):
     """Delete Channel (AdminDeleteChannel)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Delete user channel
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}
 
         method: DELETE
 
         tags: ["Admin Channel"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_get_channel.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_get_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedGetChannelResponse
 from ...models import ResponseError
 
 
 class AdminGetChannel(Operation):
     """Get Channels (AdminGetChannel)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
+    Get user channel paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels
 
         method: GET
 
         tags: ["Admin Channel"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_update_channel.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_channel/update_channel.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,30 +30,27 @@
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelsChannelResponse
 from ...models import ModelsUpdateChannelRequest
 from ...models import ResponseError
 
 
-class AdminUpdateChannel(Operation):
-    """Update Channel (AdminUpdateChannel)
+class UpdateChannel(Operation):
+    """Update Channel (UpdateChannel)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+    Update user channel
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}
 
         method: PUT
 
-        tags: ["Admin Channel"]
+        tags: ["Public Channel"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         body: (body) REQUIRED ModelsUpdateChannelRequest in body
 
@@ -74,18 +71,18 @@
 
         500: Internal Server Error - ResponseError (770602: Unable to save channel)
     """
 
     # region fields
 
     _url: str = (
-        "/ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}"
+        "/ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}"
     )
     _method: str = "PUT"
-    _consumes: List[str] = ["application/json"]
+    _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     body: ModelsUpdateChannelRequest  # REQUIRED in [body]
     channel_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
@@ -152,27 +149,27 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsUpdateChannelRequest) -> AdminUpdateChannel:
+    def with_body(self, value: ModelsUpdateChannelRequest) -> UpdateChannel:
         self.body = value
         return self
 
-    def with_channel_id(self, value: str) -> AdminUpdateChannel:
+    def with_channel_id(self, value: str) -> UpdateChannel:
         self.channel_id = value
         return self
 
-    def with_namespace(self, value: str) -> AdminUpdateChannel:
+    def with_namespace(self, value: str) -> UpdateChannel:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> AdminUpdateChannel:
+    def with_user_id(self, value: str) -> UpdateChannel:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -254,28 +251,28 @@
     def create(
         cls,
         body: ModelsUpdateChannelRequest,
         channel_id: str,
         namespace: str,
         user_id: str,
         **kwargs,
-    ) -> AdminUpdateChannel:
+    ) -> UpdateChannel:
         instance = cls()
         instance.body = body
         instance.channel_id = channel_id
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminUpdateChannel:
+    ) -> UpdateChannel:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
             instance.body = ModelsUpdateChannelRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
             instance.body = ModelsUpdateChannelRequest()
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/single_admin_delete_channel.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/single_admin_delete_channel.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class SingleAdminDeleteChannel(Operation):
     """Delete Channel (SingleAdminDeleteChannel)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Delete official channel
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/channels/{channelId}
 
         method: DELETE
 
         tags: ["Admin Channel"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/single_admin_get_channel.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/single_admin_get_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedGetChannelResponse
 from ...models import ResponseError
 
 
 class SingleAdminGetChannel(Operation):
     """Get Channels (SingleAdminGetChannel)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
+    Get official channel paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/channels
 
         method: GET
 
         tags: ["Admin Channel"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/single_admin_update_channel.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/single_admin_update_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsUpdateChannelRequest
 from ...models import ResponseError
 
 
 class SingleAdminUpdateChannel(Operation):
     """Update Channel (SingleAdminUpdateChannel)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+    Update official channel
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/channels/{channelId}
 
         method: PUT
 
         tags: ["Admin Channel"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_config/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_config/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_get_configs import AdminGetConfigs
 from .admin_update_config import AdminUpdateConfig
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_config/admin_get_configs.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_config/admin_get_configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedGetConfigsResponse
 from ...models import ResponseError
 
 
 class AdminGetConfigs(Operation):
     """Get configs (AdminGetConfigs)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
+    Get config paginated
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/configs
 
         method: GET
 
         tags: ["Admin Config"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_config/admin_update_config.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_config/admin_update_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,18 @@
 from ...models import ModelsUpdateConfigRequest
 from ...models import ResponseError
 
 
 class AdminUpdateConfig(Operation):
     """Update config (AdminUpdateConfig)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE].
-    It will create a new config if the key doesn't exist.
-    Allowed key value:
-    - contentReview : enabled , disabled
+    This endpoint will create a new config if the *key* doesn't exist.
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
+    Allowed key value:
+    - *contentReview*: *enabled*,*disabled*
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/configs/{key}
 
         method: PATCH
 
         tags: ["Admin Config"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_delete_content import AdminDeleteContent
 from .admin_delete_content_sc_eeb785 import AdminDeleteContentScreenshot
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_delete_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_delete_content.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_delete_content_sc_eeb785.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_content_sc_bf1900.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,28 +28,25 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class AdminDeleteContentScreenshot(Operation):
-    """Delete screenshots content (AdminDeleteContentScreenshot)
+class AdminDeleteContentScreenshotV2(Operation):
+    """Delete screenshots content (AdminDeleteContentScreenshotV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete screenshot from a content
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/contents/{contentId}/screenshots/{screenshotId}
+        url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/screenshots/{screenshotId}
 
         method: DELETE
 
-        tags: ["Admin Content"]
+        tags: ["Admin Content V2"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -71,15 +68,15 @@
         404: Not Found - ResponseError (772603: Content not found)
 
         500: Internal Server Error - ResponseError (772602: Unable to check user ban status/Unable to get updated ugc content)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/admin/namespaces/{namespace}/contents/{contentId}/screenshots/{screenshotId}"
+    _url: str = "/ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/screenshots/{screenshotId}"
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     content_id: str  # REQUIRED in [path]
@@ -141,23 +138,23 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_content_id(self, value: str) -> AdminDeleteContentScreenshot:
+    def with_content_id(self, value: str) -> AdminDeleteContentScreenshotV2:
         self.content_id = value
         return self
 
-    def with_namespace(self, value: str) -> AdminDeleteContentScreenshot:
+    def with_namespace(self, value: str) -> AdminDeleteContentScreenshotV2:
         self.namespace = value
         return self
 
-    def with_screenshot_id(self, value: str) -> AdminDeleteContentScreenshot:
+    def with_screenshot_id(self, value: str) -> AdminDeleteContentScreenshotV2:
         self.screenshot_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -232,27 +229,27 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, content_id: str, namespace: str, screenshot_id: str, **kwargs
-    ) -> AdminDeleteContentScreenshot:
+    ) -> AdminDeleteContentScreenshotV2:
         instance = cls()
         instance.content_id = content_id
         instance.namespace = namespace
         instance.screenshot_id = screenshot_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminDeleteContentScreenshot:
+    ) -> AdminDeleteContentScreenshotV2:
         instance = cls()
         if "contentId" in dict_ and dict_["contentId"] is not None:
             instance.content_id = str(dict_["contentId"])
         elif include_empty:
             instance.content_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_download_content_preview.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_download_content_preview.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_content.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_content_bulk.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_bulk_get_content__b85ce3.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,59 +26,55 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelsAdminGetContentBulkRequest
-from ...models import ModelsContentDownloadResponse
+from ...models import ModelsContentDownloadResponseV2
 from ...models import ResponseError
 
 
-class AdminGetContentBulk(Operation):
-    """Bulk get content by content IDs (AdminGetContentBulk)
+class AdminBulkGetContentByIDsV2(Operation):
+    """Bulk get content by content IDs (AdminBulkGetContentByIDsV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
     Maximum contentId per request 100
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
-
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/contents/bulk
+        url: /ugc/v2/admin/namespaces/{namespace}/contents/bulk
 
         method: POST
 
-        tags: ["Admin Content"]
+        tags: ["Admin Content V2"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         body: (body) REQUIRED ModelsAdminGetContentBulkRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - List[ModelsContentDownloadResponse] (Bulk get content by content IDs)
+        200: OK - List[ModelsContentDownloadResponseV2] (Bulk get content by content IDs)
 
         400: Bad Request - ResponseError (773900: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
         403: Forbidden - ResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ResponseError (773901: Unable to get ugc content: database/Unable to get creator | 773902: Failed generate download URL)
+        500: Internal Server Error - ResponseError (773901: Unable to get ugc content: database/Unable to get creator | 770801: Unable to get ugc content: database/Unable to get creator | 773902: Failed generate download URL)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/admin/namespaces/{namespace}/contents/bulk"
+    _url: str = "/ugc/v2/admin/namespaces/{namespace}/contents/bulk"
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     body: ModelsAdminGetContentBulkRequest  # REQUIRED in [body]
@@ -141,19 +137,21 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsAdminGetContentBulkRequest) -> AdminGetContentBulk:
+    def with_body(
+        self, value: ModelsAdminGetContentBulkRequest
+    ) -> AdminBulkGetContentByIDsV2:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> AdminGetContentBulk:
+    def with_namespace(self, value: str) -> AdminBulkGetContentByIDsV2:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -173,28 +171,28 @@
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, List[ModelsContentDownloadResponse]],
+        Union[None, List[ModelsContentDownloadResponseV2]],
         Union[None, HttpResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - List[ModelsContentDownloadResponse] (Bulk get content by content IDs)
+        200: OK - List[ModelsContentDownloadResponseV2] (Bulk get content by content IDs)
 
         400: Bad Request - ResponseError (773900: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
         403: Forbidden - ResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ResponseError (773901: Unable to get ugc content: database/Unable to get creator | 773902: Failed generate download URL)
+        500: Internal Server Error - ResponseError (773901: Unable to get ugc content: database/Unable to get creator | 770801: Unable to get ugc content: database/Unable to get creator | 773902: Failed generate download URL)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -203,15 +201,15 @@
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
             return [
-                ModelsContentDownloadResponse.create_from_dict(i) for i in content
+                ModelsContentDownloadResponseV2.create_from_dict(i) for i in content
             ], None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 403:
             return None, ResponseError.create_from_dict(content)
@@ -225,26 +223,26 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, body: ModelsAdminGetContentBulkRequest, namespace: str, **kwargs
-    ) -> AdminGetContentBulk:
+    ) -> AdminBulkGetContentByIDsV2:
         instance = cls()
         instance.body = body
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminGetContentBulk:
+    ) -> AdminBulkGetContentByIDsV2:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
             instance.body = ModelsAdminGetContentBulkRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
             instance.body = ModelsAdminGetContentBulkRequest()
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_content_bulk__102504.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_content_bulk__102504.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_specific_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_specific_content.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_user_content__d4dc92.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_get_user_content__d4dc92.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_hide_user_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_hide_user_content.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_search_channel_sp_40f87c.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_search_channel_sp_40f87c.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_search_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_search_content.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_content_direct.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_content_direct.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_content_s3.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_content_s3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_content_s3_bb64ed.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_content_s3_bb64ed.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_screenshots.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_update_screenshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 from ...models import ModelsUpdateScreenshotResponse
 from ...models import ResponseError
 
 
 class AdminUpdateScreenshots(Operation):
     """Update screenshot of content (AdminUpdateScreenshots)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/contents/{contentId}/screenshots
 
         method: PUT
 
         tags: ["Admin Content"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_upload_content_direct.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_upload_content_direct.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_upload_content_s3.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_upload_content_s3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_upload_content_sc_b38ae0.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_upload_content_sc_b38ae0.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,25 +31,21 @@
 
 from ...models import ModelsCreateScreenshotRequest
 from ...models import ModelsCreateScreenshotResponse
 from ...models import ResponseError
 
 
 class AdminUploadContentScreenshot(Operation):
-    """Upload screenshots for content (AdminUploadContentScreenshot)
+    """Upload screenshots for official content (AdminUploadContentScreenshot)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-    All request body are required except for contentType field.
-    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the presigned URL.
-    If not specified, it will use fileExtension value.
-    Supported file extensions: pjp, jpg, jpeg, jfif, bmp, png.
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    All request body are required except for *contentType* field.
+    *contentType* values is used to enforce the *Content-Type* header needed by the client to upload the content using the presigned URL.
+    If not specified, it will use *fileExtension* value.
+    Supported file extensions: *pjp*, *jpg*, *jpeg*, *jfif*, *bmp*, *png*.
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/contents/{contentId}/screenshots
 
         method: POST
 
         tags: ["Admin Content"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/delete_content_by_share_code.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/delete_content_by_share_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/list_content_versions.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/list_content_versions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/rollback_content_version.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/rollback_content_version.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_delete_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_delete_content.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_get_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_get_content.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_update_con_1f2ab1.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_update_con_1f2ab1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_update_content_s3.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/single_admin_update_content_s3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_bulk_get_content__b85ce3 import AdminBulkGetContentByIDsV2
 from .admin_create_content_v2 import AdminCreateContentV2
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_bulk_get_content__b85ce3.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_bulk_get_content_a86be5.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,67 +25,62 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsAdminGetContentBulkRequest
 from ...models import ModelsContentDownloadResponseV2
+from ...models import ModelsPublicGetContentBulkRequest
 from ...models import ResponseError
 
 
-class AdminBulkGetContentByIDsV2(Operation):
-    """Bulk get content by content IDs (AdminBulkGetContentByIDsV2)
+class PublicBulkGetContentByIDV2(Operation):
+    """Get contents by content Ids  (PublicBulkGetContentByIDV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
-    Maximum contentId per request 100
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
+    Maximum requested Ids: 100.
+    Public user can access without token or if token specified, requires valid user token
 
     Properties:
-        url: /ugc/v2/admin/namespaces/{namespace}/contents/bulk
+        url: /ugc/v2/public/namespaces/{namespace}/contents/bulk
 
         method: POST
 
-        tags: ["Admin Content V2"]
+        tags: ["Public Content V2"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsAdminGetContentBulkRequest in body
+        body: (body) REQUIRED ModelsPublicGetContentBulkRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - List[ModelsContentDownloadResponseV2] (Bulk get content by content IDs)
+        200: OK - List[ModelsContentDownloadResponseV2] (Get contents by content Ids)
 
         400: Bad Request - ResponseError (773900: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        403: Forbidden - ResponseError (20013: insufficient permission)
-
-        500: Internal Server Error - ResponseError (773901: Unable to get ugc content: database/Unable to get creator | 770801: Unable to get ugc content: database/Unable to get creator | 773902: Failed generate download URL)
+        500: Internal Server Error - ResponseError (770801: Unable to get ugc content: database/Unable to get creator | 773902: Failed generate download URL)
     """
 
     # region fields
 
-    _url: str = "/ugc/v2/admin/namespaces/{namespace}/contents/bulk"
+    _url: str = "/ugc/v2/public/namespaces/{namespace}/contents/bulk"
     _method: str = "POST"
-    _consumes: List[str] = ["application/json"]
+    _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsAdminGetContentBulkRequest  # REQUIRED in [body]
+    body: ModelsPublicGetContentBulkRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
@@ -142,33 +137,33 @@
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
     def with_body(
-        self, value: ModelsAdminGetContentBulkRequest
-    ) -> AdminBulkGetContentByIDsV2:
+        self, value: ModelsPublicGetContentBulkRequest
+    ) -> PublicBulkGetContentByIDV2:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> AdminBulkGetContentByIDsV2:
+    def with_namespace(self, value: str) -> PublicBulkGetContentByIDV2:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsAdminGetContentBulkRequest()
+            result["body"] = ModelsPublicGetContentBulkRequest()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         return result
 
     # endregion to methods
@@ -180,23 +175,21 @@
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
         Union[None, List[ModelsContentDownloadResponseV2]],
         Union[None, HttpResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - List[ModelsContentDownloadResponseV2] (Bulk get content by content IDs)
+        200: OK - List[ModelsContentDownloadResponseV2] (Get contents by content Ids)
 
         400: Bad Request - ResponseError (773900: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        403: Forbidden - ResponseError (20013: insufficient permission)
-
-        500: Internal Server Error - ResponseError (773901: Unable to get ugc content: database/Unable to get creator | 770801: Unable to get ugc content: database/Unable to get creator | 773902: Failed generate download URL)
+        500: Internal Server Error - ResponseError (770801: Unable to get ugc content: database/Unable to get creator | 773902: Failed generate download URL)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -211,49 +204,47 @@
             return [
                 ModelsContentDownloadResponseV2.create_from_dict(i) for i in content
             ], None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
-        if code == 403:
-            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, body: ModelsAdminGetContentBulkRequest, namespace: str, **kwargs
-    ) -> AdminBulkGetContentByIDsV2:
+        cls, body: ModelsPublicGetContentBulkRequest, namespace: str, **kwargs
+    ) -> PublicBulkGetContentByIDV2:
         instance = cls()
         instance.body = body
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminBulkGetContentByIDsV2:
+    ) -> PublicBulkGetContentByIDV2:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsAdminGetContentBulkRequest.create_from_dict(
+            instance.body = ModelsPublicGetContentBulkRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsAdminGetContentBulkRequest()
+            instance.body = ModelsPublicGetContentBulkRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_create_content_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_create_content_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsCreateContentResponseV2
 from ...models import ResponseError
 
 
 class AdminCreateContentV2(Operation):
     """Create a content (AdminCreateContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    Create official content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents
 
         method: POST
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_content_by_cd2201.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_content_by_cd2201.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class AdminDeleteContentByShareCodeV2(Operation):
     """Delete content by share code (AdminDeleteContentByShareCodeV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete content by share code
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/sharecodes/{shareCode}
 
         method: DELETE
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_content_sc_bf1900.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content/admin_delete_content_sc_eeb785.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,28 +28,25 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class AdminDeleteContentScreenshotV2(Operation):
-    """Delete screenshots content (AdminDeleteContentScreenshotV2)
+class AdminDeleteContentScreenshot(Operation):
+    """Delete content's screenshot (AdminDeleteContentScreenshot)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing screenshot from a content
 
     Properties:
-        url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/screenshots/{screenshotId}
+        url: /ugc/v1/admin/namespaces/{namespace}/contents/{contentId}/screenshots/{screenshotId}
 
         method: DELETE
 
-        tags: ["Admin Content V2"]
+        tags: ["Admin Content"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -71,15 +68,15 @@
         404: Not Found - ResponseError (772603: Content not found)
 
         500: Internal Server Error - ResponseError (772602: Unable to check user ban status/Unable to get updated ugc content)
     """
 
     # region fields
 
-    _url: str = "/ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/screenshots/{screenshotId}"
+    _url: str = "/ugc/v1/admin/namespaces/{namespace}/contents/{contentId}/screenshots/{screenshotId}"
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     content_id: str  # REQUIRED in [path]
@@ -141,23 +138,23 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_content_id(self, value: str) -> AdminDeleteContentScreenshotV2:
+    def with_content_id(self, value: str) -> AdminDeleteContentScreenshot:
         self.content_id = value
         return self
 
-    def with_namespace(self, value: str) -> AdminDeleteContentScreenshotV2:
+    def with_namespace(self, value: str) -> AdminDeleteContentScreenshot:
         self.namespace = value
         return self
 
-    def with_screenshot_id(self, value: str) -> AdminDeleteContentScreenshotV2:
+    def with_screenshot_id(self, value: str) -> AdminDeleteContentScreenshot:
         self.screenshot_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -232,27 +229,27 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, content_id: str, namespace: str, screenshot_id: str, **kwargs
-    ) -> AdminDeleteContentScreenshotV2:
+    ) -> AdminDeleteContentScreenshot:
         instance = cls()
         instance.content_id = content_id
         instance.namespace = namespace
         instance.screenshot_id = screenshot_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminDeleteContentScreenshotV2:
+    ) -> AdminDeleteContentScreenshot:
         instance = cls()
         if "contentId" in dict_ and dict_["contentId"] is not None:
             instance.content_id = str(dict_["contentId"])
         elif include_empty:
             instance.content_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_official_c_0e2f56.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_official_c_0e2f56.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class AdminDeleteOfficialContentV2(Operation):
     """Delete official content (AdminDeleteOfficialContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing official content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents/{contentId}
 
         method: DELETE
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_user_content_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_delete_user_content_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class AdminDeleteUserContentV2(Operation):
     """Delete user content (AdminDeleteUserContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete user content by content ID
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}
 
         method: DELETE
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_generate_official_791850.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_generate_official_791850.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsGenerateContentUploadURLResponse
 from ...models import ResponseError
 
 
 class AdminGenerateOfficialContentUploadURLV2(Operation):
     """Generate official content upload URL (AdminGenerateOfficialContentUploadURLV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Generate official content upload URL
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents/{contentId}/uploadUrl
 
         method: PATCH
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_generate_user_con_cdad13.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_generate_user_con_cdad13.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsGenerateContentUploadURLResponse
 from ...models import ResponseError
 
 
 class AdminGenerateUserContentUploadURLV2(Operation):
     """Generate user content upload URL (AdminGenerateUserContentUploadURLV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    generate user content upload URL
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/uploadUrl
 
         method: PATCH
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_bulk__b58c74.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_bulk__b58c74.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,20 +33,16 @@
 from ...models import ModelsGetContentBulkByShareCodesRequest
 from ...models import ResponseError
 
 
 class AdminGetContentBulkByShareCodesV2(Operation):
     """Bulk get content by content sharecodes (AdminGetContentBulkByShareCodesV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
     Maximum sharecodes per request 100
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
-
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/sharecodes/bulk
 
         method: POST
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_ch_c1fd57.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_ch_c1fd57.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedContentDownloadResponseV2
 from ...models import ResponseError
 
 
 class AdminGetContentByChannelIDV2(Operation):
     """List contents specific to a channel (AdminGetContentByChannelIDV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    List content specific to a channel
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents
 
         method: GET
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_co_c26e1e.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_co_c26e1e.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsContentDownloadResponseV2
 from ...models import ResponseError
 
 
 class AdminGetContentByContentIDV2(Operation):
     """Get content by content ID (AdminGetContentByContentIDV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
+    Get content by content ID
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}
 
         method: GET
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_sh_03305f.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_sh_03305f.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsContentDownloadResponseV2
 from ...models import ResponseError
 
 
 class AdminGetContentByShareCodeV2(Operation):
     """Get content by sharecode (AdminGetContentByShareCodeV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
+    Get content by share code
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/sharecodes/{shareCode}
 
         method: GET
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_user_idv2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_get_content_by_user_idv2.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedContentDownloadResponseV2
 from ...models import ResponseError
 
 
 class AdminGetContentByUserIDV2(Operation):
     """Get user's generated contents (AdminGetContentByUserIDV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get user cotent
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/contents
 
         method: GET
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_list_content_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_list_content_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,32 +32,31 @@
 from ...models import ModelsPaginatedContentDownloadResponseV2
 from ...models import ResponseError
 
 
 class AdminListContentV2(Operation):
     """List contents (AdminListContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
-    For advance tag filtering supports & as AND operator and | as OR operator and parentheses () for priority. e.g:
+    For advance tag filtering supports & as AND operator and | as OR operator and parentheses ( ) for priority. e.g:
 
-    `tags=red`
-    `tags=red&animal;`
-    `tags=red|animal`
-    `tags=red&animal;|wild`
-    `tags=red&(animal|wild)`
+
+    *tags=red*
+    *tags=red&animal;*
+    *tags=red|animal*
+    *tags=red&animal;|wild*
+    *tags=red&(animal|wild)*
 
     The precedence of logical operator is AND > OR, so if no parentheses, AND logical operator will be executed first.
 
-    Allowed character for operand: alphanumeric, underscore `_` and dash `-`
-    Allowed character for operator: `&` `|` `(` `)`
+    Allowed character for operand: alphanumeric, underscore _ and dash -
+
+    Allowed character for operator: & | ( )
 
-     Please note that value of tags query param should be URL encoded
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
+    **Please note that value of tags query param should be URL encoded**
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents
 
         method: GET
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_content_by_e139ff.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_content_by_e139ff.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,18 @@
 from ...models import ModelsCreateContentResponseV2
 from ...models import ResponseError
 
 
 class AdminUpdateContentByShareCodeV2(Operation):
     """Update content to S3 bucket by share code (AdminUpdateContentByShareCodeV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
+    *shareCode* format should follows:
 
-    `shareCode` format should follows:
-
-    Max length: 7
-    Available characters: abcdefhkpqrstuxyz
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    "Max length: 7
+    "Available characters: abcdefhkpqrstuxyz
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/s3/sharecodes/{shareCode}
 
         method: PUT
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_content_hi_72a875.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_content_hi_72a875.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsHideContentRequest
 from ...models import ResponseError
 
 
 class AdminUpdateContentHideStatusV2(Operation):
     """Hide/Unhide user's generated contents (AdminUpdateContentHideStatusV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Hide/Unhide user's generated contents
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/contents/{contentId}/hide
 
         method: PUT
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_official_c_348c5f.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_official_c_348c5f.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 from ...models import ModelsUpdateFileLocationRequest
 from ...models import ResponseError
 
 
 class AdminUpdateOfficialContentFileLocation(Operation):
     """Update content file location (AdminUpdateOfficialContentFileLocation)
 
-    This endpoint should be used after calling generate official content upload url endpoint to commit the changes.
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    This endpoint should be used after calling generate official content upload url endpoint to commit the changes
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents/{contentId}/fileLocation
 
         method: PATCH
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_official_c_e7d890.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_official_c_e7d890.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsUpdateContentResponseV2
 from ...models import ResponseError
 
 
 class AdminUpdateOfficialContentV2(Operation):
     """Update official content (AdminUpdateOfficialContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update existing official content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents/{contentId}
 
         method: PATCH
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_screenshots_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_screenshots_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 from ...models import ModelsUpdateScreenshotResponse
 from ...models import ResponseError
 
 
 class AdminUpdateScreenshotsV2(Operation):
     """Update screenshot of content (AdminUpdateScreenshotsV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/screenshots
 
         method: PUT
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_user_conte_8a8bc8.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_user_conte_8a8bc8.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 from ...models import ModelsUpdateFileLocationRequest
 from ...models import ResponseError
 
 
 class AdminUpdateUserContentFileLocation(Operation):
     """Update user content file location (AdminUpdateUserContentFileLocation)
 
-    This endpoint should be used after calling generate user content upload url endpoint to commit the changes.
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    This endpoint should be used after calling generate user content upload url endpoint to commit the changes
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/fileLocation
 
         method: PATCH
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_user_content_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_update_user_content_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsUpdateContentResponseV2
 from ...models import ResponseError
 
 
 class AdminUpdateUserContentV2(Operation):
     """Update user content (AdminUpdateUserContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update existing user content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}
 
         method: PATCH
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_upload_content_sc_3461bc.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/admin_upload_content_sc_3461bc.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,18 @@
 from ...models import ModelsCreateScreenshotResponse
 from ...models import ResponseError
 
 
 class AdminUploadContentScreenshotV2(Operation):
     """Upload screenshots for content (AdminUploadContentScreenshotV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-    All request body are required except for contentType field.
-    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the presigned URL.
-    If not specified, it will use fileExtension value.
+    This endpoint used to request upload URL from content's screenshot.
+    If *contentType* is not specified, it will use *fileExtension* value.
     Supported file extensions: pjp, jpg, jpeg, jfif, bmp, png.
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/screenshots
 
         method: POST
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/list_content_versions_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/list_content_versions_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,20 +32,16 @@
 from ...models import ModelsListContentVersionsResponse
 from ...models import ResponseError
 
 
 class ListContentVersionsV2(Operation):
     """List content's payload versions (ListContentVersionsV2)
 
-    Required permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
     Content's payload versions created when UGC is created or updated with `updateContentFile` set to true. Only list up to 10 latest versions.
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
-
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/versions
 
         method: GET
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/rollback_content_version_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_content_v2/rollback_content_version_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,19 +32,15 @@
 from ...models import ModelsContentDownloadResponse
 from ...models import ResponseError
 
 
 class RollbackContentVersionV2(Operation):
     """Rollback content's payload version (RollbackContentVersionV2)
 
-    Required permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
-    Rollback content's payload to specified version.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Rollback content's payload to specified version
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/rollback/{versionId}
 
         method: PUT
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_group import AdminCreateGroup
 from .admin_delete_group import AdminDeleteGroup
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_create_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_create_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsCreateGroupResponse
 from ...models import ResponseError
 
 
 class AdminCreateGroup(Operation):
     """Create groups (AdminCreateGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [CREATE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [CREATE]
+    Create group
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups
 
         method: POST
 
         tags: ["Admin Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_delete_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_delete_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class AdminDeleteGroup(Operation):
     """Delete group (AdminDeleteGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    Delete group
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
         method: DELETE
 
         tags: ["Admin Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_all_groups.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_all_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedGroupResponse
 from ...models import ResponseError
 
 
 class AdminGetAllGroups(Operation):
     """Get all user groups (AdminGetAllGroups)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get user group paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups
 
         method: GET
 
         tags: ["Admin Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_get_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,24 +29,21 @@
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelsCreateGroupResponse
 from ...models import ResponseError
 
 
-class AdminGetGroup(Operation):
-    """Get specific user group (AdminGetGroup)
+class SingleAdminGetGroup(Operation):
+    """Get specific user group (SingleAdminGetGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get user group by group ID
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}
+        url: /ugc/v1/admin/namespaces/{namespace}/groups/{groupId}
 
         method: GET
 
         tags: ["Admin Group"]
 
         consumes: ["application/json"]
 
@@ -54,38 +51,35 @@
 
         securities: [BEARER_AUTH]
 
         group_id: (groupId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
-        user_id: (userId) REQUIRED str in path
-
     Responses:
-        200: OK - ModelsCreateGroupResponse (Get specific user group)
+        200: OK - ModelsCreateGroupResponse (Get specific group)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
         404: Not Found - ResponseError (773002: Group not found)
 
         500: Internal Server Error - ResponseError (773001: Unable get group)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}"
+    _url: str = "/ugc/v1/admin/namespaces/{namespace}/groups/{groupId}"
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     group_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
-    user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -126,71 +120,61 @@
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "group_id"):
             result["groupId"] = self.group_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
-        if hasattr(self, "user_id"):
-            result["userId"] = self.user_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_group_id(self, value: str) -> AdminGetGroup:
+    def with_group_id(self, value: str) -> SingleAdminGetGroup:
         self.group_id = value
         return self
 
-    def with_namespace(self, value: str) -> AdminGetGroup:
+    def with_namespace(self, value: str) -> SingleAdminGetGroup:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> AdminGetGroup:
-        self.user_id = value
-        return self
-
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "group_id") and self.group_id:
             result["groupId"] = str(self.group_id)
         elif include_empty:
             result["groupId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "user_id") and self.user_id:
-            result["userId"] = str(self.user_id)
-        elif include_empty:
-            result["userId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
         Union[None, ModelsCreateGroupResponse], Union[None, HttpResponse, ResponseError]
     ]:
         """Parse the given response.
 
-        200: OK - ModelsCreateGroupResponse (Get specific user group)
+        200: OK - ModelsCreateGroupResponse (Get specific group)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
         404: Not Found - ResponseError (773002: Group not found)
 
         500: Internal Server Error - ResponseError (773001: Unable get group)
 
@@ -221,54 +205,45 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(
-        cls, group_id: str, namespace: str, user_id: str, **kwargs
-    ) -> AdminGetGroup:
+    def create(cls, group_id: str, namespace: str, **kwargs) -> SingleAdminGetGroup:
         instance = cls()
         instance.group_id = group_id
         instance.namespace = namespace
-        instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminGetGroup:
+    ) -> SingleAdminGetGroup:
         instance = cls()
         if "groupId" in dict_ and dict_["groupId"] is not None:
             instance.group_id = str(dict_["groupId"])
         elif include_empty:
             instance.group_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "userId" in dict_ and dict_["userId"] is not None:
-            instance.user_id = str(dict_["userId"])
-        elif include_empty:
-            instance.user_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "groupId": "group_id",
             "namespace": "namespace",
-            "userId": "user_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "groupId": True,
             "namespace": True,
-            "userId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_group_contents.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_group_contents.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedContentDownloadResponse
 from ...models import ResponseError
 
 
 class AdminGetGroupContents(Operation):
     """(Legacy) Get contents belong to a group (AdminGetGroupContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get content belong to a group
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents
 
         method: GET
 
         tags: ["Admin Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_official_grou_23b467.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_official_grou_23b467.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedContentDownloadResponseV2
 from ...models import ResponseError
 
 
 class AdminGetOfficialGroupContentsV2(Operation):
     """Get contents belong to a group (AdminGetOfficialGroupContentsV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get contents belong to a group
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/groups/{groupId}/contents
 
         method: GET
 
         tags: ["Admin Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_user_group_co_73e55d.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_user_group_co_73e55d.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedContentDownloadResponseV2
 from ...models import ResponseError
 
 
 class AdminGetUserGroupContentsV2(Operation):
     """Get contents belong to a group (AdminGetUserGroupContentsV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get contents belong to a group
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents
 
         method: GET
 
         tags: ["Admin Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_update_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_update_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 from ...models import ModelsCreateGroupResponse
 from ...models import ResponseError
 
 
 class AdminUpdateGroup(Operation):
     """Update group (AdminUpdateGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
-    replace group name and contents with new ones.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
+    Replace group name and contents with new ones.
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
         method: PUT
 
         tags: ["Admin Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_delete_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_delete_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class SingleAdminDeleteGroup(Operation):
     """Delete group (SingleAdminDeleteGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    Delete group by group ID
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups/{groupId}
 
         method: DELETE
 
         tags: ["Admin Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_get_all_groups.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_get_all_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedGroupResponse
 from ...models import ResponseError
 
 
 class SingleAdminGetAllGroups(Operation):
     """Get all user groups (SingleAdminGetAllGroups)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get user group paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups
 
         method: GET
 
         tags: ["Admin Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_get_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/admin_get_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,24 +29,21 @@
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelsCreateGroupResponse
 from ...models import ResponseError
 
 
-class SingleAdminGetGroup(Operation):
-    """Get specific user group (SingleAdminGetGroup)
+class AdminGetGroup(Operation):
+    """Get specific user group (AdminGetGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get user group by group ID
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/groups/{groupId}
+        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
         method: GET
 
         tags: ["Admin Group"]
 
         consumes: ["application/json"]
 
@@ -54,35 +51,38 @@
 
         securities: [BEARER_AUTH]
 
         group_id: (groupId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
+        user_id: (userId) REQUIRED str in path
+
     Responses:
-        200: OK - ModelsCreateGroupResponse (Get specific group)
+        200: OK - ModelsCreateGroupResponse (Get specific user group)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
         404: Not Found - ResponseError (773002: Group not found)
 
         500: Internal Server Error - ResponseError (773001: Unable get group)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/admin/namespaces/{namespace}/groups/{groupId}"
+    _url: str = "/ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}"
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     group_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
+    user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -123,61 +123,71 @@
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "group_id"):
             result["groupId"] = self.group_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
+        if hasattr(self, "user_id"):
+            result["userId"] = self.user_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_group_id(self, value: str) -> SingleAdminGetGroup:
+    def with_group_id(self, value: str) -> AdminGetGroup:
         self.group_id = value
         return self
 
-    def with_namespace(self, value: str) -> SingleAdminGetGroup:
+    def with_namespace(self, value: str) -> AdminGetGroup:
         self.namespace = value
         return self
 
+    def with_user_id(self, value: str) -> AdminGetGroup:
+        self.user_id = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "group_id") and self.group_id:
             result["groupId"] = str(self.group_id)
         elif include_empty:
             result["groupId"] = ""
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
     ) -> Tuple[
         Union[None, ModelsCreateGroupResponse], Union[None, HttpResponse, ResponseError]
     ]:
         """Parse the given response.
 
-        200: OK - ModelsCreateGroupResponse (Get specific group)
+        200: OK - ModelsCreateGroupResponse (Get specific user group)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
         404: Not Found - ResponseError (773002: Group not found)
 
         500: Internal Server Error - ResponseError (773001: Unable get group)
 
@@ -208,45 +218,54 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, group_id: str, namespace: str, **kwargs) -> SingleAdminGetGroup:
+    def create(
+        cls, group_id: str, namespace: str, user_id: str, **kwargs
+    ) -> AdminGetGroup:
         instance = cls()
         instance.group_id = group_id
         instance.namespace = namespace
+        instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> SingleAdminGetGroup:
+    ) -> AdminGetGroup:
         instance = cls()
         if "groupId" in dict_ and dict_["groupId"] is not None:
             instance.group_id = str(dict_["groupId"])
         elif include_empty:
             instance.group_id = ""
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
             "groupId": "group_id",
             "namespace": "namespace",
+            "userId": "user_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "groupId": True,
             "namespace": True,
+            "userId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_get_group__c6800e.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_get_group__c6800e.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedContentDownloadResponse
 from ...models import ResponseError
 
 
 class SingleAdminGetGroupContents(Operation):
     """(Legacy) Get contents belong to a group (SingleAdminGetGroupContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get content belong to a group
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups/{groupId}/contents
 
         method: GET
 
         tags: ["Admin Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_update_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_group/single_admin_update_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 from ...models import ModelsCreateGroupResponse
 from ...models import ResponseError
 
 
 class SingleAdminUpdateGroup(Operation):
     """Update group (SingleAdminUpdateGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
-    replace group name and contents with new ones.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
+    Replace group name and contents with new ones.
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups/{groupId}
 
         method: PUT
 
         tags: ["Admin Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_approve_staging_content import AdminApproveStagingContent
 from .admin_get_staging_conte_7fe68e import AdminGetStagingContentByID
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_approve_staging_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_approve_staging_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsStagingContentResponse
 from ...models import ResponseError
 
 
 class AdminApproveStagingContent(Operation):
     """Approve or reject content (AdminApproveStagingContent)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:CONTENT:APPROVAL [CREATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:CONTENT:APPROVAL [CREATE]
+    Approved content will shown to public player. Rejected content stays in staging area and couldn't be seen by other player
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/staging-contents/{contentId}/approve
 
         method: POST
 
         tags: ["Admin Staging Content"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_get_staging_conte_7fe68e.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_get_staging_conte_7fe68e.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsStagingContentResponse
 from ...models import ResponseError
 
 
 class AdminGetStagingContentByID(Operation):
     """Get staging content by id (AdminGetStagingContentByID)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get staging content by ID
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/staging-contents/{contentId}
 
         method: GET
 
         tags: ["Admin Staging Content"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_list_staging_contents.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_list_staging_contents.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedListStagingContentResponse
 from ...models import ResponseError
 
 
 class AdminListStagingContents(Operation):
     """List staging contents (AdminListStagingContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    List content that need admin's approval
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/staging-contents
 
         method: GET
 
         tags: ["Admin Staging Content"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_list_user_staging_d2fe4e.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_staging_content/admin_list_user_staging_d2fe4e.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedListStagingContentResponse
 from ...models import ResponseError
 
 
 class AdminListUserStagingContents(Operation):
     """List user staging contents (AdminListUserStagingContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    List user content's that need admin approval
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/staging-contents
 
         method: GET
 
         tags: ["Admin Staging Content"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_type/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
-from .admin_create_tag import AdminCreateTag
-from .admin_delete_tag import AdminDeleteTag
-from .admin_get_tag import AdminGetTag
-from .admin_update_tag import AdminUpdateTag
+from .admin_create_type import AdminCreateType
+from .admin_delete_type import AdminDeleteType
+from .admin_get_type import AdminGetType
+from .admin_update_type import AdminUpdateType
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_create_tag.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_update_tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,63 +30,64 @@
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelsCreateTagRequest
 from ...models import ModelsCreateTagResponse
 from ...models import ResponseError
 
 
-class AdminCreateTag(Operation):
-    """Create tags (AdminCreateTag)
+class AdminUpdateTag(Operation):
+    """Update tag (AdminUpdateTag)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [CREATE]
-    creates a new tag
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [CREATE]
+    Update existing tag
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/tags
+        url: /ugc/v1/admin/namespaces/{namespace}/tags/{tagId}
 
-        method: POST
+        method: PUT
 
         tags: ["Admin Tag"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         body: (body) REQUIRED ModelsCreateTagRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
+        tag_id: (tagId) REQUIRED str in path
+
     Responses:
-        201: Created - ModelsCreateTagResponse (Tags created)
+        200: OK - ModelsCreateTagResponse (Tags updated)
 
-        400: Bad Request - ResponseError (771401: Malformed request/Invalid request body)
+        400: Bad Request - ResponseError (772801: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        409: Conflict - ResponseError (771403: Conflicted resource indentifier)
+        404: Not Found - ResponseError (772803: Tag not found)
+
+        409: Conflict - ResponseError (772804: Proposed Tag already exist)
 
-        500: Internal Server Error - ResponseError (771402: Unable to save ugc tag)
+        500: Internal Server Error - ResponseError (772802: Unable update tags)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/admin/namespaces/{namespace}/tags"
-    _method: str = "POST"
+    _url: str = "/ugc/v1/admin/namespaces/{namespace}/tags/{tagId}"
+    _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     body: ModelsCreateTagRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
+    tag_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -131,89 +132,103 @@
             return None
         return self.body.to_dict()
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
+        if hasattr(self, "tag_id"):
+            result["tagId"] = self.tag_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsCreateTagRequest) -> AdminCreateTag:
+    def with_body(self, value: ModelsCreateTagRequest) -> AdminUpdateTag:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> AdminCreateTag:
+    def with_namespace(self, value: str) -> AdminUpdateTag:
         self.namespace = value
         return self
 
+    def with_tag_id(self, value: str) -> AdminUpdateTag:
+        self.tag_id = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
             result["body"] = ModelsCreateTagRequest()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
+        if hasattr(self, "tag_id") and self.tag_id:
+            result["tagId"] = str(self.tag_id)
+        elif include_empty:
+            result["tagId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
         Union[None, ModelsCreateTagResponse], Union[None, HttpResponse, ResponseError]
     ]:
         """Parse the given response.
 
-        201: Created - ModelsCreateTagResponse (Tags created)
+        200: OK - ModelsCreateTagResponse (Tags updated)
 
-        400: Bad Request - ResponseError (771401: Malformed request/Invalid request body)
+        400: Bad Request - ResponseError (772801: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        409: Conflict - ResponseError (771403: Conflicted resource indentifier)
+        404: Not Found - ResponseError (772803: Tag not found)
+
+        409: Conflict - ResponseError (772804: Proposed Tag already exist)
 
-        500: Internal Server Error - ResponseError (771402: Unable to save ugc tag)
+        500: Internal Server Error - ResponseError (772802: Unable update tags)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 201:
+        if code == 200:
             return ModelsCreateTagResponse.create_from_dict(content), None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
+        if code == 404:
+            return None, ResponseError.create_from_dict(content)
         if code == 409:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
@@ -221,48 +236,55 @@
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, body: ModelsCreateTagRequest, namespace: str, **kwargs
-    ) -> AdminCreateTag:
+        cls, body: ModelsCreateTagRequest, namespace: str, tag_id: str, **kwargs
+    ) -> AdminUpdateTag:
         instance = cls()
         instance.body = body
         instance.namespace = namespace
+        instance.tag_id = tag_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminCreateTag:
+    ) -> AdminUpdateTag:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
             instance.body = ModelsCreateTagRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
             instance.body = ModelsCreateTagRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
+        if "tagId" in dict_ and dict_["tagId"] is not None:
+            instance.tag_id = str(dict_["tagId"])
+        elif include_empty:
+            instance.tag_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "body": "body",
             "namespace": "namespace",
+            "tagId": "tag_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "body": True,
             "namespace": True,
+            "tagId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_delete_tag.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_delete_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class AdminDeleteTag(Operation):
     """Delete tags (AdminDeleteTag)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [DELETE]
+    Delete existing tag
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/tags/{tagId}
 
         method: DELETE
 
         tags: ["Admin Tag"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_get_tag.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_get_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedGetTagResponse
 from ...models import ResponseError
 
 
 class AdminGetTag(Operation):
     """Get tags (AdminGetTag)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
+    Get available tags paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/tags
 
         method: GET
 
         tags: ["Admin Tag"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_update_tag.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_update_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,73 +25,69 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsCreateTagRequest
-from ...models import ModelsCreateTagResponse
+from ...models import ModelsCreateTypeRequest
+from ...models import ModelsCreateTypeResponse
 from ...models import ResponseError
 
 
-class AdminUpdateTag(Operation):
-    """Update tag (AdminUpdateTag)
+class AdminUpdateType(Operation):
+    """Update types (AdminUpdateType)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
-    updates a tag
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
+    Updates a type and subtype
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/tags/{tagId}
+        url: /ugc/v1/admin/namespaces/{namespace}/types/{typeId}
 
         method: PUT
 
-        tags: ["Admin Tag"]
+        tags: ["Admin Type"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsCreateTagRequest in body
+        body: (body) REQUIRED ModelsCreateTypeRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
-        tag_id: (tagId) REQUIRED str in path
+        type_id: (typeId) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsCreateTagResponse (Tags updated)
+        200: OK - ModelsCreateTypeResponse (Types updated)
 
-        400: Bad Request - ResponseError (772801: Malformed request/Invalid request body)
+        400: Bad Request - ResponseError (771901: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (772803: Tag not found)
+        404: Not Found - ResponseError (771903: Type not found)
 
-        409: Conflict - ResponseError (772804: Proposed Tag already exist)
+        409: Conflict - ResponseError (771904: Proposed Type already exist)
 
-        500: Internal Server Error - ResponseError (772802: Unable update tags)
+        500: Internal Server Error - ResponseError (771902: Unable update types)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/admin/namespaces/{namespace}/tags/{tagId}"
+    _url: str = "/ugc/v1/admin/namespaces/{namespace}/types/{typeId}"
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsCreateTagRequest  # REQUIRED in [body]
+    body: ModelsCreateTypeRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
-    tag_id: str  # REQUIRED in [path]
+    type_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -136,81 +132,81 @@
             return None
         return self.body.to_dict()
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
-        if hasattr(self, "tag_id"):
-            result["tagId"] = self.tag_id
+        if hasattr(self, "type_id"):
+            result["typeId"] = self.type_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsCreateTagRequest) -> AdminUpdateTag:
+    def with_body(self, value: ModelsCreateTypeRequest) -> AdminUpdateType:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> AdminUpdateTag:
+    def with_namespace(self, value: str) -> AdminUpdateType:
         self.namespace = value
         return self
 
-    def with_tag_id(self, value: str) -> AdminUpdateTag:
-        self.tag_id = value
+    def with_type_id(self, value: str) -> AdminUpdateType:
+        self.type_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsCreateTagRequest()
+            result["body"] = ModelsCreateTypeRequest()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "tag_id") and self.tag_id:
-            result["tagId"] = str(self.tag_id)
+        if hasattr(self, "type_id") and self.type_id:
+            result["typeId"] = str(self.type_id)
         elif include_empty:
-            result["tagId"] = ""
+            result["typeId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsCreateTagResponse], Union[None, HttpResponse, ResponseError]
+        Union[None, ModelsCreateTypeResponse], Union[None, HttpResponse, ResponseError]
     ]:
         """Parse the given response.
 
-        200: OK - ModelsCreateTagResponse (Tags updated)
+        200: OK - ModelsCreateTypeResponse (Types updated)
 
-        400: Bad Request - ResponseError (772801: Malformed request/Invalid request body)
+        400: Bad Request - ResponseError (771901: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (772803: Tag not found)
+        404: Not Found - ResponseError (771903: Type not found)
 
-        409: Conflict - ResponseError (772804: Proposed Tag already exist)
+        409: Conflict - ResponseError (771904: Proposed Type already exist)
 
-        500: Internal Server Error - ResponseError (772802: Unable update tags)
+        500: Internal Server Error - ResponseError (771902: Unable update types)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -218,15 +214,15 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsCreateTagResponse.create_from_dict(content), None
+            return ModelsCreateTypeResponse.create_from_dict(content), None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
         if code == 409:
@@ -240,55 +236,55 @@
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, body: ModelsCreateTagRequest, namespace: str, tag_id: str, **kwargs
-    ) -> AdminUpdateTag:
+        cls, body: ModelsCreateTypeRequest, namespace: str, type_id: str, **kwargs
+    ) -> AdminUpdateType:
         instance = cls()
         instance.body = body
         instance.namespace = namespace
-        instance.tag_id = tag_id
+        instance.type_id = type_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminUpdateTag:
+    ) -> AdminUpdateType:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsCreateTagRequest.create_from_dict(
+            instance.body = ModelsCreateTypeRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsCreateTagRequest()
+            instance.body = ModelsCreateTypeRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "tagId" in dict_ and dict_["tagId"] is not None:
-            instance.tag_id = str(dict_["tagId"])
+        if "typeId" in dict_ and dict_["typeId"] is not None:
+            instance.type_id = str(dict_["typeId"])
         elif include_empty:
-            instance.tag_id = ""
+            instance.type_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "body": "body",
             "namespace": "namespace",
-            "tagId": "tag_id",
+            "typeId": "type_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "body": True,
             "namespace": True,
-            "tagId": True,
+            "typeId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_create_type.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_create_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 from ...models import ModelsCreateTypeResponse
 from ...models import ResponseError
 
 
 class AdminCreateType(Operation):
     """Create types (AdminCreateType)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [CREATE]
-    creates a new type and subtype
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [CREATE]
+    Creates a new type and subtype
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/types
 
         method: POST
 
         tags: ["Admin Type"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_delete_type.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_delete_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,20 +29,17 @@
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
 class AdminDeleteType(Operation):
-    """Delete types (AdminDeleteType)
+    """Delete type (AdminDeleteType)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [DELETE]
+    Delete existing type
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/types/{typeId}
 
         method: DELETE
 
         tags: ["Admin Type"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_get_type.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_get_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedGetTypeResponse
 from ...models import ResponseError
 
 
 class AdminGetType(Operation):
     """Get types (AdminGetType)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
+    Get available types paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/types
 
         method: GET
 
         tags: ["Admin Type"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/admin_type/admin_update_type.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_type/get_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,73 +25,64 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsCreateTypeRequest
-from ...models import ModelsCreateTypeResponse
+from ...models import ModelsPaginatedGetTypeResponse
 from ...models import ResponseError
 
 
-class AdminUpdateType(Operation):
-    """Update types (AdminUpdateType)
+class GetType(Operation):
+    """Get types (GetType)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
-    updates a type and subtype
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
+    Get available types paginated
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/types/{typeId}
+        url: /ugc/v1/public/namespaces/{namespace}/types
 
-        method: PUT
+        method: GET
 
-        tags: ["Admin Type"]
+        tags: ["Public Type"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsCreateTypeRequest in body
-
         namespace: (namespace) REQUIRED str in path
 
-        type_id: (typeId) REQUIRED str in path
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
 
     Responses:
-        200: OK - ModelsCreateTypeResponse (Types updated)
+        200: OK - ModelsPaginatedGetTypeResponse (Get types)
 
-        400: Bad Request - ResponseError (771901: Malformed request/Invalid request body)
+        400: Bad Request - ResponseError (771801: invalid paging parameter)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (771903: Type not found)
-
-        409: Conflict - ResponseError (771904: Proposed Type already exist)
-
-        500: Internal Server Error - ResponseError (771902: Unable update types)
+        500: Internal Server Error - ResponseError (771802: Unable get types)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/admin/namespaces/{namespace}/types/{typeId}"
-    _method: str = "PUT"
-    _consumes: List[str] = ["application/json"]
+    _url: str = "/ugc/v1/public/namespaces/{namespace}/types"
+    _method: str = "GET"
+    _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsCreateTypeRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
-    type_id: str  # REQUIRED in [path]
+    limit: int  # OPTIONAL in [query]
+    offset: int  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -123,94 +114,92 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
-            "body": self.get_body_params(),
             "path": self.get_path_params(),
+            "query": self.get_query_params(),
         }
 
-    def get_body_params(self) -> Any:
-        if not hasattr(self, "body") or self.body is None:
-            return None
-        return self.body.to_dict()
-
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
-        if hasattr(self, "type_id"):
-            result["typeId"] = self.type_id
+        return result
+
+    def get_query_params(self) -> dict:
+        result = {}
+        if hasattr(self, "limit"):
+            result["limit"] = self.limit
+        if hasattr(self, "offset"):
+            result["offset"] = self.offset
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsCreateTypeRequest) -> AdminUpdateType:
-        self.body = value
+    def with_namespace(self, value: str) -> GetType:
+        self.namespace = value
         return self
 
-    def with_namespace(self, value: str) -> AdminUpdateType:
-        self.namespace = value
+    def with_limit(self, value: int) -> GetType:
+        self.limit = value
         return self
 
-    def with_type_id(self, value: str) -> AdminUpdateType:
-        self.type_id = value
+    def with_offset(self, value: int) -> GetType:
+        self.offset = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "body") and self.body:
-            result["body"] = self.body.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["body"] = ModelsCreateTypeRequest()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "type_id") and self.type_id:
-            result["typeId"] = str(self.type_id)
+        if hasattr(self, "limit") and self.limit:
+            result["limit"] = int(self.limit)
+        elif include_empty:
+            result["limit"] = 0
+        if hasattr(self, "offset") and self.offset:
+            result["offset"] = int(self.offset)
         elif include_empty:
-            result["typeId"] = ""
+            result["offset"] = 0
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsCreateTypeResponse], Union[None, HttpResponse, ResponseError]
+        Union[None, ModelsPaginatedGetTypeResponse],
+        Union[None, HttpResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - ModelsCreateTypeResponse (Types updated)
+        200: OK - ModelsPaginatedGetTypeResponse (Get types)
 
-        400: Bad Request - ResponseError (771901: Malformed request/Invalid request body)
+        400: Bad Request - ResponseError (771801: invalid paging parameter)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (771903: Type not found)
-
-        409: Conflict - ResponseError (771904: Proposed Type already exist)
-
-        500: Internal Server Error - ResponseError (771902: Unable update types)
+        500: Internal Server Error - ResponseError (771802: Unable get types)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -218,77 +207,75 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsCreateTypeResponse.create_from_dict(content), None
+            return ModelsPaginatedGetTypeResponse.create_from_dict(content), None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
-        if code == 404:
-            return None, ResponseError.create_from_dict(content)
-        if code == 409:
-            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, body: ModelsCreateTypeRequest, namespace: str, type_id: str, **kwargs
-    ) -> AdminUpdateType:
+        cls,
+        namespace: str,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        **kwargs,
+    ) -> GetType:
         instance = cls()
-        instance.body = body
         instance.namespace = namespace
-        instance.type_id = type_id
+        if limit is not None:
+            instance.limit = limit
+        if offset is not None:
+            instance.offset = offset
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> AdminUpdateType:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> GetType:
         instance = cls()
-        if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsCreateTypeRequest.create_from_dict(
-                dict_["body"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.body = ModelsCreateTypeRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "typeId" in dict_ and dict_["typeId"] is not None:
-            instance.type_id = str(dict_["typeId"])
+        if "limit" in dict_ and dict_["limit"] is not None:
+            instance.limit = int(dict_["limit"])
+        elif include_empty:
+            instance.limit = 0
+        if "offset" in dict_ and dict_["offset"] is not None:
+            instance.offset = int(dict_["offset"])
         elif include_empty:
-            instance.type_id = ""
+            instance.offset = 0
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "body": "body",
             "namespace": "namespace",
-            "typeId": "type_id",
+            "limit": "limit",
+            "offset": "offset",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "body": True,
             "namespace": True,
-            "typeId": True,
+            "limit": False,
+            "offset": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_delete_all_user_channels import AdminDeleteAllUserChannels
 from .admin_delete_all_user_contents import AdminDeleteAllUserContents
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_channels.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_channels.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class AdminDeleteAllUserChannels(Operation):
     """Delete all user channel (AdminDeleteAllUserChannels)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Delete all user channel
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels
 
         method: DELETE
 
         tags: ["Anonymization"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_contents.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_contents.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,54 +28,51 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class AdminDeleteAllUserGroup(Operation):
-    """Delete all user group (AdminDeleteAllUserGroup)
+class DeleteAllUserGroup(Operation):
+    """Delete all user group (DeleteAllUserGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    Delete all user group
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups
 
         method: DELETE
 
         tags: ["Anonymization"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (Groups deleted)
+        204: No Content - (groups deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
         404: Not Found - ResponseError (773302: Groups not found)
 
         500: Internal Server Error - ResponseError (773301: Unable to find all user group)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups"
+    _url: str = "/ugc/v1/public/namespaces/{namespace}/users/{userId}/groups"
     _method: str = "DELETE"
-    _consumes: List[str] = ["application/json"]
+    _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
@@ -132,19 +129,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> AdminDeleteAllUserGroup:
+    def with_namespace(self, value: str) -> DeleteAllUserGroup:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> AdminDeleteAllUserGroup:
+    def with_user_id(self, value: str) -> DeleteAllUserGroup:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -166,15 +163,15 @@
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
         """Parse the given response.
 
-        204: No Content - (Groups deleted)
+        204: No Content - (groups deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
         404: Not Found - ResponseError (773302: Groups not found)
 
         500: Internal Server Error - ResponseError (773301: Unable to find all user group)
 
@@ -205,26 +202,26 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, user_id: str, **kwargs) -> AdminDeleteAllUserGroup:
+    def create(cls, namespace: str, user_id: str, **kwargs) -> DeleteAllUserGroup:
         instance = cls()
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminDeleteAllUserGroup:
+    ) -> DeleteAllUserGroup:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "userId" in dict_ and dict_["userId"] is not None:
             instance.user_id = str(dict_["userId"])
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_states.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_states.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_channel.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_contents.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class DeleteAllUserChannel(Operation):
-    """Delete all user channel (DeleteAllUserChannel)
+class DeleteAllUserContents(Operation):
+    """Delete all user content (DeleteAllUserContents)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents
 
         method: DELETE
 
         tags: ["Anonymization"]
 
         consumes: ["application/json", "application/octet-stream"]
 
@@ -54,26 +54,26 @@
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (Content deleted)
+        204: No Content - (User content's deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773502: Channel not found)
+        404: Not Found - ResponseError (773402: Content not found | 771601: Creator not found)
 
-        500: Internal Server Error - ResponseError (773501: Unable to delete channel)
+        500: Internal Server Error - ResponseError (773401: Unable to get all user content)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/public/namespaces/{namespace}/users/{userId}/channels"
+    _url: str = "/ugc/v1/public/namespaces/{namespace}/users/{userId}/contents"
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     namespace: str  # REQUIRED in [path]
@@ -132,19 +132,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> DeleteAllUserChannel:
+    def with_namespace(self, value: str) -> DeleteAllUserContents:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> DeleteAllUserChannel:
+    def with_user_id(self, value: str) -> DeleteAllUserContents:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -166,21 +166,21 @@
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
         """Parse the given response.
 
-        204: No Content - (Content deleted)
+        204: No Content - (User content's deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773502: Channel not found)
+        404: Not Found - ResponseError (773402: Content not found | 771601: Creator not found)
 
-        500: Internal Server Error - ResponseError (773501: Unable to delete channel)
+        500: Internal Server Error - ResponseError (773401: Unable to get all user content)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -205,26 +205,26 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, user_id: str, **kwargs) -> DeleteAllUserChannel:
+    def create(cls, namespace: str, user_id: str, **kwargs) -> DeleteAllUserContents:
         instance = cls()
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> DeleteAllUserChannel:
+    ) -> DeleteAllUserContents:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "userId" in dict_ and dict_["userId"] is not None:
             instance.user_id = str(dict_["userId"])
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_contents.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/admin_delete_all_user_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,54 +28,51 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class DeleteAllUserContents(Operation):
-    """Delete all user content (DeleteAllUserContents)
+class AdminDeleteAllUserGroup(Operation):
+    """Delete all user group (AdminDeleteAllUserGroup)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete all user group
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents
+        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups
 
         method: DELETE
 
         tags: ["Anonymization"]
 
-        consumes: ["application/json", "application/octet-stream"]
+        consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (User content's deleted)
+        204: No Content - (Groups deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773402: Content not found | 771601: Creator not found)
+        404: Not Found - ResponseError (773302: Groups not found)
 
-        500: Internal Server Error - ResponseError (773401: Unable to get all user content)
+        500: Internal Server Error - ResponseError (773301: Unable to find all user group)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/public/namespaces/{namespace}/users/{userId}/contents"
+    _url: str = "/ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups"
     _method: str = "DELETE"
-    _consumes: List[str] = ["application/json", "application/octet-stream"]
+    _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
@@ -132,19 +129,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> DeleteAllUserContents:
+    def with_namespace(self, value: str) -> AdminDeleteAllUserGroup:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> DeleteAllUserContents:
+    def with_user_id(self, value: str) -> AdminDeleteAllUserGroup:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -166,21 +163,21 @@
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
         """Parse the given response.
 
-        204: No Content - (User content's deleted)
+        204: No Content - (Groups deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773402: Content not found | 771601: Creator not found)
+        404: Not Found - ResponseError (773302: Groups not found)
 
-        500: Internal Server Error - ResponseError (773401: Unable to get all user content)
+        500: Internal Server Error - ResponseError (773301: Unable to find all user group)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -205,26 +202,26 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, user_id: str, **kwargs) -> DeleteAllUserContents:
+    def create(cls, namespace: str, user_id: str, **kwargs) -> AdminDeleteAllUserGroup:
         instance = cls()
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> DeleteAllUserContents:
+    ) -> AdminDeleteAllUserGroup:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "userId" in dict_ and dict_["userId"] is not None:
             instance.user_id = str(dict_["userId"])
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/create_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,61 +25,63 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
+from ...models import ModelsCreateGroupRequest
+from ...models import ModelsCreateGroupResponse
 from ...models import ResponseError
 
 
-class DeleteAllUserGroup(Operation):
-    """Delete all user group (DeleteAllUserGroup)
+class CreateGroup(Operation):
+    """Create groups (CreateGroup)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    Create group
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups
 
-        method: DELETE
+        method: POST
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        body: (body) REQUIRED ModelsCreateGroupRequest in body
+
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (groups deleted)
+        201: Created - ModelsCreateGroupResponse (Group Created)
 
-        401: Unauthorized - ResponseError (20001: unauthorized access)
+        400: Bad Request - ResponseError (772101: Malformed request/Invalid request body)
 
-        404: Not Found - ResponseError (773302: Groups not found)
+        401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (773301: Unable to find all user group)
+        500: Internal Server Error - ResponseError (772102: Unable to create group)
     """
 
     # region fields
 
     _url: str = "/ugc/v1/public/namespaces/{namespace}/users/{userId}/groups"
-    _method: str = "DELETE"
+    _method: str = "POST"
     _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    body: ModelsCreateGroupRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
@@ -113,17 +115,23 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
+            "body": self.get_body_params(),
             "path": self.get_path_params(),
         }
 
+    def get_body_params(self) -> Any:
+        if not hasattr(self, "body") or self.body is None:
+            return None
+        return self.body.to_dict()
+
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         if hasattr(self, "user_id"):
             result["userId"] = self.user_id
         return result
@@ -132,28 +140,36 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> DeleteAllUserGroup:
+    def with_body(self, value: ModelsCreateGroupRequest) -> CreateGroup:
+        self.body = value
+        return self
+
+    def with_namespace(self, value: str) -> CreateGroup:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> DeleteAllUserGroup:
+    def with_user_id(self, value: str) -> CreateGroup:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "body") and self.body:
+            result["body"] = self.body.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["body"] = ModelsCreateGroupRequest()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         if hasattr(self, "user_id") and self.user_id:
             result["userId"] = str(self.user_id)
         elif include_empty:
@@ -163,87 +179,98 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
+    ) -> Tuple[
+        Union[None, ModelsCreateGroupResponse], Union[None, HttpResponse, ResponseError]
+    ]:
         """Parse the given response.
 
-        204: No Content - (groups deleted)
+        201: Created - ModelsCreateGroupResponse (Group Created)
 
-        401: Unauthorized - ResponseError (20001: unauthorized access)
+        400: Bad Request - ResponseError (772101: Malformed request/Invalid request body)
 
-        404: Not Found - ResponseError (773302: Groups not found)
+        401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (773301: Unable to find all user group)
+        500: Internal Server Error - ResponseError (772102: Unable to create group)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 204:
-            return None, None
-        if code == 401:
+        if code == 201:
+            return ModelsCreateGroupResponse.create_from_dict(content), None
+        if code == 400:
             return None, ResponseError.create_from_dict(content)
-        if code == 404:
+        if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, user_id: str, **kwargs) -> DeleteAllUserGroup:
+    def create(
+        cls, body: ModelsCreateGroupRequest, namespace: str, user_id: str, **kwargs
+    ) -> CreateGroup:
         instance = cls()
+        instance.body = body
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> DeleteAllUserGroup:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> CreateGroup:
         instance = cls()
+        if "body" in dict_ and dict_["body"] is not None:
+            instance.body = ModelsCreateGroupRequest.create_from_dict(
+                dict_["body"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.body = ModelsCreateGroupRequest()
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
+            "body": "body",
             "namespace": "namespace",
             "userId": "user_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
+            "body": True,
             "namespace": True,
             "userId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_states.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_states.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_channel/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_channel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_channel import DeleteChannel
 from .get_channels import GetChannels
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_channel/delete_channel.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_channel/delete_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class DeleteChannel(Operation):
     """Delete Channel (DeleteChannel)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Delete user channel
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}
 
         method: DELETE
 
         tags: ["Public Channel"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_channel/get_channels.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_channel/get_channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedGetChannelResponse
 from ...models import ResponseError
 
 
 class GetChannels(Operation):
     """Get Channels (GetChannels)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
+    Get user channel paginated
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels
 
         method: GET
 
         tags: ["Public Channel"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_channel/public_create_channel.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_channel/public_create_channel.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsPublicChannelRequest
 from ...models import ResponseError
 
 
 class PublicCreateChannel(Operation):
     """Create Channel (PublicCreateChannel)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [CREATE]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [CREATE]
+    Create user channel
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels
 
         method: POST
 
         tags: ["Public Channel"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_channel/update_channel.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/create_content_direct.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,73 +24,74 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
+from accelbyte_py_sdk.core import deprecated
 
-from ...models import ModelsChannelResponse
-from ...models import ModelsUpdateChannelRequest
+from ...models import ModelsCreateContentRequest
+from ...models import ModelsCreateContentResponse
 from ...models import ResponseError
 
 
-class UpdateChannel(Operation):
-    """Update Channel (UpdateChannel)
+class CreateContentDirect(Operation):
+    """Upload content to a channel (CreateContentDirect)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
+
+    All request body are required except preview, tags and customAttributes.
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents
 
-        method: PUT
+        method: POST
 
-        tags: ["Public Channel"]
+        tags: ["Public Content (Legacy)"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsUpdateChannelRequest in body
+        body: (body) REQUIRED ModelsCreateContentRequest in body
 
         channel_id: (channelId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsChannelResponse (Channel updated)
+        201: Created - ModelsCreateContentResponse (Content uploaded)
 
-        400: Bad Request - ResponseError (770600: Invalid request body)
+        400: Bad Request - ResponseError (770100: Malformed request/Invalid request body/channel do not exist)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (770603: Channel was not found)
+        403: Forbidden - ResponseError (770104: User has been banned to create content)
 
-        500: Internal Server Error - ResponseError (770602: Unable to save channel)
+        500: Internal Server Error - ResponseError (770102: Unable to check user ban status/Unable to save ugc content: unable to get channel | 770103: Unable to save ugc content: shareCode exceed the limit)
     """
 
     # region fields
 
-    _url: str = (
-        "/ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}"
-    )
-    _method: str = "PUT"
+    _url: str = "/ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents"
+    _method: str = "POST"
     _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsUpdateChannelRequest  # REQUIRED in [body]
+    body: ModelsCreateContentRequest  # REQUIRED in [body]
     channel_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
@@ -152,40 +153,40 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsUpdateChannelRequest) -> UpdateChannel:
+    def with_body(self, value: ModelsCreateContentRequest) -> CreateContentDirect:
         self.body = value
         return self
 
-    def with_channel_id(self, value: str) -> UpdateChannel:
+    def with_channel_id(self, value: str) -> CreateContentDirect:
         self.channel_id = value
         return self
 
-    def with_namespace(self, value: str) -> UpdateChannel:
+    def with_namespace(self, value: str) -> CreateContentDirect:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> UpdateChannel:
+    def with_user_id(self, value: str) -> CreateContentDirect:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsUpdateChannelRequest()
+            result["body"] = ModelsCreateContentRequest()
         if hasattr(self, "channel_id") and self.channel_id:
             result["channelId"] = str(self.channel_id)
         elif include_empty:
             result["channelId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
@@ -200,48 +201,49 @@
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsChannelResponse], Union[None, HttpResponse, ResponseError]
+        Union[None, ModelsCreateContentResponse],
+        Union[None, HttpResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - ModelsChannelResponse (Channel updated)
+        201: Created - ModelsCreateContentResponse (Content uploaded)
 
-        400: Bad Request - ResponseError (770600: Invalid request body)
+        400: Bad Request - ResponseError (770100: Malformed request/Invalid request body/channel do not exist)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (770603: Channel was not found)
+        403: Forbidden - ResponseError (770104: User has been banned to create content)
 
-        500: Internal Server Error - ResponseError (770602: Unable to save channel)
+        500: Internal Server Error - ResponseError (770102: Unable to check user ban status/Unable to save ugc content: unable to get channel | 770103: Unable to save ugc content: shareCode exceed the limit)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return ModelsChannelResponse.create_from_dict(content), None
+        if code == 201:
+            return ModelsCreateContentResponse.create_from_dict(content), None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
-        if code == 404:
+        if code == 403:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
@@ -249,40 +251,40 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: ModelsUpdateChannelRequest,
+        body: ModelsCreateContentRequest,
         channel_id: str,
         namespace: str,
         user_id: str,
         **kwargs,
-    ) -> UpdateChannel:
+    ) -> CreateContentDirect:
         instance = cls()
         instance.body = body
         instance.channel_id = channel_id
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> UpdateChannel:
+    ) -> CreateContentDirect:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsUpdateChannelRequest.create_from_dict(
+            instance.body = ModelsCreateContentRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsUpdateChannelRequest()
+            instance.body = ModelsCreateContentRequest()
         if "channelId" in dict_ and dict_["channelId"] is not None:
             instance.channel_id = str(dict_["channelId"])
         elif include_empty:
             instance.channel_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_content_direct import CreateContentDirect
 from .create_content_s3 import CreateContentS3
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/create_content_direct.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/create_content_s3.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,74 +24,79 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
-from accelbyte_py_sdk.core import deprecated
 
-from ...models import ModelsCreateContentRequest
 from ...models import ModelsCreateContentResponse
+from ...models import ModelsPublicCreateContentRequestS3
 from ...models import ResponseError
 
 
-class CreateContentDirect(Operation):
-    """Upload content to a channel (CreateContentDirect)
+class CreateContentS3(Operation):
+    """Upload content to S3 bucket (CreateContentS3)
 
     Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
 
-    All request body are required except preview, tags and customAttributes.
+    All request body are required except payload, preview, tags, contentType and customAttributes.
+    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the S3 presigned URL.
+    If not specified, it will use fileExtension value.
+
+
+
+    NOTE: Preview is Legacy Code, please use Screenshot for better solution to display preview of a content
 
     Required Permission(s):
         - NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/s3
 
         method: POST
 
         tags: ["Public Content (Legacy)"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsCreateContentRequest in body
+        body: (body) REQUIRED ModelsPublicCreateContentRequestS3 in body
 
         channel_id: (channelId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        201: Created - ModelsCreateContentResponse (Content uploaded)
+        201: Created - ModelsCreateContentResponse (Content uploaded to S3 bucket)
 
-        400: Bad Request - ResponseError (770100: Malformed request/Invalid request body/channel do not exist)
+        400: Bad Request - ResponseError (770100: Malformed request/Invalid request body/channel do not exist | 770102: Unable to check user ban status/Unable to save ugc content: unable to get channel)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
         403: Forbidden - ResponseError (770104: User has been banned to create content)
 
-        500: Internal Server Error - ResponseError (770102: Unable to check user ban status/Unable to save ugc content: unable to get channel | 770103: Unable to save ugc content: shareCode exceed the limit)
+        500: Internal Server Error - ResponseError (770102: Unable to check user ban status/Unable to save ugc content: unable to get channel | 770105: Unable to save ugc content: failed generate upload URL | 770103: Unable to save ugc content: shareCode exceed the limit)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents"
+    _url: str = "/ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/s3"
     _method: str = "POST"
     _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsCreateContentRequest  # REQUIRED in [body]
+    body: ModelsPublicCreateContentRequestS3  # REQUIRED in [body]
     channel_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
@@ -153,40 +158,40 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsCreateContentRequest) -> CreateContentDirect:
+    def with_body(self, value: ModelsPublicCreateContentRequestS3) -> CreateContentS3:
         self.body = value
         return self
 
-    def with_channel_id(self, value: str) -> CreateContentDirect:
+    def with_channel_id(self, value: str) -> CreateContentS3:
         self.channel_id = value
         return self
 
-    def with_namespace(self, value: str) -> CreateContentDirect:
+    def with_namespace(self, value: str) -> CreateContentS3:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> CreateContentDirect:
+    def with_user_id(self, value: str) -> CreateContentS3:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsCreateContentRequest()
+            result["body"] = ModelsPublicCreateContentRequestS3()
         if hasattr(self, "channel_id") and self.channel_id:
             result["channelId"] = str(self.channel_id)
         elif include_empty:
             result["channelId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
@@ -206,23 +211,23 @@
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
         Union[None, ModelsCreateContentResponse],
         Union[None, HttpResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        201: Created - ModelsCreateContentResponse (Content uploaded)
+        201: Created - ModelsCreateContentResponse (Content uploaded to S3 bucket)
 
-        400: Bad Request - ResponseError (770100: Malformed request/Invalid request body/channel do not exist)
+        400: Bad Request - ResponseError (770100: Malformed request/Invalid request body/channel do not exist | 770102: Unable to check user ban status/Unable to save ugc content: unable to get channel)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
         403: Forbidden - ResponseError (770104: User has been banned to create content)
 
-        500: Internal Server Error - ResponseError (770102: Unable to check user ban status/Unable to save ugc content: unable to get channel | 770103: Unable to save ugc content: shareCode exceed the limit)
+        500: Internal Server Error - ResponseError (770102: Unable to check user ban status/Unable to save ugc content: unable to get channel | 770105: Unable to save ugc content: failed generate upload URL | 770103: Unable to save ugc content: shareCode exceed the limit)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -251,40 +256,40 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: ModelsCreateContentRequest,
+        body: ModelsPublicCreateContentRequestS3,
         channel_id: str,
         namespace: str,
         user_id: str,
         **kwargs,
-    ) -> CreateContentDirect:
+    ) -> CreateContentS3:
         instance = cls()
         instance.body = body
         instance.channel_id = channel_id
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> CreateContentDirect:
+    ) -> CreateContentS3:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsCreateContentRequest.create_from_dict(
+            instance.body = ModelsPublicCreateContentRequestS3.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsCreateContentRequest()
+            instance.body = ModelsPublicCreateContentRequestS3()
         if "channelId" in dict_ and dict_["channelId"] is not None:
             instance.channel_id = str(dict_["channelId"])
         elif include_empty:
             instance.channel_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/create_content_s3.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/update_content_share_code_v2.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,79 +25,79 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsCreateContentResponse
-from ...models import ModelsPublicCreateContentRequestS3
+from ...models import ModelsCreateContentResponseV2
+from ...models import ModelsUpdateContentShareCodeRequest
 from ...models import ResponseError
 
 
-class CreateContentS3(Operation):
-    """Upload content to S3 bucket (CreateContentS3)
+class UpdateContentShareCodeV2(Operation):
+    """Update content share code (UpdateContentShareCodeV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
+    This endpoint is used to modify the shareCode of a content. However, this operation is restricted by default and requires the above permission to be granted to the User role.
 
-    All request body are required except payload, preview, tags, contentType and customAttributes.
-    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the S3 presigned URL.
-    If not specified, it will use fileExtension value.
-
-
-
-    NOTE: Preview is Legacy Code, please use Screenshot for better solution to display preview of a content
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    `shareCode` format should follows:
+    Max length: 7
+    Available characters: abcdefhkpqrstuxyz
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/s3
+        url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/sharecode
 
-        method: POST
+        method: PATCH
 
-        tags: ["Public Content (Legacy)"]
+        tags: ["Public Content V2"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsPublicCreateContentRequestS3 in body
+        body: (body) REQUIRED ModelsUpdateContentShareCodeRequest in body
 
         channel_id: (channelId) REQUIRED str in path
 
+        content_id: (contentId) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        201: Created - ModelsCreateContentResponse (Content uploaded to S3 bucket)
+        200: OK - ModelsCreateContentResponseV2 (Update content sharecode)
 
-        400: Bad Request - ResponseError (770100: Malformed request/Invalid request body/channel do not exist | 770102: Unable to check user ban status/Unable to save ugc content: unable to get channel)
+        400: Bad Request - ResponseError (772601: Malformed request | 772607: Unable to update ugc content: invalid shareCode format)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        403: Forbidden - ResponseError (770104: User has been banned to create content)
+        403: Forbidden - ResponseError (772604: User has been banned to update content | 20013: insufficient permission)
+
+        404: Not Found - ResponseError (772603: Content not found)
 
-        500: Internal Server Error - ResponseError (770102: Unable to check user ban status/Unable to save ugc content: unable to get channel | 770105: Unable to save ugc content: failed generate upload URL | 770103: Unable to save ugc content: shareCode exceed the limit)
+        409: Conflict - ResponseError (772606: Share code already used)
+
+        500: Internal Server Error - ResponseError (772602: Unable to check user ban status/Unable to get updated ugc content)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/s3"
-    _method: str = "POST"
+    _url: str = "/ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/sharecode"
+    _method: str = "PATCH"
     _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsPublicCreateContentRequestS3  # REQUIRED in [body]
+    body: ModelsUpdateContentShareCodeRequest  # REQUIRED in [body]
     channel_id: str  # REQUIRED in [path]
+    content_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
@@ -144,58 +144,70 @@
             return None
         return self.body.to_dict()
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "channel_id"):
             result["channelId"] = self.channel_id
+        if hasattr(self, "content_id"):
+            result["contentId"] = self.content_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         if hasattr(self, "user_id"):
             result["userId"] = self.user_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsPublicCreateContentRequestS3) -> CreateContentS3:
+    def with_body(
+        self, value: ModelsUpdateContentShareCodeRequest
+    ) -> UpdateContentShareCodeV2:
         self.body = value
         return self
 
-    def with_channel_id(self, value: str) -> CreateContentS3:
+    def with_channel_id(self, value: str) -> UpdateContentShareCodeV2:
         self.channel_id = value
         return self
 
-    def with_namespace(self, value: str) -> CreateContentS3:
+    def with_content_id(self, value: str) -> UpdateContentShareCodeV2:
+        self.content_id = value
+        return self
+
+    def with_namespace(self, value: str) -> UpdateContentShareCodeV2:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> CreateContentS3:
+    def with_user_id(self, value: str) -> UpdateContentShareCodeV2:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsPublicCreateContentRequestS3()
+            result["body"] = ModelsUpdateContentShareCodeRequest()
         if hasattr(self, "channel_id") and self.channel_id:
             result["channelId"] = str(self.channel_id)
         elif include_empty:
             result["channelId"] = ""
+        if hasattr(self, "content_id") and self.content_id:
+            result["contentId"] = str(self.content_id)
+        elif include_empty:
+            result["contentId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         if hasattr(self, "user_id") and self.user_id:
             result["userId"] = str(self.user_id)
         elif include_empty:
@@ -206,94 +218,108 @@
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsCreateContentResponse],
+        Union[None, ModelsCreateContentResponseV2],
         Union[None, HttpResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        201: Created - ModelsCreateContentResponse (Content uploaded to S3 bucket)
+        200: OK - ModelsCreateContentResponseV2 (Update content sharecode)
 
-        400: Bad Request - ResponseError (770100: Malformed request/Invalid request body/channel do not exist | 770102: Unable to check user ban status/Unable to save ugc content: unable to get channel)
+        400: Bad Request - ResponseError (772601: Malformed request | 772607: Unable to update ugc content: invalid shareCode format)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        403: Forbidden - ResponseError (770104: User has been banned to create content)
+        403: Forbidden - ResponseError (772604: User has been banned to update content | 20013: insufficient permission)
+
+        404: Not Found - ResponseError (772603: Content not found)
+
+        409: Conflict - ResponseError (772606: Share code already used)
 
-        500: Internal Server Error - ResponseError (770102: Unable to check user ban status/Unable to save ugc content: unable to get channel | 770105: Unable to save ugc content: failed generate upload URL | 770103: Unable to save ugc content: shareCode exceed the limit)
+        500: Internal Server Error - ResponseError (772602: Unable to check user ban status/Unable to get updated ugc content)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 201:
-            return ModelsCreateContentResponse.create_from_dict(content), None
+        if code == 200:
+            return ModelsCreateContentResponseV2.create_from_dict(content), None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 403:
             return None, ResponseError.create_from_dict(content)
+        if code == 404:
+            return None, ResponseError.create_from_dict(content)
+        if code == 409:
+            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: ModelsPublicCreateContentRequestS3,
+        body: ModelsUpdateContentShareCodeRequest,
         channel_id: str,
+        content_id: str,
         namespace: str,
         user_id: str,
         **kwargs,
-    ) -> CreateContentS3:
+    ) -> UpdateContentShareCodeV2:
         instance = cls()
         instance.body = body
         instance.channel_id = channel_id
+        instance.content_id = content_id
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> CreateContentS3:
+    ) -> UpdateContentShareCodeV2:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsPublicCreateContentRequestS3.create_from_dict(
+            instance.body = ModelsUpdateContentShareCodeRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsPublicCreateContentRequestS3()
+            instance.body = ModelsUpdateContentShareCodeRequest()
         if "channelId" in dict_ and dict_["channelId"] is not None:
             instance.channel_id = str(dict_["channelId"])
         elif include_empty:
             instance.channel_id = ""
+        if "contentId" in dict_ and dict_["contentId"] is not None:
+            instance.content_id = str(dict_["contentId"])
+        elif include_empty:
+            instance.content_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "userId" in dict_ and dict_["userId"] is not None:
             instance.user_id = str(dict_["userId"])
         elif include_empty:
@@ -301,21 +327,23 @@
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "body": "body",
             "channelId": "channel_id",
+            "contentId": "content_id",
             "namespace": "namespace",
             "userId": "user_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "body": True,
             "channelId": True,
+            "contentId": True,
             "namespace": True,
             "userId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/delete_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/delete_content.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/delete_content_screenshot.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/delete_content_screenshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,17 @@
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
 class DeleteContentScreenshot(Operation):
-    """Delete screenshots content (DeleteContentScreenshot)
+    """Delete content's screenshot (DeleteContentScreenshot)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing screenshot from a content
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots/{screenshotId}
 
         method: DELETE
 
         tags: ["Public Content (Legacy)"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_delete_content_b_e67ae8.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_delete_content_b_e67ae8.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_download_content_2d5c80.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_download_content_2d5c80.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_download_content_32df1f.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_download_content_32df1f.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_download_content_511956.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_download_content_511956.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_get_content_bulk.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_get_content_bulk.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_get_content_bulk_382fb9.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_get_content_bulk_382fb9.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_get_user_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_get_user_content.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_search_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_search_content.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_update_content_b_7f10f2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/public_update_content_b_7f10f2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/search_channel_specific_10d5e8.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/search_channel_specific_10d5e8.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_content_direct.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_content_direct.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_content_s3.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_content_s3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_content_share_code.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_content_share_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_screenshots.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/update_screenshots.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 from ...models import ModelsUpdateScreenshotResponse
 from ...models import ResponseError
 
 
 class UpdateScreenshots(Operation):
     """Update screenshot of content (UpdateScreenshots)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots
 
         method: PUT
 
         tags: ["Public Content (Legacy)"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/upload_content_screenshot.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_legacy/upload_content_screenshot.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,23 +33,19 @@
 from ...models import ModelsCreateScreenshotResponse
 from ...models import ResponseError
 
 
 class UploadContentScreenshot(Operation):
     """Upload screenshots for content (UploadContentScreenshot)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-    All request body are required except for contentType field.
-    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the presigned URL.
-    If not specified, it will use fileExtension value.
-    Supported file extensions: pjp, jpg, jpeg, jfif, bmp, png.
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    All request body are required except for *contentType* field.
+    *contentType* values is used to enforce the *Content-Type* header needed by the client to upload the content using the presigned URL.
+    If not specified, it will use *fileExtension* value.
+    Supported file extensions: *pjp*, *jpg*, *jpeg*, *jfif*, *bmp*, *png*.
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots
 
         method: POST
 
         tags: ["Public Content (Legacy)"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_content_screenshot_v2 import DeleteContentScreenshotV2
 from .public_bulk_get_content_a86be5 import PublicBulkGetContentByIDV2
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/delete_content_screenshot_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/delete_content_screenshot_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class DeleteContentScreenshotV2(Operation):
     """Delete screenshots content (DeleteContentScreenshotV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete screenshot from a content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots/{screenshotId}
 
         method: DELETE
 
         tags: ["Public Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_bulk_get_content_a86be5.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_channel/admin_create_channel.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,62 +25,63 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsContentDownloadResponseV2
-from ...models import ModelsPublicGetContentBulkRequest
+from ...models import ModelsChannelRequest
+from ...models import ModelsChannelResponse
 from ...models import ResponseError
 
 
-class PublicBulkGetContentByIDV2(Operation):
-    """Get contents by content Ids  (PublicBulkGetContentByIDV2)
+class AdminCreateChannel(Operation):
+    """Create Channel (AdminCreateChannel)
 
-    Maximum requested Ids: 100.
-    Public user can access without token or if token specified, requires valid user token
+    Create official channel
 
     Properties:
-        url: /ugc/v2/public/namespaces/{namespace}/contents/bulk
+        url: /ugc/v1/admin/namespaces/{namespace}/channels
 
         method: POST
 
-        tags: ["Public Content V2"]
+        tags: ["Admin Channel"]
 
-        consumes: ["application/json", "application/octet-stream"]
+        consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsPublicGetContentBulkRequest in body
+        body: (body) REQUIRED ModelsChannelRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - List[ModelsContentDownloadResponseV2] (Get contents by content Ids)
+        201: Created - ModelsChannelResponse (Channel created)
 
-        400: Bad Request - ResponseError (773900: Malformed request/Invalid request body)
+        400: Bad Request - ResponseError (770503: Invalid channel {ID}: should uuid without hypen)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (770801: Unable to get ugc content: database/Unable to get creator | 773902: Failed generate download URL)
+        409: Conflict - ResponseError (770504: Channel already exist)
+
+        500: Internal Server Error - ResponseError (770502: Unable to save channel)
     """
 
     # region fields
 
-    _url: str = "/ugc/v2/public/namespaces/{namespace}/contents/bulk"
+    _url: str = "/ugc/v1/admin/namespaces/{namespace}/channels"
     _method: str = "POST"
-    _consumes: List[str] = ["application/json", "application/octet-stream"]
+    _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsPublicGetContentBulkRequest  # REQUIRED in [body]
+    body: ModelsChannelRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
@@ -136,115 +137,114 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(
-        self, value: ModelsPublicGetContentBulkRequest
-    ) -> PublicBulkGetContentByIDV2:
+    def with_body(self, value: ModelsChannelRequest) -> AdminCreateChannel:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> PublicBulkGetContentByIDV2:
+    def with_namespace(self, value: str) -> AdminCreateChannel:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsPublicGetContentBulkRequest()
+            result["body"] = ModelsChannelRequest()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, List[ModelsContentDownloadResponseV2]],
-        Union[None, HttpResponse, ResponseError],
+        Union[None, ModelsChannelResponse], Union[None, HttpResponse, ResponseError]
     ]:
         """Parse the given response.
 
-        200: OK - List[ModelsContentDownloadResponseV2] (Get contents by content Ids)
+        201: Created - ModelsChannelResponse (Channel created)
 
-        400: Bad Request - ResponseError (773900: Malformed request/Invalid request body)
+        400: Bad Request - ResponseError (770503: Invalid channel {ID}: should uuid without hypen)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (770801: Unable to get ugc content: database/Unable to get creator | 773902: Failed generate download URL)
+        409: Conflict - ResponseError (770504: Channel already exist)
+
+        500: Internal Server Error - ResponseError (770502: Unable to save channel)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return [
-                ModelsContentDownloadResponseV2.create_from_dict(i) for i in content
-            ], None
+        if code == 201:
+            return ModelsChannelResponse.create_from_dict(content), None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
+        if code == 409:
+            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, body: ModelsPublicGetContentBulkRequest, namespace: str, **kwargs
-    ) -> PublicBulkGetContentByIDV2:
+        cls, body: ModelsChannelRequest, namespace: str, **kwargs
+    ) -> AdminCreateChannel:
         instance = cls()
         instance.body = body
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublicBulkGetContentByIDV2:
+    ) -> AdminCreateChannel:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsPublicGetContentBulkRequest.create_from_dict(
+            instance.body = ModelsChannelRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsPublicGetContentBulkRequest()
+            instance.body = ModelsChannelRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_create_content_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_create_content_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsCreateContentResponseV2
 from ...models import ResponseError
 
 
 class PublicCreateContentV2(Operation):
     """Create a content (PublicCreateContentV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    Create a new content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents
 
         method: POST
 
         tags: ["Public Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_delete_content_b_4792d8.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_delete_content_b_4792d8.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class PublicDeleteContentByShareCodeV2(Operation):
     """Delete content by share code (PublicDeleteContentByShareCodeV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing content by share code
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/sharecodes/{shareCode}
 
         method: DELETE
 
         tags: ["Public Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_delete_content_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_delete_content_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class PublicDeleteContentV2(Operation):
     """Delete content (PublicDeleteContentV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}
 
         method: DELETE
 
         tags: ["Public Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_generate_content_ffec28.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_generate_content_ffec28.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsGenerateContentUploadURLResponse
 from ...models import ResponseError
 
 
 class PublicGenerateContentUploadURLV2(Operation):
     """Generate content upload URL (PublicGenerateContentUploadURLV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Generate content upload URL
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/uploadUrl
 
         method: PATCH
 
         tags: ["Public Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_bulk_503347.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_bulk_503347.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_c_87966e.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_c_87966e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_idv2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_idv2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_s_4f7083.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_s_4f7083.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_u_635e0b.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_get_content_by_u_635e0b.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_list_content_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_list_content_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,28 +32,31 @@
 from ...models import ModelsPaginatedContentDownloadResponseV2
 from ...models import ResponseError
 
 
 class PublicListContentV2(Operation):
     """List contents (PublicListContentV2)
 
-    For advance tag filtering supports & as AND operator and | as OR operator and parentheses () for priority. e.g:
+    For advance tag filtering supports & as AND operator and | as OR operator and parentheses ( ) for priority. e.g:
 
-    `tags=red`
-    `tags=red&animal;`
-    `tags=red|animal`
-    `tags=red&animal;|wild`
-    `tags=red&(animal|wild)`
+
+    *tags=red*
+    *tags=red&animal;*
+    *tags=red|animal*
+    *tags=red&animal;|wild*
+    *tags=red&(animal|wild)*
 
     The precedence of logical operator is AND > OR, so if no parentheses, AND logical operator will be executed first.
 
-    Allowed character for operand: alphanumeric, underscore `_` and dash `-`
-    Allowed character for operator: `&` `|` `(` `)`
+    Allowed character for operand: alphanumeric, underscore _ and dash -
+
+    Allowed character for operator: & | ( )
+
 
-     Please note that value of tags query param should be URL encoded
+    **Please note that value of tags query param should be URL encoded**
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/contents
 
         method: GET
 
         tags: ["Public Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_update_content_b_0c4d9c.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_update_content_b_0c4d9c.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsUpdateContentRequestV2
 from ...models import ResponseError
 
 
 class PublicUpdateContentByShareCodeV2(Operation):
     """Update content to S3 bucket by share code (PublicUpdateContentByShareCodeV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update content by share code
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/s3/sharecodes/{shareCode}
 
         method: PUT
 
         tags: ["Public Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_update_content_f_55e48b.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_update_content_f_55e48b.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 from ...models import ModelsUpdateFileLocationRequest
 from ...models import ResponseError
 
 
 class PublicUpdateContentFileLocation(Operation):
     """Update content file location (PublicUpdateContentFileLocation)
 
-    This endpoint should be used after calling generate upload url endpoint to commit the changes.
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    This endpoint should be used after calling generate upload url endpoint to commit the changes
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/fileLocation
 
         method: PATCH
 
         tags: ["Public Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_update_content_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/public_update_content_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsUpdateContentResponseV2
 from ...models import ResponseError
 
 
 class PublicUpdateContentV2(Operation):
     """Update content (PublicUpdateContentV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update existing content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}
 
         method: PATCH
 
         tags: ["Public Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/update_content_share_code_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/public_get_group_contents_v2.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,86 +25,74 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsCreateContentResponseV2
-from ...models import ModelsUpdateContentShareCodeRequest
+from ...models import ModelsPaginatedContentDownloadResponseV2
 from ...models import ResponseError
 
 
-class UpdateContentShareCodeV2(Operation):
-    """Update content share code (UpdateContentShareCodeV2)
+class PublicGetGroupContentsV2(Operation):
+    """Get contents belong to a group (PublicGetGroupContentsV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT:SHARECODE [UPDATE].
-
-    This endpoint is used to modify the shareCode of a content. However, this operation is restricted by default and requires the above permission to be granted to the User role.
-
-    `shareCode` format should follows:
-    Max length: 7
-    Available characters: abcdefhkpqrstuxyz
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT:SHARECODE [UPDATE]
+    Get content belong to a group
 
     Properties:
-        url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/sharecode
+        url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents
 
-        method: PATCH
+        method: GET
 
-        tags: ["Public Content V2"]
+        tags: ["Public Group"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsUpdateContentShareCodeRequest in body
-
-        channel_id: (channelId) REQUIRED str in path
-
-        content_id: (contentId) REQUIRED str in path
+        group_id: (groupId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
-    Responses:
-        200: OK - ModelsCreateContentResponseV2 (Update content sharecode)
+        limit: (limit) OPTIONAL int in query
 
-        400: Bad Request - ResponseError (772601: Malformed request | 772607: Unable to update ugc content: invalid shareCode format)
+        offset: (offset) OPTIONAL int in query
 
-        401: Unauthorized - ResponseError (20001: unauthorized access)
+    Responses:
+        200: OK - ModelsPaginatedContentDownloadResponseV2 (Get content belong to a group)
 
-        403: Forbidden - ResponseError (772604: User has been banned to update content | 20013: insufficient permission)
+        400: Bad Request - ResponseError (773101: invalid paging parameter)
 
-        404: Not Found - ResponseError (772603: Content not found)
+        401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        409: Conflict - ResponseError (772606: Share code already used)
+        404: Not Found - ResponseError (773103: No group content was found)
 
-        500: Internal Server Error - ResponseError (772602: Unable to check user ban status/Unable to get updated ugc content)
+        500: Internal Server Error - ResponseError (773102: Unable to get ugc content: database error | 770901: Unable to get ugc content: database error/Unable to get creator | 770801: Unable to get ugc content: database/Unable to get creator | 770903: Failed generate download URL)
     """
 
     # region fields
 
-    _url: str = "/ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/sharecode"
-    _method: str = "PATCH"
+    _url: str = (
+        "/ugc/v2/public/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents"
+    )
+    _method: str = "GET"
     _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsUpdateContentShareCodeRequest  # REQUIRED in [body]
-    channel_id: str  # REQUIRED in [path]
-    content_id: str  # REQUIRED in [path]
+    group_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
+    limit: int  # OPTIONAL in [query]
+    offset: int  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -136,119 +124,114 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
-            "body": self.get_body_params(),
             "path": self.get_path_params(),
+            "query": self.get_query_params(),
         }
 
-    def get_body_params(self) -> Any:
-        if not hasattr(self, "body") or self.body is None:
-            return None
-        return self.body.to_dict()
-
     def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "channel_id"):
-            result["channelId"] = self.channel_id
-        if hasattr(self, "content_id"):
-            result["contentId"] = self.content_id
+        if hasattr(self, "group_id"):
+            result["groupId"] = self.group_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         if hasattr(self, "user_id"):
             result["userId"] = self.user_id
         return result
 
+    def get_query_params(self) -> dict:
+        result = {}
+        if hasattr(self, "limit"):
+            result["limit"] = self.limit
+        if hasattr(self, "offset"):
+            result["offset"] = self.offset
+        return result
+
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(
-        self, value: ModelsUpdateContentShareCodeRequest
-    ) -> UpdateContentShareCodeV2:
-        self.body = value
+    def with_group_id(self, value: str) -> PublicGetGroupContentsV2:
+        self.group_id = value
         return self
 
-    def with_channel_id(self, value: str) -> UpdateContentShareCodeV2:
-        self.channel_id = value
+    def with_namespace(self, value: str) -> PublicGetGroupContentsV2:
+        self.namespace = value
         return self
 
-    def with_content_id(self, value: str) -> UpdateContentShareCodeV2:
-        self.content_id = value
+    def with_user_id(self, value: str) -> PublicGetGroupContentsV2:
+        self.user_id = value
         return self
 
-    def with_namespace(self, value: str) -> UpdateContentShareCodeV2:
-        self.namespace = value
+    def with_limit(self, value: int) -> PublicGetGroupContentsV2:
+        self.limit = value
         return self
 
-    def with_user_id(self, value: str) -> UpdateContentShareCodeV2:
-        self.user_id = value
+    def with_offset(self, value: int) -> PublicGetGroupContentsV2:
+        self.offset = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "body") and self.body:
-            result["body"] = self.body.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["body"] = ModelsUpdateContentShareCodeRequest()
-        if hasattr(self, "channel_id") and self.channel_id:
-            result["channelId"] = str(self.channel_id)
+        if hasattr(self, "group_id") and self.group_id:
+            result["groupId"] = str(self.group_id)
         elif include_empty:
-            result["channelId"] = ""
-        if hasattr(self, "content_id") and self.content_id:
-            result["contentId"] = str(self.content_id)
-        elif include_empty:
-            result["contentId"] = ""
+            result["groupId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         if hasattr(self, "user_id") and self.user_id:
             result["userId"] = str(self.user_id)
         elif include_empty:
             result["userId"] = ""
+        if hasattr(self, "limit") and self.limit:
+            result["limit"] = int(self.limit)
+        elif include_empty:
+            result["limit"] = 0
+        if hasattr(self, "offset") and self.offset:
+            result["offset"] = int(self.offset)
+        elif include_empty:
+            result["offset"] = 0
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsCreateContentResponseV2],
+        Union[None, ModelsPaginatedContentDownloadResponseV2],
         Union[None, HttpResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - ModelsCreateContentResponseV2 (Update content sharecode)
+        200: OK - ModelsPaginatedContentDownloadResponseV2 (Get content belong to a group)
 
-        400: Bad Request - ResponseError (772601: Malformed request | 772607: Unable to update ugc content: invalid shareCode format)
+        400: Bad Request - ResponseError (773101: invalid paging parameter)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        403: Forbidden - ResponseError (772604: User has been banned to update content | 20013: insufficient permission)
-
-        404: Not Found - ResponseError (772603: Content not found)
+        404: Not Found - ResponseError (773103: No group content was found)
 
-        409: Conflict - ResponseError (772606: Share code already used)
-
-        500: Internal Server Error - ResponseError (772602: Unable to check user ban status/Unable to get updated ugc content)
+        500: Internal Server Error - ResponseError (773102: Unable to get ugc content: database error | 770901: Unable to get ugc content: database error/Unable to get creator | 770801: Unable to get ugc content: database/Unable to get creator | 770903: Failed generate download URL)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -256,99 +239,98 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsCreateContentResponseV2.create_from_dict(content), None
+            return (
+                ModelsPaginatedContentDownloadResponseV2.create_from_dict(content),
+                None,
+            )
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
-        if code == 403:
-            return None, ResponseError.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
-        if code == 409:
-            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: ModelsUpdateContentShareCodeRequest,
-        channel_id: str,
-        content_id: str,
+        group_id: str,
         namespace: str,
         user_id: str,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
         **kwargs,
-    ) -> UpdateContentShareCodeV2:
+    ) -> PublicGetGroupContentsV2:
         instance = cls()
-        instance.body = body
-        instance.channel_id = channel_id
-        instance.content_id = content_id
+        instance.group_id = group_id
         instance.namespace = namespace
         instance.user_id = user_id
+        if limit is not None:
+            instance.limit = limit
+        if offset is not None:
+            instance.offset = offset
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> UpdateContentShareCodeV2:
+    ) -> PublicGetGroupContentsV2:
         instance = cls()
-        if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsUpdateContentShareCodeRequest.create_from_dict(
-                dict_["body"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.body = ModelsUpdateContentShareCodeRequest()
-        if "channelId" in dict_ and dict_["channelId"] is not None:
-            instance.channel_id = str(dict_["channelId"])
+        if "groupId" in dict_ and dict_["groupId"] is not None:
+            instance.group_id = str(dict_["groupId"])
         elif include_empty:
-            instance.channel_id = ""
-        if "contentId" in dict_ and dict_["contentId"] is not None:
-            instance.content_id = str(dict_["contentId"])
-        elif include_empty:
-            instance.content_id = ""
+            instance.group_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "userId" in dict_ and dict_["userId"] is not None:
             instance.user_id = str(dict_["userId"])
         elif include_empty:
             instance.user_id = ""
+        if "limit" in dict_ and dict_["limit"] is not None:
+            instance.limit = int(dict_["limit"])
+        elif include_empty:
+            instance.limit = 0
+        if "offset" in dict_ and dict_["offset"] is not None:
+            instance.offset = int(dict_["offset"])
+        elif include_empty:
+            instance.offset = 0
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "body": "body",
-            "channelId": "channel_id",
-            "contentId": "content_id",
+            "groupId": "group_id",
             "namespace": "namespace",
             "userId": "user_id",
+            "limit": "limit",
+            "offset": "offset",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "body": True,
-            "channelId": True,
-            "contentId": True,
+            "groupId": True,
             "namespace": True,
             "userId": True,
+            "limit": False,
+            "offset": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/update_screenshots_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/update_screenshots_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 from ...models import ModelsUpdateScreenshotResponse
 from ...models import ResponseError
 
 
 class UpdateScreenshotsV2(Operation):
     """Update screenshot of content (UpdateScreenshotsV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots
 
         method: PUT
 
         tags: ["Public Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/upload_content_screenshot_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_content_v2/upload_content_screenshot_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,23 +33,18 @@
 from ...models import ModelsCreateScreenshotResponse
 from ...models import ResponseError
 
 
 class UploadContentScreenshotV2(Operation):
     """Upload screenshots for content (UploadContentScreenshotV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-    All request body are required except for contentType field.
-    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the presigned URL.
-    If not specified, it will use fileExtension value.
+    This endpoint used to request upload URL from content's screenshot.
+    If *contentType* is not specified, it will use *fileExtension* value.
     Supported file extensions: pjp, jpg, jpeg, jfif, bmp, png.
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots
 
         method: POST
 
         tags: ["Public Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_creator/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_creator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_get_creator import PublicGetCreator
 from .public_search_creator import PublicSearchCreator
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_creator/public_get_creator.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_creator/public_get_creator.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_creator/public_search_creator.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_creator/public_search_creator.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_legacy/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
-from .add_download_count import AddDownloadCount
+from .public_list_content_like_v2 import PublicListContentLikeV2
+from .update_content_like_status_v2 import UpdateContentLikeStatusV2
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_legacy/add_download_count.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_legacy/add_download_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from ...models import ModelsAddDownloadCountResponse
 from ...models import ResponseError
 
 
 class AddDownloadCount(Operation):
     """Add unique download count to a content (AddDownloadCount)
 
-    Requires valid user token
+    This endpoint can be used to count how many the ugc downloaded
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/contents/{contentId}/downloadcount
 
         method: POST
 
         tags: ["Public Download Count (Legacy)"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_add_download_count_v2 import PublicAddDownloadCountV2
 from .public_list_content_dow_d23b3d import PublicListContentDownloaderV2
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/public_add_download_count_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/public_add_download_count_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from ...models import ModelsAddDownloadCountResponse
 from ...models import ResponseError
 
 
 class PublicAddDownloadCountV2(Operation):
     """Add unique download count to a content (PublicAddDownloadCountV2)
 
-    Requires valid user token
+    This endpoint can be used to count how many the ugc downloaded
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/contents/{contentId}/downloadcount
 
         method: POST
 
         tags: ["Public Download Count V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/public_list_content_dow_d23b3d.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_v2/public_list_content_dow_d23b3d.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_follow/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_follow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_followed_content import GetFollowedContent
 from .get_followed_users import GetFollowedUsers
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_followed_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_followed_content.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_followed_users.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_followed_users.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_public_followers.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_public_followers.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_public_following.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_follow/get_public_following.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_follow/update_user_follow_status.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_follow/update_user_follow_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_group import CreateGroup
 from .delete_group import DeleteGroup
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/create_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/get_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,66 +25,62 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsCreateGroupRequest
 from ...models import ModelsCreateGroupResponse
 from ...models import ResponseError
 
 
-class CreateGroup(Operation):
-    """Create groups (CreateGroup)
+class GetGroup(Operation):
+    """Get user's groups (GetGroup)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [CREATE]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [CREATE]
+    Get user groups by group ID
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
-        method: POST
+        method: GET
 
         tags: ["Public Group"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsCreateGroupRequest in body
+        group_id: (groupId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        201: Created - ModelsCreateGroupResponse (Group Created)
-
-        400: Bad Request - ResponseError (772101: Malformed request/Invalid request body)
+        200: OK - ModelsCreateGroupResponse (Get user's group)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (772102: Unable to create group)
+        404: Not Found - ResponseError (773002: Group not found)
+
+        500: Internal Server Error - ResponseError (773001: Unable get group)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/public/namespaces/{namespace}/users/{userId}/groups"
-    _method: str = "POST"
+    _url: str = "/ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}"
+    _method: str = "GET"
     _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsCreateGroupRequest  # REQUIRED in [body]
+    group_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
@@ -118,61 +114,57 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
-            "body": self.get_body_params(),
             "path": self.get_path_params(),
         }
 
-    def get_body_params(self) -> Any:
-        if not hasattr(self, "body") or self.body is None:
-            return None
-        return self.body.to_dict()
-
     def get_path_params(self) -> dict:
         result = {}
+        if hasattr(self, "group_id"):
+            result["groupId"] = self.group_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         if hasattr(self, "user_id"):
             result["userId"] = self.user_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsCreateGroupRequest) -> CreateGroup:
-        self.body = value
+    def with_group_id(self, value: str) -> GetGroup:
+        self.group_id = value
         return self
 
-    def with_namespace(self, value: str) -> CreateGroup:
+    def with_namespace(self, value: str) -> GetGroup:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> CreateGroup:
+    def with_user_id(self, value: str) -> GetGroup:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "body") and self.body:
-            result["body"] = self.body.to_dict(include_empty=include_empty)
+        if hasattr(self, "group_id") and self.group_id:
+            result["groupId"] = str(self.group_id)
         elif include_empty:
-            result["body"] = ModelsCreateGroupRequest()
+            result["groupId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         if hasattr(self, "user_id") and self.user_id:
             result["userId"] = str(self.user_id)
         elif include_empty:
@@ -187,93 +179,89 @@
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
         Union[None, ModelsCreateGroupResponse], Union[None, HttpResponse, ResponseError]
     ]:
         """Parse the given response.
 
-        201: Created - ModelsCreateGroupResponse (Group Created)
-
-        400: Bad Request - ResponseError (772101: Malformed request/Invalid request body)
+        200: OK - ModelsCreateGroupResponse (Get user's group)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (772102: Unable to create group)
+        404: Not Found - ResponseError (773002: Group not found)
+
+        500: Internal Server Error - ResponseError (773001: Unable get group)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 201:
+        if code == 200:
             return ModelsCreateGroupResponse.create_from_dict(content), None
-        if code == 400:
-            return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
+        if code == 404:
+            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(
-        cls, body: ModelsCreateGroupRequest, namespace: str, user_id: str, **kwargs
-    ) -> CreateGroup:
+    def create(cls, group_id: str, namespace: str, user_id: str, **kwargs) -> GetGroup:
         instance = cls()
-        instance.body = body
+        instance.group_id = group_id
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> CreateGroup:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> GetGroup:
         instance = cls()
-        if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsCreateGroupRequest.create_from_dict(
-                dict_["body"], include_empty=include_empty
-            )
+        if "groupId" in dict_ and dict_["groupId"] is not None:
+            instance.group_id = str(dict_["groupId"])
         elif include_empty:
-            instance.body = ModelsCreateGroupRequest()
+            instance.group_id = ""
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
-            "body": "body",
+            "groupId": "group_id",
             "namespace": "namespace",
             "userId": "user_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "body": True,
+            "groupId": True,
             "namespace": True,
             "userId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/delete_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/delete_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class DeleteGroup(Operation):
     """Delete group (DeleteGroup)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    Delete user group by group ID
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
         method: DELETE
 
         tags: ["Public Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/get_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_tag/get_tag.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,67 +25,64 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsCreateGroupResponse
+from ...models import ModelsPaginatedGetTagResponse
 from ...models import ResponseError
 
 
-class GetGroup(Operation):
-    """Get user's groups (GetGroup)
+class GetTag(Operation):
+    """Get tags (GetTag)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get available tags paginated
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}
+        url: /ugc/v1/public/namespaces/{namespace}/tags
 
         method: GET
 
-        tags: ["Public Group"]
+        tags: ["Public Tag"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        group_id: (groupId) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
-        user_id: (userId) REQUIRED str in path
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
 
     Responses:
-        200: OK - ModelsCreateGroupResponse (Get user's group)
+        200: OK - ModelsPaginatedGetTagResponse (Get tags)
 
-        401: Unauthorized - ResponseError (20001: unauthorized access)
+        400: Bad Request - ResponseError (771501: invalid paging parameter)
 
-        404: Not Found - ResponseError (773002: Group not found)
+        401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (773001: Unable get group)
+        500: Internal Server Error - ResponseError (771502: Unable get user tags)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}"
+    _url: str = "/ugc/v1/public/namespaces/{namespace}/tags"
     _method: str = "GET"
     _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    group_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
-    user_id: str  # REQUIRED in [path]
+    limit: int  # OPTIONAL in [query]
+    offset: int  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -118,85 +115,91 @@
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
             "path": self.get_path_params(),
+            "query": self.get_query_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "group_id"):
-            result["groupId"] = self.group_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
-        if hasattr(self, "user_id"):
-            result["userId"] = self.user_id
+        return result
+
+    def get_query_params(self) -> dict:
+        result = {}
+        if hasattr(self, "limit"):
+            result["limit"] = self.limit
+        if hasattr(self, "offset"):
+            result["offset"] = self.offset
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_group_id(self, value: str) -> GetGroup:
-        self.group_id = value
+    def with_namespace(self, value: str) -> GetTag:
+        self.namespace = value
         return self
 
-    def with_namespace(self, value: str) -> GetGroup:
-        self.namespace = value
+    def with_limit(self, value: int) -> GetTag:
+        self.limit = value
         return self
 
-    def with_user_id(self, value: str) -> GetGroup:
-        self.user_id = value
+    def with_offset(self, value: int) -> GetTag:
+        self.offset = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "group_id") and self.group_id:
-            result["groupId"] = str(self.group_id)
-        elif include_empty:
-            result["groupId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "user_id") and self.user_id:
-            result["userId"] = str(self.user_id)
+        if hasattr(self, "limit") and self.limit:
+            result["limit"] = int(self.limit)
+        elif include_empty:
+            result["limit"] = 0
+        if hasattr(self, "offset") and self.offset:
+            result["offset"] = int(self.offset)
         elif include_empty:
-            result["userId"] = ""
+            result["offset"] = 0
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsCreateGroupResponse], Union[None, HttpResponse, ResponseError]
+        Union[None, ModelsPaginatedGetTagResponse],
+        Union[None, HttpResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - ModelsCreateGroupResponse (Get user's group)
+        200: OK - ModelsPaginatedGetTagResponse (Get tags)
 
-        401: Unauthorized - ResponseError (20001: unauthorized access)
+        400: Bad Request - ResponseError (771501: invalid paging parameter)
 
-        404: Not Found - ResponseError (773002: Group not found)
+        401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (773001: Unable get group)
+        500: Internal Server Error - ResponseError (771502: Unable get user tags)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -204,67 +207,75 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsCreateGroupResponse.create_from_dict(content), None
-        if code == 401:
+            return ModelsPaginatedGetTagResponse.create_from_dict(content), None
+        if code == 400:
             return None, ResponseError.create_from_dict(content)
-        if code == 404:
+        if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, group_id: str, namespace: str, user_id: str, **kwargs) -> GetGroup:
+    def create(
+        cls,
+        namespace: str,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        **kwargs,
+    ) -> GetTag:
         instance = cls()
-        instance.group_id = group_id
         instance.namespace = namespace
-        instance.user_id = user_id
+        if limit is not None:
+            instance.limit = limit
+        if offset is not None:
+            instance.offset = offset
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> GetGroup:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> GetTag:
         instance = cls()
-        if "groupId" in dict_ and dict_["groupId"] is not None:
-            instance.group_id = str(dict_["groupId"])
-        elif include_empty:
-            instance.group_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "userId" in dict_ and dict_["userId"] is not None:
-            instance.user_id = str(dict_["userId"])
+        if "limit" in dict_ and dict_["limit"] is not None:
+            instance.limit = int(dict_["limit"])
+        elif include_empty:
+            instance.limit = 0
+        if "offset" in dict_ and dict_["offset"] is not None:
+            instance.offset = int(dict_["offset"])
         elif include_empty:
-            instance.user_id = ""
+            instance.offset = 0
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "groupId": "group_id",
             "namespace": "namespace",
-            "userId": "user_id",
+            "limit": "limit",
+            "offset": "offset",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "groupId": True,
             "namespace": True,
-            "userId": True,
+            "limit": False,
+            "offset": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/get_group_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/get_group_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedContentDownloadResponse
 from ...models import ResponseError
 
 
 class GetGroupContent(Operation):
     """(Legacy) Get contents belong to a group (GetGroupContent)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get content that belong to a group
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents
 
         method: GET
 
         tags: ["Public Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/get_groups.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/get_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsPaginatedGroupResponse
 from ...models import ResponseError
 
 
 class GetGroups(Operation):
     """Get all user groups (GetGroups)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get user groups paginated
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups
 
         method: GET
 
         tags: ["Public Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/public_get_group_contents_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/public_list_content_like_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,77 +25,70 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsPaginatedContentDownloadResponseV2
+from ...models import ModelsPaginatedContentLikersResponse
 from ...models import ResponseError
 
 
-class PublicGetGroupContentsV2(Operation):
-    """Get contents belong to a group (PublicGetGroupContentsV2)
+class PublicListContentLikeV2(Operation):
+    """Retrieve list of user that like specified content. (PublicListContentLikeV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    This endpoint will only display the list of users who performed like from v2 endpoint.
 
     Properties:
-        url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents
+        url: /ugc/v2/public/namespaces/{namespace}/contents/{contentId}/like
 
         method: GET
 
-        tags: ["Public Group"]
+        tags: ["Public Like V2"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        group_id: (groupId) REQUIRED str in path
+        content_id: (contentId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
-        user_id: (userId) REQUIRED str in path
-
         limit: (limit) OPTIONAL int in query
 
         offset: (offset) OPTIONAL int in query
 
+        sort_by: (sortBy) OPTIONAL str in query
+
     Responses:
-        200: OK - ModelsPaginatedContentDownloadResponseV2 (Get content belong to a group)
+        200: OK - ModelsPaginatedContentLikersResponse (Retrieve list of user liked content)
 
-        400: Bad Request - ResponseError (773101: invalid paging parameter)
+        400: Bad Request - ResponseError (771004: invalid paging parameter)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773103: No group content was found)
-
-        500: Internal Server Error - ResponseError (773102: Unable to get ugc content: database error | 770901: Unable to get ugc content: database error/Unable to get creator | 770801: Unable to get ugc content: database/Unable to get creator | 770903: Failed generate download URL)
+        500: Internal Server Error - ResponseError (771006: unable to get list of content like: database error)
     """
 
     # region fields
 
-    _url: str = (
-        "/ugc/v2/public/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents"
-    )
+    _url: str = "/ugc/v2/public/namespaces/{namespace}/contents/{contentId}/like"
     _method: str = "GET"
     _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    group_id: str  # REQUIRED in [path]
+    content_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
-    user_id: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
+    sort_by: str  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -133,108 +126,106 @@
         return {
             "path": self.get_path_params(),
             "query": self.get_query_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "group_id"):
-            result["groupId"] = self.group_id
+        if hasattr(self, "content_id"):
+            result["contentId"] = self.content_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
-        if hasattr(self, "user_id"):
-            result["userId"] = self.user_id
         return result
 
     def get_query_params(self) -> dict:
         result = {}
         if hasattr(self, "limit"):
             result["limit"] = self.limit
         if hasattr(self, "offset"):
             result["offset"] = self.offset
+        if hasattr(self, "sort_by"):
+            result["sortBy"] = self.sort_by
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_group_id(self, value: str) -> PublicGetGroupContentsV2:
-        self.group_id = value
+    def with_content_id(self, value: str) -> PublicListContentLikeV2:
+        self.content_id = value
         return self
 
-    def with_namespace(self, value: str) -> PublicGetGroupContentsV2:
+    def with_namespace(self, value: str) -> PublicListContentLikeV2:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> PublicGetGroupContentsV2:
-        self.user_id = value
-        return self
-
-    def with_limit(self, value: int) -> PublicGetGroupContentsV2:
+    def with_limit(self, value: int) -> PublicListContentLikeV2:
         self.limit = value
         return self
 
-    def with_offset(self, value: int) -> PublicGetGroupContentsV2:
+    def with_offset(self, value: int) -> PublicListContentLikeV2:
         self.offset = value
         return self
 
+    def with_sort_by(self, value: str) -> PublicListContentLikeV2:
+        self.sort_by = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "group_id") and self.group_id:
-            result["groupId"] = str(self.group_id)
+        if hasattr(self, "content_id") and self.content_id:
+            result["contentId"] = str(self.content_id)
         elif include_empty:
-            result["groupId"] = ""
+            result["contentId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "user_id") and self.user_id:
-            result["userId"] = str(self.user_id)
-        elif include_empty:
-            result["userId"] = ""
         if hasattr(self, "limit") and self.limit:
             result["limit"] = int(self.limit)
         elif include_empty:
             result["limit"] = 0
         if hasattr(self, "offset") and self.offset:
             result["offset"] = int(self.offset)
         elif include_empty:
             result["offset"] = 0
+        if hasattr(self, "sort_by") and self.sort_by:
+            result["sortBy"] = str(self.sort_by)
+        elif include_empty:
+            result["sortBy"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsPaginatedContentDownloadResponseV2],
+        Union[None, ModelsPaginatedContentLikersResponse],
         Union[None, HttpResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - ModelsPaginatedContentDownloadResponseV2 (Get content belong to a group)
+        200: OK - ModelsPaginatedContentLikersResponse (Retrieve list of user liked content)
 
-        400: Bad Request - ResponseError (773101: invalid paging parameter)
+        400: Bad Request - ResponseError (771004: invalid paging parameter)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773103: No group content was found)
-
-        500: Internal Server Error - ResponseError (773102: Unable to get ugc content: database error | 770901: Unable to get ugc content: database error/Unable to get creator | 770801: Unable to get ugc content: database/Unable to get creator | 770903: Failed generate download URL)
+        500: Internal Server Error - ResponseError (771006: unable to get list of content like: database error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -242,98 +233,94 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return (
-                ModelsPaginatedContentDownloadResponseV2.create_from_dict(content),
-                None,
-            )
+            return ModelsPaginatedContentLikersResponse.create_from_dict(content), None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
-        if code == 404:
-            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        group_id: str,
+        content_id: str,
         namespace: str,
-        user_id: str,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
+        sort_by: Optional[str] = None,
         **kwargs,
-    ) -> PublicGetGroupContentsV2:
+    ) -> PublicListContentLikeV2:
         instance = cls()
-        instance.group_id = group_id
+        instance.content_id = content_id
         instance.namespace = namespace
-        instance.user_id = user_id
         if limit is not None:
             instance.limit = limit
         if offset is not None:
             instance.offset = offset
+        if sort_by is not None:
+            instance.sort_by = sort_by
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublicGetGroupContentsV2:
+    ) -> PublicListContentLikeV2:
         instance = cls()
-        if "groupId" in dict_ and dict_["groupId"] is not None:
-            instance.group_id = str(dict_["groupId"])
+        if "contentId" in dict_ and dict_["contentId"] is not None:
+            instance.content_id = str(dict_["contentId"])
         elif include_empty:
-            instance.group_id = ""
+            instance.content_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "userId" in dict_ and dict_["userId"] is not None:
-            instance.user_id = str(dict_["userId"])
-        elif include_empty:
-            instance.user_id = ""
         if "limit" in dict_ and dict_["limit"] is not None:
             instance.limit = int(dict_["limit"])
         elif include_empty:
             instance.limit = 0
         if "offset" in dict_ and dict_["offset"] is not None:
             instance.offset = int(dict_["offset"])
         elif include_empty:
             instance.offset = 0
+        if "sortBy" in dict_ and dict_["sortBy"] is not None:
+            instance.sort_by = str(dict_["sortBy"])
+        elif include_empty:
+            instance.sort_by = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "groupId": "group_id",
+            "contentId": "content_id",
             "namespace": "namespace",
-            "userId": "user_id",
             "limit": "limit",
             "offset": "offset",
+            "sortBy": "sort_by",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "groupId": True,
+            "contentId": True,
             "namespace": True,
-            "userId": True,
             "limit": False,
             "offset": False,
+            "sortBy": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_group/update_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_group/update_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 from ...models import ModelsCreateGroupResponse
 from ...models import ResponseError
 
 
 class UpdateGroup(Operation):
     """Update group (UpdateGroup)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
-    replace group name and contents with new ones
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
+    Replace group name and contents with new ones
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
         method: PUT
 
         tags: ["Public Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_liked_content import GetLikedContent
 from .update_content_like_status import UpdateContentLikeStatus
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/get_liked_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/get_liked_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,35 +32,31 @@
 from ...models import ModelsPaginatedContentDownloadResponse
 from ...models import ResponseError
 
 
 class GetLikedContent(Operation):
     """Get liked contents (GetLikedContent)
 
-    Requires valid user token.
+    For advance tag filtering supports & as AND operator and | as OR operator and parentheses ( ) for priority. e.g:
 
-    For advance tag filtering supports & as AND operator and | as OR operator and parentheses () for priority. e.g:
 
-    `tags=red`
-
-    `tags=red&animal;`
-
-    `tags=red|animal`
-
-    `tags=red&animal;|wild`
-
-    `tags=red&(animal|wild)`
+    *tags=red*
+    *tags=red&animal;*
+    *tags=red|animal*
+    *tags=red&animal;|wild*
+    *tags=red&(animal|wild)*
 
     The precedence of logical operator is AND > OR, so if no parentheses, AND logical operator will be executed first.
 
-    Allowed character for operand: alphanumeric, underscore `_` and dash `-`
+    Allowed character for operand: alphanumeric, underscore _ and dash -
+
+    Allowed character for operator: & | ( )
 
-    Allowed character for operator: `&` `|` `(` `)`
 
-     Please note that value of tags query param should be URL encoded
+    **Please note that value of tags query param should be URL encoded**
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/contents/liked
 
         method: GET
 
         tags: ["Public Like (Legacy)"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/update_content_like_status.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_legacy/update_content_like_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from ...models import ModelsContentLikeResponse
 from ...models import ResponseError
 
 
 class UpdateContentLikeStatus(Operation):
     """Update like/unlike status to a content (UpdateContentLikeStatus)
 
-    Requires valid user token
+    This endpoint will update like/unlike state from a content
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/contents/{contentId}/like
 
         method: PUT
 
         tags: ["Public Like (Legacy)"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_download_count_legacy/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
-from .public_list_content_like_v2 import PublicListContentLikeV2
-from .update_content_like_status_v2 import UpdateContentLikeStatusV2
+from .add_download_count import AddDownloadCount
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/public_list_content_like_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/list_user_staging_contents.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,70 +25,75 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsPaginatedContentLikersResponse
+from ...models import ModelsPaginatedListStagingContentResponse
 from ...models import ResponseError
 
 
-class PublicListContentLikeV2(Operation):
-    """Retrieve list of user that like specified content. (PublicListContentLikeV2)
+class ListUserStagingContents(Operation):
+    """List user staging contents (ListUserStagingContents)
 
-    This endpoint will only display the list of users who performed like from v2 endpoint.
+    List user staging contents
 
     Properties:
-        url: /ugc/v2/public/namespaces/{namespace}/contents/{contentId}/like
+        url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents
 
         method: GET
 
-        tags: ["Public Like V2"]
+        tags: ["Public Staging Content"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        content_id: (contentId) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
+        user_id: (userId) REQUIRED str in path
+
         limit: (limit) OPTIONAL int in query
 
         offset: (offset) OPTIONAL int in query
 
         sort_by: (sortBy) OPTIONAL str in query
 
+        status: (status) OPTIONAL str in query
+
     Responses:
-        200: OK - ModelsPaginatedContentLikersResponse (Retrieve list of user liked content)
+        200: OK - ModelsPaginatedListStagingContentResponse (list user's staging content)
 
-        400: Bad Request - ResponseError (771004: invalid paging parameter)
+        400: Bad Request - ResponseError (774301: invalid paging parameter)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (771006: unable to get list of content like: database error)
+        403: Forbidden - ResponseError (20013: insufficient permission)
+
+        500: Internal Server Error - ResponseError (774302: unable to get staging content | 774303: unable to generate presigned URL)
     """
 
     # region fields
 
-    _url: str = "/ugc/v2/public/namespaces/{namespace}/contents/{contentId}/like"
+    _url: str = "/ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents"
     _method: str = "GET"
     _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    content_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
+    user_id: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     sort_by: str  # OPTIONAL in [query]
+    status: str  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -126,106 +131,118 @@
         return {
             "path": self.get_path_params(),
             "query": self.get_query_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "content_id"):
-            result["contentId"] = self.content_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
+        if hasattr(self, "user_id"):
+            result["userId"] = self.user_id
         return result
 
     def get_query_params(self) -> dict:
         result = {}
         if hasattr(self, "limit"):
             result["limit"] = self.limit
         if hasattr(self, "offset"):
             result["offset"] = self.offset
         if hasattr(self, "sort_by"):
             result["sortBy"] = self.sort_by
+        if hasattr(self, "status"):
+            result["status"] = self.status
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_content_id(self, value: str) -> PublicListContentLikeV2:
-        self.content_id = value
+    def with_namespace(self, value: str) -> ListUserStagingContents:
+        self.namespace = value
         return self
 
-    def with_namespace(self, value: str) -> PublicListContentLikeV2:
-        self.namespace = value
+    def with_user_id(self, value: str) -> ListUserStagingContents:
+        self.user_id = value
         return self
 
-    def with_limit(self, value: int) -> PublicListContentLikeV2:
+    def with_limit(self, value: int) -> ListUserStagingContents:
         self.limit = value
         return self
 
-    def with_offset(self, value: int) -> PublicListContentLikeV2:
+    def with_offset(self, value: int) -> ListUserStagingContents:
         self.offset = value
         return self
 
-    def with_sort_by(self, value: str) -> PublicListContentLikeV2:
+    def with_sort_by(self, value: str) -> ListUserStagingContents:
         self.sort_by = value
         return self
 
+    def with_status(self, value: str) -> ListUserStagingContents:
+        self.status = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "content_id") and self.content_id:
-            result["contentId"] = str(self.content_id)
-        elif include_empty:
-            result["contentId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
+        if hasattr(self, "user_id") and self.user_id:
+            result["userId"] = str(self.user_id)
+        elif include_empty:
+            result["userId"] = ""
         if hasattr(self, "limit") and self.limit:
             result["limit"] = int(self.limit)
         elif include_empty:
             result["limit"] = 0
         if hasattr(self, "offset") and self.offset:
             result["offset"] = int(self.offset)
         elif include_empty:
             result["offset"] = 0
         if hasattr(self, "sort_by") and self.sort_by:
             result["sortBy"] = str(self.sort_by)
         elif include_empty:
             result["sortBy"] = ""
+        if hasattr(self, "status") and self.status:
+            result["status"] = str(self.status)
+        elif include_empty:
+            result["status"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsPaginatedContentLikersResponse],
+        Union[None, ModelsPaginatedListStagingContentResponse],
         Union[None, HttpResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - ModelsPaginatedContentLikersResponse (Retrieve list of user liked content)
+        200: OK - ModelsPaginatedListStagingContentResponse (list user's staging content)
 
-        400: Bad Request - ResponseError (771004: invalid paging parameter)
+        400: Bad Request - ResponseError (774301: invalid paging parameter)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (771006: unable to get list of content like: database error)
+        403: Forbidden - ResponseError (20013: insufficient permission)
+
+        500: Internal Server Error - ResponseError (774302: unable to get staging content | 774303: unable to generate presigned URL)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -233,94 +250,108 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsPaginatedContentLikersResponse.create_from_dict(content), None
+            return (
+                ModelsPaginatedListStagingContentResponse.create_from_dict(content),
+                None,
+            )
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
+        if code == 403:
+            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        content_id: str,
         namespace: str,
+        user_id: str,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         sort_by: Optional[str] = None,
+        status: Optional[str] = None,
         **kwargs,
-    ) -> PublicListContentLikeV2:
+    ) -> ListUserStagingContents:
         instance = cls()
-        instance.content_id = content_id
         instance.namespace = namespace
+        instance.user_id = user_id
         if limit is not None:
             instance.limit = limit
         if offset is not None:
             instance.offset = offset
         if sort_by is not None:
             instance.sort_by = sort_by
+        if status is not None:
+            instance.status = status
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublicListContentLikeV2:
+    ) -> ListUserStagingContents:
         instance = cls()
-        if "contentId" in dict_ and dict_["contentId"] is not None:
-            instance.content_id = str(dict_["contentId"])
-        elif include_empty:
-            instance.content_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
+        if "userId" in dict_ and dict_["userId"] is not None:
+            instance.user_id = str(dict_["userId"])
+        elif include_empty:
+            instance.user_id = ""
         if "limit" in dict_ and dict_["limit"] is not None:
             instance.limit = int(dict_["limit"])
         elif include_empty:
             instance.limit = 0
         if "offset" in dict_ and dict_["offset"] is not None:
             instance.offset = int(dict_["offset"])
         elif include_empty:
             instance.offset = 0
         if "sortBy" in dict_ and dict_["sortBy"] is not None:
             instance.sort_by = str(dict_["sortBy"])
         elif include_empty:
             instance.sort_by = ""
+        if "status" in dict_ and dict_["status"] is not None:
+            instance.status = str(dict_["status"])
+        elif include_empty:
+            instance.status = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "contentId": "content_id",
             "namespace": "namespace",
+            "userId": "user_id",
             "limit": "limit",
             "offset": "offset",
             "sortBy": "sort_by",
+            "status": "status",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "contentId": True,
             "namespace": True,
+            "userId": True,
             "limit": False,
             "offset": False,
             "sortBy": False,
+            "status": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/update_content_like_status_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_like_v2/update_content_like_status_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from ...models import ModelsContentLikeResponse
 from ...models import ResponseError
 
 
 class UpdateContentLikeStatusV2(Operation):
     """Update like/unlike status to a content (UpdateContentLikeStatusV2)
 
-    Requires valid user token
+    This endpoint will update like/unlike state from a content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/contents/{contentId}/like
 
         method: PUT
 
         tags: ["Public Like V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_user_staging_con_254bae import DeleteUserStagingContentByID
 from .get_user_staging_content_by_id import GetUserStagingContentByID
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/delete_user_staging_con_254bae.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/delete_user_staging_con_254bae.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ResponseError
 
 
 class DeleteUserStagingContentByID(Operation):
     """Delete user staging content by id (DeleteUserStagingContentByID)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete user staging content by ID
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents/{contentId}
 
         method: DELETE
 
         tags: ["Public Staging Content"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/get_user_staging_content_by_id.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/get_user_staging_content_by_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 from ...models import ModelsStagingContentResponse
 from ...models import ResponseError
 
 
 class GetUserStagingContentByID(Operation):
     """Get user staging content by id (GetUserStagingContentByID)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get user staging content by ID
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents/{contentId}
 
         method: GET
 
         tags: ["Public Staging Content"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/list_user_staging_contents.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_like_legacy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,360 +1,342 @@
 # Copyright (c) 2021 AccelByte Inc. All Rights Reserved.
 # This is licensed software from AccelByte Inc, for limitations
 # and restrictions contact your company contract manager.
 #
 # Code generated. DO NOT EDIT!
 
-# template file: operation.j2
+# template file: wrapper.j2
 
 # pylint: disable=duplicate-code
 # pylint: disable=line-too-long
 # pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring
 # pylint: disable=missing-module-docstring
 # pylint: disable=too-many-arguments
 # pylint: disable=too-many-branches
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=too-many-lines
 # pylint: disable=too-many-locals
 # pylint: disable=too-many-public-methods
 # pylint: disable=too-many-return-statements
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
-# AccelByte Gaming Services Ugc Service
-
-from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
-from accelbyte_py_sdk.core import HttpResponse
+from accelbyte_py_sdk.core import get_namespace as get_services_namespace
+from accelbyte_py_sdk.core import run_request
+from accelbyte_py_sdk.core import run_request_async
+from accelbyte_py_sdk.core import same_doc_as
+
+from ..models import ModelsContentLikeRequest
+from ..models import ModelsContentLikeResponse
+from ..models import ModelsPaginatedContentDownloadResponse
+from ..models import ResponseError
+
+from ..operations.public_like_legacy import GetLikedContent
+from ..operations.public_like_legacy import UpdateContentLikeStatus
+
+
+@same_doc_as(GetLikedContent)
+def get_liked_content(
+    isofficial: Optional[bool] = None,
+    limit: Optional[int] = None,
+    name: Optional[str] = None,
+    offset: Optional[int] = None,
+    orderby: Optional[str] = None,
+    sortby: Optional[str] = None,
+    subtype: Optional[str] = None,
+    tags: Optional[List[str]] = None,
+    type_: Optional[str] = None,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Get liked contents (GetLikedContent)
+
+    For advance tag filtering supports & as AND operator and | as OR operator and parentheses ( ) for priority. e.g:
+
+
+    *tags=red*
+    *tags=red&animal;*
+    *tags=red|animal*
+    *tags=red&animal;|wild*
+    *tags=red&(animal|wild)*
 
-from ...models import ModelsPaginatedListStagingContentResponse
-from ...models import ResponseError
+    The precedence of logical operator is AND > OR, so if no parentheses, AND logical operator will be executed first.
 
+    Allowed character for operand: alphanumeric, underscore _ and dash -
 
-class ListUserStagingContents(Operation):
-    """List user staging contents (ListUserStagingContents)
+    Allowed character for operator: & | ( )
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
 
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    **Please note that value of tags query param should be URL encoded**
 
     Properties:
-        url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents
+        url: /ugc/v1/public/namespaces/{namespace}/contents/liked
 
         method: GET
 
-        tags: ["Public Staging Content"]
+        tags: ["Public Like (Legacy)"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
-        user_id: (userId) REQUIRED str in path
+        isofficial: (isofficial) OPTIONAL bool in query
 
         limit: (limit) OPTIONAL int in query
 
+        name: (name) OPTIONAL str in query
+
         offset: (offset) OPTIONAL int in query
 
-        sort_by: (sortBy) OPTIONAL str in query
+        orderby: (orderby) OPTIONAL str in query
+
+        sortby: (sortby) OPTIONAL str in query
+
+        subtype: (subtype) OPTIONAL str in query
 
-        status: (status) OPTIONAL str in query
+        tags: (tags) OPTIONAL List[str] in query
+
+        type_: (type) OPTIONAL str in query
 
     Responses:
-        200: OK - ModelsPaginatedListStagingContentResponse (list user's staging content)
+        200: OK - ModelsPaginatedContentDownloadResponse (Get liked contents)
 
-        400: Bad Request - ResponseError (774301: invalid paging parameter)
+        400: Bad Request - ResponseError (771100: unable to parse isofficial param)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        403: Forbidden - ResponseError (20013: insufficient permission)
+        500: Internal Server Error - ResponseError (771101: Unable to get ugc content: database error | 770801: Unable to get ugc content: database/Unable to get creator | 770803: Failed generate download URL)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = GetLikedContent.create(
+        isofficial=isofficial,
+        limit=limit,
+        name=name,
+        offset=offset,
+        orderby=orderby,
+        sortby=sortby,
+        subtype=subtype,
+        tags=tags,
+        type_=type_,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(GetLikedContent)
+async def get_liked_content_async(
+    isofficial: Optional[bool] = None,
+    limit: Optional[int] = None,
+    name: Optional[str] = None,
+    offset: Optional[int] = None,
+    orderby: Optional[str] = None,
+    sortby: Optional[str] = None,
+    subtype: Optional[str] = None,
+    tags: Optional[List[str]] = None,
+    type_: Optional[str] = None,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Get liked contents (GetLikedContent)
+
+    For advance tag filtering supports & as AND operator and | as OR operator and parentheses ( ) for priority. e.g:
+
+
+    *tags=red*
+    *tags=red&animal;*
+    *tags=red|animal*
+    *tags=red&animal;|wild*
+    *tags=red&(animal|wild)*
+
+    The precedence of logical operator is AND > OR, so if no parentheses, AND logical operator will be executed first.
+
+    Allowed character for operand: alphanumeric, underscore _ and dash -
+
+    Allowed character for operator: & | ( )
+
+
+    **Please note that value of tags query param should be URL encoded**
+
+    Properties:
+        url: /ugc/v1/public/namespaces/{namespace}/contents/liked
+
+        method: GET
+
+        tags: ["Public Like (Legacy)"]
+
+        consumes: ["application/json", "application/octet-stream"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+        isofficial: (isofficial) OPTIONAL bool in query
+
+        limit: (limit) OPTIONAL int in query
+
+        name: (name) OPTIONAL str in query
+
+        offset: (offset) OPTIONAL int in query
+
+        orderby: (orderby) OPTIONAL str in query
+
+        sortby: (sortby) OPTIONAL str in query
+
+        subtype: (subtype) OPTIONAL str in query
+
+        tags: (tags) OPTIONAL List[str] in query
+
+        type_: (type) OPTIONAL str in query
+
+    Responses:
+        200: OK - ModelsPaginatedContentDownloadResponse (Get liked contents)
 
-        500: Internal Server Error - ResponseError (774302: unable to get staging content | 774303: unable to generate presigned URL)
+        400: Bad Request - ResponseError (771100: unable to parse isofficial param)
+
+        401: Unauthorized - ResponseError (20001: unauthorized access)
+
+        500: Internal Server Error - ResponseError (771101: Unable to get ugc content: database error | 770801: Unable to get ugc content: database/Unable to get creator | 770803: Failed generate download URL)
     """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = GetLikedContent.create(
+        isofficial=isofficial,
+        limit=limit,
+        name=name,
+        offset=offset,
+        orderby=orderby,
+        sortby=sortby,
+        subtype=subtype,
+        tags=tags,
+        type_=type_,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
+
+@same_doc_as(UpdateContentLikeStatus)
+def update_content_like_status(
+    body: ModelsContentLikeRequest,
+    content_id: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Update like/unlike status to a content (UpdateContentLikeStatus)
+
+    This endpoint will update like/unlike state from a content
+
+    Properties:
+        url: /ugc/v1/public/namespaces/{namespace}/contents/{contentId}/like
 
-    # region fields
+        method: PUT
 
-    _url: str = "/ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents"
-    _method: str = "GET"
-    _consumes: List[str] = ["application/json", "application/octet-stream"]
-    _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"]]
-    _location_query: str = None
-
-    namespace: str  # REQUIRED in [path]
-    user_id: str  # REQUIRED in [path]
-    limit: int  # OPTIONAL in [query]
-    offset: int  # OPTIONAL in [query]
-    sort_by: str  # OPTIONAL in [query]
-    status: str  # OPTIONAL in [query]
-
-    # endregion fields
-
-    # region properties
-
-    @property
-    def url(self) -> str:
-        return self._url
-
-    @property
-    def method(self) -> str:
-        return self._method
-
-    @property
-    def consumes(self) -> List[str]:
-        return self._consumes
-
-    @property
-    def produces(self) -> List[str]:
-        return self._produces
-
-    @property
-    def securities(self) -> List[List[str]]:
-        return self._securities
-
-    @property
-    def location_query(self) -> str:
-        return self._location_query
-
-    # endregion properties
-
-    # region get methods
-
-    # endregion get methods
-
-    # region get_x_params methods
-
-    def get_all_params(self) -> dict:
-        return {
-            "path": self.get_path_params(),
-            "query": self.get_query_params(),
-        }
-
-    def get_path_params(self) -> dict:
-        result = {}
-        if hasattr(self, "namespace"):
-            result["namespace"] = self.namespace
-        if hasattr(self, "user_id"):
-            result["userId"] = self.user_id
-        return result
-
-    def get_query_params(self) -> dict:
-        result = {}
-        if hasattr(self, "limit"):
-            result["limit"] = self.limit
-        if hasattr(self, "offset"):
-            result["offset"] = self.offset
-        if hasattr(self, "sort_by"):
-            result["sortBy"] = self.sort_by
-        if hasattr(self, "status"):
-            result["status"] = self.status
-        return result
-
-    # endregion get_x_params methods
-
-    # region is/has methods
-
-    # endregion is/has methods
-
-    # region with_x methods
-
-    def with_namespace(self, value: str) -> ListUserStagingContents:
-        self.namespace = value
-        return self
-
-    def with_user_id(self, value: str) -> ListUserStagingContents:
-        self.user_id = value
-        return self
-
-    def with_limit(self, value: int) -> ListUserStagingContents:
-        self.limit = value
-        return self
-
-    def with_offset(self, value: int) -> ListUserStagingContents:
-        self.offset = value
-        return self
-
-    def with_sort_by(self, value: str) -> ListUserStagingContents:
-        self.sort_by = value
-        return self
-
-    def with_status(self, value: str) -> ListUserStagingContents:
-        self.status = value
-        return self
-
-    # endregion with_x methods
-
-    # region to methods
-
-    def to_dict(self, include_empty: bool = False) -> dict:
-        result: dict = {}
-        if hasattr(self, "namespace") and self.namespace:
-            result["namespace"] = str(self.namespace)
-        elif include_empty:
-            result["namespace"] = ""
-        if hasattr(self, "user_id") and self.user_id:
-            result["userId"] = str(self.user_id)
-        elif include_empty:
-            result["userId"] = ""
-        if hasattr(self, "limit") and self.limit:
-            result["limit"] = int(self.limit)
-        elif include_empty:
-            result["limit"] = 0
-        if hasattr(self, "offset") and self.offset:
-            result["offset"] = int(self.offset)
-        elif include_empty:
-            result["offset"] = 0
-        if hasattr(self, "sort_by") and self.sort_by:
-            result["sortBy"] = str(self.sort_by)
-        elif include_empty:
-            result["sortBy"] = ""
-        if hasattr(self, "status") and self.status:
-            result["status"] = str(self.status)
-        elif include_empty:
-            result["status"] = ""
-        return result
-
-    # endregion to methods
-
-    # region response methods
-
-    # noinspection PyMethodMayBeStatic
-    def parse_response(
-        self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, ModelsPaginatedListStagingContentResponse],
-        Union[None, HttpResponse, ResponseError],
-    ]:
-        """Parse the given response.
+        tags: ["Public Like (Legacy)"]
 
-        200: OK - ModelsPaginatedListStagingContentResponse (list user's staging content)
+        consumes: ["application/json", "application/octet-stream"]
 
-        400: Bad Request - ResponseError (774301: invalid paging parameter)
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        body: (body) REQUIRED ModelsContentLikeRequest in body
+
+        content_id: (contentId) REQUIRED str in path
+
+        namespace: (namespace) REQUIRED str in path
+
+    Responses:
+        200: OK - ModelsContentLikeResponse (Update like/unlike status to a content)
+
+        400: Bad Request - ResponseError (771000: Malformed request/Content not found/Unable to update like status: content not found)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        403: Forbidden - ResponseError (20013: insufficient permission)
+        404: Not Found - ResponseError (771000: Malformed request/Content not found/Unable to update like status: content not found | 771001: unable to like content/Unable to update like status: database error | 771000: Malformed request/Content not found/Unable to update like status: content not found)
 
-        500: Internal Server Error - ResponseError (774302: unable to get staging content | 774303: unable to generate presigned URL)
+        500: Internal Server Error - ResponseError (771001: unable to like content/Unable to update like status: database error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = UpdateContentLikeStatus.create(
+        body=body,
+        content_id=content_id,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(UpdateContentLikeStatus)
+async def update_content_like_status_async(
+    body: ModelsContentLikeRequest,
+    content_id: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Update like/unlike status to a content (UpdateContentLikeStatus)
 
-        ---: HttpResponse (Undocumented Response)
+    This endpoint will update like/unlike state from a content
 
-        ---: HttpResponse (Unexpected Content-Type Error)
+    Properties:
+        url: /ugc/v1/public/namespaces/{namespace}/contents/{contentId}/like
 
-        ---: HttpResponse (Unhandled Error)
-        """
-        pre_processed_response, error = self.pre_process_response(
-            code=code, content_type=content_type, content=content
-        )
-        if error is not None:
-            return None, None if error.is_no_content() else error
-        code, content_type, content = pre_processed_response
-
-        if code == 200:
-            return (
-                ModelsPaginatedListStagingContentResponse.create_from_dict(content),
-                None,
-            )
-        if code == 400:
-            return None, ResponseError.create_from_dict(content)
-        if code == 401:
-            return None, ResponseError.create_from_dict(content)
-        if code == 403:
-            return None, ResponseError.create_from_dict(content)
-        if code == 500:
-            return None, ResponseError.create_from_dict(content)
-
-        return self.handle_undocumented_response(
-            code=code, content_type=content_type, content=content
-        )
-
-    # endregion response methods
-
-    # region static methods
-
-    @classmethod
-    def create(
-        cls,
-        namespace: str,
-        user_id: str,
-        limit: Optional[int] = None,
-        offset: Optional[int] = None,
-        sort_by: Optional[str] = None,
-        status: Optional[str] = None,
-        **kwargs,
-    ) -> ListUserStagingContents:
-        instance = cls()
-        instance.namespace = namespace
-        instance.user_id = user_id
-        if limit is not None:
-            instance.limit = limit
-        if offset is not None:
-            instance.offset = offset
-        if sort_by is not None:
-            instance.sort_by = sort_by
-        if status is not None:
-            instance.status = status
-        if x_flight_id := kwargs.get("x_flight_id", None):
-            instance.x_flight_id = x_flight_id
-        return instance
-
-    @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> ListUserStagingContents:
-        instance = cls()
-        if "namespace" in dict_ and dict_["namespace"] is not None:
-            instance.namespace = str(dict_["namespace"])
-        elif include_empty:
-            instance.namespace = ""
-        if "userId" in dict_ and dict_["userId"] is not None:
-            instance.user_id = str(dict_["userId"])
-        elif include_empty:
-            instance.user_id = ""
-        if "limit" in dict_ and dict_["limit"] is not None:
-            instance.limit = int(dict_["limit"])
-        elif include_empty:
-            instance.limit = 0
-        if "offset" in dict_ and dict_["offset"] is not None:
-            instance.offset = int(dict_["offset"])
-        elif include_empty:
-            instance.offset = 0
-        if "sortBy" in dict_ and dict_["sortBy"] is not None:
-            instance.sort_by = str(dict_["sortBy"])
-        elif include_empty:
-            instance.sort_by = ""
-        if "status" in dict_ and dict_["status"] is not None:
-            instance.status = str(dict_["status"])
-        elif include_empty:
-            instance.status = ""
-        return instance
-
-    @staticmethod
-    def get_field_info() -> Dict[str, str]:
-        return {
-            "namespace": "namespace",
-            "userId": "user_id",
-            "limit": "limit",
-            "offset": "offset",
-            "sortBy": "sort_by",
-            "status": "status",
-        }
-
-    @staticmethod
-    def get_required_map() -> Dict[str, bool]:
-        return {
-            "namespace": True,
-            "userId": True,
-            "limit": False,
-            "offset": False,
-            "sortBy": False,
-            "status": False,
-        }
+        method: PUT
 
-    # endregion static methods
+        tags: ["Public Like (Legacy)"]
+
+        consumes: ["application/json", "application/octet-stream"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        body: (body) REQUIRED ModelsContentLikeRequest in body
+
+        content_id: (contentId) REQUIRED str in path
+
+        namespace: (namespace) REQUIRED str in path
+
+    Responses:
+        200: OK - ModelsContentLikeResponse (Update like/unlike status to a content)
+
+        400: Bad Request - ResponseError (771000: Malformed request/Content not found/Unable to update like status: content not found)
+
+        401: Unauthorized - ResponseError (20001: unauthorized access)
+
+        404: Not Found - ResponseError (771000: Malformed request/Content not found/Unable to update like status: content not found | 771001: unable to like content/Unable to update like status: database error | 771000: Malformed request/Content not found/Unable to update like status: content not found)
+
+        500: Internal Server Error - ResponseError (771001: unable to like content/Unable to update like status: database error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = UpdateContentLikeStatus.create(
+        body=body,
+        content_id=content_id,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/update_staging_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/public_staging_content/update_staging_content.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from ...models import ModelsUpdateStagingContentRequest
 from ...models import ResponseError
 
 
 class UpdateStagingContent(Operation):
     """Update staging content (UpdateStagingContent)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update staging content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents/{contentId}
 
         method: PUT
 
         tags: ["Public Staging Content"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_tag/get_tag.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/admin_tag/admin_create_tag.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,64 +25,64 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsPaginatedGetTagResponse
+from ...models import ModelsCreateTagRequest
+from ...models import ModelsCreateTagResponse
 from ...models import ResponseError
 
 
-class GetTag(Operation):
-    """Get tags (GetTag)
+class AdminCreateTag(Operation):
+    """Create tags (AdminCreateTag)
 
-    Publicly accessible
+    Creates a new tag
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/tags
+        url: /ugc/v1/admin/namespaces/{namespace}/tags
 
-        method: GET
+        method: POST
 
-        tags: ["Public Tag"]
+        tags: ["Admin Tag"]
 
-        consumes: ["application/json", "application/octet-stream"]
+        consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        namespace: (namespace) REQUIRED str in path
-
-        limit: (limit) OPTIONAL int in query
+        body: (body) REQUIRED ModelsCreateTagRequest in body
 
-        offset: (offset) OPTIONAL int in query
+        namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsPaginatedGetTagResponse (Get tags)
+        201: Created - ModelsCreateTagResponse (Tags created)
 
-        400: Bad Request - ResponseError (771501: invalid paging parameter)
+        400: Bad Request - ResponseError (771401: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (771502: Unable get user tags)
+        409: Conflict - ResponseError (771403: Conflicted resource indentifier)
+
+        500: Internal Server Error - ResponseError (771402: Unable to save ugc tag)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/public/namespaces/{namespace}/tags"
-    _method: str = "GET"
-    _consumes: List[str] = ["application/json", "application/octet-stream"]
+    _url: str = "/ugc/v1/admin/namespaces/{namespace}/tags"
+    _method: str = "POST"
+    _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    body: ModelsCreateTagRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
-    limit: int  # OPTIONAL in [query]
-    offset: int  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -114,168 +114,151 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
+            "body": self.get_body_params(),
             "path": self.get_path_params(),
-            "query": self.get_query_params(),
         }
 
+    def get_body_params(self) -> Any:
+        if not hasattr(self, "body") or self.body is None:
+            return None
+        return self.body.to_dict()
+
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
-    def get_query_params(self) -> dict:
-        result = {}
-        if hasattr(self, "limit"):
-            result["limit"] = self.limit
-        if hasattr(self, "offset"):
-            result["offset"] = self.offset
-        return result
-
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> GetTag:
-        self.namespace = value
-        return self
-
-    def with_limit(self, value: int) -> GetTag:
-        self.limit = value
+    def with_body(self, value: ModelsCreateTagRequest) -> AdminCreateTag:
+        self.body = value
         return self
 
-    def with_offset(self, value: int) -> GetTag:
-        self.offset = value
+    def with_namespace(self, value: str) -> AdminCreateTag:
+        self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "body") and self.body:
+            result["body"] = self.body.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["body"] = ModelsCreateTagRequest()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "limit") and self.limit:
-            result["limit"] = int(self.limit)
-        elif include_empty:
-            result["limit"] = 0
-        if hasattr(self, "offset") and self.offset:
-            result["offset"] = int(self.offset)
-        elif include_empty:
-            result["offset"] = 0
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsPaginatedGetTagResponse],
-        Union[None, HttpResponse, ResponseError],
+        Union[None, ModelsCreateTagResponse], Union[None, HttpResponse, ResponseError]
     ]:
         """Parse the given response.
 
-        200: OK - ModelsPaginatedGetTagResponse (Get tags)
+        201: Created - ModelsCreateTagResponse (Tags created)
 
-        400: Bad Request - ResponseError (771501: invalid paging parameter)
+        400: Bad Request - ResponseError (771401: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (771502: Unable get user tags)
+        409: Conflict - ResponseError (771403: Conflicted resource indentifier)
+
+        500: Internal Server Error - ResponseError (771402: Unable to save ugc tag)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return ModelsPaginatedGetTagResponse.create_from_dict(content), None
+        if code == 201:
+            return ModelsCreateTagResponse.create_from_dict(content), None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
+        if code == 409:
+            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls,
-        namespace: str,
-        limit: Optional[int] = None,
-        offset: Optional[int] = None,
-        **kwargs,
-    ) -> GetTag:
+        cls, body: ModelsCreateTagRequest, namespace: str, **kwargs
+    ) -> AdminCreateTag:
         instance = cls()
+        instance.body = body
         instance.namespace = namespace
-        if limit is not None:
-            instance.limit = limit
-        if offset is not None:
-            instance.offset = offset
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> GetTag:
+    def create_from_dict(
+        cls, dict_: dict, include_empty: bool = False
+    ) -> AdminCreateTag:
         instance = cls()
+        if "body" in dict_ and dict_["body"] is not None:
+            instance.body = ModelsCreateTagRequest.create_from_dict(
+                dict_["body"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.body = ModelsCreateTagRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "limit" in dict_ and dict_["limit"] is not None:
-            instance.limit = int(dict_["limit"])
-        elif include_empty:
-            instance.limit = 0
-        if "offset" in dict_ and dict_["offset"] is not None:
-            instance.offset = int(dict_["offset"])
-        elif include_empty:
-            instance.offset = 0
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
+            "body": "body",
             "namespace": "namespace",
-            "limit": "limit",
-            "offset": "offset",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
+            "body": True,
             "namespace": True,
-            "limit": False,
-            "offset": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/operations/public_type/get_type.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/operations/anonymization/delete_all_user_channel.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,64 +25,60 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsPaginatedGetTypeResponse
 from ...models import ResponseError
 
 
-class GetType(Operation):
-    """Get types (GetType)
+class DeleteAllUserChannel(Operation):
+    """Delete all user channel (DeleteAllUserChannel)
 
-    Requires valid user token
+    Delete all user channel
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/types
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels
 
-        method: GET
+        method: DELETE
 
-        tags: ["Public Type"]
+        tags: ["Anonymization"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
-        limit: (limit) OPTIONAL int in query
-
-        offset: (offset) OPTIONAL int in query
+        user_id: (userId) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsPaginatedGetTypeResponse (Get types)
-
-        400: Bad Request - ResponseError (771801: invalid paging parameter)
+        204: No Content - (Content deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (771802: Unable get types)
+        404: Not Found - ResponseError (773502: Channel not found)
+
+        500: Internal Server Error - ResponseError (773501: Unable to delete channel)
     """
 
     # region fields
 
-    _url: str = "/ugc/v1/public/namespaces/{namespace}/types"
-    _method: str = "GET"
+    _url: str = "/ugc/v1/public/namespaces/{namespace}/users/{userId}/channels"
+    _method: str = "DELETE"
     _consumes: List[str] = ["application/json", "application/octet-stream"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     namespace: str  # REQUIRED in [path]
-    limit: int  # OPTIONAL in [query]
-    offset: int  # OPTIONAL in [query]
+    user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -115,167 +111,136 @@
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
             "path": self.get_path_params(),
-            "query": self.get_query_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
-        return result
-
-    def get_query_params(self) -> dict:
-        result = {}
-        if hasattr(self, "limit"):
-            result["limit"] = self.limit
-        if hasattr(self, "offset"):
-            result["offset"] = self.offset
+        if hasattr(self, "user_id"):
+            result["userId"] = self.user_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> GetType:
+    def with_namespace(self, value: str) -> DeleteAllUserChannel:
         self.namespace = value
         return self
 
-    def with_limit(self, value: int) -> GetType:
-        self.limit = value
-        return self
-
-    def with_offset(self, value: int) -> GetType:
-        self.offset = value
+    def with_user_id(self, value: str) -> DeleteAllUserChannel:
+        self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "limit") and self.limit:
-            result["limit"] = int(self.limit)
-        elif include_empty:
-            result["limit"] = 0
-        if hasattr(self, "offset") and self.offset:
-            result["offset"] = int(self.offset)
+        if hasattr(self, "user_id") and self.user_id:
+            result["userId"] = str(self.user_id)
         elif include_empty:
-            result["offset"] = 0
+            result["userId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, ModelsPaginatedGetTypeResponse],
-        Union[None, HttpResponse, ResponseError],
-    ]:
+    ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
         """Parse the given response.
 
-        200: OK - ModelsPaginatedGetTypeResponse (Get types)
-
-        400: Bad Request - ResponseError (771801: invalid paging parameter)
+        204: No Content - (Content deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (771802: Unable get types)
+        404: Not Found - ResponseError (773502: Channel not found)
+
+        500: Internal Server Error - ResponseError (773501: Unable to delete channel)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return ModelsPaginatedGetTypeResponse.create_from_dict(content), None
-        if code == 400:
-            return None, ResponseError.create_from_dict(content)
+        if code == 204:
+            return None, None
         if code == 401:
             return None, ResponseError.create_from_dict(content)
+        if code == 404:
+            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(
-        cls,
-        namespace: str,
-        limit: Optional[int] = None,
-        offset: Optional[int] = None,
-        **kwargs,
-    ) -> GetType:
+    def create(cls, namespace: str, user_id: str, **kwargs) -> DeleteAllUserChannel:
         instance = cls()
         instance.namespace = namespace
-        if limit is not None:
-            instance.limit = limit
-        if offset is not None:
-            instance.offset = offset
+        instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> GetType:
+    def create_from_dict(
+        cls, dict_: dict, include_empty: bool = False
+    ) -> DeleteAllUserChannel:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "limit" in dict_ and dict_["limit"] is not None:
-            instance.limit = int(dict_["limit"])
-        elif include_empty:
-            instance.limit = 0
-        if "offset" in dict_ and dict_["offset"] is not None:
-            instance.offset = int(dict_["offset"])
+        if "userId" in dict_ and dict_["userId"] is not None:
+            instance.user_id = str(dict_["userId"])
         elif include_empty:
-            instance.offset = 0
+            instance.user_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "namespace": "namespace",
-            "limit": "limit",
-            "offset": "offset",
+            "userId": "user_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "namespace": True,
-            "limit": False,
-            "offset": False,
+            "userId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/__init__.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ugc Service."""
 
-__version__ = "2.19.6"
+__version__ = "2.19.7"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._admin_channel import admin_create_channel
 from ._admin_channel import admin_create_channel_async
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_channel.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_anonymization.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,824 +25,825 @@
 
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import get_namespace as get_services_namespace
 from accelbyte_py_sdk.core import run_request
 from accelbyte_py_sdk.core import run_request_async
 from accelbyte_py_sdk.core import same_doc_as
 
-from ..models import ModelsChannelRequest
-from ..models import ModelsChannelResponse
-from ..models import ModelsPaginatedGetChannelResponse
-from ..models import ModelsUpdateChannelRequest
 from ..models import ResponseError
 
-from ..operations.admin_channel import AdminCreateChannel
-from ..operations.admin_channel import AdminDeleteChannel
-from ..operations.admin_channel import AdminGetChannel
-from ..operations.admin_channel import AdminUpdateChannel
-from ..operations.admin_channel import SingleAdminDeleteChannel
-from ..operations.admin_channel import SingleAdminGetChannel
-from ..operations.admin_channel import SingleAdminUpdateChannel
+from ..operations.anonymization import AdminDeleteAllUserChannels
+from ..operations.anonymization import AdminDeleteAllUserContents
+from ..operations.anonymization import AdminDeleteAllUserGroup
+from ..operations.anonymization import AdminDeleteAllUserStates
+from ..operations.anonymization import DeleteAllUserChannel
+from ..operations.anonymization import DeleteAllUserContents
+from ..operations.anonymization import DeleteAllUserGroup
+from ..operations.anonymization import DeleteAllUserStates
 
 
-@same_doc_as(AdminCreateChannel)
-def admin_create_channel(
-    body: ModelsChannelRequest,
+@same_doc_as(AdminDeleteAllUserChannels)
+def admin_delete_all_user_channels(
+    user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Create Channel (AdminCreateChannel)
-
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [CREATE]
+    """Delete all user channel (AdminDeleteAllUserChannels)
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [CREATE]
+    Delete all user channel
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/channels
+        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels
 
-        method: POST
+        method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsChannelRequest in body
-
         namespace: (namespace) REQUIRED str in path
 
-    Responses:
-        201: Created - ModelsChannelResponse (Channel created)
+        user_id: (userId) REQUIRED str in path
 
-        400: Bad Request - ResponseError (770503: Invalid channel {ID}: should uuid without hypen)
+    Responses:
+        204: No Content - (Channel deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        409: Conflict - ResponseError (770504: Channel already exist)
+        404: Not Found - ResponseError (773502: Channel not found)
 
-        500: Internal Server Error - ResponseError (770502: Unable to save channel)
+        500: Internal Server Error - ResponseError (773501: Unable to delete channel)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminCreateChannel.create(
-        body=body,
+    request = AdminDeleteAllUserChannels.create(
+        user_id=user_id,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(AdminCreateChannel)
-async def admin_create_channel_async(
-    body: ModelsChannelRequest,
+@same_doc_as(AdminDeleteAllUserChannels)
+async def admin_delete_all_user_channels_async(
+    user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Create Channel (AdminCreateChannel)
-
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [CREATE]
+    """Delete all user channel (AdminDeleteAllUserChannels)
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [CREATE]
+    Delete all user channel
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/channels
+        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels
 
-        method: POST
+        method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsChannelRequest in body
-
         namespace: (namespace) REQUIRED str in path
 
-    Responses:
-        201: Created - ModelsChannelResponse (Channel created)
+        user_id: (userId) REQUIRED str in path
 
-        400: Bad Request - ResponseError (770503: Invalid channel {ID}: should uuid without hypen)
+    Responses:
+        204: No Content - (Channel deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        409: Conflict - ResponseError (770504: Channel already exist)
+        404: Not Found - ResponseError (773502: Channel not found)
 
-        500: Internal Server Error - ResponseError (770502: Unable to save channel)
+        500: Internal Server Error - ResponseError (773501: Unable to delete channel)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminCreateChannel.create(
-        body=body,
+    request = AdminDeleteAllUserChannels.create(
+        user_id=user_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(AdminDeleteChannel)
-def admin_delete_channel(
-    channel_id: str,
+@same_doc_as(AdminDeleteAllUserContents)
+def admin_delete_all_user_contents(
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete Channel (AdminDeleteChannel)
+    """Delete all user content (AdminDeleteAllUserContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}
+        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/contents
 
         method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        channel_id: (channelId) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (Channel deleted)
+        204: No Content - (Users content's deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (772502: Channel not found)
+        404: Not Found - ResponseError (773402: Content not found)
 
-        500: Internal Server Error - ResponseError (772501: Unable to delete channel)
+        500: Internal Server Error - ResponseError (773401: Unable to get all user content)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminDeleteChannel.create(
-        channel_id=channel_id,
+    request = AdminDeleteAllUserContents.create(
         user_id=user_id,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(AdminDeleteChannel)
-async def admin_delete_channel_async(
-    channel_id: str,
+@same_doc_as(AdminDeleteAllUserContents)
+async def admin_delete_all_user_contents_async(
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete Channel (AdminDeleteChannel)
+    """Delete all user content (AdminDeleteAllUserContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}
+        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/contents
 
         method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        channel_id: (channelId) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (Channel deleted)
+        204: No Content - (Users content's deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (772502: Channel not found)
+        404: Not Found - ResponseError (773402: Content not found)
 
-        500: Internal Server Error - ResponseError (772501: Unable to delete channel)
+        500: Internal Server Error - ResponseError (773401: Unable to get all user content)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminDeleteChannel.create(
-        channel_id=channel_id,
+    request = AdminDeleteAllUserContents.create(
         user_id=user_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(AdminGetChannel)
-def admin_get_channel(
+@same_doc_as(AdminDeleteAllUserGroup)
+def admin_delete_all_user_group(
     user_id: str,
-    limit: Optional[int] = None,
-    name: Optional[str] = None,
-    offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Get Channels (AdminGetChannel)
-
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
+    """Delete all user group (AdminDeleteAllUserGroup)
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
+    Delete all user group
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels
+        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups
 
-        method: GET
+        method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
-        limit: (limit) OPTIONAL int in query
-
-        name: (name) OPTIONAL str in query
-
-        offset: (offset) OPTIONAL int in query
-
     Responses:
-        200: OK - ModelsPaginatedGetChannelResponse (Get channels)
-
-        400: Bad Request - ResponseError (770702: invalid paging parameter)
+        204: No Content - (Groups deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (770700: Unable get user channels)
+        404: Not Found - ResponseError (773302: Groups not found)
+
+        500: Internal Server Error - ResponseError (773301: Unable to find all user group)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminGetChannel.create(
+    request = AdminDeleteAllUserGroup.create(
         user_id=user_id,
-        limit=limit,
-        name=name,
-        offset=offset,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(AdminGetChannel)
-async def admin_get_channel_async(
+@same_doc_as(AdminDeleteAllUserGroup)
+async def admin_delete_all_user_group_async(
     user_id: str,
-    limit: Optional[int] = None,
-    name: Optional[str] = None,
-    offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Get Channels (AdminGetChannel)
-
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
+    """Delete all user group (AdminDeleteAllUserGroup)
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
+    Delete all user group
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels
+        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups
 
-        method: GET
+        method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
-        limit: (limit) OPTIONAL int in query
-
-        name: (name) OPTIONAL str in query
-
-        offset: (offset) OPTIONAL int in query
-
     Responses:
-        200: OK - ModelsPaginatedGetChannelResponse (Get channels)
-
-        400: Bad Request - ResponseError (770702: invalid paging parameter)
+        204: No Content - (Groups deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (770700: Unable get user channels)
+        404: Not Found - ResponseError (773302: Groups not found)
+
+        500: Internal Server Error - ResponseError (773301: Unable to find all user group)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminGetChannel.create(
+    request = AdminDeleteAllUserGroup.create(
         user_id=user_id,
-        limit=limit,
-        name=name,
-        offset=offset,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(AdminUpdateChannel)
-def admin_update_channel(
-    body: ModelsUpdateChannelRequest,
-    channel_id: str,
+@same_doc_as(AdminDeleteAllUserStates)
+def admin_delete_all_user_states(
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Update Channel (AdminUpdateChannel)
+    """Remove all user related state: likes, downloads, followers, following (AdminDeleteAllUserStates)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId} [DELETE]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId} [DELETE]
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}
+        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/states
 
-        method: PUT
+        method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsUpdateChannelRequest in body
-
-        channel_id: (channelId) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsChannelResponse (Channel updated)
-
-        400: Bad Request - ResponseError (770600: Invalid request body)
+        204: No Content - (User stats deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (770603: Channel was not found)
+        404: Not Found - ResponseError (773602: user states are not found: content not found)
 
-        500: Internal Server Error - ResponseError (770602: Unable to save channel)
+        500: Internal Server Error - ResponseError (773601: Unable to get all user contents/Unable to delete user states)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminUpdateChannel.create(
-        body=body,
-        channel_id=channel_id,
+    request = AdminDeleteAllUserStates.create(
         user_id=user_id,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(AdminUpdateChannel)
-async def admin_update_channel_async(
-    body: ModelsUpdateChannelRequest,
-    channel_id: str,
+@same_doc_as(AdminDeleteAllUserStates)
+async def admin_delete_all_user_states_async(
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Update Channel (AdminUpdateChannel)
+    """Remove all user related state: likes, downloads, followers, following (AdminDeleteAllUserStates)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId} [DELETE]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId} [DELETE]
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}
+        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/states
 
-        method: PUT
+        method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsUpdateChannelRequest in body
+        namespace: (namespace) REQUIRED str in path
+
+        user_id: (userId) REQUIRED str in path
+
+    Responses:
+        204: No Content - (User stats deleted)
+
+        401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        channel_id: (channelId) REQUIRED str in path
+        404: Not Found - ResponseError (773602: user states are not found: content not found)
+
+        500: Internal Server Error - ResponseError (773601: Unable to get all user contents/Unable to delete user states)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminDeleteAllUserStates.create(
+        user_id=user_id,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
+
+@same_doc_as(DeleteAllUserChannel)
+def delete_all_user_channel(
+    user_id: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Delete all user channel (DeleteAllUserChannel)
+
+    Delete all user channel
+
+    Properties:
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels
+
+        method: DELETE
+
+        tags: ["Anonymization"]
+
+        consumes: ["application/json", "application/octet-stream"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsChannelResponse (Channel updated)
+        204: No Content - (Content deleted)
+
+        401: Unauthorized - ResponseError (20001: unauthorized access)
+
+        404: Not Found - ResponseError (773502: Channel not found)
+
+        500: Internal Server Error - ResponseError (773501: Unable to delete channel)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = DeleteAllUserChannel.create(
+        user_id=user_id,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(DeleteAllUserChannel)
+async def delete_all_user_channel_async(
+    user_id: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Delete all user channel (DeleteAllUserChannel)
+
+    Delete all user channel
+
+    Properties:
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels
 
-        400: Bad Request - ResponseError (770600: Invalid request body)
+        method: DELETE
+
+        tags: ["Anonymization"]
+
+        consumes: ["application/json", "application/octet-stream"]
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
+        204: No Content - (Content deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (770603: Channel was not found)
+        404: Not Found - ResponseError (773502: Channel not found)
 
-        500: Internal Server Error - ResponseError (770602: Unable to save channel)
+        500: Internal Server Error - ResponseError (773501: Unable to delete channel)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminUpdateChannel.create(
-        body=body,
-        channel_id=channel_id,
+    request = DeleteAllUserChannel.create(
         user_id=user_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(SingleAdminDeleteChannel)
-def single_admin_delete_channel(
-    channel_id: str,
+@same_doc_as(DeleteAllUserContents)
+def delete_all_user_contents(
+    user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete Channel (SingleAdminDeleteChannel)
+    """Delete all user content (DeleteAllUserContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/channels/{channelId}
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents
 
         method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        channel_id: (channelId) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
+        user_id: (userId) REQUIRED str in path
+
     Responses:
-        204: No Content - (Channel deleted)
+        204: No Content - (User content's deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (772502: Channel not found)
+        404: Not Found - ResponseError (773402: Content not found | 771601: Creator not found)
 
-        500: Internal Server Error - ResponseError (772501: Unable to delete channel)
+        500: Internal Server Error - ResponseError (773401: Unable to get all user content)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = SingleAdminDeleteChannel.create(
-        channel_id=channel_id,
+    request = DeleteAllUserContents.create(
+        user_id=user_id,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(SingleAdminDeleteChannel)
-async def single_admin_delete_channel_async(
-    channel_id: str,
+@same_doc_as(DeleteAllUserContents)
+async def delete_all_user_contents_async(
+    user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete Channel (SingleAdminDeleteChannel)
+    """Delete all user content (DeleteAllUserContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/channels/{channelId}
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents
 
         method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        channel_id: (channelId) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
+        user_id: (userId) REQUIRED str in path
+
     Responses:
-        204: No Content - (Channel deleted)
+        204: No Content - (User content's deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (772502: Channel not found)
+        404: Not Found - ResponseError (773402: Content not found | 771601: Creator not found)
 
-        500: Internal Server Error - ResponseError (772501: Unable to delete channel)
+        500: Internal Server Error - ResponseError (773401: Unable to get all user content)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = SingleAdminDeleteChannel.create(
-        channel_id=channel_id,
+    request = DeleteAllUserContents.create(
+        user_id=user_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(SingleAdminGetChannel)
-def single_admin_get_channel(
-    limit: Optional[int] = None,
-    offset: Optional[int] = None,
+@same_doc_as(DeleteAllUserGroup)
+def delete_all_user_group(
+    user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Get Channels (SingleAdminGetChannel)
+    """Delete all user group (DeleteAllUserGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
+    Delete all user group
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/channels
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups
 
-        method: GET
+        method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
-        limit: (limit) OPTIONAL int in query
-
-        offset: (offset) OPTIONAL int in query
+        user_id: (userId) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsPaginatedGetChannelResponse (Get channels)
-
-        400: Bad Request - ResponseError (770702: invalid paging parameter)
+        204: No Content - (groups deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (770700: Unable get user channels)
+        404: Not Found - ResponseError (773302: Groups not found)
+
+        500: Internal Server Error - ResponseError (773301: Unable to find all user group)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = SingleAdminGetChannel.create(
-        limit=limit,
-        offset=offset,
+    request = DeleteAllUserGroup.create(
+        user_id=user_id,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(SingleAdminGetChannel)
-async def single_admin_get_channel_async(
-    limit: Optional[int] = None,
-    offset: Optional[int] = None,
+@same_doc_as(DeleteAllUserGroup)
+async def delete_all_user_group_async(
+    user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Get Channels (SingleAdminGetChannel)
+    """Delete all user group (DeleteAllUserGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
+    Delete all user group
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/channels
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups
 
-        method: GET
+        method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
-        limit: (limit) OPTIONAL int in query
-
-        offset: (offset) OPTIONAL int in query
+        user_id: (userId) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsPaginatedGetChannelResponse (Get channels)
-
-        400: Bad Request - ResponseError (770702: invalid paging parameter)
+        204: No Content - (groups deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (770700: Unable get user channels)
+        404: Not Found - ResponseError (773302: Groups not found)
+
+        500: Internal Server Error - ResponseError (773301: Unable to find all user group)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = SingleAdminGetChannel.create(
-        limit=limit,
-        offset=offset,
+    request = DeleteAllUserGroup.create(
+        user_id=user_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(SingleAdminUpdateChannel)
-def single_admin_update_channel(
-    body: ModelsUpdateChannelRequest,
-    channel_id: str,
+@same_doc_as(DeleteAllUserStates)
+def delete_all_user_states(
+    user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Update Channel (SingleAdminUpdateChannel)
+    """Remove all user related state: likes, downloads, followers, following (DeleteAllUserStates)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+    Required permission NAMESPACE:{namespace}:USER:{userId}" [DELETE]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+        - NAMESPACE:{namespace}:USER:{userId} [DELETE]
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/channels/{channelId}
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/states
 
-        method: PUT
+        method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsUpdateChannelRequest in body
-
-        channel_id: (channelId) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
+        user_id: (userId) REQUIRED str in path
+
     Responses:
-        200: OK - ModelsChannelResponse (Channel updated)
+        204: No Content - (User stats deleted)
 
-        400: Bad Request - ResponseError (770600: Invalid request body)
+        400: Bad Request - ResponseError (773602: user states are not found: content not found)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (770603: Channel was not found)
-
-        500: Internal Server Error - ResponseError (770602: Unable to save channel)
+        500: Internal Server Error - ResponseError (773601: Unable to get all user contents/Unable to delete user states)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = SingleAdminUpdateChannel.create(
-        body=body,
-        channel_id=channel_id,
+    request = DeleteAllUserStates.create(
+        user_id=user_id,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(SingleAdminUpdateChannel)
-async def single_admin_update_channel_async(
-    body: ModelsUpdateChannelRequest,
-    channel_id: str,
+@same_doc_as(DeleteAllUserStates)
+async def delete_all_user_states_async(
+    user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Update Channel (SingleAdminUpdateChannel)
+    """Remove all user related state: likes, downloads, followers, following (DeleteAllUserStates)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+    Required permission NAMESPACE:{namespace}:USER:{userId}" [DELETE]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+        - NAMESPACE:{namespace}:USER:{userId} [DELETE]
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/channels/{channelId}
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/states
 
-        method: PUT
+        method: DELETE
 
-        tags: ["Admin Channel"]
+        tags: ["Anonymization"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsUpdateChannelRequest in body
-
-        channel_id: (channelId) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
+        user_id: (userId) REQUIRED str in path
+
     Responses:
-        200: OK - ModelsChannelResponse (Channel updated)
+        204: No Content - (User stats deleted)
 
-        400: Bad Request - ResponseError (770600: Invalid request body)
+        400: Bad Request - ResponseError (773602: user states are not found: content not found)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (770603: Channel was not found)
-
-        500: Internal Server Error - ResponseError (770602: Unable to save channel)
+        500: Internal Server Error - ResponseError (773601: Unable to get all user contents/Unable to delete user states)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = SingleAdminUpdateChannel.create(
-        body=body,
-        channel_id=channel_id,
+    request = DeleteAllUserStates.create(
+        user_id=user_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_config.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,18 +43,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get configs (AdminGetConfigs)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
+    Get config paginated
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/configs
 
         method: GET
 
         tags: ["Admin Config"]
@@ -100,18 +97,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get configs (AdminGetConfigs)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
+    Get config paginated
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/configs
 
         method: GET
 
         tags: ["Admin Config"]
@@ -159,21 +153,18 @@
     key: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update config (AdminUpdateConfig)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE].
-    It will create a new config if the key doesn't exist.
-    Allowed key value:
-    - contentReview : enabled , disabled
+    This endpoint will create a new config if the *key* doesn't exist.
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
+    Allowed key value:
+    - *contentReview*: *enabled*,*disabled*
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/configs/{key}
 
         method: PATCH
 
         tags: ["Admin Config"]
@@ -219,21 +210,18 @@
     key: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update config (AdminUpdateConfig)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE].
-    It will create a new config if the key doesn't exist.
-    Allowed key value:
-    - contentReview : enabled , disabled
+    This endpoint will create a new config if the *key* doesn't exist.
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
+    Allowed key value:
+    - *contentReview*: *enabled*,*disabled*
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/configs/{key}
 
         method: PATCH
 
         tags: ["Admin Config"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,20 +199,17 @@
 def admin_delete_content_screenshot(
     content_id: str,
     screenshot_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete screenshots content (AdminDeleteContentScreenshot)
+    """Delete content's screenshot (AdminDeleteContentScreenshot)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing screenshot from a content
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/contents/{contentId}/screenshots/{screenshotId}
 
         method: DELETE
 
         tags: ["Admin Content"]
@@ -258,20 +255,17 @@
 async def admin_delete_content_screenshot_async(
     content_id: str,
     screenshot_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete screenshots content (AdminDeleteContentScreenshot)
+    """Delete content's screenshot (AdminDeleteContentScreenshot)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing screenshot from a content
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/contents/{contentId}/screenshots/{screenshotId}
 
         method: DELETE
 
         tags: ["Admin Content"]
@@ -2067,19 +2061,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update screenshot of content (AdminUpdateScreenshots)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/contents/{contentId}/screenshots
 
         method: PUT
 
         tags: ["Admin Content"]
@@ -2127,19 +2117,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update screenshot of content (AdminUpdateScreenshots)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/contents/{contentId}/screenshots
 
         method: PUT
 
         tags: ["Admin Content"]
@@ -2461,25 +2447,21 @@
 def admin_upload_content_screenshot(
     body: ModelsCreateScreenshotRequest,
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Upload screenshots for content (AdminUploadContentScreenshot)
+    """Upload screenshots for official content (AdminUploadContentScreenshot)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-    All request body are required except for contentType field.
-    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the presigned URL.
-    If not specified, it will use fileExtension value.
-    Supported file extensions: pjp, jpg, jpeg, jfif, bmp, png.
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    All request body are required except for *contentType* field.
+    *contentType* values is used to enforce the *Content-Type* header needed by the client to upload the content using the presigned URL.
+    If not specified, it will use *fileExtension* value.
+    Supported file extensions: *pjp*, *jpg*, *jpeg*, *jfif*, *bmp*, *png*.
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/contents/{contentId}/screenshots
 
         method: POST
 
         tags: ["Admin Content"]
@@ -2525,25 +2507,21 @@
 async def admin_upload_content_screenshot_async(
     body: ModelsCreateScreenshotRequest,
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Upload screenshots for content (AdminUploadContentScreenshot)
-
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-    All request body are required except for contentType field.
-    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the presigned URL.
-    If not specified, it will use fileExtension value.
-    Supported file extensions: pjp, jpg, jpeg, jfif, bmp, png.
-    Maximum description length: 1024.
+    """Upload screenshots for official content (AdminUploadContentScreenshot)
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    All request body are required except for *contentType* field.
+    *contentType* values is used to enforce the *Content-Type* header needed by the client to upload the content using the presigned URL.
+    If not specified, it will use *fileExtension* value.
+    Supported file extensions: *pjp*, *jpg*, *jpeg*, *jfif*, *bmp*, *png*.
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/contents/{contentId}/screenshots
 
         method: POST
 
         tags: ["Admin Content"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_content_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_content_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,20 +82,16 @@
     body: ModelsAdminGetContentBulkRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Bulk get content by content IDs (AdminBulkGetContentByIDsV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
     Maximum contentId per request 100
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
-
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/bulk
 
         method: POST
 
         tags: ["Admin Content V2"]
 
@@ -136,20 +132,16 @@
     body: ModelsAdminGetContentBulkRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Bulk get content by content IDs (AdminBulkGetContentByIDsV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
     Maximum contentId per request 100
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
-
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/bulk
 
         method: POST
 
         tags: ["Admin Content V2"]
 
@@ -193,18 +185,15 @@
     channel_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a content (AdminCreateContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    Create official content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents
 
         method: POST
 
         tags: ["Admin Content V2"]
@@ -252,18 +241,15 @@
     channel_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a content (AdminCreateContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    Create official content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents
 
         method: POST
 
         tags: ["Admin Content V2"]
@@ -314,18 +300,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete content by share code (AdminDeleteContentByShareCodeV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete content by share code
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/sharecodes/{shareCode}
 
         method: DELETE
 
         tags: ["Admin Content V2"]
@@ -373,18 +356,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete content by share code (AdminDeleteContentByShareCodeV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete content by share code
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/sharecodes/{shareCode}
 
         method: DELETE
 
         tags: ["Admin Content V2"]
@@ -433,18 +413,15 @@
     screenshot_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete screenshots content (AdminDeleteContentScreenshotV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete screenshot from a content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/screenshots/{screenshotId}
 
         method: DELETE
 
         tags: ["Admin Content V2"]
@@ -492,18 +469,15 @@
     screenshot_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete screenshots content (AdminDeleteContentScreenshotV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete screenshot from a content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/screenshots/{screenshotId}
 
         method: DELETE
 
         tags: ["Admin Content V2"]
@@ -553,18 +527,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete official content (AdminDeleteOfficialContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing official content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents/{contentId}
 
         method: DELETE
 
         tags: ["Admin Content V2"]
@@ -608,18 +579,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete official content (AdminDeleteOfficialContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing official content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents/{contentId}
 
         method: DELETE
 
         tags: ["Admin Content V2"]
@@ -666,18 +634,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete user content (AdminDeleteUserContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete user content by content ID
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}
 
         method: DELETE
 
         tags: ["Admin Content V2"]
@@ -725,18 +690,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete user content (AdminDeleteUserContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete user content by content ID
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}
 
         method: DELETE
 
         tags: ["Admin Content V2"]
@@ -786,18 +748,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Generate official content upload URL (AdminGenerateOfficialContentUploadURLV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Generate official content upload URL
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents/{contentId}/uploadUrl
 
         method: PATCH
 
         tags: ["Admin Content V2"]
@@ -847,18 +806,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Generate official content upload URL (AdminGenerateOfficialContentUploadURLV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Generate official content upload URL
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents/{contentId}/uploadUrl
 
         method: PATCH
 
         tags: ["Admin Content V2"]
@@ -911,18 +867,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Generate user content upload URL (AdminGenerateUserContentUploadURLV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    generate user content upload URL
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/uploadUrl
 
         method: PATCH
 
         tags: ["Admin Content V2"]
@@ -976,18 +929,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Generate user content upload URL (AdminGenerateUserContentUploadURLV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    generate user content upload URL
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/uploadUrl
 
         method: PATCH
 
         tags: ["Admin Content V2"]
@@ -1040,20 +990,16 @@
     body: ModelsGetContentBulkByShareCodesRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Bulk get content by content sharecodes (AdminGetContentBulkByShareCodesV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
     Maximum sharecodes per request 100
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
-
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/sharecodes/bulk
 
         method: POST
 
         tags: ["Admin Content V2"]
 
@@ -1094,20 +1040,16 @@
     body: ModelsGetContentBulkByShareCodesRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Bulk get content by content sharecodes (AdminGetContentBulkByShareCodesV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
     Maximum sharecodes per request 100
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
-
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/sharecodes/bulk
 
         method: POST
 
         tags: ["Admin Content V2"]
 
@@ -1154,18 +1096,15 @@
     sort_by: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List contents specific to a channel (AdminGetContentByChannelIDV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    List content specific to a channel
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents
 
         method: GET
 
         tags: ["Admin Content V2"]
@@ -1221,18 +1160,15 @@
     sort_by: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List contents specific to a channel (AdminGetContentByChannelIDV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    List content specific to a channel
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents
 
         method: GET
 
         tags: ["Admin Content V2"]
@@ -1286,18 +1222,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get content by content ID (AdminGetContentByContentIDV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
+    Get content by content ID
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}
 
         method: GET
 
         tags: ["Admin Content V2"]
@@ -1337,18 +1270,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get content by content ID (AdminGetContentByContentIDV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
+    Get content by content ID
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}
 
         method: GET
 
         tags: ["Admin Content V2"]
@@ -1390,18 +1320,15 @@
     share_code: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get content by sharecode (AdminGetContentByShareCodeV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
+    Get content by share code
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/sharecodes/{shareCode}
 
         method: GET
 
         tags: ["Admin Content V2"]
@@ -1441,18 +1368,15 @@
     share_code: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get content by sharecode (AdminGetContentByShareCodeV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
+    Get content by share code
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/sharecodes/{shareCode}
 
         method: GET
 
         tags: ["Admin Content V2"]
@@ -1497,18 +1421,15 @@
     sort_by: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get user's generated contents (AdminGetContentByUserIDV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get user cotent
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/contents
 
         method: GET
 
         tags: ["Admin Content V2"]
@@ -1560,18 +1481,15 @@
     sort_by: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get user's generated contents (AdminGetContentByUserIDV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get user cotent
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/contents
 
         method: GET
 
         tags: ["Admin Content V2"]
@@ -1629,32 +1547,31 @@
     type_: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List contents (AdminListContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
-    For advance tag filtering supports & as AND operator and | as OR operator and parentheses () for priority. e.g:
+    For advance tag filtering supports & as AND operator and | as OR operator and parentheses ( ) for priority. e.g:
 
-    `tags=red`
-    `tags=red&animal;`
-    `tags=red|animal`
-    `tags=red&animal;|wild`
-    `tags=red&(animal|wild)`
+
+    *tags=red*
+    *tags=red&animal;*
+    *tags=red|animal*
+    *tags=red&animal;|wild*
+    *tags=red&(animal|wild)*
 
     The precedence of logical operator is AND > OR, so if no parentheses, AND logical operator will be executed first.
 
-    Allowed character for operand: alphanumeric, underscore `_` and dash `-`
-    Allowed character for operator: `&` `|` `(` `)`
+    Allowed character for operand: alphanumeric, underscore _ and dash -
+
+    Allowed character for operator: & | ( )
 
-     Please note that value of tags query param should be URL encoded
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
+    **Please note that value of tags query param should be URL encoded**
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents
 
         method: GET
 
         tags: ["Admin Content V2"]
@@ -1722,32 +1639,31 @@
     type_: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List contents (AdminListContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
-    For advance tag filtering supports & as AND operator and | as OR operator and parentheses () for priority. e.g:
+    For advance tag filtering supports & as AND operator and | as OR operator and parentheses ( ) for priority. e.g:
 
-    `tags=red`
-    `tags=red&animal;`
-    `tags=red|animal`
-    `tags=red&animal;|wild`
-    `tags=red&(animal|wild)`
+
+    *tags=red*
+    *tags=red&animal;*
+    *tags=red|animal*
+    *tags=red&animal;|wild*
+    *tags=red&(animal|wild)*
 
     The precedence of logical operator is AND > OR, so if no parentheses, AND logical operator will be executed first.
 
-    Allowed character for operand: alphanumeric, underscore `_` and dash `-`
-    Allowed character for operator: `&` `|` `(` `)`
+    Allowed character for operand: alphanumeric, underscore _ and dash -
+
+    Allowed character for operator: & | ( )
 
-     Please note that value of tags query param should be URL encoded
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:*:CONTENT [READ]
+    **Please note that value of tags query param should be URL encoded**
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents
 
         method: GET
 
         tags: ["Admin Content V2"]
@@ -1813,23 +1729,18 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update content to S3 bucket by share code (AdminUpdateContentByShareCodeV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
+    *shareCode* format should follows:
 
-    `shareCode` format should follows:
-
-    Max length: 7
-    Available characters: abcdefhkpqrstuxyz
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    "Max length: 7
+    "Available characters: abcdefhkpqrstuxyz
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/s3/sharecodes/{shareCode}
 
         method: PUT
 
         tags: ["Admin Content V2"]
@@ -1887,23 +1798,18 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update content to S3 bucket by share code (AdminUpdateContentByShareCodeV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    `shareCode` format should follows:
+    *shareCode* format should follows:
 
-    Max length: 7
-    Available characters: abcdefhkpqrstuxyz
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    "Max length: 7
+    "Available characters: abcdefhkpqrstuxyz
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/s3/sharecodes/{shareCode}
 
         method: PUT
 
         tags: ["Admin Content V2"]
@@ -1962,18 +1868,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Hide/Unhide user's generated contents (AdminUpdateContentHideStatusV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Hide/Unhide user's generated contents
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/contents/{contentId}/hide
 
         method: PUT
 
         tags: ["Admin Content V2"]
@@ -2025,18 +1928,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Hide/Unhide user's generated contents (AdminUpdateContentHideStatusV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Hide/Unhide user's generated contents
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/contents/{contentId}/hide
 
         method: PUT
 
         tags: ["Admin Content V2"]
@@ -2090,19 +1990,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update content file location (AdminUpdateOfficialContentFileLocation)
 
-    This endpoint should be used after calling generate official content upload url endpoint to commit the changes.
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    This endpoint should be used after calling generate official content upload url endpoint to commit the changes
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents/{contentId}/fileLocation
 
         method: PATCH
 
         tags: ["Admin Content V2"]
@@ -2154,19 +2050,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update content file location (AdminUpdateOfficialContentFileLocation)
 
-    This endpoint should be used after calling generate official content upload url endpoint to commit the changes.
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    This endpoint should be used after calling generate official content upload url endpoint to commit the changes
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents/{contentId}/fileLocation
 
         method: PATCH
 
         tags: ["Admin Content V2"]
@@ -2220,18 +2112,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update official content (AdminUpdateOfficialContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update existing official content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents/{contentId}
 
         method: PATCH
 
         tags: ["Admin Content V2"]
@@ -2283,18 +2172,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update official content (AdminUpdateOfficialContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update existing official content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/channels/{channelId}/contents/{contentId}
 
         method: PATCH
 
         tags: ["Admin Content V2"]
@@ -2347,19 +2233,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update screenshot of content (AdminUpdateScreenshotsV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/screenshots
 
         method: PUT
 
         tags: ["Admin Content V2"]
@@ -2407,19 +2289,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update screenshot of content (AdminUpdateScreenshotsV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/screenshots
 
         method: PUT
 
         tags: ["Admin Content V2"]
@@ -2471,19 +2349,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update user content file location (AdminUpdateUserContentFileLocation)
 
-    This endpoint should be used after calling generate user content upload url endpoint to commit the changes.
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    This endpoint should be used after calling generate user content upload url endpoint to commit the changes
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/fileLocation
 
         method: PATCH
 
         tags: ["Admin Content V2"]
@@ -2539,19 +2413,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update user content file location (AdminUpdateUserContentFileLocation)
 
-    This endpoint should be used after calling generate user content upload url endpoint to commit the changes.
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    This endpoint should be used after calling generate user content upload url endpoint to commit the changes
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/fileLocation
 
         method: PATCH
 
         tags: ["Admin Content V2"]
@@ -2609,18 +2479,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update user content (AdminUpdateUserContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update existing user content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}
 
         method: PATCH
 
         tags: ["Admin Content V2"]
@@ -2676,18 +2543,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update user content (AdminUpdateUserContentV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update existing user content
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}
 
         method: PATCH
 
         tags: ["Admin Content V2"]
@@ -2743,23 +2607,18 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Upload screenshots for content (AdminUploadContentScreenshotV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-    All request body are required except for contentType field.
-    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the presigned URL.
-    If not specified, it will use fileExtension value.
+    This endpoint used to request upload URL from content's screenshot.
+    If *contentType* is not specified, it will use *fileExtension* value.
     Supported file extensions: pjp, jpg, jpeg, jfif, bmp, png.
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/screenshots
 
         method: POST
 
         tags: ["Admin Content V2"]
@@ -2807,23 +2666,18 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Upload screenshots for content (AdminUploadContentScreenshotV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-    All request body are required except for contentType field.
-    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the presigned URL.
-    If not specified, it will use fileExtension value.
+    This endpoint used to request upload URL from content's screenshot.
+    If *contentType* is not specified, it will use *fileExtension* value.
     Supported file extensions: pjp, jpg, jpeg, jfif, bmp, png.
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/screenshots
 
         method: POST
 
         tags: ["Admin Content V2"]
@@ -2872,20 +2726,16 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List content's payload versions (ListContentVersionsV2)
 
-    Required permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
     Content's payload versions created when UGC is created or updated with `updateContentFile` set to true. Only list up to 10 latest versions.
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
-
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/versions
 
         method: GET
 
         tags: ["Admin Content V2"]
 
@@ -2924,20 +2774,16 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List content's payload versions (ListContentVersionsV2)
 
-    Required permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
     Content's payload versions created when UGC is created or updated with `updateContentFile` set to true. Only list up to 10 latest versions.
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
-
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/versions
 
         method: GET
 
         tags: ["Admin Content V2"]
 
@@ -2979,19 +2825,15 @@
     version_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Rollback content's payload version (RollbackContentVersionV2)
 
-    Required permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
-    Rollback content's payload to specified version.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Rollback content's payload to specified version
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/rollback/{versionId}
 
         method: PUT
 
         tags: ["Admin Content V2"]
@@ -3037,19 +2879,15 @@
     version_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Rollback content's payload version (RollbackContentVersionV2)
 
-    Required permission: ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
-    Rollback content's payload to specified version.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Rollback content's payload to specified version
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/contents/{contentId}/rollback/{versionId}
 
         method: PUT
 
         tags: ["Admin Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_group.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_group.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,18 +56,15 @@
     body: ModelsCreateGroupRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create groups (AdminCreateGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [CREATE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [CREATE]
+    Create group
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups
 
         method: POST
 
         tags: ["Admin Group"]
@@ -107,18 +104,15 @@
     body: ModelsCreateGroupRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create groups (AdminCreateGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [CREATE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [CREATE]
+    Create group
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups
 
         method: POST
 
         tags: ["Admin Group"]
@@ -161,18 +155,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete group (AdminDeleteGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    Delete group
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
         method: DELETE
 
         tags: ["Admin Group"]
@@ -216,18 +207,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete group (AdminDeleteGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    Delete group
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
         method: DELETE
 
         tags: ["Admin Group"]
@@ -274,18 +262,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get all user groups (AdminGetAllGroups)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get user group paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups
 
         method: GET
 
         tags: ["Admin Group"]
@@ -333,18 +318,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get all user groups (AdminGetAllGroups)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get user group paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups
 
         method: GET
 
         tags: ["Admin Group"]
@@ -393,18 +375,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get specific user group (AdminGetGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get user group by group ID
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
         method: GET
 
         tags: ["Admin Group"]
@@ -448,18 +427,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get specific user group (AdminGetGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get user group by group ID
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
         method: GET
 
         tags: ["Admin Group"]
@@ -507,18 +483,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """(Legacy) Get contents belong to a group (AdminGetGroupContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get content belong to a group
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents
 
         method: GET
 
         tags: ["Admin Group"]
@@ -572,18 +545,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """(Legacy) Get contents belong to a group (AdminGetGroupContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get content belong to a group
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents
 
         method: GET
 
         tags: ["Admin Group"]
@@ -638,18 +608,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get contents belong to a group (AdminGetOfficialGroupContentsV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get contents belong to a group
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/groups/{groupId}/contents
 
         method: GET
 
         tags: ["Admin Group"]
@@ -699,18 +666,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get contents belong to a group (AdminGetOfficialGroupContentsV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get contents belong to a group
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/groups/{groupId}/contents
 
         method: GET
 
         tags: ["Admin Group"]
@@ -763,18 +727,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get contents belong to a group (AdminGetUserGroupContentsV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get contents belong to a group
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents
 
         method: GET
 
         tags: ["Admin Group"]
@@ -828,18 +789,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get contents belong to a group (AdminGetUserGroupContentsV2)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get contents belong to a group
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents
 
         method: GET
 
         tags: ["Admin Group"]
@@ -894,19 +852,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update group (AdminUpdateGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
-    replace group name and contents with new ones.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
+    Replace group name and contents with new ones.
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
         method: PUT
 
         tags: ["Admin Group"]
@@ -956,19 +910,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update group (AdminUpdateGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
-    replace group name and contents with new ones.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
+    Replace group name and contents with new ones.
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
         method: PUT
 
         tags: ["Admin Group"]
@@ -1018,18 +968,15 @@
     group_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete group (SingleAdminDeleteGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    Delete group by group ID
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups/{groupId}
 
         method: DELETE
 
         tags: ["Admin Group"]
@@ -1069,18 +1016,15 @@
     group_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete group (SingleAdminDeleteGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    Delete group by group ID
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups/{groupId}
 
         method: DELETE
 
         tags: ["Admin Group"]
@@ -1123,18 +1067,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get all user groups (SingleAdminGetAllGroups)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get user group paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups
 
         method: GET
 
         tags: ["Admin Group"]
@@ -1178,18 +1119,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get all user groups (SingleAdminGetAllGroups)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get user group paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups
 
         method: GET
 
         tags: ["Admin Group"]
@@ -1234,18 +1172,15 @@
     group_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get specific user group (SingleAdminGetGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get user group by group ID
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups/{groupId}
 
         method: GET
 
         tags: ["Admin Group"]
@@ -1285,18 +1220,15 @@
     group_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get specific user group (SingleAdminGetGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [READ]
+    Get user group by group ID
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups/{groupId}
 
         method: GET
 
         tags: ["Admin Group"]
@@ -1340,18 +1272,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """(Legacy) Get contents belong to a group (SingleAdminGetGroupContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get content belong to a group
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups/{groupId}/contents
 
         method: GET
 
         tags: ["Admin Group"]
@@ -1401,18 +1330,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """(Legacy) Get contents belong to a group (SingleAdminGetGroupContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get content belong to a group
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups/{groupId}/contents
 
         method: GET
 
         tags: ["Admin Group"]
@@ -1463,19 +1389,15 @@
     group_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update group (SingleAdminUpdateGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
-    replace group name and contents with new ones.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
+    Replace group name and contents with new ones.
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups/{groupId}
 
         method: PUT
 
         tags: ["Admin Group"]
@@ -1521,19 +1443,15 @@
     group_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update group (SingleAdminUpdateGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
-    replace group name and contents with new ones.
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [UPDATE]
+    Replace group name and contents with new ones.
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/groups/{groupId}
 
         method: PUT
 
         tags: ["Admin Group"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_staging_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_staging_content.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,18 +47,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Approve or reject content (AdminApproveStagingContent)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:CONTENT:APPROVAL [CREATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:CONTENT:APPROVAL [CREATE]
+    Approved content will shown to public player. Rejected content stays in staging area and couldn't be seen by other player
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/staging-contents/{contentId}/approve
 
         method: POST
 
         tags: ["Admin Staging Content"]
@@ -106,18 +103,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Approve or reject content (AdminApproveStagingContent)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:CONTENT:APPROVAL [CREATE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:CONTENT:APPROVAL [CREATE]
+    Approved content will shown to public player. Rejected content stays in staging area and couldn't be seen by other player
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/staging-contents/{contentId}/approve
 
         method: POST
 
         tags: ["Admin Staging Content"]
@@ -166,18 +160,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get staging content by id (AdminGetStagingContentByID)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get staging content by ID
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/staging-contents/{contentId}
 
         method: GET
 
         tags: ["Admin Staging Content"]
@@ -219,18 +210,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get staging content by id (AdminGetStagingContentByID)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get staging content by ID
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/staging-contents/{contentId}
 
         method: GET
 
         tags: ["Admin Staging Content"]
@@ -277,18 +265,15 @@
     status: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List staging contents (AdminListStagingContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    List content that need admin's approval
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/staging-contents
 
         method: GET
 
         tags: ["Admin Staging Content"]
@@ -342,18 +327,15 @@
     status: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List staging contents (AdminListStagingContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    List content that need admin's approval
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/staging-contents
 
         method: GET
 
         tags: ["Admin Staging Content"]
@@ -410,18 +392,15 @@
     status: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List user staging contents (AdminListUserStagingContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    List user content's that need admin approval
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/staging-contents
 
         method: GET
 
         tags: ["Admin Staging Content"]
@@ -479,18 +458,15 @@
     status: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List user staging contents (AdminListUserStagingContents)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    List user content's that need admin approval
 
     Properties:
         url: /ugc/v2/admin/namespaces/{namespace}/users/{userId}/staging-contents
 
         method: GET
 
         tags: ["Admin Staging Content"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_tag.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_tag.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,19 +45,15 @@
     body: ModelsCreateTagRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create tags (AdminCreateTag)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [CREATE]
-    creates a new tag
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [CREATE]
+    Creates a new tag
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/tags
 
         method: POST
 
         tags: ["Admin Tag"]
@@ -99,19 +95,15 @@
     body: ModelsCreateTagRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create tags (AdminCreateTag)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [CREATE]
-    creates a new tag
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [CREATE]
+    Creates a new tag
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/tags
 
         method: POST
 
         tags: ["Admin Tag"]
@@ -155,18 +147,15 @@
     tag_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete tags (AdminDeleteTag)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [DELETE]
+    Delete existing tag
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/tags/{tagId}
 
         method: DELETE
 
         tags: ["Admin Tag"]
@@ -206,18 +195,15 @@
     tag_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete tags (AdminDeleteTag)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [DELETE]
+    Delete existing tag
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/tags/{tagId}
 
         method: DELETE
 
         tags: ["Admin Tag"]
@@ -260,18 +246,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get tags (AdminGetTag)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
+    Get available tags paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/tags
 
         method: GET
 
         tags: ["Admin Tag"]
@@ -315,18 +298,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get tags (AdminGetTag)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
+    Get available tags paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/tags
 
         method: GET
 
         tags: ["Admin Tag"]
@@ -372,19 +352,15 @@
     tag_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update tag (AdminUpdateTag)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
-    updates a tag
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
+    Update existing tag
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/tags/{tagId}
 
         method: PUT
 
         tags: ["Admin Tag"]
@@ -432,19 +408,15 @@
     tag_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update tag (AdminUpdateTag)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
-    updates a tag
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
+    Update existing tag
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/tags/{tagId}
 
         method: PUT
 
         tags: ["Admin Tag"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_type.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_admin_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,19 +45,15 @@
     body: ModelsCreateTypeRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create types (AdminCreateType)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [CREATE]
-    creates a new type and subtype
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [CREATE]
+    Creates a new type and subtype
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/types
 
         method: POST
 
         tags: ["Admin Type"]
@@ -99,19 +95,15 @@
     body: ModelsCreateTypeRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create types (AdminCreateType)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [CREATE]
-    creates a new type and subtype
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [CREATE]
+    Creates a new type and subtype
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/types
 
         method: POST
 
         tags: ["Admin Type"]
@@ -153,20 +145,17 @@
 @same_doc_as(AdminDeleteType)
 def admin_delete_type(
     type_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete types (AdminDeleteType)
+    """Delete type (AdminDeleteType)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [DELETE]
+    Delete existing type
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/types/{typeId}
 
         method: DELETE
 
         tags: ["Admin Type"]
@@ -204,20 +193,17 @@
 @same_doc_as(AdminDeleteType)
 async def admin_delete_type_async(
     type_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete types (AdminDeleteType)
-
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [DELETE]
+    """Delete type (AdminDeleteType)
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [DELETE]
+    Delete existing type
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/types/{typeId}
 
         method: DELETE
 
         tags: ["Admin Type"]
@@ -260,18 +246,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get types (AdminGetType)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
+    Get available types paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/types
 
         method: GET
 
         tags: ["Admin Type"]
@@ -315,18 +298,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get types (AdminGetType)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [READ]
+    Get available types paginated
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/types
 
         method: GET
 
         tags: ["Admin Type"]
@@ -372,19 +352,15 @@
     type_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update types (AdminUpdateType)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
-    updates a type and subtype
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
+    Updates a type and subtype
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/types/{typeId}
 
         method: PUT
 
         tags: ["Admin Type"]
@@ -432,19 +408,15 @@
     type_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update types (AdminUpdateType)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
-    updates a type and subtype
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:UGCCONFIG [UPDATE]
+    Updates a type and subtype
 
     Properties:
         url: /ugc/v1/admin/namespaces/{namespace}/types/{typeId}
 
         method: PUT
 
         tags: ["Admin Type"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_anonymization.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,849 +25,823 @@
 
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import get_namespace as get_services_namespace
 from accelbyte_py_sdk.core import run_request
 from accelbyte_py_sdk.core import run_request_async
 from accelbyte_py_sdk.core import same_doc_as
 
+from ..models import ModelsCreateGroupRequest
+from ..models import ModelsCreateGroupResponse
+from ..models import ModelsPaginatedContentDownloadResponse
+from ..models import ModelsPaginatedContentDownloadResponseV2
+from ..models import ModelsPaginatedGroupResponse
 from ..models import ResponseError
 
-from ..operations.anonymization import AdminDeleteAllUserChannels
-from ..operations.anonymization import AdminDeleteAllUserContents
-from ..operations.anonymization import AdminDeleteAllUserGroup
-from ..operations.anonymization import AdminDeleteAllUserStates
-from ..operations.anonymization import DeleteAllUserChannel
-from ..operations.anonymization import DeleteAllUserContents
-from ..operations.anonymization import DeleteAllUserGroup
-from ..operations.anonymization import DeleteAllUserStates
+from ..operations.public_group import CreateGroup
+from ..operations.public_group import DeleteGroup
+from ..operations.public_group import GetGroup
+from ..operations.public_group import GetGroupContent
+from ..operations.public_group import GetGroups
+from ..operations.public_group import PublicGetGroupContentsV2
+from ..operations.public_group import UpdateGroup
 
 
-@same_doc_as(AdminDeleteAllUserChannels)
-def admin_delete_all_user_channels(
+@same_doc_as(CreateGroup)
+def create_group(
+    body: ModelsCreateGroupRequest,
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete all user channel (AdminDeleteAllUserChannels)
+    """Create groups (CreateGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Create group
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups
 
-        method: DELETE
+        method: POST
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        namespace: (namespace) REQUIRED str in path
-
-        user_id: (userId) REQUIRED str in path
-
-    Responses:
-        204: No Content - (Channel deleted)
-
-        401: Unauthorized - ResponseError (20001: unauthorized access)
-
-        404: Not Found - ResponseError (773502: Channel not found)
-
-        500: Internal Server Error - ResponseError (773501: Unable to delete channel)
-    """
-    if namespace is None:
-        namespace, error = get_services_namespace()
-        if error:
-            return None, error
-    request = AdminDeleteAllUserChannels.create(
-        user_id=user_id,
-        namespace=namespace,
-    )
-    return run_request(request, additional_headers=x_additional_headers, **kwargs)
-
-
-@same_doc_as(AdminDeleteAllUserChannels)
-async def admin_delete_all_user_channels_async(
-    user_id: str,
-    namespace: Optional[str] = None,
-    x_additional_headers: Optional[Dict[str, str]] = None,
-    **kwargs
-):
-    """Delete all user channel (AdminDeleteAllUserChannels)
-
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
-
-    Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/channels
-
-        method: DELETE
-
-        tags: ["Anonymization"]
-
-        consumes: ["application/json"]
-
-        produces: ["application/json"]
-
-        securities: [BEARER_AUTH]
+        body: (body) REQUIRED ModelsCreateGroupRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (Channel deleted)
-
-        401: Unauthorized - ResponseError (20001: unauthorized access)
-
-        404: Not Found - ResponseError (773502: Channel not found)
-
-        500: Internal Server Error - ResponseError (773501: Unable to delete channel)
-    """
-    if namespace is None:
-        namespace, error = get_services_namespace()
-        if error:
-            return None, error
-    request = AdminDeleteAllUserChannels.create(
-        user_id=user_id,
-        namespace=namespace,
-    )
-    return await run_request_async(
-        request, additional_headers=x_additional_headers, **kwargs
-    )
-
-
-@same_doc_as(AdminDeleteAllUserContents)
-def admin_delete_all_user_contents(
-    user_id: str,
-    namespace: Optional[str] = None,
-    x_additional_headers: Optional[Dict[str, str]] = None,
-    **kwargs
-):
-    """Delete all user content (AdminDeleteAllUserContents)
-
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
-
-    Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/contents
-
-        method: DELETE
-
-        tags: ["Anonymization"]
-
-        consumes: ["application/json"]
-
-        produces: ["application/json"]
-
-        securities: [BEARER_AUTH]
-
-        namespace: (namespace) REQUIRED str in path
+        201: Created - ModelsCreateGroupResponse (Group Created)
 
-        user_id: (userId) REQUIRED str in path
-
-    Responses:
-        204: No Content - (Users content's deleted)
+        400: Bad Request - ResponseError (772101: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773402: Content not found)
-
-        500: Internal Server Error - ResponseError (773401: Unable to get all user content)
+        500: Internal Server Error - ResponseError (772102: Unable to create group)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminDeleteAllUserContents.create(
+    request = CreateGroup.create(
+        body=body,
         user_id=user_id,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(AdminDeleteAllUserContents)
-async def admin_delete_all_user_contents_async(
+@same_doc_as(CreateGroup)
+async def create_group_async(
+    body: ModelsCreateGroupRequest,
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete all user content (AdminDeleteAllUserContents)
+    """Create groups (CreateGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Create group
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/contents
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups
 
-        method: DELETE
+        method: POST
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        body: (body) REQUIRED ModelsCreateGroupRequest in body
+
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (Users content's deleted)
+        201: Created - ModelsCreateGroupResponse (Group Created)
 
-        401: Unauthorized - ResponseError (20001: unauthorized access)
+        400: Bad Request - ResponseError (772101: Malformed request/Invalid request body)
 
-        404: Not Found - ResponseError (773402: Content not found)
+        401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (773401: Unable to get all user content)
+        500: Internal Server Error - ResponseError (772102: Unable to create group)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminDeleteAllUserContents.create(
+    request = CreateGroup.create(
+        body=body,
         user_id=user_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(AdminDeleteAllUserGroup)
-def admin_delete_all_user_group(
+@same_doc_as(DeleteGroup)
+def delete_group(
+    group_id: str,
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete all user group (AdminDeleteAllUserGroup)
-
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    """Delete group (DeleteGroup)
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    Delete user group by group ID
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
         method: DELETE
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        group_id: (groupId) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (Groups deleted)
+        204: No Content - (Group deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773302: Groups not found)
+        404: Not Found - ResponseError (772403: Group not found)
 
-        500: Internal Server Error - ResponseError (773301: Unable to find all user group)
+        500: Internal Server Error - ResponseError (772402: Unable delete groups)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminDeleteAllUserGroup.create(
+    request = DeleteGroup.create(
+        group_id=group_id,
         user_id=user_id,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(AdminDeleteAllUserGroup)
-async def admin_delete_all_user_group_async(
+@same_doc_as(DeleteGroup)
+async def delete_group_async(
+    group_id: str,
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete all user group (AdminDeleteAllUserGroup)
+    """Delete group (DeleteGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    Delete user group by group ID
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/groups
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
         method: DELETE
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        group_id: (groupId) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (Groups deleted)
+        204: No Content - (Group deleted)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773302: Groups not found)
+        404: Not Found - ResponseError (772403: Group not found)
 
-        500: Internal Server Error - ResponseError (773301: Unable to find all user group)
+        500: Internal Server Error - ResponseError (772402: Unable delete groups)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminDeleteAllUserGroup.create(
+    request = DeleteGroup.create(
+        group_id=group_id,
         user_id=user_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(AdminDeleteAllUserStates)
-def admin_delete_all_user_states(
+@same_doc_as(GetGroup)
+def get_group(
+    group_id: str,
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Remove all user related state: likes, downloads, followers, following (AdminDeleteAllUserStates)
-
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId} [DELETE]
+    """Get user's groups (GetGroup)
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId} [DELETE]
+    Get user groups by group ID
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/states
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
-        method: DELETE
+        method: GET
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        group_id: (groupId) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (User stats deleted)
+        200: OK - ModelsCreateGroupResponse (Get user's group)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773602: user states are not found: content not found)
+        404: Not Found - ResponseError (773002: Group not found)
 
-        500: Internal Server Error - ResponseError (773601: Unable to get all user contents/Unable to delete user states)
+        500: Internal Server Error - ResponseError (773001: Unable get group)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminDeleteAllUserStates.create(
+    request = GetGroup.create(
+        group_id=group_id,
         user_id=user_id,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(AdminDeleteAllUserStates)
-async def admin_delete_all_user_states_async(
+@same_doc_as(GetGroup)
+async def get_group_async(
+    group_id: str,
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Remove all user related state: likes, downloads, followers, following (AdminDeleteAllUserStates)
+    """Get user's groups (GetGroup)
 
-    Required permission ADMIN:NAMESPACE:{namespace}:USER:{userId} [DELETE]
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId} [DELETE]
+    Get user groups by group ID
 
     Properties:
-        url: /ugc/v1/admin/namespaces/{namespace}/users/{userId}/states
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
-        method: DELETE
+        method: GET
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
-        consumes: ["application/json"]
+        consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        group_id: (groupId) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (User stats deleted)
+        200: OK - ModelsCreateGroupResponse (Get user's group)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773602: user states are not found: content not found)
+        404: Not Found - ResponseError (773002: Group not found)
 
-        500: Internal Server Error - ResponseError (773601: Unable to get all user contents/Unable to delete user states)
+        500: Internal Server Error - ResponseError (773001: Unable get group)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminDeleteAllUserStates.create(
+    request = GetGroup.create(
+        group_id=group_id,
         user_id=user_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(DeleteAllUserChannel)
-def delete_all_user_channel(
+@same_doc_as(GetGroupContent)
+def get_group_content(
+    group_id: str,
     user_id: str,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete all user channel (DeleteAllUserChannel)
-
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    """(Legacy) Get contents belong to a group (GetGroupContent)
 
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Get content that belong to a group
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents
 
-        method: DELETE
+        method: GET
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        group_id: (groupId) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
     Responses:
-        204: No Content - (Content deleted)
+        200: OK - ModelsPaginatedContentDownloadResponse (Get contents belong to a group)
+
+        400: Bad Request - ResponseError (773101: invalid paging parameter)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773502: Channel not found)
+        404: Not Found - ResponseError (773103: No group content was found)
 
-        500: Internal Server Error - ResponseError (773501: Unable to delete channel)
+        500: Internal Server Error - ResponseError (773102: Unable to get ugc content: database error | 770901: Unable to get ugc content: database error/Unable to get creator | 770903: Failed generate download URL)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = DeleteAllUserChannel.create(
+    request = GetGroupContent.create(
+        group_id=group_id,
         user_id=user_id,
+        limit=limit,
+        offset=offset,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(DeleteAllUserChannel)
-async def delete_all_user_channel_async(
+@same_doc_as(GetGroupContent)
+async def get_group_content_async(
+    group_id: str,
     user_id: str,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete all user channel (DeleteAllUserChannel)
+    """(Legacy) Get contents belong to a group (GetGroupContent)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Get content that belong to a group
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents
 
-        method: DELETE
+        method: GET
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        group_id: (groupId) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
     Responses:
-        204: No Content - (Content deleted)
+        200: OK - ModelsPaginatedContentDownloadResponse (Get contents belong to a group)
+
+        400: Bad Request - ResponseError (773101: invalid paging parameter)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773502: Channel not found)
+        404: Not Found - ResponseError (773103: No group content was found)
 
-        500: Internal Server Error - ResponseError (773501: Unable to delete channel)
+        500: Internal Server Error - ResponseError (773102: Unable to get ugc content: database error | 770901: Unable to get ugc content: database error/Unable to get creator | 770903: Failed generate download URL)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = DeleteAllUserChannel.create(
+    request = GetGroupContent.create(
+        group_id=group_id,
         user_id=user_id,
+        limit=limit,
+        offset=offset,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(DeleteAllUserContents)
-def delete_all_user_contents(
+@same_doc_as(GetGroups)
+def get_groups(
     user_id: str,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete all user content (DeleteAllUserContents)
+    """Get all user groups (GetGroups)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Get user groups paginated
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups
 
-        method: DELETE
+        method: GET
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
     Responses:
-        204: No Content - (User content's deleted)
+        200: OK - ModelsPaginatedGroupResponse (Get all user group)
 
-        401: Unauthorized - ResponseError (20001: unauthorized access)
+        400: Bad Request - ResponseError (772301: invalid paging parameter)
 
-        404: Not Found - ResponseError (773402: Content not found | 771601: Creator not found)
+        401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (773401: Unable to get all user content)
+        500: Internal Server Error - ResponseError (772302: Unable get groups)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = DeleteAllUserContents.create(
+    request = GetGroups.create(
         user_id=user_id,
+        limit=limit,
+        offset=offset,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(DeleteAllUserContents)
-async def delete_all_user_contents_async(
+@same_doc_as(GetGroups)
+async def get_groups_async(
     user_id: str,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete all user content (DeleteAllUserContents)
-
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
+    """Get all user groups (GetGroups)
 
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Get user groups paginated
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups
 
-        method: DELETE
+        method: GET
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
     Responses:
-        204: No Content - (User content's deleted)
+        200: OK - ModelsPaginatedGroupResponse (Get all user group)
 
-        401: Unauthorized - ResponseError (20001: unauthorized access)
+        400: Bad Request - ResponseError (772301: invalid paging parameter)
 
-        404: Not Found - ResponseError (773402: Content not found | 771601: Creator not found)
+        401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (773401: Unable to get all user content)
+        500: Internal Server Error - ResponseError (772302: Unable get groups)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = DeleteAllUserContents.create(
+    request = GetGroups.create(
         user_id=user_id,
+        limit=limit,
+        offset=offset,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(DeleteAllUserGroup)
-def delete_all_user_group(
+@same_doc_as(PublicGetGroupContentsV2)
+def public_get_group_contents_v2(
+    group_id: str,
     user_id: str,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete all user group (DeleteAllUserGroup)
-
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    """Get contents belong to a group (PublicGetGroupContentsV2)
 
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    Get content belong to a group
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups
+        url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents
 
-        method: DELETE
+        method: GET
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        group_id: (groupId) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
     Responses:
-        204: No Content - (groups deleted)
+        200: OK - ModelsPaginatedContentDownloadResponseV2 (Get content belong to a group)
+
+        400: Bad Request - ResponseError (773101: invalid paging parameter)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773302: Groups not found)
+        404: Not Found - ResponseError (773103: No group content was found)
 
-        500: Internal Server Error - ResponseError (773301: Unable to find all user group)
+        500: Internal Server Error - ResponseError (773102: Unable to get ugc content: database error | 770901: Unable to get ugc content: database error/Unable to get creator | 770801: Unable to get ugc content: database/Unable to get creator | 770903: Failed generate download URL)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = DeleteAllUserGroup.create(
+    request = PublicGetGroupContentsV2.create(
+        group_id=group_id,
         user_id=user_id,
+        limit=limit,
+        offset=offset,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(DeleteAllUserGroup)
-async def delete_all_user_group_async(
+@same_doc_as(PublicGetGroupContentsV2)
+async def public_get_group_contents_v2_async(
+    group_id: str,
     user_id: str,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete all user group (DeleteAllUserGroup)
-
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    """Get contents belong to a group (PublicGetGroupContentsV2)
 
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENTGROUP [DELETE]
+    Get content belong to a group
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups
+        url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/groups/{groupId}/contents
 
-        method: DELETE
+        method: GET
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        group_id: (groupId) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
     Responses:
-        204: No Content - (groups deleted)
+        200: OK - ModelsPaginatedContentDownloadResponseV2 (Get content belong to a group)
+
+        400: Bad Request - ResponseError (773101: invalid paging parameter)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (773302: Groups not found)
+        404: Not Found - ResponseError (773103: No group content was found)
 
-        500: Internal Server Error - ResponseError (773301: Unable to find all user group)
+        500: Internal Server Error - ResponseError (773102: Unable to get ugc content: database error | 770901: Unable to get ugc content: database error/Unable to get creator | 770801: Unable to get ugc content: database/Unable to get creator | 770903: Failed generate download URL)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = DeleteAllUserGroup.create(
+    request = PublicGetGroupContentsV2.create(
+        group_id=group_id,
         user_id=user_id,
+        limit=limit,
+        offset=offset,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(DeleteAllUserStates)
-def delete_all_user_states(
+@same_doc_as(UpdateGroup)
+def update_group(
+    body: ModelsCreateGroupRequest,
+    group_id: str,
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Remove all user related state: likes, downloads, followers, following (DeleteAllUserStates)
-
-    Required permission NAMESPACE:{namespace}:USER:{userId}" [DELETE]
+    """Update group (UpdateGroup)
 
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId} [DELETE]
+    Replace group name and contents with new ones
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/states
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
-        method: DELETE
+        method: PUT
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        body: (body) REQUIRED ModelsCreateGroupRequest in body
+
+        group_id: (groupId) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (User stats deleted)
+        200: OK - ModelsCreateGroupResponse (Group updated)
 
-        400: Bad Request - ResponseError (773602: user states are not found: content not found)
+        400: Bad Request - ResponseError (772201: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (773601: Unable to get all user contents/Unable to delete user states)
+        404: Not Found - ResponseError (772203: Group not found)
+
+        500: Internal Server Error - ResponseError (772202: Unable to update group)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = DeleteAllUserStates.create(
+    request = UpdateGroup.create(
+        body=body,
+        group_id=group_id,
         user_id=user_id,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(DeleteAllUserStates)
-async def delete_all_user_states_async(
+@same_doc_as(UpdateGroup)
+async def update_group_async(
+    body: ModelsCreateGroupRequest,
+    group_id: str,
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Remove all user related state: likes, downloads, followers, following (DeleteAllUserStates)
-
-    Required permission NAMESPACE:{namespace}:USER:{userId}" [DELETE]
+    """Update group (UpdateGroup)
 
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId} [DELETE]
+    Replace group name and contents with new ones
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/states
+        url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/groups/{groupId}
 
-        method: DELETE
+        method: PUT
 
-        tags: ["Anonymization"]
+        tags: ["Public Group"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        body: (body) REQUIRED ModelsCreateGroupRequest in body
+
+        group_id: (groupId) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        204: No Content - (User stats deleted)
+        200: OK - ModelsCreateGroupResponse (Group updated)
 
-        400: Bad Request - ResponseError (773602: user states are not found: content not found)
+        400: Bad Request - ResponseError (772201: Malformed request/Invalid request body)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (773601: Unable to get all user contents/Unable to delete user states)
+        404: Not Found - ResponseError (772203: Group not found)
+
+        500: Internal Server Error - ResponseError (772202: Unable to update group)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = DeleteAllUserStates.create(
+    request = UpdateGroup.create(
+        body=body,
+        group_id=group_id,
         user_id=user_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_channel.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_channel.py`

 * *Files 22% similar despite different names*

```diff
@@ -47,18 +47,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete Channel (DeleteChannel)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Delete user channel
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}
 
         method: DELETE
 
         tags: ["Public Channel"]
@@ -102,18 +99,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete Channel (DeleteChannel)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [DELETE]
+    Delete user channel
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}
 
         method: DELETE
 
         tags: ["Public Channel"]
@@ -161,18 +155,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get Channels (GetChannels)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
+    Get user channel paginated
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels
 
         method: GET
 
         tags: ["Public Channel"]
@@ -224,18 +215,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get Channels (GetChannels)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [READ]
+    Get user channel paginated
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels
 
         method: GET
 
         tags: ["Public Channel"]
@@ -287,18 +275,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create Channel (PublicCreateChannel)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [CREATE]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [CREATE]
+    Create user channel
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels
 
         method: POST
 
         tags: ["Public Channel"]
@@ -342,18 +327,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create Channel (PublicCreateChannel)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [CREATE]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [CREATE]
+    Create user channel
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels
 
         method: POST
 
         tags: ["Public Channel"]
@@ -400,18 +382,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Channel (UpdateChannel)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+    Update user channel
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}
 
         method: PUT
 
         tags: ["Public Channel"]
@@ -461,18 +440,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Channel (UpdateChannel)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CHANNEL [UPDATE]
+    Update user channel
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/channels/{channelId}
 
         method: PUT
 
         tags: ["Public Channel"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_content_legacy.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_content_legacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,20 +463,17 @@
     content_id: str,
     screenshot_id: str,
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete screenshots content (DeleteContentScreenshot)
+    """Delete content's screenshot (DeleteContentScreenshot)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing screenshot from a content
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots/{screenshotId}
 
         method: DELETE
 
         tags: ["Public Content (Legacy)"]
@@ -526,20 +523,17 @@
     content_id: str,
     screenshot_id: str,
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Delete screenshots content (DeleteContentScreenshot)
+    """Delete content's screenshot (DeleteContentScreenshot)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing screenshot from a content
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots/{screenshotId}
 
         method: DELETE
 
         tags: ["Public Content (Legacy)"]
@@ -2407,19 +2401,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update screenshot of content (UpdateScreenshots)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots
 
         method: PUT
 
         tags: ["Public Content (Legacy)"]
@@ -2471,19 +2461,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update screenshot of content (UpdateScreenshots)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots
 
         method: PUT
 
         tags: ["Public Content (Legacy)"]
@@ -2537,23 +2523,19 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Upload screenshots for content (UploadContentScreenshot)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-    All request body are required except for contentType field.
-    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the presigned URL.
-    If not specified, it will use fileExtension value.
-    Supported file extensions: pjp, jpg, jpeg, jfif, bmp, png.
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    All request body are required except for *contentType* field.
+    *contentType* values is used to enforce the *Content-Type* header needed by the client to upload the content using the presigned URL.
+    If not specified, it will use *fileExtension* value.
+    Supported file extensions: *pjp*, *jpg*, *jpeg*, *jfif*, *bmp*, *png*.
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots
 
         method: POST
 
         tags: ["Public Content (Legacy)"]
@@ -2605,23 +2587,19 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Upload screenshots for content (UploadContentScreenshot)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-    All request body are required except for contentType field.
-    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the presigned URL.
-    If not specified, it will use fileExtension value.
-    Supported file extensions: pjp, jpg, jpeg, jfif, bmp, png.
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    All request body are required except for *contentType* field.
+    *contentType* values is used to enforce the *Content-Type* header needed by the client to upload the content using the presigned URL.
+    If not specified, it will use *fileExtension* value.
+    Supported file extensions: *pjp*, *jpg*, *jpeg*, *jfif*, *bmp*, *png*.
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots
 
         method: POST
 
         tags: ["Public Content (Legacy)"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_content_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_content_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,18 +76,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete screenshots content (DeleteContentScreenshotV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete screenshot from a content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots/{screenshotId}
 
         method: DELETE
 
         tags: ["Public Content V2"]
@@ -139,18 +136,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete screenshots content (DeleteContentScreenshotV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete screenshot from a content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots/{screenshotId}
 
         method: DELETE
 
         tags: ["Public Content V2"]
@@ -304,18 +298,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a content (PublicCreateContentV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    Create a new content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents
 
         method: POST
 
         tags: ["Public Content V2"]
@@ -365,18 +356,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a content (PublicCreateContentV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    Create a new content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents
 
         method: POST
 
         tags: ["Public Content V2"]
@@ -428,18 +416,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete content by share code (PublicDeleteContentByShareCodeV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing content by share code
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/sharecodes/{shareCode}
 
         method: DELETE
 
         tags: ["Public Content V2"]
@@ -487,18 +472,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete content by share code (PublicDeleteContentByShareCodeV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing content by share code
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/sharecodes/{shareCode}
 
         method: DELETE
 
         tags: ["Public Content V2"]
@@ -548,18 +530,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete content (PublicDeleteContentV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}
 
         method: DELETE
 
         tags: ["Public Content V2"]
@@ -607,18 +586,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete content (PublicDeleteContentV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete existing content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}
 
         method: DELETE
 
         tags: ["Public Content V2"]
@@ -669,18 +645,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Generate content upload URL (PublicGenerateContentUploadURLV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Generate content upload URL
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/uploadUrl
 
         method: PATCH
 
         tags: ["Public Content V2"]
@@ -736,18 +709,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Generate content upload URL (PublicGenerateContentUploadURLV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Generate content upload URL
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/uploadUrl
 
         method: PATCH
 
         tags: ["Public Content V2"]
@@ -1367,28 +1337,31 @@
     type_: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List contents (PublicListContentV2)
 
-    For advance tag filtering supports & as AND operator and | as OR operator and parentheses () for priority. e.g:
+    For advance tag filtering supports & as AND operator and | as OR operator and parentheses ( ) for priority. e.g:
 
-    `tags=red`
-    `tags=red&animal;`
-    `tags=red|animal`
-    `tags=red&animal;|wild`
-    `tags=red&(animal|wild)`
+
+    *tags=red*
+    *tags=red&animal;*
+    *tags=red|animal*
+    *tags=red&animal;|wild*
+    *tags=red&(animal|wild)*
 
     The precedence of logical operator is AND > OR, so if no parentheses, AND logical operator will be executed first.
 
-    Allowed character for operand: alphanumeric, underscore `_` and dash `-`
-    Allowed character for operator: `&` `|` `(` `)`
+    Allowed character for operand: alphanumeric, underscore _ and dash -
+
+    Allowed character for operator: & | ( )
+
 
-     Please note that value of tags query param should be URL encoded
+    **Please note that value of tags query param should be URL encoded**
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/contents
 
         method: GET
 
         tags: ["Public Content V2"]
@@ -1456,28 +1429,31 @@
     type_: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List contents (PublicListContentV2)
 
-    For advance tag filtering supports & as AND operator and | as OR operator and parentheses () for priority. e.g:
+    For advance tag filtering supports & as AND operator and | as OR operator and parentheses ( ) for priority. e.g:
 
-    `tags=red`
-    `tags=red&animal;`
-    `tags=red|animal`
-    `tags=red&animal;|wild`
-    `tags=red&(animal|wild)`
+
+    *tags=red*
+    *tags=red&animal;*
+    *tags=red|animal*
+    *tags=red&animal;|wild*
+    *tags=red&(animal|wild)*
 
     The precedence of logical operator is AND > OR, so if no parentheses, AND logical operator will be executed first.
 
-    Allowed character for operand: alphanumeric, underscore `_` and dash `-`
-    Allowed character for operator: `&` `|` `(` `)`
+    Allowed character for operand: alphanumeric, underscore _ and dash -
+
+    Allowed character for operator: & | ( )
+
 
-     Please note that value of tags query param should be URL encoded
+    **Please note that value of tags query param should be URL encoded**
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/contents
 
         method: GET
 
         tags: ["Public Content V2"]
@@ -1543,18 +1519,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update content to S3 bucket by share code (PublicUpdateContentByShareCodeV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update content by share code
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/s3/sharecodes/{shareCode}
 
         method: PUT
 
         tags: ["Public Content V2"]
@@ -1612,18 +1585,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update content to S3 bucket by share code (PublicUpdateContentByShareCodeV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update content by share code
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/s3/sharecodes/{shareCode}
 
         method: PUT
 
         tags: ["Public Content V2"]
@@ -1683,19 +1653,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update content file location (PublicUpdateContentFileLocation)
 
-    This endpoint should be used after calling generate upload url endpoint to commit the changes.
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    This endpoint should be used after calling generate upload url endpoint to commit the changes
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/fileLocation
 
         method: PATCH
 
         tags: ["Public Content V2"]
@@ -1751,19 +1717,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update content file location (PublicUpdateContentFileLocation)
 
-    This endpoint should be used after calling generate upload url endpoint to commit the changes.
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    This endpoint should be used after calling generate upload url endpoint to commit the changes
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/fileLocation
 
         method: PATCH
 
         tags: ["Public Content V2"]
@@ -1821,18 +1783,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update content (PublicUpdateContentV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update existing content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}
 
         method: PATCH
 
         tags: ["Public Content V2"]
@@ -1888,18 +1847,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update content (PublicUpdateContentV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update existing content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}
 
         method: PATCH
 
         tags: ["Public Content V2"]
@@ -1957,25 +1913,20 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update content share code (UpdateContentShareCodeV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT:SHARECODE [UPDATE].
-
     This endpoint is used to modify the shareCode of a content. However, this operation is restricted by default and requires the above permission to be granted to the User role.
 
     `shareCode` format should follows:
     Max length: 7
     Available characters: abcdefhkpqrstuxyz
 
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT:SHARECODE [UPDATE]
-
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/sharecode
 
         method: PATCH
 
         tags: ["Public Content V2"]
 
@@ -2032,25 +1983,20 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update content share code (UpdateContentShareCodeV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT:SHARECODE [UPDATE].
-
     This endpoint is used to modify the shareCode of a content. However, this operation is restricted by default and requires the above permission to be granted to the User role.
 
     `shareCode` format should follows:
     Max length: 7
     Available characters: abcdefhkpqrstuxyz
 
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT:SHARECODE [UPDATE]
-
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/channels/{channelId}/contents/{contentId}/sharecode
 
         method: PATCH
 
         tags: ["Public Content V2"]
 
@@ -2108,19 +2054,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update screenshot of content (UpdateScreenshotsV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots
 
         method: PUT
 
         tags: ["Public Content V2"]
@@ -2172,19 +2114,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update screenshot of content (UpdateScreenshotsV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots
 
         method: PUT
 
         tags: ["Public Content V2"]
@@ -2238,23 +2176,18 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Upload screenshots for content (UploadContentScreenshotV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-    All request body are required except for contentType field.
-    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the presigned URL.
-    If not specified, it will use fileExtension value.
+    This endpoint used to request upload URL from content's screenshot.
+    If *contentType* is not specified, it will use *fileExtension* value.
     Supported file extensions: pjp, jpg, jpeg, jfif, bmp, png.
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots
 
         method: POST
 
         tags: ["Public Content V2"]
@@ -2304,23 +2237,18 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Upload screenshots for content (UploadContentScreenshotV2)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE].
-    All request body are required except for contentType field.
-    contentType values is used to enforce the Content-Type header needed by the client to upload the content using the presigned URL.
-    If not specified, it will use fileExtension value.
+    This endpoint used to request upload URL from content's screenshot.
+    If *contentType* is not specified, it will use *fileExtension* value.
     Supported file extensions: pjp, jpg, jpeg, jfif, bmp, png.
-    Maximum description length: 1024.
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [CREATE]
+    Maximum description length: 1024
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/contents/{contentId}/screenshots
 
         method: POST
 
         tags: ["Public Content V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_creator.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_creator.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_download_count_legacy.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_download_count_legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Add unique download count to a content (AddDownloadCount)
 
-    Requires valid user token
+    This endpoint can be used to count how many the ugc downloaded
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/contents/{contentId}/downloadcount
 
         method: POST
 
         tags: ["Public Download Count (Legacy)"]
@@ -88,15 +88,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Add unique download count to a content (AddDownloadCount)
 
-    Requires valid user token
+    This endpoint can be used to count how many the ugc downloaded
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/contents/{contentId}/downloadcount
 
         method: POST
 
         tags: ["Public Download Count (Legacy)"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_download_count_v2.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_download_count_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Add unique download count to a content (PublicAddDownloadCountV2)
 
-    Requires valid user token
+    This endpoint can be used to count how many the ugc downloaded
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/contents/{contentId}/downloadcount
 
         method: POST
 
         tags: ["Public Download Count V2"]
@@ -92,15 +92,15 @@
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Add unique download count to a content (PublicAddDownloadCountV2)
 
-    Requires valid user token
+    This endpoint can be used to count how many the ugc downloaded
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/contents/{contentId}/downloadcount
 
         method: POST
 
         tags: ["Public Download Count V2"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_follow.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_follow.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_like_legacy.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_like_v2.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,241 +27,161 @@
 from accelbyte_py_sdk.core import get_namespace as get_services_namespace
 from accelbyte_py_sdk.core import run_request
 from accelbyte_py_sdk.core import run_request_async
 from accelbyte_py_sdk.core import same_doc_as
 
 from ..models import ModelsContentLikeRequest
 from ..models import ModelsContentLikeResponse
-from ..models import ModelsPaginatedContentDownloadResponse
+from ..models import ModelsPaginatedContentLikersResponse
 from ..models import ResponseError
 
-from ..operations.public_like_legacy import GetLikedContent
-from ..operations.public_like_legacy import UpdateContentLikeStatus
+from ..operations.public_like_v2 import PublicListContentLikeV2
+from ..operations.public_like_v2 import UpdateContentLikeStatusV2
 
 
-@same_doc_as(GetLikedContent)
-def get_liked_content(
-    isofficial: Optional[bool] = None,
+@same_doc_as(PublicListContentLikeV2)
+def public_list_content_like_v2(
+    content_id: str,
     limit: Optional[int] = None,
-    name: Optional[str] = None,
     offset: Optional[int] = None,
-    orderby: Optional[str] = None,
-    sortby: Optional[str] = None,
-    subtype: Optional[str] = None,
-    tags: Optional[List[str]] = None,
-    type_: Optional[str] = None,
+    sort_by: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Get liked contents (GetLikedContent)
-
-    Requires valid user token.
-
-    For advance tag filtering supports & as AND operator and | as OR operator and parentheses () for priority. e.g:
-
-    `tags=red`
-
-    `tags=red&animal;`
-
-    `tags=red|animal`
-
-    `tags=red&animal;|wild`
-
-    `tags=red&(animal|wild)`
-
-    The precedence of logical operator is AND > OR, so if no parentheses, AND logical operator will be executed first.
-
-    Allowed character for operand: alphanumeric, underscore `_` and dash `-`
-
-    Allowed character for operator: `&` `|` `(` `)`
+    """Retrieve list of user that like specified content. (PublicListContentLikeV2)
 
-     Please note that value of tags query param should be URL encoded
+    This endpoint will only display the list of users who performed like from v2 endpoint.
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/contents/liked
+        url: /ugc/v2/public/namespaces/{namespace}/contents/{contentId}/like
 
         method: GET
 
-        tags: ["Public Like (Legacy)"]
+        tags: ["Public Like V2"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        namespace: (namespace) REQUIRED str in path
+        content_id: (contentId) REQUIRED str in path
 
-        isofficial: (isofficial) OPTIONAL bool in query
+        namespace: (namespace) REQUIRED str in path
 
         limit: (limit) OPTIONAL int in query
 
-        name: (name) OPTIONAL str in query
-
         offset: (offset) OPTIONAL int in query
 
-        orderby: (orderby) OPTIONAL str in query
-
-        sortby: (sortby) OPTIONAL str in query
-
-        subtype: (subtype) OPTIONAL str in query
-
-        tags: (tags) OPTIONAL List[str] in query
-
-        type_: (type) OPTIONAL str in query
+        sort_by: (sortBy) OPTIONAL str in query
 
     Responses:
-        200: OK - ModelsPaginatedContentDownloadResponse (Get liked contents)
+        200: OK - ModelsPaginatedContentLikersResponse (Retrieve list of user liked content)
 
-        400: Bad Request - ResponseError (771100: unable to parse isofficial param)
+        400: Bad Request - ResponseError (771004: invalid paging parameter)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (771101: Unable to get ugc content: database error | 770801: Unable to get ugc content: database/Unable to get creator | 770803: Failed generate download URL)
+        500: Internal Server Error - ResponseError (771006: unable to get list of content like: database error)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = GetLikedContent.create(
-        isofficial=isofficial,
+    request = PublicListContentLikeV2.create(
+        content_id=content_id,
         limit=limit,
-        name=name,
         offset=offset,
-        orderby=orderby,
-        sortby=sortby,
-        subtype=subtype,
-        tags=tags,
-        type_=type_,
+        sort_by=sort_by,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(GetLikedContent)
-async def get_liked_content_async(
-    isofficial: Optional[bool] = None,
+@same_doc_as(PublicListContentLikeV2)
+async def public_list_content_like_v2_async(
+    content_id: str,
     limit: Optional[int] = None,
-    name: Optional[str] = None,
     offset: Optional[int] = None,
-    orderby: Optional[str] = None,
-    sortby: Optional[str] = None,
-    subtype: Optional[str] = None,
-    tags: Optional[List[str]] = None,
-    type_: Optional[str] = None,
+    sort_by: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Get liked contents (GetLikedContent)
+    """Retrieve list of user that like specified content. (PublicListContentLikeV2)
 
-    Requires valid user token.
-
-    For advance tag filtering supports & as AND operator and | as OR operator and parentheses () for priority. e.g:
-
-    `tags=red`
-
-    `tags=red&animal;`
-
-    `tags=red|animal`
-
-    `tags=red&animal;|wild`
-
-    `tags=red&(animal|wild)`
-
-    The precedence of logical operator is AND > OR, so if no parentheses, AND logical operator will be executed first.
-
-    Allowed character for operand: alphanumeric, underscore `_` and dash `-`
-
-    Allowed character for operator: `&` `|` `(` `)`
-
-     Please note that value of tags query param should be URL encoded
+    This endpoint will only display the list of users who performed like from v2 endpoint.
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/contents/liked
+        url: /ugc/v2/public/namespaces/{namespace}/contents/{contentId}/like
 
         method: GET
 
-        tags: ["Public Like (Legacy)"]
+        tags: ["Public Like V2"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        namespace: (namespace) REQUIRED str in path
+        content_id: (contentId) REQUIRED str in path
 
-        isofficial: (isofficial) OPTIONAL bool in query
+        namespace: (namespace) REQUIRED str in path
 
         limit: (limit) OPTIONAL int in query
 
-        name: (name) OPTIONAL str in query
-
         offset: (offset) OPTIONAL int in query
 
-        orderby: (orderby) OPTIONAL str in query
-
-        sortby: (sortby) OPTIONAL str in query
-
-        subtype: (subtype) OPTIONAL str in query
-
-        tags: (tags) OPTIONAL List[str] in query
-
-        type_: (type) OPTIONAL str in query
+        sort_by: (sortBy) OPTIONAL str in query
 
     Responses:
-        200: OK - ModelsPaginatedContentDownloadResponse (Get liked contents)
+        200: OK - ModelsPaginatedContentLikersResponse (Retrieve list of user liked content)
 
-        400: Bad Request - ResponseError (771100: unable to parse isofficial param)
+        400: Bad Request - ResponseError (771004: invalid paging parameter)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        500: Internal Server Error - ResponseError (771101: Unable to get ugc content: database error | 770801: Unable to get ugc content: database/Unable to get creator | 770803: Failed generate download URL)
+        500: Internal Server Error - ResponseError (771006: unable to get list of content like: database error)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = GetLikedContent.create(
-        isofficial=isofficial,
+    request = PublicListContentLikeV2.create(
+        content_id=content_id,
         limit=limit,
-        name=name,
         offset=offset,
-        orderby=orderby,
-        sortby=sortby,
-        subtype=subtype,
-        tags=tags,
-        type_=type_,
+        sort_by=sort_by,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(UpdateContentLikeStatus)
-def update_content_like_status(
+@same_doc_as(UpdateContentLikeStatusV2)
+def update_content_like_status_v2(
     body: ModelsContentLikeRequest,
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Update like/unlike status to a content (UpdateContentLikeStatus)
+    """Update like/unlike status to a content (UpdateContentLikeStatusV2)
 
-    Requires valid user token
+    This endpoint will update like/unlike state from a content
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/contents/{contentId}/like
+        url: /ugc/v2/public/namespaces/{namespace}/contents/{contentId}/like
 
         method: PUT
 
-        tags: ["Public Like (Legacy)"]
+        tags: ["Public Like V2"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -274,48 +194,50 @@
     Responses:
         200: OK - ModelsContentLikeResponse (Update like/unlike status to a content)
 
         400: Bad Request - ResponseError (771000: Malformed request/Content not found/Unable to update like status: content not found)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (771000: Malformed request/Content not found/Unable to update like status: content not found | 771001: unable to like content/Unable to update like status: database error | 771000: Malformed request/Content not found/Unable to update like status: content not found)
+        404: Not Found - ResponseError (770200: Content not found | 771001: unable to like content/Unable to update like status: database error | 771000: Malformed request/Content not found/Unable to update like status: content not found)
+
+        429: Too Many Requests - ResponseError (771003: Unable to like content: too many request)
 
         500: Internal Server Error - ResponseError (771001: unable to like content/Unable to update like status: database error)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = UpdateContentLikeStatus.create(
+    request = UpdateContentLikeStatusV2.create(
         body=body,
         content_id=content_id,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(UpdateContentLikeStatus)
-async def update_content_like_status_async(
+@same_doc_as(UpdateContentLikeStatusV2)
+async def update_content_like_status_v2_async(
     body: ModelsContentLikeRequest,
     content_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Update like/unlike status to a content (UpdateContentLikeStatus)
+    """Update like/unlike status to a content (UpdateContentLikeStatusV2)
 
-    Requires valid user token
+    This endpoint will update like/unlike state from a content
 
     Properties:
-        url: /ugc/v1/public/namespaces/{namespace}/contents/{contentId}/like
+        url: /ugc/v2/public/namespaces/{namespace}/contents/{contentId}/like
 
         method: PUT
 
-        tags: ["Public Like (Legacy)"]
+        tags: ["Public Like V2"]
 
         consumes: ["application/json", "application/octet-stream"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -328,23 +250,25 @@
     Responses:
         200: OK - ModelsContentLikeResponse (Update like/unlike status to a content)
 
         400: Bad Request - ResponseError (771000: Malformed request/Content not found/Unable to update like status: content not found)
 
         401: Unauthorized - ResponseError (20001: unauthorized access)
 
-        404: Not Found - ResponseError (771000: Malformed request/Content not found/Unable to update like status: content not found | 771001: unable to like content/Unable to update like status: database error | 771000: Malformed request/Content not found/Unable to update like status: content not found)
+        404: Not Found - ResponseError (770200: Content not found | 771001: unable to like content/Unable to update like status: database error | 771000: Malformed request/Content not found/Unable to update like status: content not found)
+
+        429: Too Many Requests - ResponseError (771003: Unable to like content: too many request)
 
         500: Internal Server Error - ResponseError (771001: unable to like content/Unable to update like status: database error)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = UpdateContentLikeStatus.create(
+    request = UpdateContentLikeStatusV2.create(
         body=body,
         content_id=content_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_staging_content.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_staging_content.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,18 +47,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete user staging content by id (DeleteUserStagingContentByID)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete user staging content by ID
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents/{contentId}
 
         method: DELETE
 
         tags: ["Public Staging Content"]
@@ -104,18 +101,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete user staging content by id (DeleteUserStagingContentByID)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [DELETE]
+    Delete user staging content by ID
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents/{contentId}
 
         method: DELETE
 
         tags: ["Public Staging Content"]
@@ -163,18 +157,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get user staging content by id (GetUserStagingContentByID)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get user staging content by ID
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents/{contentId}
 
         method: GET
 
         tags: ["Public Staging Content"]
@@ -220,18 +211,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get user staging content by id (GetUserStagingContentByID)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    Get user staging content by ID
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents/{contentId}
 
         method: GET
 
         tags: ["Public Staging Content"]
@@ -282,18 +270,15 @@
     status: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List user staging contents (ListUserStagingContents)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    List user staging contents
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents
 
         method: GET
 
         tags: ["Public Staging Content"]
@@ -351,18 +336,15 @@
     status: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """List user staging contents (ListUserStagingContents)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [READ]
+    List user staging contents
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents
 
         method: GET
 
         tags: ["Public Staging Content"]
@@ -420,18 +402,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update staging content (UpdateStagingContent)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update staging content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents/{contentId}
 
         method: PUT
 
         tags: ["Public Staging Content"]
@@ -483,18 +462,15 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update staging content (UpdateStagingContent)
 
-    Required permission NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE].
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:USER:{userId}:CONTENT [UPDATE]
+    Update staging content
 
     Properties:
         url: /ugc/v2/public/namespaces/{namespace}/users/{userId}/staging-contents/{contentId}
 
         method: PUT
 
         tags: ["Public Staging Content"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_tag.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get tags (GetTag)
 
-    Publicly accessible
+    Get available tags paginated
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/tags
 
         method: GET
 
         tags: ["Public Tag"]
@@ -93,15 +93,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get tags (GetTag)
 
-    Publicly accessible
+    Get available tags paginated
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/tags
 
         method: GET
 
         tags: ["Public Tag"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk/api/ugc/wrappers/_public_type.py` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk/api/ugc/wrappers/_public_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get types (GetType)
 
-    Requires valid user token
+    Get available types paginated
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/types
 
         method: GET
 
         tags: ["Public Type"]
@@ -93,15 +93,15 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get types (GetType)
 
-    Requires valid user token
+    Get available types paginated
 
     Properties:
         url: /ugc/v1/public/namespaces/{namespace}/types
 
         method: GET
 
         tags: ["Public Type"]
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk_service_ugc.egg-info/PKG-INFO` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk_service_ugc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-ugc
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Ugc Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Ugc Service
-* Version: 2.19.6
+* Version: 2.19.7
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-ugc-0.8.0/accelbyte_py_sdk_service_ugc.egg-info/SOURCES.txt` & `accelbyte-py-sdk-service-ugc-0.9.0/accelbyte_py_sdk_service_ugc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

