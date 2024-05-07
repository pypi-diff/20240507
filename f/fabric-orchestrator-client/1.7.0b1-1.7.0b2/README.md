# Comparing `tmp/fabric-orchestrator-client-1.7.0b1.tar.gz` & `tmp/fabric-orchestrator-client-1.7.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-orchestrator-client-1.7.0b1.tar", last modified: Mon Apr 15 21:31:29 2024, max compression
+gzip compressed data, was "fabric-orchestrator-client-1.7.0b2.tar", last modified: Tue May  7 21:30:34 2024, max compression
```

## Comparing `fabric-orchestrator-client-1.7.0b1.tar` & `fabric-orchestrator-client-1.7.0b2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0      793 2024-01-12 03:42:46.101822 fabric-orchestrator-client-1.7.0b1/.gitignore
--rw-r--r--   0        0        0     1030 2024-01-12 03:42:46.102099 fabric-orchestrator-client-1.7.0b1/.swagger-codegen-ignore
--rw-r--r--   0        0        0        7 2024-04-05 22:19:27.031216 fabric-orchestrator-client-1.7.0b1/.swagger-codegen/VERSION
--rw-r--r--   0        0        0      349 2024-01-12 03:42:46.102462 fabric-orchestrator-client-1.7.0b1/.travis.yml
--rw-r--r--   0        0        0      770 2024-01-12 03:42:46.103447 fabric-orchestrator-client-1.7.0b1/CODEGEN.md
--rw-r--r--   0        0        0     1071 2024-01-12 03:42:46.103789 fabric-orchestrator-client-1.7.0b1/LICENSE
--rw-r--r--   0        0        0       59 2024-01-12 03:42:46.103927 fabric-orchestrator-client-1.7.0b1/MANIFEST.in
--rw-r--r--   0        0        0    10034 2024-04-05 22:21:50.264153 fabric-orchestrator-client-1.7.0b1/README.md
--rw-r--r--   0        0        0      340 2024-01-12 03:42:46.104503 fabric-orchestrator-client-1.7.0b1/docs/Poa.md
--rw-r--r--   0        0        0      557 2024-01-12 03:42:46.104673 fabric-orchestrator-client-1.7.0b1/docs/PoaData.md
--rw-r--r--   0        0        0      376 2024-01-12 03:42:46.104783 fabric-orchestrator-client-1.7.0b1/docs/PoaPost.md
--rw-r--r--   0        0        0      506 2024-01-12 03:42:46.104909 fabric-orchestrator-client-1.7.0b1/docs/PoaPostData.md
--rw-r--r--   0        0        0      344 2024-01-12 03:42:46.105043 fabric-orchestrator-client-1.7.0b1/docs/PoaPostDataKeys.md
--rw-r--r--   0        0        0      347 2024-01-12 03:42:46.105181 fabric-orchestrator-client-1.7.0b1/docs/PoaPostDataVcpuCpuMap.md
--rw-r--r--   0        0        0     6404 2024-01-12 03:42:46.105378 fabric-orchestrator-client-1.7.0b1/docs/PoasApi.md
--rw-r--r--   0        0        0     5067 2024-04-15 15:10:09.775273 fabric-orchestrator-client-1.7.0b1/docs/ResourcesApi.md
--rw-r--r--   0        0        0    21005 2024-04-05 22:21:01.694717 fabric-orchestrator-client-1.7.0b1/docs/SlicesApi.md
--rw-r--r--   0        0        0     4102 2024-01-12 03:42:46.105832 fabric-orchestrator-client-1.7.0b1/docs/SliversApi.md
--rw-r--r--   0        0        0      335 2024-01-12 03:42:46.105947 fabric-orchestrator-client-1.7.0b1/docs/Success.md
--rw-r--r--   0        0        0      352 2024-01-12 03:42:46.106047 fabric-orchestrator-client-1.7.0b1/docs/Version.md
--rw-r--r--   0        0        0       24 2024-04-15 21:30:48.912389 fabric-orchestrator-client-1.7.0b1/fabric_cf/__init__.py
--rw-r--r--   0        0        0        0 2024-01-12 03:42:46.106357 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0        0        0    23053 2024-04-15 15:14:36.619887 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/orchestrator_proxy.py
--rw-r--r--   0        0        0     3649 2024-01-12 03:42:46.106764 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/__init__.py
--rw-r--r--   0        0        0      468 2024-01-12 03:42:46.106916 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/__init__.py
--rw-r--r--   0        0        0    13557 2024-01-12 03:42:46.107141 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/poas_api.py
--rw-r--r--   0        0        0    10809 2024-04-15 15:11:50.036544 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/resources_api.py
--rw-r--r--   0        0        0    44836 2024-04-05 22:26:59.835003 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/slices_api.py
--rw-r--r--   0        0        0     9260 2024-01-12 03:42:46.107691 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
--rw-r--r--   0        0        0     3748 2024-01-12 03:42:46.107811 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/version_api.py
--rw-r--r--   0        0        0    25272 2024-01-12 03:42:46.107971 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api_client.py
--rw-r--r--   0        0        0     8240 2024-01-12 03:42:46.108170 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/configuration.py
--rw-r--r--   0        0        0     3070 2024-04-05 22:28:49.311561 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     3427 2024-01-12 03:42:46.108447 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa.py
--rw-r--r--   0        0        0     6654 2024-01-12 03:42:46.108554 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_data.py
--rw-r--r--   0        0        0     4057 2024-01-12 03:42:46.108900 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post.py
--rw-r--r--   0        0        0     4505 2024-01-12 03:42:46.109052 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py
--rw-r--r--   0        0        0     3804 2024-01-12 03:42:46.109164 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_keys.py
--rw-r--r--   0        0        0     3813 2024-01-12 03:42:46.109262 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     3055 2024-01-12 03:42:46.109386 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/resource.py
--rw-r--r--   0        0        0     3420 2024-01-12 03:42:46.109491 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/resources.py
--rw-r--r--   0        0        0     9914 2024-04-05 22:29:14.527230 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slice.py
--rw-r--r--   0        0        0     3444 2024-01-12 03:42:46.109991 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slice_details.py
--rw-r--r--   0        0        0     3412 2024-01-12 03:42:46.110167 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slices.py
--rw-r--r--   0        0        0     3951 2024-01-12 03:42:46.110282 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slices_post.py
--rw-r--r--   0        0        0    12331 2024-04-05 22:29:46.008920 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/sliver.py
--rw-r--r--   0        0        0     3422 2024-01-12 03:42:46.110560 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slivers.py
--rw-r--r--   0        0        0     4999 2024-01-12 03:42:46.110692 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     3832 2024-01-12 03:42:46.110803 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     6211 2024-01-12 03:42:46.110942 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     4253 2024-01-12 03:42:46.111050 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
--rw-r--r--   0        0        0     3163 2024-01-12 03:42:46.111145 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
--rw-r--r--   0        0        0     5771 2024-01-12 03:42:46.111249 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     5063 2024-01-12 03:42:46.111344 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0        0        0     3870 2024-01-12 03:42:46.111451 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     4994 2024-01-12 03:42:46.111569 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
--rw-r--r--   0        0        0     3831 2024-01-12 03:42:46.111663 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     4971 2024-01-12 03:42:46.111759 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
--rw-r--r--   0        0        0     3819 2024-01-12 03:42:46.111853 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     5224 2024-01-12 03:42:46.111956 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     3963 2024-01-12 03:42:46.112233 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     3413 2024-01-12 03:42:46.112337 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/version.py
--rw-r--r--   0        0        0     3882 2024-01-12 03:42:46.112446 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/version_data.py
--rw-r--r--   0        0        0    12985 2024-04-05 22:30:18.293171 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/rest.py
--rw-r--r--   0        0        0     1663 2024-01-12 03:42:46.112753 fabric-orchestrator-client-1.7.0b1/git_push.sh
--rw-r--r--   0        0        0     1024 2024-04-05 22:18:00.458232 fabric-orchestrator-client-1.7.0b1/pyproject.toml
--rw-r--r--   0        0        0       16 2024-01-12 03:42:46.112995 fabric-orchestrator-client-1.7.0b1/test/__init__.py
--rw-r--r--   0        0        0      809 2024-01-12 03:42:46.113118 fabric-orchestrator-client-1.7.0b1/test/test_poa.py
--rw-r--r--   0        0        0      843 2024-01-12 03:42:46.113207 fabric-orchestrator-client-1.7.0b1/test/test_poa_data.py
--rw-r--r--   0        0        0      843 2024-01-12 03:42:46.113308 fabric-orchestrator-client-1.7.0b1/test/test_poa_post.py
--rw-r--r--   0        0        0      877 2024-01-12 03:42:46.113402 fabric-orchestrator-client-1.7.0b1/test/test_poa_post_data.py
--rw-r--r--   0        0        0      963 2024-01-12 03:42:46.113498 fabric-orchestrator-client-1.7.0b1/test/test_poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     1157 2024-01-12 03:42:46.113583 fabric-orchestrator-client-1.7.0b1/test/test_poas_api.py
--rw-r--r--   0        0        0      896 2024-01-12 03:42:46.113672 fabric-orchestrator-client-1.7.0b1/test/test_resource.py
--rw-r--r--   0        0        0      950 2024-01-12 03:42:46.113770 fabric-orchestrator-client-1.7.0b1/test/test_resources.py
--rw-r--r--   0        0        0     1206 2024-01-12 03:42:46.113870 fabric-orchestrator-client-1.7.0b1/test/test_resources_api.py
--rw-r--r--   0        0        0      872 2024-01-12 03:42:46.113959 fabric-orchestrator-client-1.7.0b1/test/test_slice.py
--rw-r--r--   0        0        0      930 2024-01-12 03:42:46.114058 fabric-orchestrator-client-1.7.0b1/test/test_slice_details.py
--rw-r--r--   0        0        0      880 2024-01-12 03:42:46.114249 fabric-orchestrator-client-1.7.0b1/test/test_slices.py
--rw-r--r--   0        0        0     2165 2024-01-12 03:42:46.114383 fabric-orchestrator-client-1.7.0b1/test/test_slices_api.py
--rw-r--r--   0        0        0      867 2024-01-12 03:42:46.114477 fabric-orchestrator-client-1.7.0b1/test/test_slices_post.py
--rw-r--r--   0        0        0      880 2024-01-12 03:42:46.114575 fabric-orchestrator-client-1.7.0b1/test/test_sliver.py
--rw-r--r--   0        0        0      888 2024-01-12 03:42:46.114670 fabric-orchestrator-client-1.7.0b1/test/test_slivers.py
--rw-r--r--   0        0        0      974 2024-01-12 03:42:46.114770 fabric-orchestrator-client-1.7.0b1/test/test_slivers_api.py
--rw-r--r--   0        0        0      998 2024-01-12 03:42:46.114861 fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_no_content.py
--rw-r--r--   0        0        0     1032 2024-01-12 03:42:46.114968 fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_no_content_data.py
--rw-r--r--   0        0        0      996 2024-01-12 03:42:46.115068 fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_paginated.py
--rw-r--r--   0        0        0      972 2024-01-12 03:42:46.115159 fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_single.py
--rw-r--r--   0        0        0      988 2024-01-12 03:42:46.115251 fabric-orchestrator-client-1.7.0b1/test/test_status400_bad_request.py
--rw-r--r--   0        0        0     1038 2024-01-12 03:42:46.115351 fabric-orchestrator-client-1.7.0b1/test/test_status400_bad_request_errors.py
--rw-r--r--   0        0        0     1002 2024-01-12 03:42:46.115454 fabric-orchestrator-client-1.7.0b1/test/test_status401_unauthorized.py
--rw-r--r--   0        0        0     1052 2024-01-12 03:42:46.115553 fabric-orchestrator-client-1.7.0b1/test/test_status401_unauthorized_errors.py
--rw-r--r--   0        0        0      978 2024-01-12 03:42:46.115643 fabric-orchestrator-client-1.7.0b1/test/test_status403_forbidden.py
--rw-r--r--   0        0        0     1028 2024-01-12 03:42:46.115743 fabric-orchestrator-client-1.7.0b1/test/test_status403_forbidden_errors.py
--rw-r--r--   0        0        0      972 2024-01-12 03:42:46.115834 fabric-orchestrator-client-1.7.0b1/test/test_status404_not_found.py
--rw-r--r--   0        0        0     1022 2024-01-12 03:42:46.115939 fabric-orchestrator-client-1.7.0b1/test/test_status404_not_found_errors.py
--rw-r--r--   0        0        0     1062 2024-01-12 03:42:46.116047 fabric-orchestrator-client-1.7.0b1/test/test_status500_internal_server_error.py
--rw-r--r--   0        0        0     1112 2024-01-12 03:42:46.116160 fabric-orchestrator-client-1.7.0b1/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0        0        0      888 2024-01-12 03:42:46.116255 fabric-orchestrator-client-1.7.0b1/test/test_version.py
--rw-r--r--   0        0        0      814 2024-01-12 03:42:46.116365 fabric-orchestrator-client-1.7.0b1/test/test_version_api.py
--rw-r--r--   0        0        0      922 2024-01-12 03:42:46.116524 fabric-orchestrator-client-1.7.0b1/test/test_version_data.py
--rw-r--r--   0        0        0      143 2024-01-12 03:42:46.116674 fabric-orchestrator-client-1.7.0b1/tox.ini
--rw-r--r--   0        0        0    10985 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.7.0b1/PKG-INFO
+-rw-r--r--   0        0        0      793 2024-01-12 03:42:46.101822 fabric-orchestrator-client-1.7.0b2/.gitignore
+-rw-r--r--   0        0        0     1030 2024-01-12 03:42:46.102099 fabric-orchestrator-client-1.7.0b2/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2024-04-05 22:19:27.031216 fabric-orchestrator-client-1.7.0b2/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2024-01-12 03:42:46.102462 fabric-orchestrator-client-1.7.0b2/.travis.yml
+-rw-r--r--   0        0        0      770 2024-01-12 03:42:46.103447 fabric-orchestrator-client-1.7.0b2/CODEGEN.md
+-rw-r--r--   0        0        0     1071 2024-01-12 03:42:46.103789 fabric-orchestrator-client-1.7.0b2/LICENSE
+-rw-r--r--   0        0        0       59 2024-01-12 03:42:46.103927 fabric-orchestrator-client-1.7.0b2/MANIFEST.in
+-rw-r--r--   0        0        0    10034 2024-04-05 22:21:50.264153 fabric-orchestrator-client-1.7.0b2/README.md
+-rw-r--r--   0        0        0      340 2024-01-12 03:42:46.104503 fabric-orchestrator-client-1.7.0b2/docs/Poa.md
+-rw-r--r--   0        0        0      557 2024-01-12 03:42:46.104673 fabric-orchestrator-client-1.7.0b2/docs/PoaData.md
+-rw-r--r--   0        0        0      376 2024-01-12 03:42:46.104783 fabric-orchestrator-client-1.7.0b2/docs/PoaPost.md
+-rw-r--r--   0        0        0      506 2024-01-12 03:42:46.104909 fabric-orchestrator-client-1.7.0b2/docs/PoaPostData.md
+-rw-r--r--   0        0        0      344 2024-01-12 03:42:46.105043 fabric-orchestrator-client-1.7.0b2/docs/PoaPostDataKeys.md
+-rw-r--r--   0        0        0      347 2024-01-12 03:42:46.105181 fabric-orchestrator-client-1.7.0b2/docs/PoaPostDataVcpuCpuMap.md
+-rw-r--r--   0        0        0     6404 2024-01-12 03:42:46.105378 fabric-orchestrator-client-1.7.0b2/docs/PoasApi.md
+-rw-r--r--   0        0        0     6399 2024-04-17 02:23:54.719199 fabric-orchestrator-client-1.7.0b2/docs/ResourcesApi.md
+-rw-r--r--   0        0        0    21291 2024-04-17 15:13:57.283895 fabric-orchestrator-client-1.7.0b2/docs/SlicesApi.md
+-rw-r--r--   0        0        0     4102 2024-01-12 03:42:46.105832 fabric-orchestrator-client-1.7.0b2/docs/SliversApi.md
+-rw-r--r--   0        0        0      335 2024-01-12 03:42:46.105947 fabric-orchestrator-client-1.7.0b2/docs/Success.md
+-rw-r--r--   0        0        0      352 2024-01-12 03:42:46.106047 fabric-orchestrator-client-1.7.0b2/docs/Version.md
+-rw-r--r--   0        0        0       24 2024-04-17 15:18:33.120939 fabric-orchestrator-client-1.7.0b2/fabric_cf/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-12 03:42:46.106357 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0        0        0    23598 2024-05-07 21:26:43.695878 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/orchestrator_proxy.py
+-rw-r--r--   0        0        0     3649 2024-01-12 03:42:46.106764 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/__init__.py
+-rw-r--r--   0        0        0      468 2024-01-12 03:42:46.106916 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0    13557 2024-01-12 03:42:46.107141 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/poas_api.py
+-rw-r--r--   0        0        0    12556 2024-04-17 02:23:07.530313 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/resources_api.py
+-rw-r--r--   0        0        0    45209 2024-04-17 15:16:58.826551 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/slices_api.py
+-rw-r--r--   0        0        0     9260 2024-01-12 03:42:46.107691 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
+-rw-r--r--   0        0        0     3748 2024-01-12 03:42:46.107811 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25272 2024-01-12 03:42:46.107971 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8240 2024-01-12 03:42:46.108170 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/configuration.py
+-rw-r--r--   0        0        0     3070 2024-04-05 22:28:49.311561 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     3427 2024-01-12 03:42:46.108447 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa.py
+-rw-r--r--   0        0        0     6654 2024-01-12 03:42:46.108554 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_data.py
+-rw-r--r--   0        0        0     4057 2024-01-12 03:42:46.108900 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post.py
+-rw-r--r--   0        0        0     4505 2024-01-12 03:42:46.109052 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py
+-rw-r--r--   0        0        0     3804 2024-01-12 03:42:46.109164 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post_data_keys.py
+-rw-r--r--   0        0        0     3813 2024-01-12 03:42:46.109262 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     3055 2024-01-12 03:42:46.109386 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/resource.py
+-rw-r--r--   0        0        0     3420 2024-01-12 03:42:46.109491 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/resources.py
+-rw-r--r--   0        0        0     9914 2024-04-05 22:29:14.527230 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slice.py
+-rw-r--r--   0        0        0     3444 2024-01-12 03:42:46.109991 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slice_details.py
+-rw-r--r--   0        0        0     3412 2024-01-12 03:42:46.110167 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slices.py
+-rw-r--r--   0        0        0     3951 2024-01-12 03:42:46.110282 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slices_post.py
+-rw-r--r--   0        0        0    12331 2024-04-05 22:29:46.008920 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/sliver.py
+-rw-r--r--   0        0        0     3422 2024-01-12 03:42:46.110560 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slivers.py
+-rw-r--r--   0        0        0     4999 2024-01-12 03:42:46.110692 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3832 2024-01-12 03:42:46.110803 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     6211 2024-01-12 03:42:46.110942 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     4253 2024-01-12 03:42:46.111050 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3163 2024-01-12 03:42:46.111145 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5771 2024-01-12 03:42:46.111249 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5063 2024-01-12 03:42:46.111344 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3870 2024-01-12 03:42:46.111451 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     4994 2024-01-12 03:42:46.111569 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3831 2024-01-12 03:42:46.111663 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4971 2024-01-12 03:42:46.111759 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3819 2024-01-12 03:42:46.111853 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5224 2024-01-12 03:42:46.111956 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3963 2024-01-12 03:42:46.112233 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3413 2024-01-12 03:42:46.112337 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3882 2024-01-12 03:42:46.112446 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    12985 2024-04-05 22:30:18.293171 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2024-01-12 03:42:46.112753 fabric-orchestrator-client-1.7.0b2/git_push.sh
+-rw-r--r--   0        0        0     1024 2024-04-05 22:18:00.458232 fabric-orchestrator-client-1.7.0b2/pyproject.toml
+-rw-r--r--   0        0        0       16 2024-01-12 03:42:46.112995 fabric-orchestrator-client-1.7.0b2/test/__init__.py
+-rw-r--r--   0        0        0      809 2024-01-12 03:42:46.113118 fabric-orchestrator-client-1.7.0b2/test/test_poa.py
+-rw-r--r--   0        0        0      843 2024-01-12 03:42:46.113207 fabric-orchestrator-client-1.7.0b2/test/test_poa_data.py
+-rw-r--r--   0        0        0      843 2024-01-12 03:42:46.113308 fabric-orchestrator-client-1.7.0b2/test/test_poa_post.py
+-rw-r--r--   0        0        0      877 2024-01-12 03:42:46.113402 fabric-orchestrator-client-1.7.0b2/test/test_poa_post_data.py
+-rw-r--r--   0        0        0      963 2024-01-12 03:42:46.113498 fabric-orchestrator-client-1.7.0b2/test/test_poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     1157 2024-01-12 03:42:46.113583 fabric-orchestrator-client-1.7.0b2/test/test_poas_api.py
+-rw-r--r--   0        0        0      896 2024-01-12 03:42:46.113672 fabric-orchestrator-client-1.7.0b2/test/test_resource.py
+-rw-r--r--   0        0        0      950 2024-01-12 03:42:46.113770 fabric-orchestrator-client-1.7.0b2/test/test_resources.py
+-rw-r--r--   0        0        0     1206 2024-01-12 03:42:46.113870 fabric-orchestrator-client-1.7.0b2/test/test_resources_api.py
+-rw-r--r--   0        0        0      872 2024-01-12 03:42:46.113959 fabric-orchestrator-client-1.7.0b2/test/test_slice.py
+-rw-r--r--   0        0        0      930 2024-01-12 03:42:46.114058 fabric-orchestrator-client-1.7.0b2/test/test_slice_details.py
+-rw-r--r--   0        0        0      880 2024-01-12 03:42:46.114249 fabric-orchestrator-client-1.7.0b2/test/test_slices.py
+-rw-r--r--   0        0        0     2165 2024-01-12 03:42:46.114383 fabric-orchestrator-client-1.7.0b2/test/test_slices_api.py
+-rw-r--r--   0        0        0      867 2024-01-12 03:42:46.114477 fabric-orchestrator-client-1.7.0b2/test/test_slices_post.py
+-rw-r--r--   0        0        0      880 2024-01-12 03:42:46.114575 fabric-orchestrator-client-1.7.0b2/test/test_sliver.py
+-rw-r--r--   0        0        0      888 2024-01-12 03:42:46.114670 fabric-orchestrator-client-1.7.0b2/test/test_slivers.py
+-rw-r--r--   0        0        0      974 2024-01-12 03:42:46.114770 fabric-orchestrator-client-1.7.0b2/test/test_slivers_api.py
+-rw-r--r--   0        0        0      998 2024-01-12 03:42:46.114861 fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1032 2024-01-12 03:42:46.114968 fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      996 2024-01-12 03:42:46.115068 fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_paginated.py
+-rw-r--r--   0        0        0      972 2024-01-12 03:42:46.115159 fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      988 2024-01-12 03:42:46.115251 fabric-orchestrator-client-1.7.0b2/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1038 2024-01-12 03:42:46.115351 fabric-orchestrator-client-1.7.0b2/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0     1002 2024-01-12 03:42:46.115454 fabric-orchestrator-client-1.7.0b2/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1052 2024-01-12 03:42:46.115553 fabric-orchestrator-client-1.7.0b2/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      978 2024-01-12 03:42:46.115643 fabric-orchestrator-client-1.7.0b2/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1028 2024-01-12 03:42:46.115743 fabric-orchestrator-client-1.7.0b2/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      972 2024-01-12 03:42:46.115834 fabric-orchestrator-client-1.7.0b2/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1022 2024-01-12 03:42:46.115939 fabric-orchestrator-client-1.7.0b2/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1062 2024-01-12 03:42:46.116047 fabric-orchestrator-client-1.7.0b2/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1112 2024-01-12 03:42:46.116160 fabric-orchestrator-client-1.7.0b2/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      888 2024-01-12 03:42:46.116255 fabric-orchestrator-client-1.7.0b2/test/test_version.py
+-rw-r--r--   0        0        0      814 2024-01-12 03:42:46.116365 fabric-orchestrator-client-1.7.0b2/test/test_version_api.py
+-rw-r--r--   0        0        0      922 2024-01-12 03:42:46.116524 fabric-orchestrator-client-1.7.0b2/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2024-01-12 03:42:46.116674 fabric-orchestrator-client-1.7.0b2/tox.ini
+-rw-r--r--   0        0        0    10985 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.7.0b2/PKG-INFO
```

### Comparing `fabric-orchestrator-client-1.7.0b1/.gitignore` & `fabric-orchestrator-client-1.7.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/.swagger-codegen-ignore` & `fabric-orchestrator-client-1.7.0b2/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/CODEGEN.md` & `fabric-orchestrator-client-1.7.0b2/CODEGEN.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/LICENSE` & `fabric-orchestrator-client-1.7.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/README.md` & `fabric-orchestrator-client-1.7.0b2/README.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/docs/PoaData.md` & `fabric-orchestrator-client-1.7.0b2/docs/PoaData.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/docs/PoasApi.md` & `fabric-orchestrator-client-1.7.0b2/docs/PoasApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/docs/ResourcesApi.md` & `fabric-orchestrator-client-1.7.0b2/docs/ResourcesApi.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
 [**portalresources_get**](ResourcesApi.md#portalresources_get) | **GET** /portalresources | Retrieve a listing and description of available resources for portal
 [**resources_get**](ResourcesApi.md#resources_get) | **GET** /resources | Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.
 
 # **portalresources_get**
-> Resources portalresources_get(graph_format)
+> Resources portalresources_get(graph_format, level=level, force_refresh=force_refresh, start_date=start_date, end_date=end_date, includes=includes, excludes=excludes)
 
 Retrieve a listing and description of available resources for portal
 
 Retrieve a listing and description of available resources for portal
 
 ### Example
 ```python
@@ -21,28 +21,40 @@
 from fabric_cf.orchestrator.swagger_client import ResourcesApi, Configuration, ApiClient
 from fabric_cf.orchestrator.swagger_client.rest import ApiException
 from pprint import pprint
 
 # create an instance of the API class
 api_instance = ResourcesApi()
 graph_format = 'GRAPHML' # str | graph format (default to GRAPHML)
+level = 1 # int | Level of details (optional) (default to 1)
+force_refresh = false # bool | Force to retrieve current available resource information. (optional) (default to false)
+start_date = 'start_date_example' # str | starting date to check availability from (optional)
+end_date = 'end_date_example' # str | end date to check availability until (optional)
+includes = 'includes_example' # str | comma separated lists of sites to include (optional)
+excludes = 'excludes_example' # str | comma separated lists of sites to exclude (optional)
 
 try:
     # Retrieve a listing and description of available resources for portal
-    api_response = api_instance.portalresources_get(graph_format)
+    api_response = api_instance.portalresources_get(graph_format, level=level, force_refresh=force_refresh, start_date=start_date, end_date=end_date, includes=includes, excludes=excludes)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling ResourcesApi->portalresources_get: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **graph_format** | **str**| graph format | [default to GRAPHML]
+ **level** | **int**| Level of details | [optional] [default to 1]
+ **force_refresh** | **bool**| Force to retrieve current available resource information. | [optional] [default to false]
+ **start_date** | **str**| starting date to check availability from | [optional] 
+ **end_date** | **str**| end date to check availability until | [optional] 
+ **includes** | **str**| comma separated lists of sites to include | [optional] 
+ **excludes** | **str**| comma separated lists of sites to exclude | [optional] 
 
 ### Return type
 
 [**Resources**](Resources.md)
 
 ### Authorization
 
@@ -83,15 +95,15 @@
 start_date = 'start_date_example' # str | starting date to check availability from (optional)
 end_date = 'end_date_example' # str | end date to check availability until (optional)
 includes = 'includes_example' # str | comma separated lists of sites to include (optional)
 excludes = 'excludes_example' # str | comma separated lists of sites to exclude (optional)
 
 try:
     # Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.
-    api_response = api_instance.resources_get(level, force_refresh, start_date=start_date, end_date=end_date)
+    api_response = api_instance.resources_get(level, force_refresh, start_date=start_date, end_date=end_date, includes=includes, excludes=excludes)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling ResourcesApi->resources_get: %s\n" % e)
 ```
 
 ### Parameters
```

### Comparing `fabric-orchestrator-client-1.7.0b1/docs/SlicesApi.md` & `fabric-orchestrator-client-1.7.0b2/docs/SlicesApi.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,21 +66,21 @@
 
 ### Authorization
 
 [bearerAuth](../README.md#bearerAuth)
 
 ### HTTP request headers
 
- - **Content-Type**: text/plain
+ - **Content-Type**: application/json
  - **Accept**: application/json
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **slices_creates_post**
-> Slivers slices_creates_post(body, name, lease_end_time=lease_end_time)
+> Slivers slices_creates_post(body, name, lease_start_time=lease_start_time, lease_end_time=lease_end_time)
 
 Create slice
 
 Request to create slice as described in the request. Request would be a graph ML describing the requested resources. Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources.  
 
 ### Example
 ```python
@@ -97,30 +97,32 @@
 # configuration.api_key_prefix['Authorization'] = 'Bearer'
 
 
 # create an instance of the API class
 api_instance = SlicesApi(ApiClient(configuration))
 body = SlicesPost() # SlicesPost | Create new Slice
 name = 'name_example' # str | Slice Name
+lease_start_time = 'lease_start_time_example' # str | Lease End Time for the Slice (optional)
 lease_end_time = 'lease_end_time_example' # str | Lease End Time for the Slice (optional)
 
 try:
     # Create slice
-    api_response = api_instance.slices_creates_post(body, name, lease_end_time=lease_end_time)
+    api_response = api_instance.slices_creates_post(body, name, lease_start_time=lease_start_time, lease_end_time=lease_end_time)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling SlicesApi->slices_creates_post: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **body** | [**SlicesPost**](SlicesPost.md)| Create new Slice | 
  **name** | **str**| Slice Name | 
+ **lease_start_time** | **str**| Lease End Time for the Slice | [optional] 
  **lease_end_time** | **str**| Lease End Time for the Slice | [optional] 
 
 ### Return type
 
 [**Slivers**](Slivers.md)
 
 ### Authorization
@@ -236,15 +238,15 @@
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **slices_get**
-> Slices slices_get(name=name, as_self=as_self, states=states, limit=limit, offset=offset)
+> Slices slices_get(name=name, search=search, exact_match=exact_match, as_self=as_self, states=states, limit=limit, offset=offset)
 
 Retrieve a listing of user slices
 
 Retrieve a listing of user slices. It returns list of all slices belonging to all members in a project when 'as_self' is False otherwise returns only the all user's slices in a project.
 
 ### Example
 ```python
@@ -394,15 +396,15 @@
     print("Exception when calling SlicesApi->slices_modify_slice_id_put: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
- **body** | [**str**](str.md)|  | Modify a Slice
+ **body** | [**str**](str.md)| Modify a Slice | 
  **slice_id** | **str**| Slice identified by universally unique identifier | 
 
 ### Return type
 
 [**Slivers**](Slivers.md)
 
 ### Authorization
```

### Comparing `fabric-orchestrator-client-1.7.0b1/docs/SliversApi.md` & `fabric-orchestrator-client-1.7.0b2/docs/SliversApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/orchestrator_proxy.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/orchestrator_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     StableError = enum.auto()
     StableOK = enum.auto()
     Closing = enum.auto()
     Dead = enum.auto()
     Modifying = enum.auto()
     ModifyError = enum.auto()
     ModifyOK = enum.auto()
+    AllocatedError = enum.auto()
+    AllocatedOK = enum.auto()
 
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return self.name
 
@@ -130,23 +132,24 @@
         @param token token
         """
         # Set the tokens
         self.slices_api.api_client.configuration.api_key[self.PROP_AUTHORIZATION] = token
         self.slices_api.api_client.configuration.api_key_prefix[self.PROP_AUTHORIZATION] = self.PROP_BEARER
 
     def create(self, *, token: str, slice_name: str, ssh_key: Union[str, List[str]],
-               topology: ExperimentTopology = None, slice_graph: str = None,
+               topology: ExperimentTopology = None, slice_graph: str = None, lease_start_time: str = None,
                lease_end_time: str = None) -> Tuple[Status, Union[Exception, List[Sliver]]]:
         """
         Create a slice
         @param token fabric token
         @param slice_name slice name
         @param ssh_key SSH Key(s)
         @param topology Experiment topology
         @param slice_graph Slice Graph string
+        @param lease_start_time Lease Start Time
         @param lease_end_time Lease End Time
         @return Tuple containing Status and Exception/Json containing slivers created
         """
         if token is None:
             return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Token {token} must be specified")
 
         if slice_name is None:
@@ -154,14 +157,21 @@
                    OrchestratorProxyException(f"Slice Name {slice_name} must be specified")
 
         if (topology is None and slice_graph is None) or (topology is not None and slice_graph is not None):
             return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Either topology {topology} or "
                                                                         f"slice graph {slice_graph} must "
                                                                         f"be specified")
 
+        if lease_start_time is not None:
+            try:
+                datetime.strptime(lease_start_time, self.TIME_FORMAT)
+            except Exception as e:
+                return Status.INVALID_ARGUMENTS, OrchestratorProxyException(
+                    f"Lease Stat Time {lease_start_time} should be in format: {self.TIME_FORMAT} e: {e}")
+
         if lease_end_time is not None:
             try:
                 datetime.strptime(lease_end_time, self.TIME_FORMAT)
             except Exception as e:
                 return Status.INVALID_ARGUMENTS, OrchestratorProxyException(
                     f"Lease End Time {lease_end_time} should be in format: {self.TIME_FORMAT} e: {e}")
 
@@ -173,19 +183,17 @@
                 slice_graph = topology.serialize()
 
             if isinstance(ssh_key, str):
                 ssh_keys = [ssh_key]
             else:
                 ssh_keys = ssh_key
             body = SlicesPost(graph_model=slice_graph, ssh_keys=ssh_keys)
-            if lease_end_time is not None:
-                slivers = self.slices_api.slices_creates_post(name=slice_name, body=body, lease_end_time=lease_end_time)
-            else:
-                slivers = self.slices_api.slices_creates_post(name=slice_name, body=body)
-
+            slivers = self.slices_api.slices_creates_post(name=slice_name, body=body,
+                                                          lease_end_time=lease_end_time,
+                                                          lease_start_time=lease_start_time)
             return Status.OK, slivers.data if slivers.data is not None else []
         except Exception as e:
             return Status.FAILURE, e
 
     def modify(self, *, token: str, slice_id: str, topology: ExperimentTopology = None,
                slice_graph: str = None) -> Tuple[Status, Union[Exception, List[Sliver]]]:
         """
@@ -298,15 +306,16 @@
 
         try:
             # Set the tokens
             self.__set_tokens(token=token)
 
             states = [SliceState.StableError, SliceState.StableOK, SliceState.Nascent,
                       SliceState.Configuring, SliceState.Closing, SliceState.Dead,
-                      SliceState.ModifyError, SliceState.ModifyOK, SliceState.Modifying]
+                      SliceState.ModifyError, SliceState.ModifyOK, SliceState.Modifying,
+                      SliceState.AllocatedOK, SliceState.AllocatedError]
             if includes is not None:
                 states = includes
 
             if excludes is not None:
                 for x in excludes:
                     if x in states:
                         states.remove(x)
@@ -409,16 +418,16 @@
         if token is None:
             return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Token {token} must be specified")
 
         try:
             # Set the tokens
             self.__set_tokens(token=token)
 
-            start_date = start.strftime('%Y-%m-%d %H:%M:%S %z') if start else None
-            end_date = end.strftime('%Y-%m-%d %H:%M:%S %z') if end else None
+            start_date = start.strftime(self.TIME_FORMAT) if start else None
+            end_date = end.strftime(self.TIME_FORMAT) if end else None
             resources = self.resources_api.resources_get(level=level, force_refresh=force_refresh,
                                                          start_date=start_date, end_date=end_date,
                                                          includes=', '.join(includes) if includes else None,
                                                          excludes=', '.join(excludes) if excludes else None)
             graph_string = resources.data[0].model
             substrate = None
             if graph_string is not None:
```

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/__init__.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/poas_api.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/poas_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/resources_api.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/resources_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,47 +27,65 @@
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def portalresources_get(self, graph_format, **kwargs):  # noqa: E501
         """Retrieve a listing and description of available resources for portal  # noqa: E501
+
         Retrieve a listing and description of available resources for portal  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.portalresources_get(graph_format, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str graph_format: graph format (required)
+        :param int level: Level of details
+        :param bool force_refresh: Force to retrieve current available resource information.
+        :param str start_date: starting date to check availability from
+        :param str end_date: end date to check availability until
+        :param str includes: comma separated lists of sites to include
+        :param str excludes: comma separated lists of sites to exclude
         :return: Resources
                  If the method is called asynchronously,
                  returns the request thread.
         """
+        # Remove all arguments with None value from kwargs
+        kwargs = {key: value for key, value in kwargs.items() if value is not None}
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.portalresources_get_with_http_info(graph_format, **kwargs)  # noqa: E501
         else:
             (data) = self.portalresources_get_with_http_info(graph_format, **kwargs)  # noqa: E501
             return data
 
     def portalresources_get_with_http_info(self, graph_format, **kwargs):  # noqa: E501
         """Retrieve a listing and description of available resources for portal  # noqa: E501
+
         Retrieve a listing and description of available resources for portal  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.portalresources_get_with_http_info(graph_format, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str graph_format: graph format (required)
+        :param int level: Level of details
+        :param bool force_refresh: Force to retrieve current available resource information.
+        :param str start_date: starting date to check availability from
+        :param str end_date: end date to check availability until
+        :param str includes: comma separated lists of sites to include
+        :param str excludes: comma separated lists of sites to exclude
         :return: Resources
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['graph_format']  # noqa: E501
+        all_params = ['graph_format', 'level', 'force_refresh', 'start_date', 'end_date', 'includes', 'excludes']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -86,14 +104,26 @@
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'graph_format' in params:
             query_params.append(('graph_format', params['graph_format']))  # noqa: E501
+        if 'level' in params:
+            query_params.append(('level', params['level']))  # noqa: E501
+        if 'force_refresh' in params:
+            query_params.append(('force_refresh', params['force_refresh']))  # noqa: E501
+        if 'start_date' in params:
+            query_params.append(('start_date', params['start_date']))  # noqa: E501
+        if 'end_date' in params:
+            query_params.append(('end_date', params['end_date']))  # noqa: E501
+        if 'includes' in params:
+            query_params.append(('includes', params['includes']))  # noqa: E501
+        if 'excludes' in params:
+            query_params.append(('excludes', params['excludes']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -118,19 +148,21 @@
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def resources_get(self, level, force_refresh, **kwargs):  # noqa: E501
         """Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.  # noqa: E501
+
         Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.resources_get(level, force_refresh, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param int level: Level of details (required)
         :param bool force_refresh: Force to retrieve current available resource information. (required)
         :param str start_date: starting date to check availability from
         :param str end_date: end date to check availability until
         :param str includes: comma separated lists of sites to include
         :param str excludes: comma separated lists of sites to exclude
```

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/slices_api.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/slices_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,19 +156,21 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_creates_post(body, name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param SlicesPost body: Create new Slice (required)
         :param str name: Slice Name (required)
+        :param str lease_start_time: Lease End Time for the Slice
         :param str lease_end_time: Lease End Time for the Slice
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
+        kwargs = {key: value for key, value in kwargs.items() if value is not None}
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.slices_creates_post_with_http_info(body, name, **kwargs)  # noqa: E501
         else:
             (data) = self.slices_creates_post_with_http_info(body, name, **kwargs)  # noqa: E501
             return data
 
@@ -180,21 +182,22 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_creates_post_with_http_info(body, name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param SlicesPost body: Create new Slice (required)
         :param str name: Slice Name (required)
+        :param str lease_start_time: Lease End Time for the Slice
         :param str lease_end_time: Lease End Time for the Slice
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body', 'name', 'lease_end_time']  # noqa: E501
+        all_params = ['body', 'name', 'lease_start_time', 'lease_end_time']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -217,14 +220,16 @@
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'name' in params:
             query_params.append(('name', params['name']))  # noqa: E501
+        if 'lease_start_time' in params:
+            query_params.append(('lease_start_time', params['lease_start_time']))  # noqa: E501
         if 'lease_end_time' in params:
             query_params.append(('lease_end_time', params['lease_end_time']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
```

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/version_api.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api_client.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/configuration.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/__init__.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_data.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_keys.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post_data_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/resource.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/resources.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slice.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slice_details.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slices.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slices_post.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/sliver.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slivers.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/version.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/version_data.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/rest.py` & `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/git_push.sh` & `fabric-orchestrator-client-1.7.0b2/git_push.sh`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/pyproject.toml` & `fabric-orchestrator-client-1.7.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_poa.py` & `fabric-orchestrator-client-1.7.0b2/test/test_poa.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_poa_data.py` & `fabric-orchestrator-client-1.7.0b2/test/test_poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_poa_post.py` & `fabric-orchestrator-client-1.7.0b2/test/test_poa_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_poa_post_data.py` & `fabric-orchestrator-client-1.7.0b2/test/test_poa_post_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_poa_post_data_vcpu_cpu_map.py` & `fabric-orchestrator-client-1.7.0b2/test/test_poa_post_data_vcpu_cpu_map.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_poas_api.py` & `fabric-orchestrator-client-1.7.0b2/test/test_poas_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_resource.py` & `fabric-orchestrator-client-1.7.0b2/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_resources.py` & `fabric-orchestrator-client-1.7.0b2/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_resources_api.py` & `fabric-orchestrator-client-1.7.0b2/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_slice.py` & `fabric-orchestrator-client-1.7.0b2/test/test_slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_slice_details.py` & `fabric-orchestrator-client-1.7.0b2/test/test_slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_slices.py` & `fabric-orchestrator-client-1.7.0b2/test/test_slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_slices_api.py` & `fabric-orchestrator-client-1.7.0b2/test/test_slices_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_slices_post.py` & `fabric-orchestrator-client-1.7.0b2/test/test_slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_sliver.py` & `fabric-orchestrator-client-1.7.0b2/test/test_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_slivers.py` & `fabric-orchestrator-client-1.7.0b2/test/test_slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_slivers_api.py` & `fabric-orchestrator-client-1.7.0b2/test/test_slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_no_content.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_paginated.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_single.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status400_bad_request.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status400_bad_request_errors.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status401_unauthorized.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status403_forbidden.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status403_forbidden_errors.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status404_not_found.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status404_not_found_errors.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status500_internal_server_error.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.7.0b2/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_version.py` & `fabric-orchestrator-client-1.7.0b2/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_version_api.py` & `fabric-orchestrator-client-1.7.0b2/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/test/test_version_data.py` & `fabric-orchestrator-client-1.7.0b2/test/test_version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b1/PKG-INFO` & `fabric-orchestrator-client-1.7.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-orchestrator-client
-Version: 1.7.0b1
+Version: 1.7.0b2
 Summary: Fabric Orchestrator API
 Keywords: Swagger,Fabric Orchestrator API
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

