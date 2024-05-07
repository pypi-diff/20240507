# Comparing `tmp/alphaz-next-0.6.1.tar.gz` & `tmp/alphaz-next-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.6.1.tar", last modified: Mon May  6 11:09:36 2024, max compression
+gzip compressed data, was "alphaz-next-0.6.2.tar", last modified: Tue May  7 11:25:17 2024, max compression
```

## Comparing `alphaz-next-0.6.1.tar` & `alphaz-next-0.6.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.241021 alphaz-next-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-06 11:09:36.241021 alphaz-next-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.233021 alphaz-next-0.6.1/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.233021 alphaz-next-0.6.1/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/asyncio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.233021 alphaz-next-0.6.1/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.237021 alphaz-next-0.6.1/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.237021 alphaz-next-0.6.1/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/core/responses/ujson_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.237021 alphaz-next-0.6.1/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.233021 alphaz-next-0.6.1/alphaz_next/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.237021 alphaz-next-0.6.1/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.237021 alphaz-next-0.6.1/alphaz_next/models/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.237021 alphaz-next-0.6.1/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/models/config/directories_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/models/config/openapi_config_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.233021 alphaz-next-0.6.1/alphaz_next/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.237021 alphaz-next-0.6.1/alphaz_next/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.237021 alphaz-next-0.6.1/alphaz_next/tests/utils/mocking/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/tests/utils/mocking/mock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/tests/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.241021 alphaz-next-0.6.1/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/utils/logging_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-06 11:09:34.000000 alphaz-next-0.6.1/alphaz_next/utils/loguru.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:36.233021 alphaz-next-0.6.1/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-06 11:09:36.000000 alphaz-next-0.6.1/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-06 11:09:36.000000 alphaz-next-0.6.1/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:09:36.000000 alphaz-next-0.6.1/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-06 11:09:36.000000 alphaz-next-0.6.1/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 11:09:36.000000 alphaz-next-0.6.1/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 11:09:36.241021 alphaz-next-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-06 11:09:35.000000 alphaz-next-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.714283 alphaz-next-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-07 11:25:17.714283 alphaz-next-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.706283 alphaz-next-0.6.2/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.706283 alphaz-next-0.6.2/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/asyncio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.706283 alphaz-next-0.6.2/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.706283 alphaz-next-0.6.2/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.710283 alphaz-next-0.6.2/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/core/responses/ujson_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.710283 alphaz-next-0.6.2/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.702283 alphaz-next-0.6.2/alphaz_next/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.710283 alphaz-next-0.6.2/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.710283 alphaz-next-0.6.2/alphaz_next/models/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.710283 alphaz-next-0.6.2/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/models/config/directories_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/models/config/openapi_config_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.706283 alphaz-next-0.6.2/alphaz_next/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.710283 alphaz-next-0.6.2/alphaz_next/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.710283 alphaz-next-0.6.2/alphaz_next/tests/utils/mocking/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/tests/utils/mocking/mock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/tests/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.714283 alphaz-next-0.6.2/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/utils/logging_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-07 11:25:15.000000 alphaz-next-0.6.2/alphaz_next/utils/loguru.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:17.706283 alphaz-next-0.6.2/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-07 11:25:17.000000 alphaz-next-0.6.2/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-07 11:25:17.000000 alphaz-next-0.6.2/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:25:17.000000 alphaz-next-0.6.2/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-07 11:25:17.000000 alphaz-next-0.6.2/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 11:25:17.000000 alphaz-next-0.6.2/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:25:17.714283 alphaz-next-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-07 11:25:17.000000 alphaz-next-0.6.2/setup.py
```

### Comparing `alphaz-next-0.6.1/PKG-INFO` & `alphaz-next-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.6.1
+Version: 0.6.2
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.6.1.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.6.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.6.1/README.md` & `alphaz-next-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/auth/auth.py` & `alphaz-next-0.6.2/alphaz_next/auth/auth.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/_base.py` & `alphaz-next-0.6.2/alphaz_next/core/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/_middleware.py` & `alphaz-next-0.6.2/alphaz_next/core/_middleware.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/_telemetry.py` & `alphaz-next-0.6.2/alphaz_next/core/_telemetry.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,75 +51,23 @@
     def __init__(
         self,
         labels: _Dict[str, str] | None = None,
         config: _Dict[str, _List[str]] | None = None,
     ):
         super().__init__(labels, config)
 
-        self._system_cpu_total_norm_pct_labels = self._labels.copy()
-
-    def _get_system_cpu_total_norm_pct(self, options: CallbackOptions):
-        cpu_norm_percent = _psutil.cpu_percent(interval=None) / 100.0
-        yield Observation(
-            cpu_norm_percent,
-            self._system_cpu_total_norm_pct_labels,
-        )
-
-    def _get_system_memory_actual_free(self, options: CallbackOptions):
-        memory = _psutil.virtual_memory()
-        yield Observation(
-            memory.available,
-            self._system_cpu_total_norm_pct_labels,
-        )
+        self._process = _psutil.Process()
+        self._process.cpu_percent(interval=None)
 
-    def _get_system_memory_total(self, options: CallbackOptions):
-        memory = _psutil.virtual_memory()
-        yield Observation(
-            memory.total,
-            self._system_cpu_total_norm_pct_labels,
-        )
-
-    def _get_system_process_cpu_total_norm_pct(self, options: CallbackOptions):
-        p = _psutil.Process()
-        if hasattr(p, "oneshot"):  # new in psutil 5.0
-            with p.oneshot():
-                cpu_percent = p.cpu_percent(interval=None)
-        else:
-            cpu_percent = p.cpu_percent(interval=None)
-
-        yield Observation(
-            cpu_percent / 100.0 / _psutil.cpu_count(),
-            self._system_cpu_total_norm_pct_labels,
-        )
-
-    def _get_system_process_memory_size(self, options: CallbackOptions):
-        p = _psutil.Process()
-        if hasattr(p, "oneshot"):  # new in psutil 5.0
-            with p.oneshot():
-                memory_info = p.memory_info()
-        else:
-            memory_info = p.memory_info()
-
-        yield Observation(
-            memory_info.vms,
-            self._system_cpu_total_norm_pct_labels,
-        )
-
-    def _get_system_process_memory_rss_byte(self, options: CallbackOptions):
-        p = _psutil.Process()
-        if hasattr(p, "oneshot"):  # new in psutil 5.0
-            with p.oneshot():
-                memory_info = p.memory_info()
-        else:
-            memory_info = p.memory_info()
-
-        yield Observation(
-            memory_info.rss,
-            self._system_cpu_total_norm_pct_labels,
-        )
+        self._system_cpu_total_norm_pct_labels = self._labels.copy()
+        self._system_memory_actual_free_labels = self._labels.copy()
+        self._system_memory_total_labels = self._labels.copy()
+        self._system_process_cpu_total_norm_pct_labels = self._labels.copy()
+        self._system_process_memory_size_labels = self._labels.copy()
+        self._system_process_memory_rss_byte_labels = self._labels.copy()
 
     def _instrument(self, **kwargs):
         super()._instrument(**kwargs)
 
         if "system.cpu.total.norm.pct" in self._config:
             self._meter.create_observable_gauge(
                 name="system.cpu.total.norm.pct",
@@ -158,14 +106,67 @@
         if "system.process.memory.rss.byte" in self._config:
             self._meter.create_observable_gauge(
                 name="system.process.memory.rss.bytes",
                 callbacks=[self._get_system_process_memory_rss_byte],
                 description="System process memory rss bytes",
             )
 
+    def _get_process_infos(self, p: _psutil.Process):
+        if hasattr(p, "oneshot"):  # new in psutil 5.0
+            with p.oneshot():
+                cpu_percent = p.cpu_percent(interval=None)
+                memory_info = p.memory_info()
+        else:
+            cpu_percent = p.cpu_percent(interval=None)
+            memory_info = p.memory_info()
+
+        return cpu_percent, memory_info
+
+    def _get_system_cpu_total_norm_pct(self, options: CallbackOptions):
+        cpu_norm_percent = _psutil.cpu_percent(interval=None) / 100.0
+        yield Observation(
+            cpu_norm_percent,
+            self._system_cpu_total_norm_pct_labels,
+        )
+
+    def _get_system_memory_actual_free(self, options: CallbackOptions):
+        memory = _psutil.virtual_memory()
+        yield Observation(
+            memory.available,
+            self._system_memory_actual_free_labels,
+        )
+
+    def _get_system_memory_total(self, options: CallbackOptions):
+        memory = _psutil.virtual_memory()
+        yield Observation(
+            memory.total,
+            self._system_memory_total_labels,
+        )
+
+    def _get_system_process_cpu_total_norm_pct(self, options: CallbackOptions):
+        cpu_percent, _ = self._get_process_infos(p=self._process)
+        yield Observation(
+            cpu_percent / 100.0 / _psutil.cpu_count(),
+            self._system_process_cpu_total_norm_pct_labels,
+        )
+
+    def _get_system_process_memory_size(self, options: CallbackOptions):
+        _, memory_info = self._get_process_infos(p=self._process)
+        yield Observation(
+            memory_info.vms,
+            self._system_process_memory_size_labels,
+        )
+
+    def _get_system_process_memory_rss_byte(self, options: CallbackOptions):
+        _, memory_info = self._get_process_infos(p=self._process)
+        yield Observation(
+            memory_info.rss,
+            self._system_process_memory_rss_byte_labels,
+        )
+
 
 def _setup_traces(
     default_endpoint: str,
     default_headers: _Optional[str] = None,
     certificate_file: _Optional[str] = None,
     resource: _Optional[Resource] = None,
 ) -> None:
```

### Comparing `alphaz-next-0.6.1/alphaz_next/core/application.py` & `alphaz-next-0.6.2/alphaz_next/core/application.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.6.2/alphaz_next/core/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/exceptions.py` & `alphaz-next-0.6.2/alphaz_next/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/responses/__init__.py` & `alphaz-next-0.6.2/alphaz_next/core/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.6.2/alphaz_next/core/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.6.2/alphaz_next/core/responses/html_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.6.2/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.6.2/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.6.2/alphaz_next/core/responses/plaintext_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.6.2/alphaz_next/core/responses/redirect_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/responses/response.py` & `alphaz-next-0.6.2/alphaz_next/core/responses/response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.6.2/alphaz_next/core/responses/streaming_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.6.2/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/libs/httpx.py` & `alphaz-next-0.6.2/alphaz_next/libs/httpx.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.6.2/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.6.2/alphaz_next/models/config/_base/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.6.2/alphaz_next/models/config/alpha_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/models/config/api_config.py` & `alphaz-next-0.6.2/alphaz_next/models/config/api_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.6.2/alphaz_next/models/config/apm_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.6.2/alphaz_next/models/config/config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/models/config/database_config.py` & `alphaz-next-0.6.2/alphaz_next/models/config/database_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.6.2/alphaz_next/models/config/logging_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.6.2/alphaz_next/models/config/openapi_config_schema.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/tests/utils/utils.py` & `alphaz-next-0.6.2/alphaz_next/tests/utils/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/utils/format.py` & `alphaz-next-0.6.2/alphaz_next/utils/format.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/utils/logger.py` & `alphaz-next-0.6.2/alphaz_next/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/utils/logging_filters.py` & `alphaz-next-0.6.2/alphaz_next/utils/logging_filters.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next/utils/loguru.py` & `alphaz-next-0.6.2/alphaz_next/utils/loguru.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/alphaz_next.egg-info/PKG-INFO` & `alphaz-next-0.6.2/alphaz_next.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.6.1
+Version: 0.6.2
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.6.1.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.6.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.6.1/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.6.2/alphaz_next.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.1/setup.py` & `alphaz-next-0.6.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.6.1"
+version = "0.6.2"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 
 EXTRAS_REQUIRE = {
     "dependency-injector": ["dependency-injector"],
```
