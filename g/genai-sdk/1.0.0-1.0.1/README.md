# Comparing `tmp/genai-sdk-1.0.0.tar.gz` & `tmp/genai-sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genai-sdk-1.0.0.tar", last modified: Tue May  7 13:41:08 2024, max compression
+gzip compressed data, was "genai-sdk-1.0.1.tar", last modified: Tue May  7 13:41:54 2024, max compression
```

## Comparing `genai-sdk-1.0.0.tar` & `genai-sdk-1.0.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:08.392686 genai-sdk-1.0.0/
--rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)      447 2024-05-07 13:41:08.392686 genai-sdk-1.0.0/PKG-INFO
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3973 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/README.md
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:08.352686 genai-sdk-1.0.0/content-hub-api/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1987 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/__init__.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:08.352686 genai-sdk-1.0.0/content-hub-api/api/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      130 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/api/__init__.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    24414 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/api/completion_generation_api.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    25812 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/api_client.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      652 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/api_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    14520 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/configuration.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5987 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/exceptions.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:08.360686 genai-sdk-1.0.0/content-hub-api/models/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1352 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/__init__.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2665 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/author.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4497 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/chat_completion_request.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3736 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/chat_completion_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3056 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/direct_completion_request.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3130 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/direct_completion_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3870 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/document.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5462 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/document_content.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3758 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/document_metadata.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2788 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/error.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3051 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/message.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4954 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/model_params.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2939 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/model_settings.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2985 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/position.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3080 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/prompt_config.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3192 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/models/rag_config.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     9248 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/content-hub-api/rest.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:08.364686 genai-sdk-1.0.0/genai_sdk.egg-info/
--rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)      447 2024-05-07 13:41:08.000000 genai-sdk-1.0.0/genai_sdk.egg-info/PKG-INFO
--rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)     3598 2024-05-07 13:41:08.000000 genai-sdk-1.0.0/genai_sdk.egg-info/SOURCES.txt
--rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)        1 2024-05-07 13:41:08.000000 genai-sdk-1.0.0/genai_sdk.egg-info/dependency_links.txt
--rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)       76 2024-05-07 13:41:08.000000 genai-sdk-1.0.0/genai_sdk.egg-info/requires.txt
--rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)       56 2024-05-07 13:41:08.000000 genai-sdk-1.0.0/genai_sdk.egg-info/top_level.txt
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:08.368686 genai-sdk-1.0.0/grounding-hub-api/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2037 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/grounding-hub-api/__init__.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:08.368686 genai-sdk-1.0.0/grounding-hub-api/api/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      132 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/grounding-hub-api/api/__init__.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    24428 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/grounding-hub-api/api/completion_generation_api.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    25824 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/grounding-hub-api/api_client.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      652 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/grounding-hub-api/api_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    14522 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/grounding-hub-api/configuration.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5987 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/grounding-hub-api/exceptions.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:08.376686 genai-sdk-1.0.0/grounding-hub-api/models/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1382 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/grounding-hub-api/models/__init__.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2665 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/author.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4505 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/chat_completion_request.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3738 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/chat_completion_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3058 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/direct_completion_request.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3130 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/direct_completion_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3874 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/document.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5462 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/document_content.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3762 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/document_metadata.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2788 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/error.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3051 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/message.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4954 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/model_params.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2941 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/model_settings.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2985 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/position.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3080 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/prompt_config.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3192 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/grounding-hub-api/models/rag_config.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     9250 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/grounding-hub-api/rest.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:08.380686 genai-sdk-1.0.0/prompt-repository-api/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2137 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/__init__.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:08.380686 genai-sdk-1.0.0/prompt-repository-api/api/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      136 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/api/__init__.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    24456 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/api/completion_generation_api.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    25848 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/api_client.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      652 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/api_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    14526 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/configuration.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5987 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/exceptions.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:08.388686 genai-sdk-1.0.0/prompt-repository-api/models/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1442 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/__init__.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2665 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/prompt-repository-api/models/author.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4521 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/chat_completion_request.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3742 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/chat_completion_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3062 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/direct_completion_request.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3130 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/direct_completion_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3882 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/document.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5462 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/document_content.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3770 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/document_metadata.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2788 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/error.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3051 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/message.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4954 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/model_params.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2945 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/model_settings.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2985 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/position.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3080 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/prompt_config.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3192 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/models/rag_config.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     9254 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/prompt-repository-api/rest.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1985 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/pyproject.toml
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)       69 2024-05-07 13:41:08.396686 genai-sdk-1.0.0/setup.cfg
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1367 2024-05-07 13:17:46.000000 genai-sdk-1.0.0/setup.py
-drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:08.392686 genai-sdk-1.0.0/test/
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1355 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_author.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2661 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_chat_completion_request.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2942 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_chat_completion_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1159 2024-05-07 13:17:45.000000 genai-sdk-1.0.0/test/test_completion_generation_api.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2090 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_direct_completion_request.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1764 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_direct_completion_response.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3079 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_document.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1383 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_document_content.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2077 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_document_metadata.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1336 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_error.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1411 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_message.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1479 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_model_params.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1733 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_model_settings.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1419 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_position.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1495 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_prompt_config.py
--rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1478 2024-05-07 13:17:44.000000 genai-sdk-1.0.0/test/test_rag_config.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:54.968634 genai-sdk-1.0.1/
+-rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)      447 2024-05-07 13:41:54.968634 genai-sdk-1.0.1/PKG-INFO
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3973 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/README.md
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:54.924634 genai-sdk-1.0.1/content-hub-api/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1987 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/__init__.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:54.924634 genai-sdk-1.0.1/content-hub-api/api/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      130 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/api/__init__.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    24414 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/api/completion_generation_api.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    25812 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/api_client.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      652 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/api_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    14520 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/configuration.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5987 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/exceptions.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:54.932634 genai-sdk-1.0.1/content-hub-api/models/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1352 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/__init__.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2665 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/author.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4497 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/chat_completion_request.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3736 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/chat_completion_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3056 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/direct_completion_request.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3130 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/direct_completion_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3870 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/document.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5462 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/document_content.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3758 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/document_metadata.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2788 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/error.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3051 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/message.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4954 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/model_params.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2939 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/model_settings.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2985 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/position.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3080 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/prompt_config.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3192 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/models/rag_config.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     9248 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/content-hub-api/rest.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:54.936634 genai-sdk-1.0.1/genai_sdk.egg-info/
+-rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)      447 2024-05-07 13:41:54.000000 genai-sdk-1.0.1/genai_sdk.egg-info/PKG-INFO
+-rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)     3598 2024-05-07 13:41:54.000000 genai-sdk-1.0.1/genai_sdk.egg-info/SOURCES.txt
+-rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)        1 2024-05-07 13:41:54.000000 genai-sdk-1.0.1/genai_sdk.egg-info/dependency_links.txt
+-rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)       76 2024-05-07 13:41:54.000000 genai-sdk-1.0.1/genai_sdk.egg-info/requires.txt
+-rw-r-----   0 ykovalchuk  (1000) ykovalchuk  (1000)       56 2024-05-07 13:41:54.000000 genai-sdk-1.0.1/genai_sdk.egg-info/top_level.txt
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:54.936634 genai-sdk-1.0.1/grounding-hub-api/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2037 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/grounding-hub-api/__init__.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:54.940634 genai-sdk-1.0.1/grounding-hub-api/api/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      132 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/grounding-hub-api/api/__init__.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    24428 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/grounding-hub-api/api/completion_generation_api.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    25824 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/grounding-hub-api/api_client.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      652 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/grounding-hub-api/api_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    14522 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/grounding-hub-api/configuration.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5987 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/grounding-hub-api/exceptions.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:54.948634 genai-sdk-1.0.1/grounding-hub-api/models/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1382 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/grounding-hub-api/models/__init__.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2665 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/author.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4505 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/chat_completion_request.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3738 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/chat_completion_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3058 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/direct_completion_request.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3130 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/direct_completion_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3874 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/document.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5462 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/document_content.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3762 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/document_metadata.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2788 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/error.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3051 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/message.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4954 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/model_params.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2941 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/model_settings.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2985 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/position.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3080 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/prompt_config.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3192 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/grounding-hub-api/models/rag_config.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     9250 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/grounding-hub-api/rest.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:54.948634 genai-sdk-1.0.1/prompt-repository-api/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2137 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/__init__.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:54.952634 genai-sdk-1.0.1/prompt-repository-api/api/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      136 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/api/__init__.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    24456 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/api/completion_generation_api.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    25848 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/api_client.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)      652 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/api_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)    14526 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/configuration.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5987 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/exceptions.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:54.960634 genai-sdk-1.0.1/prompt-repository-api/models/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1442 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/__init__.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2665 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/prompt-repository-api/models/author.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4521 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/chat_completion_request.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3742 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/chat_completion_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3062 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/direct_completion_request.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3130 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/direct_completion_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3882 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/document.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     5462 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/document_content.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3770 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/document_metadata.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2788 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/error.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3051 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/message.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     4954 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/model_params.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2945 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/model_settings.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2985 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/position.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3080 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/prompt_config.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3192 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/models/rag_config.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     9254 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/prompt-repository-api/rest.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1985 2024-05-07 13:17:46.000000 genai-sdk-1.0.1/pyproject.toml
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)       69 2024-05-07 13:41:54.968634 genai-sdk-1.0.1/setup.cfg
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1367 2024-05-07 13:41:52.000000 genai-sdk-1.0.1/setup.py
+drwxr-x---   0 ykovalchuk  (1000) ykovalchuk  (1000)        0 2024-05-07 13:41:54.964634 genai-sdk-1.0.1/test/
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1355 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_author.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2661 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_chat_completion_request.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2942 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_chat_completion_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1159 2024-05-07 13:17:45.000000 genai-sdk-1.0.1/test/test_completion_generation_api.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2090 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_direct_completion_request.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1764 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_direct_completion_response.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     3079 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_document.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1383 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_document_content.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     2077 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_document_metadata.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1336 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_error.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1411 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_message.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1479 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_model_params.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1733 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_model_settings.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1419 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_position.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1495 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_prompt_config.py
+-rw-rw-r--   0 ykovalchuk  (1000) ykovalchuk  (1000)     1478 2024-05-07 13:17:44.000000 genai-sdk-1.0.1/test/test_rag_config.py
```

### Comparing `genai-sdk-1.0.0/README.md` & `genai-sdk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/__init__.py` & `genai-sdk-1.0.1/content-hub-api/__init__.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/api/completion_generation_api.py` & `genai-sdk-1.0.1/content-hub-api/api/completion_generation_api.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/api_client.py` & `genai-sdk-1.0.1/content-hub-api/api_client.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/api_response.py` & `genai-sdk-1.0.1/content-hub-api/api_response.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/configuration.py` & `genai-sdk-1.0.1/content-hub-api/configuration.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/exceptions.py` & `genai-sdk-1.0.1/content-hub-api/exceptions.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/__init__.py` & `genai-sdk-1.0.1/content-hub-api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/author.py` & `genai-sdk-1.0.1/content-hub-api/models/author.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/chat_completion_request.py` & `genai-sdk-1.0.1/content-hub-api/models/chat_completion_request.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/chat_completion_response.py` & `genai-sdk-1.0.1/content-hub-api/models/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/direct_completion_request.py` & `genai-sdk-1.0.1/content-hub-api/models/direct_completion_request.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/direct_completion_response.py` & `genai-sdk-1.0.1/content-hub-api/models/direct_completion_response.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/document.py` & `genai-sdk-1.0.1/content-hub-api/models/document.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/document_content.py` & `genai-sdk-1.0.1/content-hub-api/models/document_content.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/document_metadata.py` & `genai-sdk-1.0.1/content-hub-api/models/document_metadata.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/error.py` & `genai-sdk-1.0.1/content-hub-api/models/error.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/message.py` & `genai-sdk-1.0.1/content-hub-api/models/message.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/model_params.py` & `genai-sdk-1.0.1/content-hub-api/models/model_params.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/model_settings.py` & `genai-sdk-1.0.1/content-hub-api/models/model_settings.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/position.py` & `genai-sdk-1.0.1/content-hub-api/models/position.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/prompt_config.py` & `genai-sdk-1.0.1/content-hub-api/models/prompt_config.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/models/rag_config.py` & `genai-sdk-1.0.1/content-hub-api/models/rag_config.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/content-hub-api/rest.py` & `genai-sdk-1.0.1/content-hub-api/rest.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/genai_sdk.egg-info/SOURCES.txt` & `genai-sdk-1.0.1/genai_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/__init__.py` & `genai-sdk-1.0.1/grounding-hub-api/__init__.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/api/completion_generation_api.py` & `genai-sdk-1.0.1/grounding-hub-api/api/completion_generation_api.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/api_client.py` & `genai-sdk-1.0.1/grounding-hub-api/api_client.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/api_response.py` & `genai-sdk-1.0.1/grounding-hub-api/api_response.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/configuration.py` & `genai-sdk-1.0.1/grounding-hub-api/configuration.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/exceptions.py` & `genai-sdk-1.0.1/grounding-hub-api/exceptions.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/__init__.py` & `genai-sdk-1.0.1/grounding-hub-api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/author.py` & `genai-sdk-1.0.1/grounding-hub-api/models/author.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/chat_completion_request.py` & `genai-sdk-1.0.1/grounding-hub-api/models/chat_completion_request.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/chat_completion_response.py` & `genai-sdk-1.0.1/grounding-hub-api/models/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/direct_completion_request.py` & `genai-sdk-1.0.1/grounding-hub-api/models/direct_completion_request.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/direct_completion_response.py` & `genai-sdk-1.0.1/grounding-hub-api/models/direct_completion_response.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/document.py` & `genai-sdk-1.0.1/grounding-hub-api/models/document.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/document_content.py` & `genai-sdk-1.0.1/grounding-hub-api/models/document_content.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/document_metadata.py` & `genai-sdk-1.0.1/grounding-hub-api/models/document_metadata.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/error.py` & `genai-sdk-1.0.1/grounding-hub-api/models/error.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/message.py` & `genai-sdk-1.0.1/grounding-hub-api/models/message.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/model_params.py` & `genai-sdk-1.0.1/grounding-hub-api/models/model_params.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/model_settings.py` & `genai-sdk-1.0.1/grounding-hub-api/models/model_settings.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/position.py` & `genai-sdk-1.0.1/grounding-hub-api/models/position.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/prompt_config.py` & `genai-sdk-1.0.1/grounding-hub-api/models/prompt_config.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/models/rag_config.py` & `genai-sdk-1.0.1/grounding-hub-api/models/rag_config.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/grounding-hub-api/rest.py` & `genai-sdk-1.0.1/grounding-hub-api/rest.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/__init__.py` & `genai-sdk-1.0.1/prompt-repository-api/__init__.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/api/completion_generation_api.py` & `genai-sdk-1.0.1/prompt-repository-api/api/completion_generation_api.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/api_client.py` & `genai-sdk-1.0.1/prompt-repository-api/api_client.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/api_response.py` & `genai-sdk-1.0.1/prompt-repository-api/api_response.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/configuration.py` & `genai-sdk-1.0.1/prompt-repository-api/configuration.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/exceptions.py` & `genai-sdk-1.0.1/prompt-repository-api/exceptions.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/__init__.py` & `genai-sdk-1.0.1/prompt-repository-api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/author.py` & `genai-sdk-1.0.1/prompt-repository-api/models/author.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/chat_completion_request.py` & `genai-sdk-1.0.1/prompt-repository-api/models/chat_completion_request.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/chat_completion_response.py` & `genai-sdk-1.0.1/prompt-repository-api/models/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/direct_completion_request.py` & `genai-sdk-1.0.1/prompt-repository-api/models/direct_completion_request.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/direct_completion_response.py` & `genai-sdk-1.0.1/prompt-repository-api/models/direct_completion_response.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/document.py` & `genai-sdk-1.0.1/prompt-repository-api/models/document.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/document_content.py` & `genai-sdk-1.0.1/prompt-repository-api/models/document_content.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/document_metadata.py` & `genai-sdk-1.0.1/prompt-repository-api/models/document_metadata.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/error.py` & `genai-sdk-1.0.1/prompt-repository-api/models/error.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/message.py` & `genai-sdk-1.0.1/prompt-repository-api/models/message.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/model_params.py` & `genai-sdk-1.0.1/prompt-repository-api/models/model_params.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/model_settings.py` & `genai-sdk-1.0.1/prompt-repository-api/models/model_settings.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/position.py` & `genai-sdk-1.0.1/prompt-repository-api/models/position.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/prompt_config.py` & `genai-sdk-1.0.1/prompt-repository-api/models/prompt_config.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/models/rag_config.py` & `genai-sdk-1.0.1/prompt-repository-api/models/rag_config.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/prompt-repository-api/rest.py` & `genai-sdk-1.0.1/prompt-repository-api/rest.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/pyproject.toml` & `genai-sdk-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/setup.py` & `genai-sdk-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "genai-sdk"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `genai-sdk-1.0.0/test/test_author.py` & `genai-sdk-1.0.1/test/test_author.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_chat_completion_request.py` & `genai-sdk-1.0.1/test/test_chat_completion_request.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_chat_completion_response.py` & `genai-sdk-1.0.1/test/test_chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_completion_generation_api.py` & `genai-sdk-1.0.1/test/test_completion_generation_api.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_direct_completion_request.py` & `genai-sdk-1.0.1/test/test_direct_completion_request.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_direct_completion_response.py` & `genai-sdk-1.0.1/test/test_direct_completion_response.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_document.py` & `genai-sdk-1.0.1/test/test_document.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_document_content.py` & `genai-sdk-1.0.1/test/test_document_content.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_document_metadata.py` & `genai-sdk-1.0.1/test/test_document_metadata.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_error.py` & `genai-sdk-1.0.1/test/test_error.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_message.py` & `genai-sdk-1.0.1/test/test_message.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_model_params.py` & `genai-sdk-1.0.1/test/test_model_params.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_model_settings.py` & `genai-sdk-1.0.1/test/test_model_settings.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_position.py` & `genai-sdk-1.0.1/test/test_position.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_prompt_config.py` & `genai-sdk-1.0.1/test/test_prompt_config.py`

 * *Files identical despite different names*

### Comparing `genai-sdk-1.0.0/test/test_rag_config.py` & `genai-sdk-1.0.1/test/test_rag_config.py`

 * *Files identical despite different names*

