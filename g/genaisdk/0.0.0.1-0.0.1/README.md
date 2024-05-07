# Comparing `tmp/genaisdk-0.0.0.1.tar.gz` & `tmp/genaisdk-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genaisdk-0.0.0.1.tar", last modified: Tue May  7 14:19:50 2024, max compression
+gzip compressed data, was "genaisdk-0.0.1.tar", last modified: Tue May  7 14:09:27 2024, max compression
```

## Comparing `genaisdk-0.0.0.1.tar` & `genaisdk-0.0.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:19:50.297729 genaisdk-0.0.0.1/
--rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)      446 2024-05-07 14:19:50.297729 genaisdk-0.0.0.1/PKG-INFO
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3524 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/README.md
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:19:50.257730 genaisdk-0.0.0.1/contenthub/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1065 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/contenthub/__init__.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:19:50.257730 genaisdk-0.0.0.1/contenthub/api/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      100 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/contenthub/api/__init__.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    21039 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/contenthub/api/metadata_api.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    25790 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/contenthub/api_client.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      652 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/contenthub/api_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    14523 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/contenthub/configuration.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5993 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/contenthub/exceptions.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:19:50.261730 genaisdk-0.0.0.1/contenthub/models/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      503 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/contenthub/models/__init__.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2574 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/contenthub/models/error_message.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3021 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/contenthub/models/metadata_info.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     9249 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/contenthub/rest.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:19:50.261730 genaisdk-0.0.0.1/genaisdk.egg-info/
--rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)      446 2024-05-07 14:19:50.000000 genaisdk-0.0.0.1/genaisdk.egg-info/PKG-INFO
--rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)     2966 2024-05-07 14:19:50.000000 genaisdk-0.0.0.1/genaisdk.egg-info/SOURCES.txt
--rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)        1 2024-05-07 14:19:50.000000 genaisdk-0.0.0.1/genaisdk.egg-info/dependency_links.txt
--rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)       76 2024-05-07 14:19:50.000000 genaisdk-0.0.0.1/genaisdk.egg-info/requires.txt
--rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)       41 2024-05-07 14:19:50.000000 genaisdk-0.0.0.1/genaisdk.egg-info/top_level.txt
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:19:50.265730 genaisdk-0.0.0.1/groundinghub/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1914 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/__init__.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:19:50.265730 genaisdk-0.0.0.1/groundinghub/api/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      127 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/api/__init__.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    24393 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/api/completion_generation_api.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    25796 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/api_client.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      652 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/api_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    14519 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/configuration.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5987 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/exceptions.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:19:50.273729 genaisdk-0.0.0.1/groundinghub/models/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1307 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/__init__.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2665 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/author.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4485 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/chat_completion_request.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3733 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/chat_completion_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3053 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/direct_completion_request.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3130 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/direct_completion_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3864 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/document.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4643 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/document_content.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3752 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/document_metadata.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2788 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/error.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3051 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/message.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4954 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/model_params.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2936 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/model_settings.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2985 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/position.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3080 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/prompt_config.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3192 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/models/rag_config.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     9245 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/groundinghub/rest.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:19:50.277730 genaisdk-0.0.0.1/promptrepository/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1708 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/__init__.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:19:50.281730 genaisdk-0.0.0.1/promptrepository/api/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      180 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/api/__init__.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    23795 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/api/public_prompts_api.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    12275 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/api/public_tags_api.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    25819 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/api_client.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      652 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/api_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    14522 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/configuration.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5986 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/exceptions.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:19:50.285730 genaisdk-0.0.0.1/promptrepository/models/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1012 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/models/__init__.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      858 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/promptrepository/models/binding_type.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2999 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/promptrepository/models/http_validation_error.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4855 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/promptrepository/models/location_inner.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3600 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/promptrepository/models/prompt_template_variable.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3193 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/promptrepository/models/prompt_template_with_variables.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2804 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/models/tag.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3596 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/models/tag_category_with_tags.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      751 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/models/tags_type.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3058 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/models/validation_error.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     9248 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/promptrepository/rest.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1970 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/pyproject.toml
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)       69 2024-05-07 14:19:50.297729 genaisdk-0.0.0.1/setup.cfg
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1360 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/setup.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:19:50.297729 genaisdk-0.0.0.1/test/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1350 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_author.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      706 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_binding_type.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2636 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_chat_completion_request.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2917 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_chat_completion_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1154 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_completion_generation_api.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2075 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_direct_completion_request.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1759 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_direct_completion_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3044 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_document.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1378 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_document_content.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2062 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_document_metadata.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1331 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_error.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1378 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_error_message.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1726 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_http_validation_error.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1357 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_location_inner.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1406 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_message.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      928 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_metadata_api.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1505 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_metadata_info.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1474 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_model_params.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1723 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_model_settings.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1414 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_position.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1490 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_prompt_config.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1925 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_prompt_template_variable.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2510 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/test/test_prompt_template_with_variables.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      972 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/test/test_public_prompts_api.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      813 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/test/test_public_tags_api.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1473 2024-05-07 14:17:40.000000 genaisdk-0.0.0.1/test/test_rag_config.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1687 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/test/test_tag.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2804 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/test/test_tag_category_with_tags.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      685 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/test/test_tags_type.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1630 2024-05-07 14:17:41.000000 genaisdk-0.0.0.1/test/test_validation_error.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:09:27.414578 genaisdk-0.0.1/
+-rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)      444 2024-05-07 14:09:27.414578 genaisdk-0.0.1/PKG-INFO
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3522 2024-05-07 14:08:54.000000 genaisdk-0.0.1/README.md
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:09:27.374578 genaisdk-0.0.1/contenthub/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1063 2024-05-07 14:08:53.000000 genaisdk-0.0.1/contenthub/__init__.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:09:27.374578 genaisdk-0.0.1/contenthub/api/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      100 2024-05-07 14:08:53.000000 genaisdk-0.0.1/contenthub/api/__init__.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    21039 2024-05-07 14:08:53.000000 genaisdk-0.0.1/contenthub/api/metadata_api.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    25788 2024-05-07 14:08:53.000000 genaisdk-0.0.1/contenthub/api_client.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      652 2024-05-07 14:08:53.000000 genaisdk-0.0.1/contenthub/api_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    14521 2024-05-07 14:08:53.000000 genaisdk-0.0.1/contenthub/configuration.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5993 2024-05-07 14:08:53.000000 genaisdk-0.0.1/contenthub/exceptions.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:09:27.378578 genaisdk-0.0.1/contenthub/models/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      503 2024-05-07 14:08:53.000000 genaisdk-0.0.1/contenthub/models/__init__.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2574 2024-05-07 14:08:53.000000 genaisdk-0.0.1/contenthub/models/error_message.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3021 2024-05-07 14:08:53.000000 genaisdk-0.0.1/contenthub/models/metadata_info.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     9249 2024-05-07 14:08:53.000000 genaisdk-0.0.1/contenthub/rest.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:09:27.378578 genaisdk-0.0.1/genaisdk.egg-info/
+-rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)      444 2024-05-07 14:09:27.000000 genaisdk-0.0.1/genaisdk.egg-info/PKG-INFO
+-rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)     2966 2024-05-07 14:09:27.000000 genaisdk-0.0.1/genaisdk.egg-info/SOURCES.txt
+-rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)        1 2024-05-07 14:09:27.000000 genaisdk-0.0.1/genaisdk.egg-info/dependency_links.txt
+-rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)       76 2024-05-07 14:09:27.000000 genaisdk-0.0.1/genaisdk.egg-info/requires.txt
+-rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)       41 2024-05-07 14:09:27.000000 genaisdk-0.0.1/genaisdk.egg-info/top_level.txt
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:09:27.382578 genaisdk-0.0.1/groundinghub/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1912 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/__init__.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:09:27.386578 genaisdk-0.0.1/groundinghub/api/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      127 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/api/__init__.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    24393 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/api/completion_generation_api.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    25794 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/api_client.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      652 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/api_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    14517 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/configuration.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5987 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/exceptions.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:09:27.394578 genaisdk-0.0.1/groundinghub/models/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1307 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/__init__.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2665 2024-05-07 14:08:52.000000 genaisdk-0.0.1/groundinghub/models/author.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4485 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/chat_completion_request.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3733 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/chat_completion_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3053 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/direct_completion_request.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3130 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/direct_completion_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3864 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/document.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5462 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/document_content.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3752 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/document_metadata.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2788 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/error.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3051 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/message.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4954 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/model_params.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2936 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/model_settings.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2985 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/position.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3080 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/prompt_config.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3192 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/models/rag_config.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     9245 2024-05-07 14:08:53.000000 genaisdk-0.0.1/groundinghub/rest.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:09:27.398578 genaisdk-0.0.1/promptrepository/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1706 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/__init__.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:09:27.398578 genaisdk-0.0.1/promptrepository/api/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      180 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/api/__init__.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    23795 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/api/public_prompts_api.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    12275 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/api/public_tags_api.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    25817 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/api_client.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      652 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/api_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    14520 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/configuration.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5986 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/exceptions.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:09:27.402578 genaisdk-0.0.1/promptrepository/models/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1012 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/models/__init__.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      858 2024-05-07 14:08:53.000000 genaisdk-0.0.1/promptrepository/models/binding_type.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2999 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/models/http_validation_error.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4855 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/models/location_inner.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3600 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/models/prompt_template_variable.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3193 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/models/prompt_template_with_variables.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2804 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/models/tag.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3596 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/models/tag_category_with_tags.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      751 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/models/tags_type.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3058 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/models/validation_error.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     9248 2024-05-07 14:08:54.000000 genaisdk-0.0.1/promptrepository/rest.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1968 2024-05-07 14:08:54.000000 genaisdk-0.0.1/pyproject.toml
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)       69 2024-05-07 14:09:27.414578 genaisdk-0.0.1/setup.cfg
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1358 2024-05-07 14:08:54.000000 genaisdk-0.0.1/setup.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 14:09:27.414578 genaisdk-0.0.1/test/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1350 2024-05-07 14:08:52.000000 genaisdk-0.0.1/test/test_author.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      706 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_binding_type.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2636 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_chat_completion_request.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2917 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_chat_completion_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1154 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_completion_generation_api.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2075 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_direct_completion_request.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1759 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_direct_completion_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3044 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_document.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1378 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_document_content.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2062 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_document_metadata.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1331 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_error.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1378 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_error_message.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1726 2024-05-07 14:08:54.000000 genaisdk-0.0.1/test/test_http_validation_error.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1357 2024-05-07 14:08:54.000000 genaisdk-0.0.1/test/test_location_inner.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1406 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_message.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      928 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_metadata_api.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1505 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_metadata_info.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1474 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_model_params.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1723 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_model_settings.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1414 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_position.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1490 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_prompt_config.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1925 2024-05-07 14:08:54.000000 genaisdk-0.0.1/test/test_prompt_template_variable.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2510 2024-05-07 14:08:54.000000 genaisdk-0.0.1/test/test_prompt_template_with_variables.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      972 2024-05-07 14:08:54.000000 genaisdk-0.0.1/test/test_public_prompts_api.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      813 2024-05-07 14:08:54.000000 genaisdk-0.0.1/test/test_public_tags_api.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1473 2024-05-07 14:08:53.000000 genaisdk-0.0.1/test/test_rag_config.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1687 2024-05-07 14:08:54.000000 genaisdk-0.0.1/test/test_tag.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2804 2024-05-07 14:08:54.000000 genaisdk-0.0.1/test/test_tag_category_with_tags.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      685 2024-05-07 14:08:54.000000 genaisdk-0.0.1/test/test_tags_type.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1630 2024-05-07 14:08:54.000000 genaisdk-0.0.1/test/test_validation_error.py
```

### Comparing `genaisdk-0.0.0.1/README.md` & `genaisdk-0.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # genaisdk
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1.0
-- Package version: 0.0.0.1
+- Package version: 0.0.1
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `genaisdk-0.0.0.1/contenthub/__init__.py` & `genaisdk-0.0.1/contenthub/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.0.0.1"
+__version__ = "0.0.1"
 
 # import apis into sdk package
 from contenthub.api.metadata_api import MetadataApi
 
 # import ApiClient
 from contenthub.api_response import ApiResponse
 from contenthub.api_client import ApiClient
```

### Comparing `genaisdk-0.0.0.1/contenthub/api/metadata_api.py` & `genaisdk-0.0.1/contenthub/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/contenthub/api_client.py` & `genaisdk-0.0.1/contenthub/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.0.0.1/python'
+        self.user_agent = 'OpenAPI-Generator/0.0.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `genaisdk-0.0.0.1/contenthub/api_response.py` & `genaisdk-0.0.1/contenthub/api_response.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/contenthub/configuration.py` & `genaisdk-0.0.1/contenthub/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 0.0.0.1".\
+               "SDK Package Version: 0.0.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `genaisdk-0.0.0.1/contenthub/exceptions.py` & `genaisdk-0.0.1/contenthub/exceptions.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/contenthub/models/error_message.py` & `genaisdk-0.0.1/contenthub/models/error_message.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/contenthub/models/metadata_info.py` & `genaisdk-0.0.1/contenthub/models/metadata_info.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/contenthub/rest.py` & `genaisdk-0.0.1/contenthub/rest.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/genaisdk.egg-info/SOURCES.txt` & `genaisdk-0.0.1/genaisdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/__init__.py` & `genaisdk-0.0.1/groundinghub/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.0.3
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.0.0.1"
+__version__ = "0.0.1"
 
 # import apis into sdk package
 from groundinghub.api.completion_generation_api import CompletionGenerationApi
 
 # import ApiClient
 from groundinghub.api_response import ApiResponse
 from groundinghub.api_client import ApiClient
```

### Comparing `genaisdk-0.0.0.1/groundinghub/api/completion_generation_api.py` & `genaisdk-0.0.1/groundinghub/api/completion_generation_api.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/api_client.py` & `genaisdk-0.0.1/groundinghub/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.0.0.1/python'
+        self.user_agent = 'OpenAPI-Generator/0.0.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `genaisdk-0.0.0.1/groundinghub/api_response.py` & `genaisdk-0.0.1/groundinghub/api_response.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/configuration.py` & `genaisdk-0.0.1/groundinghub/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.0.3\n"\
-               "SDK Package Version: 0.0.0.1".\
+               "SDK Package Version: 0.0.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `genaisdk-0.0.0.1/groundinghub/exceptions.py` & `genaisdk-0.0.1/groundinghub/exceptions.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/__init__.py` & `genaisdk-0.0.1/groundinghub/models/__init__.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/author.py` & `genaisdk-0.0.1/groundinghub/models/author.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/chat_completion_request.py` & `genaisdk-0.0.1/groundinghub/models/chat_completion_request.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/chat_completion_response.py` & `genaisdk-0.0.1/groundinghub/models/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/direct_completion_request.py` & `genaisdk-0.0.1/groundinghub/models/direct_completion_request.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/direct_completion_response.py` & `genaisdk-0.0.1/groundinghub/models/direct_completion_response.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/document.py` & `genaisdk-0.0.1/groundinghub/models/document.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/document_content.py` & `genaisdk-0.0.1/groundinghub/models/document_content.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,30 +11,32 @@
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 import pprint
-from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
-from typing import Any, List, Optional
+from pydantic import BaseModel, ConfigDict, Field, StrictBytes, StrictStr, ValidationError, field_validator
+from typing import Any, List, Optional, Union
 from pydantic import StrictStr, Field
 from typing import Union, List, Optional, Dict
 from typing_extensions import Literal, Self
 
-DOCUMENTCONTENT_ONE_OF_SCHEMAS = ["str"]
+DOCUMENTCONTENT_ONE_OF_SCHEMAS = ["bytearray", "str"]
 
 class DocumentContent(BaseModel):
     """
     Optional document content. The type depends on the data type, and can be string for text data or binary for files
     """
     # data type: str
     oneof_schema_1_validator: Optional[StrictStr] = None
-    actual_instance: Optional[Union[str]] = None
-    one_of_schemas: List[str] = Field(default=Literal["str"])
+    # data type: bytearray
+    oneof_schema_2_validator: Optional[Union[StrictBytes, StrictStr]] = None
+    actual_instance: Optional[Union[bytearray, str]] = None
+    one_of_schemas: List[str] = Field(default=Literal["bytearray", "str"])
 
     model_config = ConfigDict(
         validate_assignment=True,
         protected_namespaces=(),
     )
 
 
@@ -55,20 +57,26 @@
         match = 0
         # validate data type: str
         try:
             instance.oneof_schema_1_validator = v
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
+        # validate data type: bytearray
+        try:
+            instance.oneof_schema_2_validator = v
+            match += 1
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when setting `actual_instance` in DocumentContent with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when setting `actual_instance` in DocumentContent with oneOf schemas: bytearray, str. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when setting `actual_instance` in DocumentContent with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting `actual_instance` in DocumentContent with oneOf schemas: bytearray, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Union[str, Dict[str, Any]]) -> Self:
         return cls.from_json(json.dumps(obj))
 
@@ -84,35 +92,44 @@
             # validation
             instance.oneof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.oneof_schema_1_validator
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
+        # deserialize data into bytearray
+        try:
+            # validation
+            instance.oneof_schema_2_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.oneof_schema_2_validator
+            match += 1
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
 
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into DocumentContent with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when deserializing the JSON string into DocumentContent with oneOf schemas: bytearray, str. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into DocumentContent with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into DocumentContent with oneOf schemas: bytearray, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], str]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], bytearray, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `genaisdk-0.0.0.1/groundinghub/models/document_metadata.py` & `genaisdk-0.0.1/groundinghub/models/document_metadata.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/error.py` & `genaisdk-0.0.1/groundinghub/models/error.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/message.py` & `genaisdk-0.0.1/groundinghub/models/message.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/model_params.py` & `genaisdk-0.0.1/groundinghub/models/model_params.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/model_settings.py` & `genaisdk-0.0.1/groundinghub/models/model_settings.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/position.py` & `genaisdk-0.0.1/groundinghub/models/position.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/prompt_config.py` & `genaisdk-0.0.1/groundinghub/models/prompt_config.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/models/rag_config.py` & `genaisdk-0.0.1/groundinghub/models/rag_config.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/groundinghub/rest.py` & `genaisdk-0.0.1/groundinghub/rest.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/__init__.py` & `genaisdk-0.0.1/promptrepository/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.1.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.0.0.1"
+__version__ = "0.0.1"
 
 # import apis into sdk package
 from promptrepository.api.public_prompts_api import PublicPromptsApi
 from promptrepository.api.public_tags_api import PublicTagsApi
 
 # import ApiClient
 from promptrepository.api_response import ApiResponse
```

### Comparing `genaisdk-0.0.0.1/promptrepository/api/public_prompts_api.py` & `genaisdk-0.0.1/promptrepository/api/public_prompts_api.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/api/public_tags_api.py` & `genaisdk-0.0.1/promptrepository/api/public_tags_api.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/api_client.py` & `genaisdk-0.0.1/promptrepository/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.0.0.1/python'
+        self.user_agent = 'OpenAPI-Generator/0.0.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `genaisdk-0.0.0.1/promptrepository/api_response.py` & `genaisdk-0.0.1/promptrepository/api_response.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/configuration.py` & `genaisdk-0.0.1/promptrepository/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 0.0.0.1".\
+               "SDK Package Version: 0.0.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `genaisdk-0.0.0.1/promptrepository/exceptions.py` & `genaisdk-0.0.1/promptrepository/exceptions.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/models/__init__.py` & `genaisdk-0.0.1/promptrepository/models/__init__.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/models/binding_type.py` & `genaisdk-0.0.1/promptrepository/models/binding_type.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/models/http_validation_error.py` & `genaisdk-0.0.1/promptrepository/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/models/location_inner.py` & `genaisdk-0.0.1/promptrepository/models/location_inner.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/models/prompt_template_variable.py` & `genaisdk-0.0.1/promptrepository/models/prompt_template_variable.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/models/prompt_template_with_variables.py` & `genaisdk-0.0.1/promptrepository/models/prompt_template_with_variables.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/models/tag.py` & `genaisdk-0.0.1/promptrepository/models/tag.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/models/tag_category_with_tags.py` & `genaisdk-0.0.1/promptrepository/models/tag_category_with_tags.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/models/tags_type.py` & `genaisdk-0.0.1/promptrepository/models/tags_type.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/models/validation_error.py` & `genaisdk-0.0.1/promptrepository/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/promptrepository/rest.py` & `genaisdk-0.0.1/promptrepository/rest.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/pyproject.toml` & `genaisdk-0.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promptrepository"
-version = "0.0.0.1"
+version = "0.0.1"
 description = "Prompt Management API"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Prompt Management API"]
 include = ["promptrepository/py.typed"]
```

### Comparing `genaisdk-0.0.0.1/setup.py` & `genaisdk-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "genaisdk"
-VERSION = "0.0.0.1"
+VERSION = "0.0.1"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `genaisdk-0.0.0.1/test/test_author.py` & `genaisdk-0.0.1/test/test_author.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_binding_type.py` & `genaisdk-0.0.1/test/test_binding_type.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_chat_completion_request.py` & `genaisdk-0.0.1/test/test_chat_completion_request.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_chat_completion_response.py` & `genaisdk-0.0.1/test/test_chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_completion_generation_api.py` & `genaisdk-0.0.1/test/test_completion_generation_api.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_direct_completion_request.py` & `genaisdk-0.0.1/test/test_direct_completion_request.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_direct_completion_response.py` & `genaisdk-0.0.1/test/test_direct_completion_response.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_document.py` & `genaisdk-0.0.1/test/test_document.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_document_content.py` & `genaisdk-0.0.1/test/test_document_content.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_document_metadata.py` & `genaisdk-0.0.1/test/test_document_metadata.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_error.py` & `genaisdk-0.0.1/test/test_error.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_error_message.py` & `genaisdk-0.0.1/test/test_error_message.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_http_validation_error.py` & `genaisdk-0.0.1/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_location_inner.py` & `genaisdk-0.0.1/test/test_location_inner.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_message.py` & `genaisdk-0.0.1/test/test_message.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_metadata_api.py` & `genaisdk-0.0.1/test/test_metadata_api.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_metadata_info.py` & `genaisdk-0.0.1/test/test_metadata_info.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_model_params.py` & `genaisdk-0.0.1/test/test_model_params.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_model_settings.py` & `genaisdk-0.0.1/test/test_model_settings.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_position.py` & `genaisdk-0.0.1/test/test_position.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_prompt_config.py` & `genaisdk-0.0.1/test/test_prompt_config.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_prompt_template_variable.py` & `genaisdk-0.0.1/test/test_prompt_template_variable.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_prompt_template_with_variables.py` & `genaisdk-0.0.1/test/test_prompt_template_with_variables.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_public_prompts_api.py` & `genaisdk-0.0.1/test/test_public_prompts_api.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_public_tags_api.py` & `genaisdk-0.0.1/test/test_public_tags_api.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_rag_config.py` & `genaisdk-0.0.1/test/test_rag_config.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_tag.py` & `genaisdk-0.0.1/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_tag_category_with_tags.py` & `genaisdk-0.0.1/test/test_tag_category_with_tags.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_tags_type.py` & `genaisdk-0.0.1/test/test_tags_type.py`

 * *Files identical despite different names*

### Comparing `genaisdk-0.0.0.1/test/test_validation_error.py` & `genaisdk-0.0.1/test/test_validation_error.py`

 * *Files identical despite different names*

