# Comparing `tmp/azure-search-documents-11.6.0b3.tar.gz` & `tmp/azure-search-documents-11.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-search-documents-11.6.0b3.tar", last modified: Mon Apr  8 19:38:40 2024, max compression
+gzip compressed data, was "azure-search-documents-11.6.0b4.tar", last modified: Mon May  6 15:09:59 2024, max compression
```

## Comparing `azure-search-documents-11.6.0b3.tar` & `azure-search-documents-11.6.0b4.tar`

### file list

```diff
@@ -1,207 +1,205 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.980076 azure-search-documents-11.6.0b3/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16245 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      193 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    23034 2024-04-08 19:38:40.980076 azure-search-documents-11.6.0b3/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22009 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4081 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/TROUBLESHOOTING.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.944076 azure-search-documents-11.6.0b3/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      251 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.944076 azure-search-documents-11.6.0b3/azure/search/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      251 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.948076 azure-search-documents-11.6.0b3/azure/search/documents/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1822 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      482 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_api_versions.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.948076 azure-search-documents-11.6.0b3/azure/search/documents/_generated/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      737 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2644 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4709 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/_search_index_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      677 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.948076 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      737 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2654 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4832 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/_search_index_client.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.948076 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      688 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48338 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/_documents_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.952076 azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3969 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   117033 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15647 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/_search_index_client_enums.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.952076 azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      688 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    66326 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/_documents_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/py.typed
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      843 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_headers_mixin.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6159 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_index_documents_batch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6326 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_paging.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4902 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_queries.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38222 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_search_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      491 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_search_documents_error.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15064 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_search_indexing_buffered_sender.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2193 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_search_indexing_buffered_sender_base.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1903 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_utils.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      252 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.952076 azure-search-documents-11.6.0b3/azure/search/documents/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1553 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5980 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/aio/_index_documents_batch_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6013 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/aio/_paging.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39096 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/aio/_search_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15395 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/aio/_search_indexing_buffered_sender_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/aio/_timer.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.952076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1479 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.956076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      743 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2410 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5999 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_search_service_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1216 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.956076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      743 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2420 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6142 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_search_service_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      956 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.956076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1221 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27284 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27285 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    42751 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38620 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4038 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34101 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25922 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.960076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18753 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   541670 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    73409 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.960076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1221 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33426 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_aliases_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34097 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    54682 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_indexers_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47543 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_indexes_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4927 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    42553 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32425 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/py.typed
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27197 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_search_index_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30999 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_search_indexer_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3193 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_utils.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.960076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1479 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28240 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/_search_index_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30031 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/_search_indexer_client.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.964076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13422 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      624 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/_edm.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48235 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/_index.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    56166 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/_models.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.964076 azure-search-documents-11.6.0b3/azure/search/documents/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2256 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.980076 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    23034 2024-04-08 19:38:40.000000 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8934 2024-04-08 19:38:40.000000 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-08 19:38:40.000000 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-08 19:38:40.000000 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       52 2024-04-08 19:38:40.000000 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-08 19:38:40.000000 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       79 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/pyproject.toml
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.968076 azure-search-documents-11.6.0b3/samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6100 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.972076 azure-search-documents-11.6.0b3/samples/async_samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1659 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_analyze_text_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3587 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_authentication_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1679 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_autocomplete_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1899 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_buffered_sender_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2364 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_crud_operations_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3083 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_data_source_operations_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1797 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_facet_query_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1875 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_filter_query_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1721 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_get_document_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3501 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_index_alias_crud_operations_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1816 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_index_client_send_request_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4218 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_index_crud_operations_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4321 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_indexers_operations_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1912 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_query_session_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1800 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_search_client_send_request_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2369 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_semantic_search_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1705 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_simple_query_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1756 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_suggestions_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2546 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_synonym_map_operations_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7302 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_vector_search_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1560 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_analyze_text.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3361 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_authentication.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1564 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_autocomplete.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1788 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_buffered_sender.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2166 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_crud_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2826 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_data_source_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1672 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_facet_query.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1734 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_filter_query.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1590 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_get_document.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3275 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_index_alias_crud_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1733 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_index_client_send_request.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3921 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_index_crud_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6067 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_indexer_datasource_skillset.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3878 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_indexers_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1792 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_query_session.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1717 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_search_client_send_request.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2395 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_semantic_search.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1584 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_simple_query.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1630 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_suggestions.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2901 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_synonym_map_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7072 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_vector_search.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-08 19:38:40.980076 azure-search-documents-11.6.0b3/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2392 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.976076 azure-search-documents-11.6.0b3/tests/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.980076 azure-search-documents-11.6.0b3/tests/async_tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6471 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_buffered_sender_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1364 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2157 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_basic_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7227 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_buffered_sender_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6927 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_index_document_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6354 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_search_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4454 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_alias_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3921 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6323 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_data_source_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8070 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10270 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_skillset_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6112 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_synonym_map_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8040 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_indexer_client_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1263 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/conftest.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.980076 azure-search-documents-11.6.0b3/tests/perfstress_tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/perfstress_tests/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2340 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/perfstress_tests/autocomplete.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2300 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/perfstress_tests/search_documents.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2305 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/perfstress_tests/suggest.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29583 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/search_service_preparer.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6451 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_buffered_sender.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2164 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_index_documents_batch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3222 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_index_field_helpers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5887 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_queries.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4604 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_regex_flags.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14537 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2013 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_client_basic_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6790 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_client_buffered_sender_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6608 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_client_index_document_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5129 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_client_search_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5018 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_index_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4130 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_index_client_alias_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6883 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_index_client_data_source_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7627 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_index_client_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11708 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_index_client_skillset_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5759 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_index_client_synonym_map_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7675 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_indexer_client_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4093 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_serialization.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.071390 azure-search-documents-11.6.0b4/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17563 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      193 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22937 2024-05-06 15:09:59.071390 azure-search-documents-11.6.0b4/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22009 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4081 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/TROUBLESHOOTING.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.035390 azure-search-documents-11.6.0b4/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      251 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.035390 azure-search-documents-11.6.0b4/azure/search/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      251 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.039390 azure-search-documents-11.6.0b4/azure/search/documents/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1822 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      482 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_api_versions.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.039390 azure-search-documents-11.6.0b4/azure/search/documents/_generated/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      737 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2645 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4710 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/_search_index_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      678 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.039390 azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      738 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2655 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4833 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/_search_index_client.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.039390 azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      689 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48945 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/operations/_documents_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.043390 azure-search-documents-11.6.0b4/azure/search/documents/_generated/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4606 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   141379 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/models/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17461 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/models/_search_index_client_enums.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.043390 azure-search-documents-11.6.0b4/azure/search/documents/_generated/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      689 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    66933 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/operations/_documents_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_generated/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      843 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_headers_mixin.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6159 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_index_documents_batch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6326 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_paging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4902 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_queries.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38379 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_search_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      491 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_search_documents_error.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15064 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_search_indexing_buffered_sender.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2193 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_search_indexing_buffered_sender_base.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2479 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_utils.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      252 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.043390 azure-search-documents-11.6.0b4/azure/search/documents/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1553 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5980 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/aio/_index_documents_batch_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6013 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/aio/_paging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39253 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/aio/_search_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15395 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/aio/_search_indexing_buffered_sender_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/aio/_timer.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.043390 azure-search-documents-11.6.0b4/azure/search/documents/indexes/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1479 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.047390 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      744 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2411 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6000 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/_search_service_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1217 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.047390 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      744 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2421 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6143 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/_search_service_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      957 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.047390 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1222 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27707 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27708 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    43358 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39135 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4278 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34570 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26345 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.051390 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19469 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   561659 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/models/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    76063 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.051390 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1222 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33849 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_aliases_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34520 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    55289 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_indexers_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48058 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_indexes_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5167 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    43022 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32848 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27197 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_search_index_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30999 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_search_indexer_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3193 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/_utils.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.051390 azure-search-documents-11.6.0b4/azure/search/documents/indexes/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1479 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28240 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/aio/_search_index_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30031 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/aio/_search_indexer_client.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.055390 azure-search-documents-11.6.0b4/azure/search/documents/indexes/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13926 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      624 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/models/_edm.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48753 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/models/_index.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    56174 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/indexes/models/_models.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.055390 azure-search-documents-11.6.0b4/azure/search/documents/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2702 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/azure/search/documents/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.055390 azure-search-documents-11.6.0b4/azure_search_documents.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22937 2024-05-06 15:09:58.000000 azure-search-documents-11.6.0b4/azure_search_documents.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8840 2024-05-06 15:09:59.000000 azure-search-documents-11.6.0b4/azure_search_documents.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-06 15:09:58.000000 azure-search-documents-11.6.0b4/azure_search_documents.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-06 15:09:58.000000 azure-search-documents-11.6.0b4/azure_search_documents.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       52 2024-05-06 15:09:58.000000 azure-search-documents-11.6.0b4/azure_search_documents.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-05-06 15:09:58.000000 azure-search-documents-11.6.0b4/azure_search_documents.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       79 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/pyproject.toml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.059390 azure-search-documents-11.6.0b4/samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6100 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.063390 azure-search-documents-11.6.0b4/samples/async_samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1659 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_analyze_text_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3587 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_authentication_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1679 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_autocomplete_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1899 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_buffered_sender_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2364 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_crud_operations_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3083 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_data_source_operations_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1797 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_facet_query_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1875 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_filter_query_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1721 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_get_document_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3501 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_index_alias_crud_operations_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1816 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_index_client_send_request_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4218 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_index_crud_operations_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4321 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_indexers_operations_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1912 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_query_session_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1800 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_search_client_send_request_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2369 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_semantic_search_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1705 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_simple_query_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1756 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_suggestions_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2546 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_synonym_map_operations_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7302 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/async_samples/sample_vector_search_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1560 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_analyze_text.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3361 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_authentication.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1564 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_autocomplete.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1788 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_buffered_sender.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2166 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_crud_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2826 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_data_source_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1672 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_facet_query.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1734 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_filter_query.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1590 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_get_document.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3275 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_index_alias_crud_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1733 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_index_client_send_request.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3921 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_index_crud_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6067 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_indexer_datasource_skillset.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3878 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_indexers_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1792 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_query_session.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1717 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_search_client_send_request.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2395 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_semantic_search.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1584 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_simple_query.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1630 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_suggestions.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2901 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_synonym_map_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7072 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/samples/sample_vector_search.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-05-06 15:09:59.071390 azure-search-documents-11.6.0b4/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2392 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.067390 azure-search-documents-11.6.0b4/tests/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.067390 azure-search-documents-11.6.0b4/tests/async_tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6759 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/async_tests/test_buffered_sender_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1452 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/async_tests/test_search_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2157 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/async_tests/test_search_client_basic_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7227 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/async_tests/test_search_client_buffered_sender_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6927 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/async_tests/test_search_client_index_document_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6354 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/async_tests/test_search_client_search_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4454 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/async_tests/test_search_index_client_alias_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3921 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/async_tests/test_search_index_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6323 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/async_tests/test_search_index_client_data_source_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8070 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/async_tests/test_search_index_client_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10270 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/async_tests/test_search_index_client_skillset_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6112 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/async_tests/test_search_index_client_synonym_map_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8040 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/async_tests/test_search_indexer_client_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1263 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/conftest.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:09:59.071390 azure-search-documents-11.6.0b4/tests/perfstress_tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/perfstress_tests/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2340 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/perfstress_tests/autocomplete.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2300 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/perfstress_tests/search_documents.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2305 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/perfstress_tests/suggest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29583 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/search_service_preparer.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6451 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_buffered_sender.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2164 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_index_documents_batch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3222 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_index_field_helpers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5887 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_queries.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4604 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_regex_flags.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15109 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_search_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2013 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_search_client_basic_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6790 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_search_client_buffered_sender_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6608 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_search_client_index_document_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5129 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_search_client_search_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5018 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_search_index_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4130 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_search_index_client_alias_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6883 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_search_index_client_data_source_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7627 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_search_index_client_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11708 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_search_index_client_skillset_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5759 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_search_index_client_synonym_map_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7675 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_search_indexer_client_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4093 2024-05-06 15:08:25.000000 azure-search-documents-11.6.0b4/tests/test_serialization.py
```

### Comparing `azure-search-documents-11.6.0b3/CHANGELOG.md` & `azure-search-documents-11.6.0b4/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,37 @@
 # Release History
 
+## 11.6.0b4 (2024-05-07)
+
+### Features Added
+
+- Added new models:
+  - `azure.search.documents.models.HybridCountAndFacetMode`
+  - `azure.search.documents.models.HybridSearch`
+  - `azure.search.documents.models.SearchScoreThreshold`
+  - `azure.search.documents.models.VectorSimilarityThreshold`
+  - `azure.search.documents.models.VectorThreshold`
+  - `azure.search.documents.models.VectorThresholdKind`
+  - `azure.search.documents.models.VectorizableImageBinaryQuery`
+  - `azure.search.documents.models.VectorizableImageUrlQuery`
+  - `azure.search.documents.indexes.models.AIServicesVisionParameters`
+  - `azure.search.documents.indexes.models.AIServicesVisionVectorizer`
+  - `azure.search.documents.indexes.models.AIStudioModelCatalogName`
+  - `azure.search.documents.indexes.models.AzureMachineLearningParameters`
+  - `azure.search.documents.indexes.models.AzureMachineLearningVectorizer`
+  - `azure.search.documents.indexes.models.AzureOpenAIModelName`
+  - `azure.search.documents.indexes.models.VectorEncodingFormat`
+  - `azure.search.documents.indexes.models.VisionVectorizeSkill`
+- Added `hybrid_search` support for `SearchClient.search` method.
+- Updated default API version to `2024-05-01-preview`.
+
+### Bugs Fixed
+
+- Fixed the bug that SearchClient failed when both answer count and answer threshold applied.
+
 ## 11.6.0b3 (2024-04-09)
 
 ### Features Added
 
 - Added `IndexerExecutionEnvironment`, `IndexingMode`, `LineEnding`, `NativeBlobSoftDeleteDeletionDetectionPolicy`, `ScalarQuantizationCompressionConfiguration`, `ScalarQuantizationParameters`, `SearchServiceCounters`, `SearchServiceLimits`, `SearchServiceStatistics`, `VectorSearchCompressionConfiguration` & `VectorSearchCompressionTargetDataType`.
 - Added `stored` in `SearchField`.
```

### Comparing `azure-search-documents-11.6.0b3/LICENSE` & `azure-search-documents-11.6.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/PKG-INFO` & `azure-search-documents-11.6.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-search-documents
-Version: 11.6.0b3
+Version: 11.6.0b4
 Summary: Microsoft Azure Cognitive Search Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/search/azure-search-documents
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -16,17 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: azure-core>=1.28.0
-Requires-Dist: azure-common>=1.1
-Requires-Dist: isodate>=0.6.0
 
 # Azure AI Search client library for Python
 
 [Azure AI Search](https://docs.microsoft.com/azure/search/) (formerly known as "Azure Cognitive Search") is an AI-powered information retrieval platform that helps developers build rich search experiences and generative AI apps that combine large language models with enterprise data.
 
 Azure AI Search is well suited for the following application scenarios:
```

### Comparing `azure-search-documents-11.6.0b3/README.md` & `azure-search-documents-11.6.0b4/README.md`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/TROUBLESHOOTING.md` & `azure-search-documents-11.6.0b4/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/_configuration.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.pipeline import policies
 
@@ -17,21 +17,21 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param endpoint: The endpoint URL of the search service. Required.
     :type endpoint: str
     :param index_name: The name of the index. Required.
     :type index_name: str
-    :keyword api_version: Api Version. Default value is "2024-03-01-Preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2024-05-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, index_name: str, **kwargs: Any) -> None:
-        api_version: str = kwargs.pop("api_version", "2024-03-01-Preview")
+        api_version: str = kwargs.pop("api_version", "2024-05-01-preview")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
         if index_name is None:
             raise ValueError("Parameter 'index_name' must not be None.")
 
         self.endpoint = endpoint
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/_patch.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/_search_index_client.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/_search_index_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any
 
 from azure.core import PipelineClient
@@ -22,15 +22,15 @@
 
     :ivar documents: DocumentsOperations operations
     :vartype documents: azure.search.documents.operations.DocumentsOperations
     :param endpoint: The endpoint URL of the search service. Required.
     :type endpoint: str
     :param index_name: The name of the index. Required.
     :type index_name: str
-    :keyword api_version: Api Version. Default value is "2024-03-01-Preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2024-05-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, endpoint: str, index_name: str, **kwargs: Any
     ) -> None:
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/_serialization.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/_vendor.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/_vendor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from azure.core.pipeline.transport import HttpRequest
 
 
 def _convert_request(request, files=None):
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._search_index_client import SearchIndexClient
 
 try:
     from ._patch import __all__ as _patch_all
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/_configuration.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.pipeline import policies
 
@@ -17,21 +17,21 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param endpoint: The endpoint URL of the search service. Required.
     :type endpoint: str
     :param index_name: The name of the index. Required.
     :type index_name: str
-    :keyword api_version: Api Version. Default value is "2024-03-01-Preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2024-05-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, index_name: str, **kwargs: Any) -> None:
-        api_version: str = kwargs.pop("api_version", "2024-03-01-Preview")
+        api_version: str = kwargs.pop("api_version", "2024-05-01-preview")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
         if index_name is None:
             raise ValueError("Parameter 'index_name' must not be None.")
 
         self.endpoint = endpoint
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/_patch.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/_search_index_client.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/_search_index_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable
 
 from azure.core import AsyncPipelineClient
@@ -22,15 +22,15 @@
 
     :ivar documents: DocumentsOperations operations
     :vartype documents: azure.search.documents.aio.operations.DocumentsOperations
     :param endpoint: The endpoint URL of the search service. Required.
     :type endpoint: str
     :param index_name: The name of the index. Required.
     :type index_name: str
-    :keyword api_version: Api Version. Default value is "2024-03-01-Preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2024-05-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, endpoint: str, index_name: str, **kwargs: Any
     ) -> None:
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._documents_operations import DocumentsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/_documents_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/operations/_documents_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, List, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -31,14 +32,18 @@
     build_index_request,
     build_search_get_request,
     build_search_post_request,
     build_suggest_get_request,
     build_suggest_post_request,
 )
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class DocumentsOperations:
     """
     .. warning::
@@ -67,15 +72,15 @@
 
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: int or the result of cls(response)
         :rtype: int
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -141,15 +146,15 @@
         :type search_options: ~azure.search.documents.models.SearchOptions
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: SearchDocumentsResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.SearchDocumentsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -166,32 +171,32 @@
         _highlight_post_tag = None
         _highlight_pre_tag = None
         _minimum_coverage = None
         _order_by = None
         _query_type = None
         _scoring_parameters = None
         _scoring_profile = None
-        _semantic_query = None
-        _semantic_configuration = None
-        _semantic_error_handling = None
-        _semantic_max_wait_in_milliseconds = None
-        _debug = None
         _search_fields = None
-        _query_language = None
-        _speller = None
-        _answers = None
         _search_mode = None
         _scoring_statistics = None
         _session_id = None
         _select = None
         _skip = None
         _top = None
+        _x_ms_client_request_id = None
+        _semantic_configuration = None
+        _semantic_error_handling = None
+        _semantic_max_wait_in_milliseconds = None
+        _answers = None
         _captions = None
+        _semantic_query = None
+        _debug = None
+        _query_language = None
+        _speller = None
         _semantic_fields = None
-        _x_ms_client_request_id = None
         if search_options is not None:
             _answers = search_options.answers
             _captions = search_options.captions
             _debug = search_options.debug
             _facets = search_options.facets
             _filter = search_options.filter
             _highlight_fields = search_options.highlight_fields
@@ -229,32 +234,32 @@
             highlight_post_tag=_highlight_post_tag,
             highlight_pre_tag=_highlight_pre_tag,
             minimum_coverage=_minimum_coverage,
             order_by=_order_by,
             query_type=_query_type,
             scoring_parameters=_scoring_parameters,
             scoring_profile=_scoring_profile,
-            semantic_query=_semantic_query,
-            semantic_configuration=_semantic_configuration,
-            semantic_error_handling=_semantic_error_handling,
-            semantic_max_wait_in_milliseconds=_semantic_max_wait_in_milliseconds,
-            debug=_debug,
             search_fields=_search_fields,
-            query_language=_query_language,
-            speller=_speller,
-            answers=_answers,
             search_mode=_search_mode,
             scoring_statistics=_scoring_statistics,
             session_id=_session_id,
             select=_select,
             skip=_skip,
             top=_top,
+            x_ms_client_request_id=_x_ms_client_request_id,
+            semantic_configuration=_semantic_configuration,
+            semantic_error_handling=_semantic_error_handling,
+            semantic_max_wait_in_milliseconds=_semantic_max_wait_in_milliseconds,
+            answers=_answers,
             captions=_captions,
+            semantic_query=_semantic_query,
+            debug=_debug,
+            query_language=_query_language,
+            speller=_speller,
             semantic_fields=_semantic_fields,
-            x_ms_client_request_id=_x_ms_client_request_id,
             api_version=api_version,
             headers=_headers,
             params=_params,
         )
         _request = _convert_request(_request)
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
@@ -350,15 +355,15 @@
         :type search_request: ~azure.search.documents.models.SearchRequest or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: SearchDocumentsResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.SearchDocumentsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -435,15 +440,15 @@
         :type selected_fields: list[str]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: dict mapping str to any or the result of cls(response)
         :rtype: dict[str, any]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -515,15 +520,15 @@
         :type suggest_options: ~azure.search.documents.models.SuggestOptions
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: SuggestDocumentsResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.SuggestDocumentsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -668,15 +673,15 @@
         :type suggest_request: ~azure.search.documents.models.SuggestRequest or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: SuggestDocumentsResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.SuggestDocumentsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -802,15 +807,15 @@
         :type batch: ~azure.search.documents.models.IndexBatch or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: IndexDocumentsResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.IndexDocumentsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -894,15 +899,15 @@
         :type request_options: ~azure.search.documents.models.RequestOptions
         :param autocomplete_options: Parameter group. Default value is None.
         :type autocomplete_options: ~azure.search.documents.models.AutocompleteOptions
         :return: AutocompleteResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.AutocompleteResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1044,15 +1049,15 @@
         :type autocomplete_request: ~azure.search.documents.models.AutocompleteRequest or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: AutocompleteResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.AutocompleteResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/_patch.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models_py3 import AutocompleteItem
 from ._models_py3 import AutocompleteOptions
 from ._models_py3 import AutocompleteRequest
 from ._models_py3 import AutocompleteResult
 from ._models_py3 import DocumentDebugInfo
 from ._models_py3 import ErrorAdditionalInfo
 from ._models_py3 import ErrorDetail
 from ._models_py3 import ErrorResponse
 from ._models_py3 import FacetResult
+from ._models_py3 import HybridSearch
 from ._models_py3 import IndexAction
 from ._models_py3 import IndexBatch
 from ._models_py3 import IndexDocumentsResult
 from ._models_py3 import IndexingResult
 from ._models_py3 import QueryAnswerResult
 from ._models_py3 import QueryCaptionResult
 from ._models_py3 import QueryResultDocumentRerankerInput
 from ._models_py3 import QueryResultDocumentSemanticField
 from ._models_py3 import RequestOptions
 from ._models_py3 import SearchDocumentsResult
 from ._models_py3 import SearchOptions
 from ._models_py3 import SearchRequest
 from ._models_py3 import SearchResult
+from ._models_py3 import SearchScoreThreshold
 from ._models_py3 import SemanticDebugInfo
 from ._models_py3 import SuggestDocumentsResult
 from ._models_py3 import SuggestOptions
 from ._models_py3 import SuggestRequest
 from ._models_py3 import SuggestResult
 from ._models_py3 import VectorQuery
+from ._models_py3 import VectorSimilarityThreshold
+from ._models_py3 import VectorThreshold
+from ._models_py3 import VectorizableImageBinaryQuery
+from ._models_py3 import VectorizableImageUrlQuery
 from ._models_py3 import VectorizableTextQuery
 from ._models_py3 import VectorizedQuery
 
 from ._search_index_client_enums import AutocompleteMode
+from ._search_index_client_enums import HybridCountAndFacetMode
 from ._search_index_client_enums import IndexActionType
 from ._search_index_client_enums import QueryAnswerType
 from ._search_index_client_enums import QueryCaptionType
 from ._search_index_client_enums import QueryDebugMode
 from ._search_index_client_enums import QueryLanguage
 from ._search_index_client_enums import QuerySpellerType
 from ._search_index_client_enums import QueryType
@@ -48,50 +55,58 @@
 from ._search_index_client_enums import SemanticErrorMode
 from ._search_index_client_enums import SemanticErrorReason
 from ._search_index_client_enums import SemanticFieldState
 from ._search_index_client_enums import SemanticSearchResultsType
 from ._search_index_client_enums import Speller
 from ._search_index_client_enums import VectorFilterMode
 from ._search_index_client_enums import VectorQueryKind
+from ._search_index_client_enums import VectorThresholdKind
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AutocompleteItem",
     "AutocompleteOptions",
     "AutocompleteRequest",
     "AutocompleteResult",
     "DocumentDebugInfo",
     "ErrorAdditionalInfo",
     "ErrorDetail",
     "ErrorResponse",
     "FacetResult",
+    "HybridSearch",
     "IndexAction",
     "IndexBatch",
     "IndexDocumentsResult",
     "IndexingResult",
     "QueryAnswerResult",
     "QueryCaptionResult",
     "QueryResultDocumentRerankerInput",
     "QueryResultDocumentSemanticField",
     "RequestOptions",
     "SearchDocumentsResult",
     "SearchOptions",
     "SearchRequest",
     "SearchResult",
+    "SearchScoreThreshold",
     "SemanticDebugInfo",
     "SuggestDocumentsResult",
     "SuggestOptions",
     "SuggestRequest",
     "SuggestResult",
     "VectorQuery",
+    "VectorSimilarityThreshold",
+    "VectorThreshold",
+    "VectorizableImageBinaryQuery",
+    "VectorizableImageUrlQuery",
     "VectorizableTextQuery",
     "VectorizedQuery",
     "AutocompleteMode",
+    "HybridCountAndFacetMode",
     "IndexActionType",
     "QueryAnswerType",
     "QueryCaptionType",
     "QueryDebugMode",
     "QueryLanguage",
     "QuerySpellerType",
     "QueryType",
@@ -100,10 +115,11 @@
     "SemanticErrorMode",
     "SemanticErrorReason",
     "SemanticFieldState",
     "SemanticSearchResultsType",
     "Speller",
     "VectorFilterMode",
     "VectorQueryKind",
+    "VectorThresholdKind",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/_models_py3.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/models/_models_py3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 # coding=utf-8
 # pylint: disable=too-many-lines
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+import sys
 from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
 
 from .. import _serialization
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from .. import models as _models
+JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 
 
 class AutocompleteItem(_serialization.Model):
     """The result of Autocomplete requests.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -447,14 +454,60 @@
         :paramtype additional_properties: dict[str, any]
         """
         super().__init__(**kwargs)
         self.additional_properties = additional_properties
         self.count = None
 
 
+class HybridSearch(_serialization.Model):
+    """TThe query parameters to configure hybrid search behaviors.
+
+    :ivar max_text_recall_size: Determines the maximum number of documents to be retrieved by the
+     text query portion of a hybrid search request. Those documents will be combined with the
+     documents matching the vector queries to produce a single final list of results. Choosing a
+     larger maxTextRecallSize value will allow retrieving and paging through more documents (using
+     the top and skip parameters), at the cost of higher resource utilization and higher latency.
+     The value needs to be between 1 and 10,000. Default is 1000.
+    :vartype max_text_recall_size: int
+    :ivar count_and_facet_mode: Determines whether the count and facets should includes all
+     documents that matched the search query, or only the documents that are retrieved within the
+     'maxTextRecallSize' window. Known values are: "countRetrievableResults" and "countAllResults".
+    :vartype count_and_facet_mode: str or ~azure.search.documents.models.HybridCountAndFacetMode
+    """
+
+    _attribute_map = {
+        "max_text_recall_size": {"key": "maxTextRecallSize", "type": "int"},
+        "count_and_facet_mode": {"key": "countAndFacetMode", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        max_text_recall_size: Optional[int] = None,
+        count_and_facet_mode: Optional[Union[str, "_models.HybridCountAndFacetMode"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword max_text_recall_size: Determines the maximum number of documents to be retrieved by
+         the text query portion of a hybrid search request. Those documents will be combined with the
+         documents matching the vector queries to produce a single final list of results. Choosing a
+         larger maxTextRecallSize value will allow retrieving and paging through more documents (using
+         the top and skip parameters), at the cost of higher resource utilization and higher latency.
+         The value needs to be between 1 and 10,000. Default is 1000.
+        :paramtype max_text_recall_size: int
+        :keyword count_and_facet_mode: Determines whether the count and facets should includes all
+         documents that matched the search query, or only the documents that are retrieved within the
+         'maxTextRecallSize' window. Known values are: "countRetrievableResults" and "countAllResults".
+        :paramtype count_and_facet_mode: str or ~azure.search.documents.models.HybridCountAndFacetMode
+        """
+        super().__init__(**kwargs)
+        self.max_text_recall_size = max_text_recall_size
+        self.count_and_facet_mode = count_and_facet_mode
+
+
 class IndexAction(_serialization.Model):
     """Represents an index action that operates on a document.
 
     :ivar additional_properties: Unmatched properties from the message are deserialized to this
      collection.
     :vartype additional_properties: dict[str, any]
     :ivar action_type: The operation to perform on a document in an indexing batch. Known values
@@ -883,62 +936,24 @@
      example, referencePointParameter) using the format name-values. For example, if the scoring
      profile defines a function with a parameter called 'mylocation' the parameter string would be
      "mylocation--122.2,44.8" (without the quotes).
     :vartype scoring_parameters: list[str]
     :ivar scoring_profile: The name of a scoring profile to evaluate match scores for matching
      documents in order to sort the results.
     :vartype scoring_profile: str
-    :ivar semantic_query: Allows setting a separate search query that will be solely used for
-     semantic reranking, semantic captions and semantic answers. Is useful for scenarios where there
-     is a need to use different queries between the base retrieval and ranking phase, and the L2
-     semantic phase.
-    :vartype semantic_query: str
-    :ivar semantic_configuration: The name of the semantic configuration that lists which fields
-     should be used for semantic ranking, captions, highlights, and answers.
-    :vartype semantic_configuration: str
-    :ivar semantic_error_handling: Allows the user to choose whether a semantic call should fail
-     completely, or to return partial results (default). Known values are: "partial" and "fail".
-    :vartype semantic_error_handling: str or ~azure.search.documents.models.SemanticErrorMode
-    :ivar semantic_max_wait_in_milliseconds: Allows the user to set an upper bound on the amount of
-     time it takes for semantic enrichment to finish processing before the request fails.
-    :vartype semantic_max_wait_in_milliseconds: int
-    :ivar debug: Enables a debugging tool that can be used to further explore your search results.
-     Known values are: "disabled" and "semantic".
-    :vartype debug: str or ~azure.search.documents.models.QueryDebugMode
     :ivar search_fields: The list of field names to which to scope the full-text search. When using
      fielded search (fieldName:searchExpression) in a full Lucene query, the field names of each
      fielded search expression take precedence over any field names listed in this parameter.
     :vartype search_fields: list[str]
-    :ivar query_language: The language of the query. Known values are: "none", "en-us", "en-gb",
-     "en-in", "en-ca", "en-au", "fr-fr", "fr-ca", "de-de", "es-es", "es-mx", "zh-cn", "zh-tw",
-     "pt-br", "pt-pt", "it-it", "ja-jp", "ko-kr", "ru-ru", "cs-cz", "nl-be", "nl-nl", "hu-hu",
-     "pl-pl", "sv-se", "tr-tr", "hi-in", "ar-sa", "ar-eg", "ar-ma", "ar-kw", "ar-jo", "da-dk",
-     "no-no", "bg-bg", "hr-hr", "hr-ba", "ms-my", "ms-bn", "sl-sl", "ta-in", "vi-vn", "el-gr",
-     "ro-ro", "is-is", "id-id", "th-th", "lt-lt", "uk-ua", "lv-lv", "et-ee", "ca-es", "fi-fi",
-     "sr-ba", "sr-me", "sr-rs", "sk-sk", "nb-no", "hy-am", "bn-in", "eu-es", "gl-es", "gu-in",
-     "he-il", "ga-ie", "kn-in", "ml-in", "mr-in", "fa-ae", "pa-in", "te-in", and "ur-pk".
-    :vartype query_language: str or ~azure.search.documents.models.QueryLanguage
-    :ivar speller: Improve search recall by spell-correcting individual search query terms. Known
-     values are: "none" and "lexicon".
-    :vartype speller: str or ~azure.search.documents.models.Speller
-    :ivar answers: This parameter is only valid if the query type is ``semantic``. If set, the
-     query returns answers extracted from key passages in the highest ranked documents. The number
-     of answers returned can be configured by appending the pipe character ``|`` followed by the
-     ``count-<number of answers>`` option after the answers parameter value, such as
-     ``extractive|count-3``. Default count is 1. The confidence threshold can be configured by
-     appending the pipe character ``|`` followed by the ``threshold-<confidence threshold>`` option
-     after the answers parameter value, such as ``extractive|threshold-0.9``. Default threshold is
-     0.7. Known values are: "none" and "extractive".
-    :vartype answers: str or ~azure.search.documents.models.QueryAnswerType
     :ivar search_mode: A value that specifies whether any or all of the search terms must be
      matched in order to count the document as a match. Known values are: "any" and "all".
     :vartype search_mode: str or ~azure.search.documents.models.SearchMode
     :ivar scoring_statistics: A value that specifies whether we want to calculate scoring
      statistics (such as document frequency) globally for more consistent scoring, or locally, for
-     lower latency. Known values are: "local", "global", and "global".
+     lower latency. Known values are: "local" and "global".
     :vartype scoring_statistics: str or ~azure.search.documents.models.ScoringStatistics
     :ivar session_id: A value to be used to create a sticky session, which can help to get more
      consistent results. As long as the same sessionId is used, a best-effort attempt will be made
      to target the same replica set. Be wary that reusing the same sessionID values repeatedly can
      interfere with the load balancing of the requests across replicas and adversely affect the
      performance of the search service. The value used as sessionId cannot start with a '_'
      character.
@@ -951,21 +966,59 @@
      using $orderby on a totally-ordered key and $filter with a range query instead.
     :vartype skip: int
     :ivar top: The number of search results to retrieve. This can be used in conjunction with $skip
      to implement client-side paging of search results. If results are truncated due to server-side
      paging, the response will include a continuation token that can be used to issue another Search
      request for the next page of results.
     :vartype top: int
+    :ivar semantic_configuration: The name of the semantic configuration that lists which fields
+     should be used for semantic ranking, captions, highlights, and answers.
+    :vartype semantic_configuration: str
+    :ivar semantic_error_handling: Allows the user to choose whether a semantic call should fail
+     completely, or to return partial results (default). Known values are: "partial" and "fail".
+    :vartype semantic_error_handling: str or ~azure.search.documents.models.SemanticErrorMode
+    :ivar semantic_max_wait_in_milliseconds: Allows the user to set an upper bound on the amount of
+     time it takes for semantic enrichment to finish processing before the request fails.
+    :vartype semantic_max_wait_in_milliseconds: int
+    :ivar answers: This parameter is only valid if the query type is ``semantic``. If set, the
+     query returns answers extracted from key passages in the highest ranked documents. The number
+     of answers returned can be configured by appending the pipe character ``|`` followed by the
+     ``count-<number of answers>`` option after the answers parameter value, such as
+     ``extractive|count-3``. Default count is 1. The confidence threshold can be configured by
+     appending the pipe character ``|`` followed by the ``threshold-<confidence threshold>`` option
+     after the answers parameter value, such as ``extractive|threshold-0.9``. Default threshold is
+     0.7. Known values are: "none" and "extractive".
+    :vartype answers: str or ~azure.search.documents.models.QueryAnswerType
     :ivar captions: This parameter is only valid if the query type is ``semantic``. If set, the
      query returns captions extracted from key passages in the highest ranked documents. When
      Captions is set to ``extractive``\ , highlighting is enabled by default, and can be configured
      by appending the pipe character ``|`` followed by the ``highlight-<true/false>`` option, such
      as ``extractive|highlight-true``. Defaults to ``None``. Known values are: "none" and
      "extractive".
     :vartype captions: str or ~azure.search.documents.models.QueryCaptionType
+    :ivar semantic_query: Allows setting a separate search query that will be solely used for
+     semantic reranking, semantic captions and semantic answers. Is useful for scenarios where there
+     is a need to use different queries between the base retrieval and ranking phase, and the L2
+     semantic phase.
+    :vartype semantic_query: str
+    :ivar debug: Enables a debugging tool that can be used to further explore your search results.
+     Known values are: "disabled" and "semantic".
+    :vartype debug: str or ~azure.search.documents.models.QueryDebugMode
+    :ivar query_language: The language of the query. Known values are: "none", "en-us", "en-gb",
+     "en-in", "en-ca", "en-au", "fr-fr", "fr-ca", "de-de", "es-es", "es-mx", "zh-cn", "zh-tw",
+     "pt-br", "pt-pt", "it-it", "ja-jp", "ko-kr", "ru-ru", "cs-cz", "nl-be", "nl-nl", "hu-hu",
+     "pl-pl", "sv-se", "tr-tr", "hi-in", "ar-sa", "ar-eg", "ar-ma", "ar-kw", "ar-jo", "da-dk",
+     "no-no", "bg-bg", "hr-hr", "hr-ba", "ms-my", "ms-bn", "sl-sl", "ta-in", "vi-vn", "el-gr",
+     "ro-ro", "is-is", "id-id", "th-th", "lt-lt", "uk-ua", "lv-lv", "et-ee", "ca-es", "fi-fi",
+     "sr-ba", "sr-me", "sr-rs", "sk-sk", "nb-no", "hy-am", "bn-in", "eu-es", "gl-es", "gu-in",
+     "he-il", "ga-ie", "kn-in", "ml-in", "mr-in", "fa-ae", "pa-in", "te-in", and "ur-pk".
+    :vartype query_language: str or ~azure.search.documents.models.QueryLanguage
+    :ivar speller: Improve search recall by spell-correcting individual search query terms. Known
+     values are: "none" and "lexicon".
+    :vartype speller: str or ~azure.search.documents.models.Speller
     :ivar semantic_fields: The list of field names used for semantic ranking.
     :vartype semantic_fields: list[str]
     """
 
     _validation = {
         "semantic_max_wait_in_milliseconds": {"minimum": 700},
     }
@@ -978,30 +1031,30 @@
         "highlight_post_tag": {"key": "highlightPostTag", "type": "str"},
         "highlight_pre_tag": {"key": "highlightPreTag", "type": "str"},
         "minimum_coverage": {"key": "minimumCoverage", "type": "float"},
         "order_by": {"key": "OrderBy", "type": "[str]"},
         "query_type": {"key": "queryType", "type": "str"},
         "scoring_parameters": {"key": "ScoringParameters", "type": "[str]"},
         "scoring_profile": {"key": "scoringProfile", "type": "str"},
-        "semantic_query": {"key": "semanticQuery", "type": "str"},
-        "semantic_configuration": {"key": "semanticConfiguration", "type": "str"},
-        "semantic_error_handling": {"key": "semanticErrorHandling", "type": "str"},
-        "semantic_max_wait_in_milliseconds": {"key": "semanticMaxWaitInMilliseconds", "type": "int"},
-        "debug": {"key": "debug", "type": "str"},
         "search_fields": {"key": "searchFields", "type": "[str]"},
-        "query_language": {"key": "queryLanguage", "type": "str"},
-        "speller": {"key": "speller", "type": "str"},
-        "answers": {"key": "answers", "type": "str"},
         "search_mode": {"key": "searchMode", "type": "str"},
         "scoring_statistics": {"key": "scoringStatistics", "type": "str"},
         "session_id": {"key": "sessionId", "type": "str"},
         "select": {"key": "$select", "type": "[str]"},
         "skip": {"key": "$skip", "type": "int"},
         "top": {"key": "$top", "type": "int"},
+        "semantic_configuration": {"key": "semanticConfiguration", "type": "str"},
+        "semantic_error_handling": {"key": "semanticErrorHandling", "type": "str"},
+        "semantic_max_wait_in_milliseconds": {"key": "semanticMaxWaitInMilliseconds", "type": "int"},
+        "answers": {"key": "answers", "type": "str"},
         "captions": {"key": "captions", "type": "str"},
+        "semantic_query": {"key": "semanticQuery", "type": "str"},
+        "debug": {"key": "debug", "type": "str"},
+        "query_language": {"key": "queryLanguage", "type": "str"},
+        "speller": {"key": "speller", "type": "str"},
         "semantic_fields": {"key": "semanticFields", "type": "[str]"},
     }
 
     def __init__(  # pylint: disable=too-many-locals
         self,
         *,
         include_total_result_count: Optional[bool] = None,
@@ -1011,30 +1064,30 @@
         highlight_post_tag: Optional[str] = None,
         highlight_pre_tag: Optional[str] = None,
         minimum_coverage: Optional[float] = None,
         order_by: Optional[List[str]] = None,
         query_type: Optional[Union[str, "_models.QueryType"]] = None,
         scoring_parameters: Optional[List[str]] = None,
         scoring_profile: Optional[str] = None,
-        semantic_query: Optional[str] = None,
-        semantic_configuration: Optional[str] = None,
-        semantic_error_handling: Optional[Union[str, "_models.SemanticErrorMode"]] = None,
-        semantic_max_wait_in_milliseconds: Optional[int] = None,
-        debug: Optional[Union[str, "_models.QueryDebugMode"]] = None,
         search_fields: Optional[List[str]] = None,
-        query_language: Optional[Union[str, "_models.QueryLanguage"]] = None,
-        speller: Optional[Union[str, "_models.Speller"]] = None,
-        answers: Optional[Union[str, "_models.QueryAnswerType"]] = None,
         search_mode: Optional[Union[str, "_models.SearchMode"]] = None,
         scoring_statistics: Optional[Union[str, "_models.ScoringStatistics"]] = None,
         session_id: Optional[str] = None,
         select: Optional[List[str]] = None,
         skip: Optional[int] = None,
         top: Optional[int] = None,
+        semantic_configuration: Optional[str] = None,
+        semantic_error_handling: Optional[Union[str, "_models.SemanticErrorMode"]] = None,
+        semantic_max_wait_in_milliseconds: Optional[int] = None,
+        answers: Optional[Union[str, "_models.QueryAnswerType"]] = None,
         captions: Optional[Union[str, "_models.QueryCaptionType"]] = None,
+        semantic_query: Optional[str] = None,
+        debug: Optional[Union[str, "_models.QueryDebugMode"]] = None,
+        query_language: Optional[Union[str, "_models.QueryLanguage"]] = None,
+        speller: Optional[Union[str, "_models.Speller"]] = None,
         semantic_fields: Optional[List[str]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword include_total_result_count: A value that specifies whether to fetch the total count of
          results. Default is false. Setting this value to true may have a performance impact. Note that
          the count returned is an approximation.
@@ -1074,62 +1127,24 @@
          example, referencePointParameter) using the format name-values. For example, if the scoring
          profile defines a function with a parameter called 'mylocation' the parameter string would be
          "mylocation--122.2,44.8" (without the quotes).
         :paramtype scoring_parameters: list[str]
         :keyword scoring_profile: The name of a scoring profile to evaluate match scores for matching
          documents in order to sort the results.
         :paramtype scoring_profile: str
-        :keyword semantic_query: Allows setting a separate search query that will be solely used for
-         semantic reranking, semantic captions and semantic answers. Is useful for scenarios where there
-         is a need to use different queries between the base retrieval and ranking phase, and the L2
-         semantic phase.
-        :paramtype semantic_query: str
-        :keyword semantic_configuration: The name of the semantic configuration that lists which fields
-         should be used for semantic ranking, captions, highlights, and answers.
-        :paramtype semantic_configuration: str
-        :keyword semantic_error_handling: Allows the user to choose whether a semantic call should fail
-         completely, or to return partial results (default). Known values are: "partial" and "fail".
-        :paramtype semantic_error_handling: str or ~azure.search.documents.models.SemanticErrorMode
-        :keyword semantic_max_wait_in_milliseconds: Allows the user to set an upper bound on the amount
-         of time it takes for semantic enrichment to finish processing before the request fails.
-        :paramtype semantic_max_wait_in_milliseconds: int
-        :keyword debug: Enables a debugging tool that can be used to further explore your search
-         results. Known values are: "disabled" and "semantic".
-        :paramtype debug: str or ~azure.search.documents.models.QueryDebugMode
         :keyword search_fields: The list of field names to which to scope the full-text search. When
          using fielded search (fieldName:searchExpression) in a full Lucene query, the field names of
          each fielded search expression take precedence over any field names listed in this parameter.
         :paramtype search_fields: list[str]
-        :keyword query_language: The language of the query. Known values are: "none", "en-us", "en-gb",
-         "en-in", "en-ca", "en-au", "fr-fr", "fr-ca", "de-de", "es-es", "es-mx", "zh-cn", "zh-tw",
-         "pt-br", "pt-pt", "it-it", "ja-jp", "ko-kr", "ru-ru", "cs-cz", "nl-be", "nl-nl", "hu-hu",
-         "pl-pl", "sv-se", "tr-tr", "hi-in", "ar-sa", "ar-eg", "ar-ma", "ar-kw", "ar-jo", "da-dk",
-         "no-no", "bg-bg", "hr-hr", "hr-ba", "ms-my", "ms-bn", "sl-sl", "ta-in", "vi-vn", "el-gr",
-         "ro-ro", "is-is", "id-id", "th-th", "lt-lt", "uk-ua", "lv-lv", "et-ee", "ca-es", "fi-fi",
-         "sr-ba", "sr-me", "sr-rs", "sk-sk", "nb-no", "hy-am", "bn-in", "eu-es", "gl-es", "gu-in",
-         "he-il", "ga-ie", "kn-in", "ml-in", "mr-in", "fa-ae", "pa-in", "te-in", and "ur-pk".
-        :paramtype query_language: str or ~azure.search.documents.models.QueryLanguage
-        :keyword speller: Improve search recall by spell-correcting individual search query terms.
-         Known values are: "none" and "lexicon".
-        :paramtype speller: str or ~azure.search.documents.models.Speller
-        :keyword answers: This parameter is only valid if the query type is ``semantic``. If set, the
-         query returns answers extracted from key passages in the highest ranked documents. The number
-         of answers returned can be configured by appending the pipe character ``|`` followed by the
-         ``count-<number of answers>`` option after the answers parameter value, such as
-         ``extractive|count-3``. Default count is 1. The confidence threshold can be configured by
-         appending the pipe character ``|`` followed by the ``threshold-<confidence threshold>`` option
-         after the answers parameter value, such as ``extractive|threshold-0.9``. Default threshold is
-         0.7. Known values are: "none" and "extractive".
-        :paramtype answers: str or ~azure.search.documents.models.QueryAnswerType
         :keyword search_mode: A value that specifies whether any or all of the search terms must be
          matched in order to count the document as a match. Known values are: "any" and "all".
         :paramtype search_mode: str or ~azure.search.documents.models.SearchMode
         :keyword scoring_statistics: A value that specifies whether we want to calculate scoring
          statistics (such as document frequency) globally for more consistent scoring, or locally, for
-         lower latency. Known values are: "local", "global", and "global".
+         lower latency. Known values are: "local" and "global".
         :paramtype scoring_statistics: str or ~azure.search.documents.models.ScoringStatistics
         :keyword session_id: A value to be used to create a sticky session, which can help to get more
          consistent results. As long as the same sessionId is used, a best-effort attempt will be made
          to target the same replica set. Be wary that reusing the same sessionID values repeatedly can
          interfere with the load balancing of the requests across replicas and adversely affect the
          performance of the search service. The value used as sessionId cannot start with a '_'
          character.
@@ -1142,21 +1157,59 @@
          consider using $orderby on a totally-ordered key and $filter with a range query instead.
         :paramtype skip: int
         :keyword top: The number of search results to retrieve. This can be used in conjunction with
          $skip to implement client-side paging of search results. If results are truncated due to
          server-side paging, the response will include a continuation token that can be used to issue
          another Search request for the next page of results.
         :paramtype top: int
+        :keyword semantic_configuration: The name of the semantic configuration that lists which fields
+         should be used for semantic ranking, captions, highlights, and answers.
+        :paramtype semantic_configuration: str
+        :keyword semantic_error_handling: Allows the user to choose whether a semantic call should fail
+         completely, or to return partial results (default). Known values are: "partial" and "fail".
+        :paramtype semantic_error_handling: str or ~azure.search.documents.models.SemanticErrorMode
+        :keyword semantic_max_wait_in_milliseconds: Allows the user to set an upper bound on the amount
+         of time it takes for semantic enrichment to finish processing before the request fails.
+        :paramtype semantic_max_wait_in_milliseconds: int
+        :keyword answers: This parameter is only valid if the query type is ``semantic``. If set, the
+         query returns answers extracted from key passages in the highest ranked documents. The number
+         of answers returned can be configured by appending the pipe character ``|`` followed by the
+         ``count-<number of answers>`` option after the answers parameter value, such as
+         ``extractive|count-3``. Default count is 1. The confidence threshold can be configured by
+         appending the pipe character ``|`` followed by the ``threshold-<confidence threshold>`` option
+         after the answers parameter value, such as ``extractive|threshold-0.9``. Default threshold is
+         0.7. Known values are: "none" and "extractive".
+        :paramtype answers: str or ~azure.search.documents.models.QueryAnswerType
         :keyword captions: This parameter is only valid if the query type is ``semantic``. If set, the
          query returns captions extracted from key passages in the highest ranked documents. When
          Captions is set to ``extractive``\ , highlighting is enabled by default, and can be configured
          by appending the pipe character ``|`` followed by the ``highlight-<true/false>`` option, such
          as ``extractive|highlight-true``. Defaults to ``None``. Known values are: "none" and
          "extractive".
         :paramtype captions: str or ~azure.search.documents.models.QueryCaptionType
+        :keyword semantic_query: Allows setting a separate search query that will be solely used for
+         semantic reranking, semantic captions and semantic answers. Is useful for scenarios where there
+         is a need to use different queries between the base retrieval and ranking phase, and the L2
+         semantic phase.
+        :paramtype semantic_query: str
+        :keyword debug: Enables a debugging tool that can be used to further explore your search
+         results. Known values are: "disabled" and "semantic".
+        :paramtype debug: str or ~azure.search.documents.models.QueryDebugMode
+        :keyword query_language: The language of the query. Known values are: "none", "en-us", "en-gb",
+         "en-in", "en-ca", "en-au", "fr-fr", "fr-ca", "de-de", "es-es", "es-mx", "zh-cn", "zh-tw",
+         "pt-br", "pt-pt", "it-it", "ja-jp", "ko-kr", "ru-ru", "cs-cz", "nl-be", "nl-nl", "hu-hu",
+         "pl-pl", "sv-se", "tr-tr", "hi-in", "ar-sa", "ar-eg", "ar-ma", "ar-kw", "ar-jo", "da-dk",
+         "no-no", "bg-bg", "hr-hr", "hr-ba", "ms-my", "ms-bn", "sl-sl", "ta-in", "vi-vn", "el-gr",
+         "ro-ro", "is-is", "id-id", "th-th", "lt-lt", "uk-ua", "lv-lv", "et-ee", "ca-es", "fi-fi",
+         "sr-ba", "sr-me", "sr-rs", "sk-sk", "nb-no", "hy-am", "bn-in", "eu-es", "gl-es", "gu-in",
+         "he-il", "ga-ie", "kn-in", "ml-in", "mr-in", "fa-ae", "pa-in", "te-in", and "ur-pk".
+        :paramtype query_language: str or ~azure.search.documents.models.QueryLanguage
+        :keyword speller: Improve search recall by spell-correcting individual search query terms.
+         Known values are: "none" and "lexicon".
+        :paramtype speller: str or ~azure.search.documents.models.Speller
         :keyword semantic_fields: The list of field names used for semantic ranking.
         :paramtype semantic_fields: list[str]
         """
         super().__init__(**kwargs)
         self.include_total_result_count = include_total_result_count
         self.facets = facets
         self.filter = filter
@@ -1164,30 +1217,30 @@
         self.highlight_post_tag = highlight_post_tag
         self.highlight_pre_tag = highlight_pre_tag
         self.minimum_coverage = minimum_coverage
         self.order_by = order_by
         self.query_type = query_type
         self.scoring_parameters = scoring_parameters
         self.scoring_profile = scoring_profile
-        self.semantic_query = semantic_query
-        self.semantic_configuration = semantic_configuration
-        self.semantic_error_handling = semantic_error_handling
-        self.semantic_max_wait_in_milliseconds = semantic_max_wait_in_milliseconds
-        self.debug = debug
         self.search_fields = search_fields
-        self.query_language = query_language
-        self.speller = speller
-        self.answers = answers
         self.search_mode = search_mode
         self.scoring_statistics = scoring_statistics
         self.session_id = session_id
         self.select = select
         self.skip = skip
         self.top = top
+        self.semantic_configuration = semantic_configuration
+        self.semantic_error_handling = semantic_error_handling
+        self.semantic_max_wait_in_milliseconds = semantic_max_wait_in_milliseconds
+        self.answers = answers
         self.captions = captions
+        self.semantic_query = semantic_query
+        self.debug = debug
+        self.query_language = query_language
+        self.speller = speller
         self.semantic_fields = semantic_fields
 
 
 class SearchRequest(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """Parameters for filtering, sorting, faceting, paging, and other search query behaviors.
 
     :ivar include_total_result_count: A value that specifies whether to fetch the total count of
@@ -1224,15 +1277,15 @@
      'simple'. Use 'full' if your query uses the Lucene query syntax. Known values are: "simple",
      "full", and "semantic".
     :vartype query_type: str or ~azure.search.documents.models.QueryType
     :ivar scoring_statistics: A value that specifies whether we want to calculate scoring
      statistics (such as document frequency) globally for more consistent scoring, or locally, for
      lower latency. The default is 'local'. Use 'global' to aggregate scoring statistics globally
      before scoring. Using global scoring statistics can increase latency of search queries. Known
-     values are: "local", "global", and "global".
+     values are: "local" and "global".
     :vartype scoring_statistics: str or ~azure.search.documents.models.ScoringStatistics
     :ivar session_id: A value to be used to create a sticky session, which can help getting more
      consistent results. As long as the same sessionId is used, a best-effort attempt will be made
      to target the same replica set. Be wary that reusing the same sessionID values repeatedly can
      interfere with the load balancing of the requests across replicas and adversely affect the
      performance of the search service. The value used as sessionId cannot start with a '_'
      character.
@@ -1308,14 +1361,16 @@
     :vartype semantic_fields: str
     :ivar vector_queries: The query parameters for vector and hybrid search queries.
     :vartype vector_queries: list[~azure.search.documents.models.VectorQuery]
     :ivar vector_filter_mode: Determines whether or not filters are applied before or after the
      vector search is performed. Default is 'preFilter'. Known values are: "postFilter" and
      "preFilter".
     :vartype vector_filter_mode: str or ~azure.search.documents.models.VectorFilterMode
+    :ivar hybrid_search: The query parameters to configure hybrid search behaviors.
+    :vartype hybrid_search: JSON
     """
 
     _validation = {
         "semantic_max_wait_in_milliseconds": {"minimum": 700},
     }
 
     _attribute_map = {
@@ -1346,14 +1401,15 @@
         "select": {"key": "select", "type": "str"},
         "skip": {"key": "skip", "type": "int"},
         "top": {"key": "top", "type": "int"},
         "captions": {"key": "captions", "type": "str"},
         "semantic_fields": {"key": "semanticFields", "type": "str"},
         "vector_queries": {"key": "vectorQueries", "type": "[VectorQuery]"},
         "vector_filter_mode": {"key": "vectorFilterMode", "type": "str"},
+        "hybrid_search": {"key": "hybridSearch", "type": "object"},
     }
 
     def __init__(  # pylint: disable=too-many-locals
         self,
         *,
         include_total_result_count: Optional[bool] = None,
         facets: Optional[List[str]] = None,
@@ -1382,14 +1438,15 @@
         select: Optional[str] = None,
         skip: Optional[int] = None,
         top: Optional[int] = None,
         captions: Optional[Union[str, "_models.QueryCaptionType"]] = None,
         semantic_fields: Optional[str] = None,
         vector_queries: Optional[List["_models.VectorQuery"]] = None,
         vector_filter_mode: Optional[Union[str, "_models.VectorFilterMode"]] = None,
+        hybrid_search: Optional[JSON] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword include_total_result_count: A value that specifies whether to fetch the total count of
          results. Default is false. Setting this value to true may have a performance impact. Note that
          the count returned is an approximation.
         :paramtype include_total_result_count: bool
@@ -1424,15 +1481,15 @@
          'simple'. Use 'full' if your query uses the Lucene query syntax. Known values are: "simple",
          "full", and "semantic".
         :paramtype query_type: str or ~azure.search.documents.models.QueryType
         :keyword scoring_statistics: A value that specifies whether we want to calculate scoring
          statistics (such as document frequency) globally for more consistent scoring, or locally, for
          lower latency. The default is 'local'. Use 'global' to aggregate scoring statistics globally
          before scoring. Using global scoring statistics can increase latency of search queries. Known
-         values are: "local", "global", and "global".
+         values are: "local" and "global".
         :paramtype scoring_statistics: str or ~azure.search.documents.models.ScoringStatistics
         :keyword session_id: A value to be used to create a sticky session, which can help getting more
          consistent results. As long as the same sessionId is used, a best-effort attempt will be made
          to target the same replica set. Be wary that reusing the same sessionID values repeatedly can
          interfere with the load balancing of the requests across replicas and adversely affect the
          performance of the search service. The value used as sessionId cannot start with a '_'
          character.
@@ -1508,14 +1565,16 @@
         :paramtype semantic_fields: str
         :keyword vector_queries: The query parameters for vector and hybrid search queries.
         :paramtype vector_queries: list[~azure.search.documents.models.VectorQuery]
         :keyword vector_filter_mode: Determines whether or not filters are applied before or after the
          vector search is performed. Default is 'preFilter'. Known values are: "postFilter" and
          "preFilter".
         :paramtype vector_filter_mode: str or ~azure.search.documents.models.VectorFilterMode
+        :keyword hybrid_search: The query parameters to configure hybrid search behaviors.
+        :paramtype hybrid_search: JSON
         """
         super().__init__(**kwargs)
         self.include_total_result_count = include_total_result_count
         self.facets = facets
         self.filter = filter
         self.highlight_fields = highlight_fields
         self.highlight_post_tag = highlight_post_tag
@@ -1541,14 +1600,15 @@
         self.select = select
         self.skip = skip
         self.top = top
         self.captions = captions
         self.semantic_fields = semantic_fields
         self.vector_queries = vector_queries
         self.vector_filter_mode = vector_filter_mode
+        self.hybrid_search = hybrid_search
 
 
 class SearchResult(_serialization.Model):
     """Contains a document found by a search query, plus associated metadata.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -1604,14 +1664,81 @@
         self.score = None
         self.reranker_score = None
         self.highlights = None
         self.captions = None
         self.document_debug_info = None
 
 
+class VectorThreshold(_serialization.Model):
+    """The threshold used for vector queries.
+
+    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
+    SearchScoreThreshold, VectorSimilarityThreshold
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar kind: The kind of threshold used to filter vector queries. Required. Known values are:
+     "vectorSimilarity" and "searchScore".
+    :vartype kind: str or ~azure.search.documents.models.VectorThresholdKind
+    """
+
+    _validation = {
+        "kind": {"required": True},
+    }
+
+    _attribute_map = {
+        "kind": {"key": "kind", "type": "str"},
+    }
+
+    _subtype_map = {"kind": {"searchScore": "SearchScoreThreshold", "vectorSimilarity": "VectorSimilarityThreshold"}}
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.kind: Optional[str] = None
+
+
+class SearchScoreThreshold(VectorThreshold):
+    """The results of the vector query will filter based on the '@search.score' value. Note this is
+    the @search.score returned as part of the search response. The threshold direction will be
+    chosen for higher @search.score.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar kind: The kind of threshold used to filter vector queries. Required. Known values are:
+     "vectorSimilarity" and "searchScore".
+    :vartype kind: str or ~azure.search.documents.models.VectorThresholdKind
+    :ivar value: The threshold will filter based on the '@search.score' value. Note this is the
+     @search.score returned as part of the search response. The threshold direction will be chosen
+     for higher @search.score. Required.
+    :vartype value: float
+    """
+
+    _validation = {
+        "kind": {"required": True},
+        "value": {"required": True},
+    }
+
+    _attribute_map = {
+        "kind": {"key": "kind", "type": "str"},
+        "value": {"key": "value", "type": "float"},
+    }
+
+    def __init__(self, *, value: float, **kwargs: Any) -> None:
+        """
+        :keyword value: The threshold will filter based on the '@search.score' value. Note this is the
+         @search.score returned as part of the search response. The threshold direction will be chosen
+         for higher @search.score. Required.
+        :paramtype value: float
+        """
+        super().__init__(**kwargs)
+        self.kind: str = "searchScore"
+        self.value = value
+
+
 class SemanticDebugInfo(_serialization.Model):
     """SemanticDebugInfo.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar title_field: The title field that was sent to the semantic enrichment process, as well as
      how it was used.
@@ -1970,20 +2097,20 @@
         self.text = None
 
 
 class VectorQuery(_serialization.Model):
     """The query parameters for vector and hybrid search queries.
 
     You probably want to use the sub-classes and not this class directly. Known sub-classes are:
-    VectorizableTextQuery, VectorizedQuery
+    VectorizableImageBinaryQuery, VectorizableImageUrlQuery, VectorizableTextQuery, VectorizedQuery
 
     All required parameters must be populated in order to send to server.
 
-    :ivar kind: The kind of vector query being performed. Required. Known values are: "vector" and
-     "text".
+    :ivar kind: The kind of vector query being performed. Required. Known values are: "vector",
+     "text", "imageUrl", and "imageBinary".
     :vartype kind: str or ~azure.search.documents.models.VectorQueryKind
     :ivar k_nearest_neighbors: Number of nearest neighbors to return as top hits.
     :vartype k_nearest_neighbors: int
     :ivar fields: Vector Fields of type Collection(Edm.Single) to be included in the vector
      searched.
     :vartype fields: str
     :ivar exhaustive: When true, triggers an exhaustive k-nearest neighbor search across all
@@ -1991,37 +2118,58 @@
      determining ground truth values.
     :vartype exhaustive: bool
     :ivar oversampling: Oversampling factor. Minimum value is 1. It overrides the
      'defaultOversampling' parameter configured in the index definition. It can be set only when
      'rerankWithOriginalVectors' is true. This parameter is only permitted when a compression method
      is used on the underlying vector field.
     :vartype oversampling: float
+    :ivar weight: Relative weight of the vector query when compared to other vector query and/or
+     the text query within the same search request. This value is used when combining the results of
+     multiple ranking lists produced by the different vector queries and/or the results retrieved
+     through the text query. The higher the weight, the higher the documents that matched that query
+     will be in the final ranking. Default is 1.0 and the value needs to be a positive number larger
+     than zero.
+    :vartype weight: float
+    :ivar threshold: The threshold used for vector queries. Note this can only be set if all
+     'fields' use the same similarity metric.
+    :vartype threshold: ~azure.search.documents.models.VectorThreshold
     """
 
     _validation = {
         "kind": {"required": True},
     }
 
     _attribute_map = {
         "kind": {"key": "kind", "type": "str"},
         "k_nearest_neighbors": {"key": "k", "type": "int"},
         "fields": {"key": "fields", "type": "str"},
         "exhaustive": {"key": "exhaustive", "type": "bool"},
         "oversampling": {"key": "oversampling", "type": "float"},
+        "weight": {"key": "weight", "type": "float"},
+        "threshold": {"key": "threshold", "type": "VectorThreshold"},
     }
 
-    _subtype_map = {"kind": {"text": "VectorizableTextQuery", "vector": "VectorizedQuery"}}
+    _subtype_map = {
+        "kind": {
+            "imageBinary": "VectorizableImageBinaryQuery",
+            "imageUrl": "VectorizableImageUrlQuery",
+            "text": "VectorizableTextQuery",
+            "vector": "VectorizedQuery",
+        }
+    }
 
     def __init__(
         self,
         *,
         k_nearest_neighbors: Optional[int] = None,
         fields: Optional[str] = None,
         exhaustive: Optional[bool] = None,
         oversampling: Optional[float] = None,
+        weight: Optional[float] = None,
+        threshold: Optional["_models.VectorThreshold"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword k_nearest_neighbors: Number of nearest neighbors to return as top hits.
         :paramtype k_nearest_neighbors: int
         :keyword fields: Vector Fields of type Collection(Edm.Single) to be included in the vector
          searched.
@@ -2031,31 +2179,255 @@
          determining ground truth values.
         :paramtype exhaustive: bool
         :keyword oversampling: Oversampling factor. Minimum value is 1. It overrides the
          'defaultOversampling' parameter configured in the index definition. It can be set only when
          'rerankWithOriginalVectors' is true. This parameter is only permitted when a compression method
          is used on the underlying vector field.
         :paramtype oversampling: float
+        :keyword weight: Relative weight of the vector query when compared to other vector query and/or
+         the text query within the same search request. This value is used when combining the results of
+         multiple ranking lists produced by the different vector queries and/or the results retrieved
+         through the text query. The higher the weight, the higher the documents that matched that query
+         will be in the final ranking. Default is 1.0 and the value needs to be a positive number larger
+         than zero.
+        :paramtype weight: float
+        :keyword threshold: The threshold used for vector queries. Note this can only be set if all
+         'fields' use the same similarity metric.
+        :paramtype threshold: ~azure.search.documents.models.VectorThreshold
         """
         super().__init__(**kwargs)
         self.kind: Optional[str] = None
         self.k_nearest_neighbors = k_nearest_neighbors
         self.fields = fields
         self.exhaustive = exhaustive
         self.oversampling = oversampling
+        self.weight = weight
+        self.threshold = threshold
+
+
+class VectorizableImageBinaryQuery(VectorQuery):
+    """The query parameters to use for vector search when a base 64 encoded binary of an image that
+    needs to be vectorized is provided.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar kind: The kind of vector query being performed. Required. Known values are: "vector",
+     "text", "imageUrl", and "imageBinary".
+    :vartype kind: str or ~azure.search.documents.models.VectorQueryKind
+    :ivar k_nearest_neighbors: Number of nearest neighbors to return as top hits.
+    :vartype k_nearest_neighbors: int
+    :ivar fields: Vector Fields of type Collection(Edm.Single) to be included in the vector
+     searched.
+    :vartype fields: str
+    :ivar exhaustive: When true, triggers an exhaustive k-nearest neighbor search across all
+     vectors within the vector index. Useful for scenarios where exact matches are critical, such as
+     determining ground truth values.
+    :vartype exhaustive: bool
+    :ivar oversampling: Oversampling factor. Minimum value is 1. It overrides the
+     'defaultOversampling' parameter configured in the index definition. It can be set only when
+     'rerankWithOriginalVectors' is true. This parameter is only permitted when a compression method
+     is used on the underlying vector field.
+    :vartype oversampling: float
+    :ivar weight: Relative weight of the vector query when compared to other vector query and/or
+     the text query within the same search request. This value is used when combining the results of
+     multiple ranking lists produced by the different vector queries and/or the results retrieved
+     through the text query. The higher the weight, the higher the documents that matched that query
+     will be in the final ranking. Default is 1.0 and the value needs to be a positive number larger
+     than zero.
+    :vartype weight: float
+    :ivar threshold: The threshold used for vector queries. Note this can only be set if all
+     'fields' use the same similarity metric.
+    :vartype threshold: ~azure.search.documents.models.VectorThreshold
+    :ivar base64_image: The base 64 encoded binary of an image to be vectorized to perform a vector
+     search query.
+    :vartype base64_image: str
+    """
+
+    _validation = {
+        "kind": {"required": True},
+    }
+
+    _attribute_map = {
+        "kind": {"key": "kind", "type": "str"},
+        "k_nearest_neighbors": {"key": "k", "type": "int"},
+        "fields": {"key": "fields", "type": "str"},
+        "exhaustive": {"key": "exhaustive", "type": "bool"},
+        "oversampling": {"key": "oversampling", "type": "float"},
+        "weight": {"key": "weight", "type": "float"},
+        "threshold": {"key": "threshold", "type": "VectorThreshold"},
+        "base64_image": {"key": "base64Image", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        k_nearest_neighbors: Optional[int] = None,
+        fields: Optional[str] = None,
+        exhaustive: Optional[bool] = None,
+        oversampling: Optional[float] = None,
+        weight: Optional[float] = None,
+        threshold: Optional["_models.VectorThreshold"] = None,
+        base64_image: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword k_nearest_neighbors: Number of nearest neighbors to return as top hits.
+        :paramtype k_nearest_neighbors: int
+        :keyword fields: Vector Fields of type Collection(Edm.Single) to be included in the vector
+         searched.
+        :paramtype fields: str
+        :keyword exhaustive: When true, triggers an exhaustive k-nearest neighbor search across all
+         vectors within the vector index. Useful for scenarios where exact matches are critical, such as
+         determining ground truth values.
+        :paramtype exhaustive: bool
+        :keyword oversampling: Oversampling factor. Minimum value is 1. It overrides the
+         'defaultOversampling' parameter configured in the index definition. It can be set only when
+         'rerankWithOriginalVectors' is true. This parameter is only permitted when a compression method
+         is used on the underlying vector field.
+        :paramtype oversampling: float
+        :keyword weight: Relative weight of the vector query when compared to other vector query and/or
+         the text query within the same search request. This value is used when combining the results of
+         multiple ranking lists produced by the different vector queries and/or the results retrieved
+         through the text query. The higher the weight, the higher the documents that matched that query
+         will be in the final ranking. Default is 1.0 and the value needs to be a positive number larger
+         than zero.
+        :paramtype weight: float
+        :keyword threshold: The threshold used for vector queries. Note this can only be set if all
+         'fields' use the same similarity metric.
+        :paramtype threshold: ~azure.search.documents.models.VectorThreshold
+        :keyword base64_image: The base 64 encoded binary of an image to be vectorized to perform a
+         vector search query.
+        :paramtype base64_image: str
+        """
+        super().__init__(
+            k_nearest_neighbors=k_nearest_neighbors,
+            fields=fields,
+            exhaustive=exhaustive,
+            oversampling=oversampling,
+            weight=weight,
+            threshold=threshold,
+            **kwargs
+        )
+        self.kind: str = "imageBinary"
+        self.base64_image = base64_image
+
+
+class VectorizableImageUrlQuery(VectorQuery):
+    """The query parameters to use for vector search when an url that represents an image value that
+    needs to be vectorized is provided.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar kind: The kind of vector query being performed. Required. Known values are: "vector",
+     "text", "imageUrl", and "imageBinary".
+    :vartype kind: str or ~azure.search.documents.models.VectorQueryKind
+    :ivar k_nearest_neighbors: Number of nearest neighbors to return as top hits.
+    :vartype k_nearest_neighbors: int
+    :ivar fields: Vector Fields of type Collection(Edm.Single) to be included in the vector
+     searched.
+    :vartype fields: str
+    :ivar exhaustive: When true, triggers an exhaustive k-nearest neighbor search across all
+     vectors within the vector index. Useful for scenarios where exact matches are critical, such as
+     determining ground truth values.
+    :vartype exhaustive: bool
+    :ivar oversampling: Oversampling factor. Minimum value is 1. It overrides the
+     'defaultOversampling' parameter configured in the index definition. It can be set only when
+     'rerankWithOriginalVectors' is true. This parameter is only permitted when a compression method
+     is used on the underlying vector field.
+    :vartype oversampling: float
+    :ivar weight: Relative weight of the vector query when compared to other vector query and/or
+     the text query within the same search request. This value is used when combining the results of
+     multiple ranking lists produced by the different vector queries and/or the results retrieved
+     through the text query. The higher the weight, the higher the documents that matched that query
+     will be in the final ranking. Default is 1.0 and the value needs to be a positive number larger
+     than zero.
+    :vartype weight: float
+    :ivar threshold: The threshold used for vector queries. Note this can only be set if all
+     'fields' use the same similarity metric.
+    :vartype threshold: ~azure.search.documents.models.VectorThreshold
+    :ivar url: The URL of an image to be vectorized to perform a vector search query.
+    :vartype url: str
+    """
+
+    _validation = {
+        "kind": {"required": True},
+    }
+
+    _attribute_map = {
+        "kind": {"key": "kind", "type": "str"},
+        "k_nearest_neighbors": {"key": "k", "type": "int"},
+        "fields": {"key": "fields", "type": "str"},
+        "exhaustive": {"key": "exhaustive", "type": "bool"},
+        "oversampling": {"key": "oversampling", "type": "float"},
+        "weight": {"key": "weight", "type": "float"},
+        "threshold": {"key": "threshold", "type": "VectorThreshold"},
+        "url": {"key": "url", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        k_nearest_neighbors: Optional[int] = None,
+        fields: Optional[str] = None,
+        exhaustive: Optional[bool] = None,
+        oversampling: Optional[float] = None,
+        weight: Optional[float] = None,
+        threshold: Optional["_models.VectorThreshold"] = None,
+        url: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword k_nearest_neighbors: Number of nearest neighbors to return as top hits.
+        :paramtype k_nearest_neighbors: int
+        :keyword fields: Vector Fields of type Collection(Edm.Single) to be included in the vector
+         searched.
+        :paramtype fields: str
+        :keyword exhaustive: When true, triggers an exhaustive k-nearest neighbor search across all
+         vectors within the vector index. Useful for scenarios where exact matches are critical, such as
+         determining ground truth values.
+        :paramtype exhaustive: bool
+        :keyword oversampling: Oversampling factor. Minimum value is 1. It overrides the
+         'defaultOversampling' parameter configured in the index definition. It can be set only when
+         'rerankWithOriginalVectors' is true. This parameter is only permitted when a compression method
+         is used on the underlying vector field.
+        :paramtype oversampling: float
+        :keyword weight: Relative weight of the vector query when compared to other vector query and/or
+         the text query within the same search request. This value is used when combining the results of
+         multiple ranking lists produced by the different vector queries and/or the results retrieved
+         through the text query. The higher the weight, the higher the documents that matched that query
+         will be in the final ranking. Default is 1.0 and the value needs to be a positive number larger
+         than zero.
+        :paramtype weight: float
+        :keyword threshold: The threshold used for vector queries. Note this can only be set if all
+         'fields' use the same similarity metric.
+        :paramtype threshold: ~azure.search.documents.models.VectorThreshold
+        :keyword url: The URL of an image to be vectorized to perform a vector search query.
+        :paramtype url: str
+        """
+        super().__init__(
+            k_nearest_neighbors=k_nearest_neighbors,
+            fields=fields,
+            exhaustive=exhaustive,
+            oversampling=oversampling,
+            weight=weight,
+            threshold=threshold,
+            **kwargs
+        )
+        self.kind: str = "imageUrl"
+        self.url = url
 
 
 class VectorizableTextQuery(VectorQuery):
     """The query parameters to use for vector search when a text value that needs to be vectorized is
     provided.
 
     All required parameters must be populated in order to send to server.
 
-    :ivar kind: The kind of vector query being performed. Required. Known values are: "vector" and
-     "text".
+    :ivar kind: The kind of vector query being performed. Required. Known values are: "vector",
+     "text", "imageUrl", and "imageBinary".
     :vartype kind: str or ~azure.search.documents.models.VectorQueryKind
     :ivar k_nearest_neighbors: Number of nearest neighbors to return as top hits.
     :vartype k_nearest_neighbors: int
     :ivar fields: Vector Fields of type Collection(Edm.Single) to be included in the vector
      searched.
     :vartype fields: str
     :ivar exhaustive: When true, triggers an exhaustive k-nearest neighbor search across all
@@ -2063,14 +2435,24 @@
      determining ground truth values.
     :vartype exhaustive: bool
     :ivar oversampling: Oversampling factor. Minimum value is 1. It overrides the
      'defaultOversampling' parameter configured in the index definition. It can be set only when
      'rerankWithOriginalVectors' is true. This parameter is only permitted when a compression method
      is used on the underlying vector field.
     :vartype oversampling: float
+    :ivar weight: Relative weight of the vector query when compared to other vector query and/or
+     the text query within the same search request. This value is used when combining the results of
+     multiple ranking lists produced by the different vector queries and/or the results retrieved
+     through the text query. The higher the weight, the higher the documents that matched that query
+     will be in the final ranking. Default is 1.0 and the value needs to be a positive number larger
+     than zero.
+    :vartype weight: float
+    :ivar threshold: The threshold used for vector queries. Note this can only be set if all
+     'fields' use the same similarity metric.
+    :vartype threshold: ~azure.search.documents.models.VectorThreshold
     :ivar text: The text to be vectorized to perform a vector search query. Required.
     :vartype text: str
     """
 
     _validation = {
         "kind": {"required": True},
         "text": {"required": True},
@@ -2078,25 +2460,29 @@
 
     _attribute_map = {
         "kind": {"key": "kind", "type": "str"},
         "k_nearest_neighbors": {"key": "k", "type": "int"},
         "fields": {"key": "fields", "type": "str"},
         "exhaustive": {"key": "exhaustive", "type": "bool"},
         "oversampling": {"key": "oversampling", "type": "float"},
+        "weight": {"key": "weight", "type": "float"},
+        "threshold": {"key": "threshold", "type": "VectorThreshold"},
         "text": {"key": "text", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         text: str,
         k_nearest_neighbors: Optional[int] = None,
         fields: Optional[str] = None,
         exhaustive: Optional[bool] = None,
         oversampling: Optional[float] = None,
+        weight: Optional[float] = None,
+        threshold: Optional["_models.VectorThreshold"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword k_nearest_neighbors: Number of nearest neighbors to return as top hits.
         :paramtype k_nearest_neighbors: int
         :keyword fields: Vector Fields of type Collection(Edm.Single) to be included in the vector
          searched.
@@ -2106,35 +2492,47 @@
          determining ground truth values.
         :paramtype exhaustive: bool
         :keyword oversampling: Oversampling factor. Minimum value is 1. It overrides the
          'defaultOversampling' parameter configured in the index definition. It can be set only when
          'rerankWithOriginalVectors' is true. This parameter is only permitted when a compression method
          is used on the underlying vector field.
         :paramtype oversampling: float
+        :keyword weight: Relative weight of the vector query when compared to other vector query and/or
+         the text query within the same search request. This value is used when combining the results of
+         multiple ranking lists produced by the different vector queries and/or the results retrieved
+         through the text query. The higher the weight, the higher the documents that matched that query
+         will be in the final ranking. Default is 1.0 and the value needs to be a positive number larger
+         than zero.
+        :paramtype weight: float
+        :keyword threshold: The threshold used for vector queries. Note this can only be set if all
+         'fields' use the same similarity metric.
+        :paramtype threshold: ~azure.search.documents.models.VectorThreshold
         :keyword text: The text to be vectorized to perform a vector search query. Required.
         :paramtype text: str
         """
         super().__init__(
             k_nearest_neighbors=k_nearest_neighbors,
             fields=fields,
             exhaustive=exhaustive,
             oversampling=oversampling,
+            weight=weight,
+            threshold=threshold,
             **kwargs
         )
         self.kind: str = "text"
         self.text = text
 
 
 class VectorizedQuery(VectorQuery):
     """The query parameters to use for vector search when a raw vector value is provided.
 
     All required parameters must be populated in order to send to server.
 
-    :ivar kind: The kind of vector query being performed. Required. Known values are: "vector" and
-     "text".
+    :ivar kind: The kind of vector query being performed. Required. Known values are: "vector",
+     "text", "imageUrl", and "imageBinary".
     :vartype kind: str or ~azure.search.documents.models.VectorQueryKind
     :ivar k_nearest_neighbors: Number of nearest neighbors to return as top hits.
     :vartype k_nearest_neighbors: int
     :ivar fields: Vector Fields of type Collection(Edm.Single) to be included in the vector
      searched.
     :vartype fields: str
     :ivar exhaustive: When true, triggers an exhaustive k-nearest neighbor search across all
@@ -2142,14 +2540,24 @@
      determining ground truth values.
     :vartype exhaustive: bool
     :ivar oversampling: Oversampling factor. Minimum value is 1. It overrides the
      'defaultOversampling' parameter configured in the index definition. It can be set only when
      'rerankWithOriginalVectors' is true. This parameter is only permitted when a compression method
      is used on the underlying vector field.
     :vartype oversampling: float
+    :ivar weight: Relative weight of the vector query when compared to other vector query and/or
+     the text query within the same search request. This value is used when combining the results of
+     multiple ranking lists produced by the different vector queries and/or the results retrieved
+     through the text query. The higher the weight, the higher the documents that matched that query
+     will be in the final ranking. Default is 1.0 and the value needs to be a positive number larger
+     than zero.
+    :vartype weight: float
+    :ivar threshold: The threshold used for vector queries. Note this can only be set if all
+     'fields' use the same similarity metric.
+    :vartype threshold: ~azure.search.documents.models.VectorThreshold
     :ivar vector: The vector representation of a search query. Required.
     :vartype vector: list[float]
     """
 
     _validation = {
         "kind": {"required": True},
         "vector": {"required": True},
@@ -2157,25 +2565,29 @@
 
     _attribute_map = {
         "kind": {"key": "kind", "type": "str"},
         "k_nearest_neighbors": {"key": "k", "type": "int"},
         "fields": {"key": "fields", "type": "str"},
         "exhaustive": {"key": "exhaustive", "type": "bool"},
         "oversampling": {"key": "oversampling", "type": "float"},
+        "weight": {"key": "weight", "type": "float"},
+        "threshold": {"key": "threshold", "type": "VectorThreshold"},
         "vector": {"key": "vector", "type": "[float]"},
     }
 
     def __init__(
         self,
         *,
         vector: List[float],
         k_nearest_neighbors: Optional[int] = None,
         fields: Optional[str] = None,
         exhaustive: Optional[bool] = None,
         oversampling: Optional[float] = None,
+        weight: Optional[float] = None,
+        threshold: Optional["_models.VectorThreshold"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword k_nearest_neighbors: Number of nearest neighbors to return as top hits.
         :paramtype k_nearest_neighbors: int
         :keyword fields: Vector Fields of type Collection(Edm.Single) to be included in the vector
          searched.
@@ -2185,19 +2597,72 @@
          determining ground truth values.
         :paramtype exhaustive: bool
         :keyword oversampling: Oversampling factor. Minimum value is 1. It overrides the
          'defaultOversampling' parameter configured in the index definition. It can be set only when
          'rerankWithOriginalVectors' is true. This parameter is only permitted when a compression method
          is used on the underlying vector field.
         :paramtype oversampling: float
+        :keyword weight: Relative weight of the vector query when compared to other vector query and/or
+         the text query within the same search request. This value is used when combining the results of
+         multiple ranking lists produced by the different vector queries and/or the results retrieved
+         through the text query. The higher the weight, the higher the documents that matched that query
+         will be in the final ranking. Default is 1.0 and the value needs to be a positive number larger
+         than zero.
+        :paramtype weight: float
+        :keyword threshold: The threshold used for vector queries. Note this can only be set if all
+         'fields' use the same similarity metric.
+        :paramtype threshold: ~azure.search.documents.models.VectorThreshold
         :keyword vector: The vector representation of a search query. Required.
         :paramtype vector: list[float]
         """
         super().__init__(
             k_nearest_neighbors=k_nearest_neighbors,
             fields=fields,
             exhaustive=exhaustive,
             oversampling=oversampling,
+            weight=weight,
+            threshold=threshold,
             **kwargs
         )
         self.kind: str = "vector"
         self.vector = vector
+
+
+class VectorSimilarityThreshold(VectorThreshold):
+    """The results of the vector query will be filtered based on the vector similarity metric. Note
+    this is the canonical definition of similarity metric, not the 'distance' version. The
+    threshold direction (larger or smaller) will be chosen automatically according to the metric
+    used by the field.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar kind: The kind of threshold used to filter vector queries. Required. Known values are:
+     "vectorSimilarity" and "searchScore".
+    :vartype kind: str or ~azure.search.documents.models.VectorThresholdKind
+    :ivar value: The threshold will filter based on the similarity metric value. Note this is the
+     canonical definition of similarity metric, not the 'distance' version. The threshold direction
+     (larger or smaller) will be chosen automatically according to the metric used by the field.
+     Required.
+    :vartype value: float
+    """
+
+    _validation = {
+        "kind": {"required": True},
+        "value": {"required": True},
+    }
+
+    _attribute_map = {
+        "kind": {"key": "kind", "type": "str"},
+        "value": {"key": "value", "type": "float"},
+    }
+
+    def __init__(self, *, value: float, **kwargs: Any) -> None:
+        """
+        :keyword value: The threshold will filter based on the similarity metric value. Note this is
+         the canonical definition of similarity metric, not the 'distance' version. The threshold
+         direction (larger or smaller) will be chosen automatically according to the metric used by the
+         field. Required.
+        :paramtype value: float
+        """
+        super().__init__(**kwargs)
+        self.kind: str = "vectorSimilarity"
+        self.value = value
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/_patch.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/_search_index_client_enums.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/models/_search_index_client_enums.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
 
 
@@ -22,14 +22,29 @@
     the suggested terms could include 'medicare coverage' and 'medical assistant'."""
     ONE_TERM_WITH_CONTEXT = "oneTermWithContext"
     """Completes the last term in a query with two or more terms, where the last two terms are a
     phrase that exists in the index. For example, if the input is 'washington medic', the suggested
     terms could include 'washington medicaid' and 'washington medical'."""
 
 
+class HybridCountAndFacetMode(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Determines whether the count and facets should includes all documents that matched the search
+    query, or only the documents that are retrieved within the 'maxTextRecallSize' window. The
+    default value is 'countAllResults'.
+    """
+
+    COUNT_RETRIEVABLE_RESULTS = "countRetrievableResults"
+    """Only include documents that were matched within the 'maxTextRecallSize' retrieval window when
+    computing 'count' and 'facets'."""
+    COUNT_ALL_RESULTS = "countAllResults"
+    """Include all documents that were matched by the search query when computing 'count' and
+    'facets', regardless of whether or not those documents are within the 'maxTextRecallSize'
+    retrieval window."""
+
+
 class IndexActionType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The operation to perform on a document in an indexing batch."""
 
     UPLOAD = "upload"
     """Inserts the document into the index if it is new and updates it if it exists. All fields are
     replaced in the update case."""
     MERGE = "merge"
@@ -358,7 +373,27 @@
 class VectorQueryKind(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The kind of vector query being performed."""
 
     VECTOR = "vector"
     """Vector query where a raw vector value is provided."""
     TEXT = "text"
     """Vector query where a text value that needs to be vectorized is provided."""
+    IMAGE_URL = "imageUrl"
+    """Vector query where an url that represents an image value that needs to be vectorized is
+    provided."""
+    IMAGE_BINARY = "imageBinary"
+    """Vector query where a base 64 encoded binary of an image that needs to be vectorized is
+    provided."""
+
+
+class VectorThresholdKind(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The kind of vector query being performed."""
+
+    VECTOR_SIMILARITY = "vectorSimilarity"
+    """The results of the vector query will be filtered based on the vector similarity metric. Note
+    this is the canonical definition of similarity metric, not the 'distance' version. The
+    threshold direction (larger or smaller) will be chosen automatically according to the metric
+    used by the field."""
+    SEARCH_SCORE = "searchScore"
+    """The results of the vector query will filter based on the '@search.score' value. Note this is
+    the @search.score returned as part of the search response. The threshold direction will be
+    chosen for higher @search.score."""
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._documents_operations import DocumentsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/_documents_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/operations/_documents_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, List, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -21,26 +22,30 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_count_request(*, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/docs/$count")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -63,38 +68,38 @@
     highlight_post_tag: Optional[str] = None,
     highlight_pre_tag: Optional[str] = None,
     minimum_coverage: Optional[float] = None,
     order_by: Optional[List[str]] = None,
     query_type: Optional[Union[str, _models.QueryType]] = None,
     scoring_parameters: Optional[List[str]] = None,
     scoring_profile: Optional[str] = None,
-    semantic_query: Optional[str] = None,
-    semantic_configuration: Optional[str] = None,
-    semantic_error_handling: Optional[Union[str, _models.SemanticErrorMode]] = None,
-    semantic_max_wait_in_milliseconds: Optional[int] = None,
-    debug: Optional[Union[str, _models.QueryDebugMode]] = None,
     search_fields: Optional[List[str]] = None,
-    query_language: Optional[Union[str, _models.QueryLanguage]] = None,
-    speller: Optional[Union[str, _models.Speller]] = None,
-    answers: Optional[Union[str, _models.QueryAnswerType]] = None,
     search_mode: Optional[Union[str, _models.SearchMode]] = None,
     scoring_statistics: Optional[Union[str, _models.ScoringStatistics]] = None,
     session_id: Optional[str] = None,
     select: Optional[List[str]] = None,
     skip: Optional[int] = None,
     top: Optional[int] = None,
+    x_ms_client_request_id: Optional[str] = None,
+    semantic_configuration: Optional[str] = None,
+    semantic_error_handling: Optional[Union[str, _models.SemanticErrorMode]] = None,
+    semantic_max_wait_in_milliseconds: Optional[int] = None,
+    answers: Optional[Union[str, _models.QueryAnswerType]] = None,
     captions: Optional[Union[str, _models.QueryCaptionType]] = None,
+    semantic_query: Optional[str] = None,
+    debug: Optional[Union[str, _models.QueryDebugMode]] = None,
+    query_language: Optional[Union[str, _models.QueryLanguage]] = None,
+    speller: Optional[Union[str, _models.Speller]] = None,
     semantic_fields: Optional[List[str]] = None,
-    x_ms_client_request_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/docs")
 
     # Construct parameters
     if search_text is not None:
@@ -119,65 +124,65 @@
         _params["queryType"] = _SERIALIZER.query("query_type", query_type, "str")
     if scoring_parameters is not None:
         _params["scoringParameter"] = [
             _SERIALIZER.query("scoring_parameters", q, "str") if q is not None else "" for q in scoring_parameters
         ]
     if scoring_profile is not None:
         _params["scoringProfile"] = _SERIALIZER.query("scoring_profile", scoring_profile, "str")
-    if semantic_query is not None:
-        _params["semanticQuery"] = _SERIALIZER.query("semantic_query", semantic_query, "str")
-    if semantic_configuration is not None:
-        _params["semanticConfiguration"] = _SERIALIZER.query("semantic_configuration", semantic_configuration, "str")
-    if semantic_error_handling is not None:
-        _params["semanticErrorHandling"] = _SERIALIZER.query("semantic_error_handling", semantic_error_handling, "str")
-    if semantic_max_wait_in_milliseconds is not None:
-        _params["semanticMaxWaitInMilliseconds"] = _SERIALIZER.query(
-            "semantic_max_wait_in_milliseconds", semantic_max_wait_in_milliseconds, "int", minimum=700
-        )
-    if debug is not None:
-        _params["debug"] = _SERIALIZER.query("debug", debug, "str")
     if search_fields is not None:
         _params["searchFields"] = _SERIALIZER.query("search_fields", search_fields, "[str]", div=",")
-    if query_language is not None:
-        _params["queryLanguage"] = _SERIALIZER.query("query_language", query_language, "str")
-    if speller is not None:
-        _params["speller"] = _SERIALIZER.query("speller", speller, "str")
-    if answers is not None:
-        _params["answers"] = _SERIALIZER.query("answers", answers, "str")
     if search_mode is not None:
         _params["searchMode"] = _SERIALIZER.query("search_mode", search_mode, "str")
     if scoring_statistics is not None:
         _params["scoringStatistics"] = _SERIALIZER.query("scoring_statistics", scoring_statistics, "str")
     if session_id is not None:
         _params["sessionId"] = _SERIALIZER.query("session_id", session_id, "str")
     if select is not None:
         _params["$select"] = _SERIALIZER.query("select", select, "[str]", div=",")
     if skip is not None:
         _params["$skip"] = _SERIALIZER.query("skip", skip, "int")
     if top is not None:
         _params["$top"] = _SERIALIZER.query("top", top, "int")
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+    if semantic_configuration is not None:
+        _params["semanticConfiguration"] = _SERIALIZER.query("semantic_configuration", semantic_configuration, "str")
+    if semantic_error_handling is not None:
+        _params["semanticErrorHandling"] = _SERIALIZER.query("semantic_error_handling", semantic_error_handling, "str")
+    if semantic_max_wait_in_milliseconds is not None:
+        _params["semanticMaxWaitInMilliseconds"] = _SERIALIZER.query(
+            "semantic_max_wait_in_milliseconds", semantic_max_wait_in_milliseconds, "int", minimum=700
+        )
+    if answers is not None:
+        _params["answers"] = _SERIALIZER.query("answers", answers, "str")
     if captions is not None:
         _params["captions"] = _SERIALIZER.query("captions", captions, "str")
+    if semantic_query is not None:
+        _params["semanticQuery"] = _SERIALIZER.query("semantic_query", semantic_query, "str")
+    if debug is not None:
+        _params["debug"] = _SERIALIZER.query("debug", debug, "str")
+    if query_language is not None:
+        _params["queryLanguage"] = _SERIALIZER.query("query_language", query_language, "str")
+    if speller is not None:
+        _params["speller"] = _SERIALIZER.query("speller", speller, "str")
     if semantic_fields is not None:
         _params["semanticFields"] = _SERIALIZER.query("semantic_fields", semantic_fields, "[str]", div=",")
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_search_post_request(*, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/docs/search.post.search")
 
     # Construct parameters
@@ -199,15 +204,15 @@
     selected_fields: Optional[List[str]] = None,
     x_ms_client_request_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/docs('{key}')")
     path_format_arguments = {
         "key": _SERIALIZER.url("key", key, "str"),
     }
@@ -242,15 +247,15 @@
     top: Optional[int] = None,
     x_ms_client_request_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/docs/search.suggest")
 
     # Construct parameters
     _params["search"] = _SERIALIZER.query("search_text", search_text, "str")
@@ -283,15 +288,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_suggest_post_request(*, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/docs/search.post.suggest")
 
     # Construct parameters
@@ -307,15 +312,15 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_index_request(*, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/docs/search.index")
 
     # Construct parameters
@@ -345,15 +350,15 @@
     search_fields: Optional[List[str]] = None,
     top: Optional[int] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/docs/search.autocomplete")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -384,15 +389,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_autocomplete_post_request(*, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/docs/search.post.autocomplete")
 
     # Construct parameters
@@ -436,15 +441,15 @@
 
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: int or the result of cls(response)
         :rtype: int
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -510,15 +515,15 @@
         :type search_options: ~azure.search.documents.models.SearchOptions
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: SearchDocumentsResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.SearchDocumentsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -535,32 +540,32 @@
         _highlight_post_tag = None
         _highlight_pre_tag = None
         _minimum_coverage = None
         _order_by = None
         _query_type = None
         _scoring_parameters = None
         _scoring_profile = None
-        _semantic_query = None
-        _semantic_configuration = None
-        _semantic_error_handling = None
-        _semantic_max_wait_in_milliseconds = None
-        _debug = None
         _search_fields = None
-        _query_language = None
-        _speller = None
-        _answers = None
         _search_mode = None
         _scoring_statistics = None
         _session_id = None
         _select = None
         _skip = None
         _top = None
+        _x_ms_client_request_id = None
+        _semantic_configuration = None
+        _semantic_error_handling = None
+        _semantic_max_wait_in_milliseconds = None
+        _answers = None
         _captions = None
+        _semantic_query = None
+        _debug = None
+        _query_language = None
+        _speller = None
         _semantic_fields = None
-        _x_ms_client_request_id = None
         if search_options is not None:
             _answers = search_options.answers
             _captions = search_options.captions
             _debug = search_options.debug
             _facets = search_options.facets
             _filter = search_options.filter
             _highlight_fields = search_options.highlight_fields
@@ -598,32 +603,32 @@
             highlight_post_tag=_highlight_post_tag,
             highlight_pre_tag=_highlight_pre_tag,
             minimum_coverage=_minimum_coverage,
             order_by=_order_by,
             query_type=_query_type,
             scoring_parameters=_scoring_parameters,
             scoring_profile=_scoring_profile,
-            semantic_query=_semantic_query,
-            semantic_configuration=_semantic_configuration,
-            semantic_error_handling=_semantic_error_handling,
-            semantic_max_wait_in_milliseconds=_semantic_max_wait_in_milliseconds,
-            debug=_debug,
             search_fields=_search_fields,
-            query_language=_query_language,
-            speller=_speller,
-            answers=_answers,
             search_mode=_search_mode,
             scoring_statistics=_scoring_statistics,
             session_id=_session_id,
             select=_select,
             skip=_skip,
             top=_top,
+            x_ms_client_request_id=_x_ms_client_request_id,
+            semantic_configuration=_semantic_configuration,
+            semantic_error_handling=_semantic_error_handling,
+            semantic_max_wait_in_milliseconds=_semantic_max_wait_in_milliseconds,
+            answers=_answers,
             captions=_captions,
+            semantic_query=_semantic_query,
+            debug=_debug,
+            query_language=_query_language,
+            speller=_speller,
             semantic_fields=_semantic_fields,
-            x_ms_client_request_id=_x_ms_client_request_id,
             api_version=api_version,
             headers=_headers,
             params=_params,
         )
         _request = _convert_request(_request)
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
@@ -719,15 +724,15 @@
         :type search_request: ~azure.search.documents.models.SearchRequest or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: SearchDocumentsResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.SearchDocumentsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -804,15 +809,15 @@
         :type selected_fields: list[str]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: dict mapping str to any or the result of cls(response)
         :rtype: dict[str, any]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -884,15 +889,15 @@
         :type suggest_options: ~azure.search.documents.models.SuggestOptions
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: SuggestDocumentsResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.SuggestDocumentsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1037,15 +1042,15 @@
         :type suggest_request: ~azure.search.documents.models.SuggestRequest or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: SuggestDocumentsResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.SuggestDocumentsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1171,15 +1176,15 @@
         :type batch: ~azure.search.documents.models.IndexBatch or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: IndexDocumentsResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.IndexDocumentsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1263,15 +1268,15 @@
         :type request_options: ~azure.search.documents.models.RequestOptions
         :param autocomplete_options: Parameter group. Default value is None.
         :type autocomplete_options: ~azure.search.documents.models.AutocompleteOptions
         :return: AutocompleteResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.AutocompleteResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1413,15 +1418,15 @@
         :type autocomplete_request: ~azure.search.documents.models.AutocompleteRequest or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.models.RequestOptions
         :return: AutocompleteResult or the result of cls(response)
         :rtype: ~azure.search.documents.models.AutocompleteResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/_patch.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_headers_mixin.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_headers_mixin.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_index_documents_batch.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_index_documents_batch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_paging.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_paging.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_queries.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_queries.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_search_client.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_search_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,21 +24,22 @@
     SearchMode,
     ScoringStatistics,
     VectorFilterMode,
     VectorQuery,
     SemanticErrorMode,
     QueryDebugMode,
     SuggestRequest,
+    HybridSearch,
 )
 from ._search_documents_error import RequestEntityTooLargeError
 from ._index_documents_batch import IndexDocumentsBatch
 from ._paging import SearchItemPaged, SearchPageIterator
 from ._queries import AutocompleteQuery, SearchQuery, SuggestQuery
 from ._headers_mixin import HeadersMixin
-from ._utils import get_authentication_policy
+from ._utils import get_authentication_policy, get_answer_query
 from ._version import SDK_MONIKER
 
 
 class SearchClient(HeadersMixin):
     """A client to interact with an existing Azure search index.
 
     :param endpoint: The URL endpoint of an Azure search service
@@ -172,14 +173,15 @@
         scoring_statistics: Optional[Union[str, ScoringStatistics]] = None,
         session_id: Optional[str] = None,
         vector_queries: Optional[List[VectorQuery]] = None,
         vector_filter_mode: Optional[Union[str, VectorFilterMode]] = None,
         semantic_error_mode: Optional[Union[str, SemanticErrorMode]] = None,
         semantic_max_wait_in_milliseconds: Optional[int] = None,
         debug: Optional[Union[str, QueryDebugMode]] = None,
+        hybrid_search: Optional[HybridSearch] = None,
         **kwargs: Any
     ) -> SearchItemPaged[Dict]:
         # pylint:disable=too-many-locals, disable=redefined-builtin
         """Search the Azure search index for documents.
 
         :param str search_text: A full-text search query expression; Use "*" or omit this parameter to
             match all documents.
@@ -288,14 +290,16 @@
             results. Known values are: "disabled", "speller", "semantic", and "all".
         :paramtype debug: str or ~azure.search.documents.models.QueryDebugMode
         :keyword vector_queries: The query parameters for vector and hybrid search queries.
         :paramtype vector_queries: list[VectorQuery]
         :keyword vector_filter_mode: Determines whether or not filters are applied before or after the
              vector search is performed. Default is 'preFilter'. Known values are: "postFilter" and "preFilter".
         :paramtype vector_filter_mode: str or VectorFilterMode
+        :keyword hybrid_search: The query parameters to configure hybrid search behaviors.
+        :paramtype hybrid_search: ~azure.search.documents.models.HybridSearch
         :return: List of search results.
         :rtype:  SearchItemPaged[dict]
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/sample_simple_query.py
                 :start-after: [START simple_query]
@@ -322,16 +326,15 @@
                 :dedent: 4
                 :caption: Get search result facets.
         """
         include_total_result_count = include_total_count
         filter_arg = filter
         search_fields_str = ",".join(search_fields) if search_fields else None
 
-        answers = query_answer if not query_answer_count else "{}|count-{}".format(query_answer, query_answer_count)
-        answers = answers if not query_answer_threshold else "{}|threshold-{}".format(answers, query_answer_threshold)
+        answers = get_answer_query(query_answer, query_answer_count, query_answer_threshold)
 
         captions = (
             query_caption
             if not query_caption_highlight_enabled
             else "{}|highlight-{}".format(query_caption, query_caption_highlight_enabled)
         )
 
@@ -365,14 +368,15 @@
             session_id=session_id,
             scoring_statistics=scoring_statistics,
             vector_queries=vector_queries,
             vector_filter_mode=vector_filter_mode,
             semantic_error_handling=semantic_error_mode,
             semantic_max_wait_in_milliseconds=semantic_max_wait_in_milliseconds,
             debug=debug,
+            hybrid_search=hybrid_search,
         )
         if isinstance(select, list):
             query.select(select)
 
         if isinstance(order_by, list):
             query.order_by(order_by)
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_search_indexing_buffered_sender.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_search_indexing_buffered_sender.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_search_indexing_buffered_sender_base.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_search_indexing_buffered_sender_base.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/_utils.py` & `azure-search-documents-11.6.0b4/azure/search/documents/_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-from typing import Any, Optional
+from typing import Any, Optional, Union
 from azure.core.pipeline.policies import (
     BearerTokenCredentialPolicy,
     AsyncBearerTokenCredentialPolicy,
 )
+from ._generated.models import QueryAnswerType
 
 DEFAULT_AUDIENCE = "https://search.azure.com"
 
 
+def get_answer_query(
+    query_answer: Optional[Union[str, QueryAnswerType]] = None,
+    query_answer_count: Optional[int] = None,
+    query_answer_threshold: Optional[float] = None,
+) -> Optional[Union[str, QueryAnswerType]]:
+    answers = query_answer
+    separator = "|"
+    if query_answer_count:
+        answers = f"{answers}{separator}count-{query_answer_count}"
+        separator = ","
+    if query_answer_threshold:
+        answers = f"{answers}{separator}threshold-{query_answer_threshold}"
+    return answers
+
+
 def is_retryable_status_code(status_code: Optional[int]) -> bool:
     if not status_code:
         return False
     return status_code in [422, 409, 503]
 
 
 def get_authentication_policy(credential, *, is_async: bool = False, **kwargs):
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/aio/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/aio/_index_documents_batch_async.py` & `azure-search-documents-11.6.0b4/azure/search/documents/aio/_index_documents_batch_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/aio/_paging.py` & `azure-search-documents-11.6.0b4/azure/search/documents/aio/_paging.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/aio/_search_client_async.py` & `azure-search-documents-11.6.0b4/azure/search/documents/aio/_search_client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import cast, List, Union, Any, Optional, Dict
 
 from azure.core.rest import HttpRequest, AsyncHttpResponse
 from azure.core.credentials import AzureKeyCredential
 from azure.core.credentials_async import AsyncTokenCredential
 from azure.core.tracing.decorator_async import distributed_trace_async
 from ._paging import AsyncSearchItemPaged, AsyncSearchPageIterator
-from .._utils import get_authentication_policy
+from .._utils import get_authentication_policy, get_answer_query
 from .._generated.aio import SearchIndexClient
 from .._generated.models import (
     AutocompleteMode,
     AutocompleteRequest,
     IndexAction,
     IndexBatch,
     IndexingResult,
@@ -26,14 +26,15 @@
     SearchMode,
     ScoringStatistics,
     VectorFilterMode,
     VectorQuery,
     SemanticErrorMode,
     QueryDebugMode,
     SuggestRequest,
+    HybridSearch,
 )
 from .._search_documents_error import RequestEntityTooLargeError
 from .._index_documents_batch import IndexDocumentsBatch
 from .._queries import AutocompleteQuery, SearchQuery, SuggestQuery
 from .._api_versions import DEFAULT_VERSION
 from .._headers_mixin import HeadersMixin
 from .._version import SDK_MONIKER
@@ -174,14 +175,15 @@
         scoring_statistics: Optional[Union[str, ScoringStatistics]] = None,
         session_id: Optional[str] = None,
         vector_queries: Optional[List[VectorQuery]] = None,
         vector_filter_mode: Optional[Union[str, VectorFilterMode]] = None,
         semantic_error_mode: Optional[Union[str, SemanticErrorMode]] = None,
         semantic_max_wait_in_milliseconds: Optional[int] = None,
         debug: Optional[Union[str, QueryDebugMode]] = None,
+        hybrid_search: Optional[HybridSearch] = None,
         **kwargs
     ) -> AsyncSearchItemPaged[Dict]:
         # pylint:disable=too-many-locals, disable=redefined-builtin
         """Search the Azure search index for documents.
 
         :param str search_text: A full-text search query expression; Use "*" or omit this parameter to
             match all documents.
@@ -291,14 +293,16 @@
             results. Known values are: "disabled", "speller", "semantic", and "all".
         :paramtype debug: str or ~azure.search.documents.models.QueryDebugMode
         :keyword vector_queries: The query parameters for vector and hybrid search queries.
         :paramtype vector_queries: list[VectorQuery]
         :keyword vector_filter_mode: Determines whether or not filters are applied before or after the
              vector search is performed. Default is 'preFilter'. Known values are: "postFilter" and "preFilter".
         :paramtype vector_filter_mode: str or VectorFilterMode
+        :keyword hybrid_search: The query parameters to configure hybrid search behaviors.
+        :paramtype hybrid_search: ~azure.search.documents.models.HybridSearch
         :return: A list of documents (dicts) matching the specified search criteria.
         :return: List of search results.
         :rtype:  AsyncSearchItemPaged[dict]
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/async_samples/sample_simple_query_async.py
@@ -325,16 +329,15 @@
                 :language: python
                 :dedent: 4
                 :caption: Get search result facets.
         """
         include_total_result_count = include_total_count
         filter_arg = filter
         search_fields_str = ",".join(search_fields) if search_fields else None
-        answers = query_answer if not query_answer_count else "{}|count-{}".format(query_answer, query_answer_count)
-        answers = answers if not query_answer_threshold else "{}|threshold-{}".format(answers, query_answer_threshold)
+        answers = get_answer_query(query_answer, query_answer_count, query_answer_threshold)
         captions = (
             query_caption
             if not query_caption_highlight_enabled
             else "{}|highlight-{}".format(query_caption, query_caption_highlight_enabled)
         )
         semantic_configuration = semantic_configuration_name
 
@@ -366,14 +369,15 @@
             session_id=session_id,
             scoring_statistics=scoring_statistics,
             vector_queries=vector_queries,
             vector_filter_mode=vector_filter_mode,
             semantic_error_handling=semantic_error_mode,
             semantic_max_wait_in_milliseconds=semantic_max_wait_in_milliseconds,
             debug=debug,
+            hybrid_search=hybrid_search,
         )
         if isinstance(select, list):
             query.select(select)
         if isinstance(order_by, list):
             query.order_by(order_by)
         kwargs["headers"] = self._merge_client_headers(kwargs.get("headers"))
         kwargs["api_version"] = self._api_version
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/aio/_search_indexing_buffered_sender_async.py` & `azure-search-documents-11.6.0b4/azure/search/documents/aio/_search_indexing_buffered_sender_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/aio/_timer.py` & `azure-search-documents-11.6.0b4/azure/search/documents/aio/_timer.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._search_service_client import SearchServiceClient
 
 try:
     from ._patch import __all__ as _patch_all
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_configuration.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.pipeline import policies
 
@@ -15,21 +15,21 @@
     """Configuration for SearchServiceClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param endpoint: The endpoint URL of the search service. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2024-03-01-Preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2024-05-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, **kwargs: Any) -> None:
-        api_version: str = kwargs.pop("api_version", "2024-03-01-Preview")
+        api_version: str = kwargs.pop("api_version", "2024-05-01-preview")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
 
         self.endpoint = endpoint
         self.api_version = api_version
         kwargs.setdefault("sdk_moniker", "searchserviceclient/{}".format(VERSION))
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_patch.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_search_service_client.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/_search_service_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any
 
 from azure.core import PipelineClient
@@ -41,15 +41,15 @@
     :vartype synonym_maps: azure.search.documents.indexes.operations.SynonymMapsOperations
     :ivar indexes: IndexesOperations operations
     :vartype indexes: azure.search.documents.indexes.operations.IndexesOperations
     :ivar aliases: AliasesOperations operations
     :vartype aliases: azure.search.documents.indexes.operations.AliasesOperations
     :param endpoint: The endpoint URL of the search service. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2024-03-01-Preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2024-05-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, endpoint: str, **kwargs: Any
     ) -> None:
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_serialization.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_vendor.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/_vendor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from abc import ABC
 from typing import TYPE_CHECKING
 
 from azure.core.pipeline.transport import HttpRequest
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._search_service_client import SearchServiceClient
 
 try:
     from ._patch import __all__ as _patch_all
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_configuration.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.pipeline import policies
 
@@ -15,21 +15,21 @@
     """Configuration for SearchServiceClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param endpoint: The endpoint URL of the search service. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2024-03-01-Preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2024-05-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, **kwargs: Any) -> None:
-        api_version: str = kwargs.pop("api_version", "2024-03-01-Preview")
+        api_version: str = kwargs.pop("api_version", "2024-05-01-preview")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
 
         self.endpoint = endpoint
         self.api_version = api_version
         kwargs.setdefault("sdk_moniker", "searchserviceclient/{}".format(VERSION))
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_patch.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_search_service_client.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/_search_service_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable
 
 from azure.core import AsyncPipelineClient
@@ -41,15 +41,15 @@
     :vartype synonym_maps: azure.search.documents.indexes.aio.operations.SynonymMapsOperations
     :ivar indexes: IndexesOperations operations
     :vartype indexes: azure.search.documents.indexes.aio.operations.IndexesOperations
     :ivar aliases: AliasesOperations operations
     :vartype aliases: azure.search.documents.indexes.aio.operations.AliasesOperations
     :param endpoint: The endpoint URL of the search service. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2024-03-01-Preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2024-05-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, endpoint: str, **kwargs: Any
     ) -> None:
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_vendor.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/_vendor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from abc import ABC
 from typing import TYPE_CHECKING
 
 from azure.core.pipeline.transport import HttpRequest
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._data_sources_operations import DataSourcesOperations
 from ._indexers_operations import IndexersOperations
 from ._skillsets_operations import SkillsetsOperations
 from ._synonym_maps_operations import SynonymMapsOperations
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -31,14 +32,18 @@
     build_create_request,
     build_delete_request,
     build_get_request,
     build_list_request,
 )
 from .._vendor import SearchServiceClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class AliasesOperations:
     """
     .. warning::
@@ -127,15 +132,15 @@
         :type alias: ~azure.search.documents.indexes.models.SearchAlias or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchAlias or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchAlias
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -209,15 +214,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ListAliasesResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -403,15 +408,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchAlias or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchAlias
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -500,15 +505,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -565,15 +570,15 @@
         :type alias_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchAlias or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchAlias
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -28,14 +29,18 @@
     build_create_request,
     build_delete_request,
     build_get_request,
     build_list_request,
 )
 from .._vendor import SearchServiceClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class DataSourcesOperations:
     """
     .. warning::
@@ -181,15 +186,15 @@
         :type skip_indexer_reset_requirement_for_cache: bool
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerDataSource or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerDataSource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -278,15 +283,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -343,15 +348,15 @@
         :type data_source_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerDataSource or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerDataSource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -412,15 +417,15 @@
         :type select: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: ListDataSourcesResult or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.ListDataSourcesResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -535,15 +540,15 @@
         :type data_source: ~azure.search.documents.indexes.models.SearchIndexerDataSource or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerDataSource or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerDataSource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -32,14 +33,18 @@
     build_list_request,
     build_reset_docs_request,
     build_reset_request,
     build_run_request,
 )
 from .._vendor import SearchServiceClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class IndexersOperations:
     """
     .. warning::
@@ -72,15 +77,15 @@
         :type indexer_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -212,15 +217,15 @@
         :param keys_or_ids: Is either a DocumentKeysOrIds type or a IO[bytes] type. Default value is
          None.
         :type keys_or_ids: ~azure.search.documents.indexes.models.DocumentKeysOrIds or IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -290,15 +295,15 @@
         :type indexer_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -478,15 +483,15 @@
         :type disable_cache_reprocessing_change_detection: bool
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexer or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexer
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -576,15 +581,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -641,15 +646,15 @@
         :type indexer_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexer or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexer
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -710,15 +715,15 @@
         :type select: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: ListIndexersResult or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.ListIndexersResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -833,15 +838,15 @@
         :type indexer: ~azure.search.documents.indexes.models.SearchIndexer or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexer or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexer
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -910,15 +915,15 @@
         :type indexer_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerStatus or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerStatus
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -33,14 +34,18 @@
     build_delete_request,
     build_get_request,
     build_get_statistics_request,
     build_list_request,
 )
 from .._vendor import SearchServiceClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class IndexesOperations:
     """
     .. warning::
@@ -129,15 +134,15 @@
         :type index: ~azure.search.documents.indexes.models.SearchIndex or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndex or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndex
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -215,15 +220,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ListIndexesResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -431,15 +436,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndex or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndex
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -530,15 +535,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -595,15 +600,15 @@
         :type index_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndex or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndex
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -662,15 +667,15 @@
         :type index_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: GetIndexStatisticsResult or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.GetIndexStatisticsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -794,15 +799,15 @@
         :type request: ~azure.search.documents.indexes.models.AnalyzeRequest or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: AnalyzeResult or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.AnalyzeResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_patch.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Optional, TypeVar
+import sys
+from typing import Any, Callable, Dict, Optional, Type, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -21,32 +22,37 @@
 from azure.core.utils import case_insensitive_dict
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._search_service_client_operations import build_get_service_statistics_request
 from .._vendor import SearchServiceClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class SearchServiceClientOperationsMixin(SearchServiceClientMixinABC):
+
     @distributed_trace_async
     async def get_service_statistics(
         self, request_options: Optional[_models.RequestOptions] = None, **kwargs: Any
     ) -> _models.SearchServiceStatistics:
         """Gets service level statistics for a search service.
 
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchServiceStatistics or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchServiceStatistics
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -29,14 +30,18 @@
     build_delete_request,
     build_get_request,
     build_list_request,
     build_reset_skills_request,
 )
 from .._vendor import SearchServiceClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class SkillsetsOperations:
     """
     .. warning::
@@ -196,15 +201,15 @@
         :type disable_cache_reprocessing_change_detection: bool
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerSkillset or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerSkillset
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -294,15 +299,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -359,15 +364,15 @@
         :type skillset_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerSkillset or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerSkillset
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -428,15 +433,15 @@
         :type select: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: ListSkillsetsResult or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.ListSkillsetsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -553,15 +558,15 @@
         :type skillset: ~azure.search.documents.indexes.models.SearchIndexerSkillset or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerSkillset or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerSkillset
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -695,15 +700,15 @@
         :type skill_names: ~azure.search.documents.indexes.models.SkillNames or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -28,14 +29,18 @@
     build_create_request,
     build_delete_request,
     build_get_request,
     build_list_request,
 )
 from .._vendor import SearchServiceClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class SynonymMapsOperations:
     """
     .. warning::
@@ -169,15 +174,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SynonymMap or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SynonymMap
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -265,15 +270,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -330,15 +335,15 @@
         :type synonym_map_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SynonymMap or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SynonymMap
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -399,15 +404,15 @@
         :type select: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: ListSynonymMapsResult or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.ListSynonymMapsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -522,15 +527,15 @@
         :type synonym_map: ~azure.search.documents.indexes.models.SynonymMap or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SynonymMap or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SynonymMap
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from ._models_py3 import AIServicesVisionParameters
+from ._models_py3 import AIServicesVisionVectorizer
 from ._models_py3 import AnalyzeRequest
 from ._models_py3 import AnalyzeResult
 from ._models_py3 import AnalyzedTokenInfo
 from ._models_py3 import AsciiFoldingTokenFilter
 from ._models_py3 import AzureActiveDirectoryApplicationCredentials
+from ._models_py3 import AzureMachineLearningParameters
 from ._models_py3 import AzureMachineLearningSkill
+from ._models_py3 import AzureMachineLearningVectorizer
 from ._models_py3 import AzureOpenAIEmbeddingSkill
 from ._models_py3 import AzureOpenAIParameters
 from ._models_py3 import AzureOpenAIVectorizer
 from ._models_py3 import BM25SimilarityAlgorithm
 from ._models_py3 import CharFilter
 from ._models_py3 import CjkBigramTokenFilter
 from ._models_py3 import ClassicSimilarityAlgorithm
@@ -173,17 +177,20 @@
 from ._models_py3 import UaxUrlEmailTokenizer
 from ._models_py3 import UniqueTokenFilter
 from ._models_py3 import VectorSearch
 from ._models_py3 import VectorSearchAlgorithmConfiguration
 from ._models_py3 import VectorSearchCompressionConfiguration
 from ._models_py3 import VectorSearchProfile
 from ._models_py3 import VectorSearchVectorizer
+from ._models_py3 import VisionVectorizeSkill
 from ._models_py3 import WebApiSkill
 from ._models_py3 import WordDelimiterTokenFilter
 
+from ._search_service_client_enums import AIStudioModelCatalogName
+from ._search_service_client_enums import AzureOpenAIModelName
 from ._search_service_client_enums import BlobIndexerDataToExtract
 from ._search_service_client_enums import BlobIndexerImageAction
 from ._search_service_client_enums import BlobIndexerPDFTextRotationAlgorithm
 from ._search_service_client_enums import BlobIndexerParsingMode
 from ._search_service_client_enums import CharFilterName
 from ._search_service_client_enums import CjkBigramTokenFilterScripts
 from ._search_service_client_enums import CustomEntityLookupSkillLanguage
@@ -219,31 +226,36 @@
 from ._search_service_client_enums import SplitSkillLanguage
 from ._search_service_client_enums import StemmerTokenFilterLanguage
 from ._search_service_client_enums import StopwordsList
 from ._search_service_client_enums import TextSplitMode
 from ._search_service_client_enums import TextTranslationSkillLanguage
 from ._search_service_client_enums import TokenCharacterKind
 from ._search_service_client_enums import TokenFilterName
+from ._search_service_client_enums import VectorEncodingFormat
 from ._search_service_client_enums import VectorSearchAlgorithmKind
 from ._search_service_client_enums import VectorSearchAlgorithmMetric
 from ._search_service_client_enums import VectorSearchCompressionKind
 from ._search_service_client_enums import VectorSearchCompressionTargetDataType
 from ._search_service_client_enums import VectorSearchVectorizerKind
 from ._search_service_client_enums import VisualFeature
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
+    "AIServicesVisionParameters",
+    "AIServicesVisionVectorizer",
     "AnalyzeRequest",
     "AnalyzeResult",
     "AnalyzedTokenInfo",
     "AsciiFoldingTokenFilter",
     "AzureActiveDirectoryApplicationCredentials",
+    "AzureMachineLearningParameters",
     "AzureMachineLearningSkill",
+    "AzureMachineLearningVectorizer",
     "AzureOpenAIEmbeddingSkill",
     "AzureOpenAIParameters",
     "AzureOpenAIVectorizer",
     "BM25SimilarityAlgorithm",
     "CharFilter",
     "CjkBigramTokenFilter",
     "ClassicSimilarityAlgorithm",
@@ -403,16 +415,19 @@
     "UaxUrlEmailTokenizer",
     "UniqueTokenFilter",
     "VectorSearch",
     "VectorSearchAlgorithmConfiguration",
     "VectorSearchCompressionConfiguration",
     "VectorSearchProfile",
     "VectorSearchVectorizer",
+    "VisionVectorizeSkill",
     "WebApiSkill",
     "WordDelimiterTokenFilter",
+    "AIStudioModelCatalogName",
+    "AzureOpenAIModelName",
     "BlobIndexerDataToExtract",
     "BlobIndexerImageAction",
     "BlobIndexerPDFTextRotationAlgorithm",
     "BlobIndexerParsingMode",
     "CharFilterName",
     "CjkBigramTokenFilterScripts",
     "CustomEntityLookupSkillLanguage",
@@ -448,14 +463,15 @@
     "SplitSkillLanguage",
     "StemmerTokenFilterLanguage",
     "StopwordsList",
     "TextSplitMode",
     "TextTranslationSkillLanguage",
     "TokenCharacterKind",
     "TokenFilterName",
+    "VectorEncodingFormat",
     "VectorSearchAlgorithmKind",
     "VectorSearchAlgorithmMetric",
     "VectorSearchCompressionKind",
     "VectorSearchCompressionTargetDataType",
     "VectorSearchVectorizerKind",
     "VisualFeature",
 ]
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/_models_py3.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/models/_models_py3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,179 @@
 # coding=utf-8
 # pylint: disable=too-many-lines
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 import datetime
 from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
 
 from .. import _serialization
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from .. import models as _models
 
 
+class AIServicesVisionParameters(_serialization.Model):
+    """Specifies the AI Services Vision parameters for vectorizing a query image or text.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar model_version: The version of the model to use when calling the AI Services Vision
+     service. It will default to the latest available when not specified. Required.
+    :vartype model_version: str
+    :ivar resource_uri: The resource URI of the AI Services resource. Required.
+    :vartype resource_uri: str
+    :ivar api_key: API key of the designated AI Services resource.
+    :vartype api_key: str
+    :ivar auth_identity: The user-assigned managed identity used for outbound connections. If an
+     authResourceId is provided and it's not specified, the system-assigned managed identity is
+     used. On updates to the index, if the identity is unspecified, the value remains unchanged. If
+     set to "none", the value of this property is cleared.
+    :vartype auth_identity: ~azure.search.documents.indexes.models.SearchIndexerDataIdentity
+    """
+
+    _validation = {
+        "model_version": {"required": True},
+        "resource_uri": {"required": True},
+    }
+
+    _attribute_map = {
+        "model_version": {"key": "modelVersion", "type": "str"},
+        "resource_uri": {"key": "resourceUri", "type": "str"},
+        "api_key": {"key": "apiKey", "type": "str"},
+        "auth_identity": {"key": "authIdentity", "type": "SearchIndexerDataIdentity"},
+    }
+
+    def __init__(
+        self,
+        *,
+        model_version: str,
+        resource_uri: str,
+        api_key: Optional[str] = None,
+        auth_identity: Optional["_models.SearchIndexerDataIdentity"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword model_version: The version of the model to use when calling the AI Services Vision
+         service. It will default to the latest available when not specified. Required.
+        :paramtype model_version: str
+        :keyword resource_uri: The resource URI of the AI Services resource. Required.
+        :paramtype resource_uri: str
+        :keyword api_key: API key of the designated AI Services resource.
+        :paramtype api_key: str
+        :keyword auth_identity: The user-assigned managed identity used for outbound connections. If an
+         authResourceId is provided and it's not specified, the system-assigned managed identity is
+         used. On updates to the index, if the identity is unspecified, the value remains unchanged. If
+         set to "none", the value of this property is cleared.
+        :paramtype auth_identity: ~azure.search.documents.indexes.models.SearchIndexerDataIdentity
+        """
+        super().__init__(**kwargs)
+        self.model_version = model_version
+        self.resource_uri = resource_uri
+        self.api_key = api_key
+        self.auth_identity = auth_identity
+
+
+class VectorSearchVectorizer(_serialization.Model):
+    """Specifies the vectorization method to be used during query time.
+
+    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
+    AIServicesVisionVectorizer, AzureMachineLearningVectorizer, AzureOpenAIVectorizer,
+    CustomVectorizer
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar name: The name to associate with this particular vectorization method. Required.
+    :vartype name: str
+    :ivar kind: The name of the kind of vectorization method being configured for use with vector
+     search. Required. Known values are: "azureOpenAI", "customWebApi", "aiServicesVision", and
+     "aml".
+    :vartype kind: str or ~azure.search.documents.indexes.models.VectorSearchVectorizerKind
+    """
+
+    _validation = {
+        "name": {"required": True},
+        "kind": {"required": True},
+    }
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "kind": {"key": "kind", "type": "str"},
+    }
+
+    _subtype_map = {
+        "kind": {
+            "aiServicesVision": "AIServicesVisionVectorizer",
+            "aml": "AzureMachineLearningVectorizer",
+            "azureOpenAI": "AzureOpenAIVectorizer",
+            "customWebApi": "CustomVectorizer",
+        }
+    }
+
+    def __init__(self, *, name: str, **kwargs: Any) -> None:
+        """
+        :keyword name: The name to associate with this particular vectorization method. Required.
+        :paramtype name: str
+        """
+        super().__init__(**kwargs)
+        self.name = name
+        self.kind: Optional[str] = None
+
+
+class AIServicesVisionVectorizer(VectorSearchVectorizer):
+    """Specifies the AI Services Vision parameters for vectorizing a query image or text.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar name: The name to associate with this particular vectorization method. Required.
+    :vartype name: str
+    :ivar kind: The name of the kind of vectorization method being configured for use with vector
+     search. Required. Known values are: "azureOpenAI", "customWebApi", "aiServicesVision", and
+     "aml".
+    :vartype kind: str or ~azure.search.documents.indexes.models.VectorSearchVectorizerKind
+    :ivar ai_services_vision_parameters: Contains the parameters specific to AI Services Vision
+     embedding vectorization.
+    :vartype ai_services_vision_parameters:
+     ~azure.search.documents.indexes.models.AIServicesVisionParameters
+    """
+
+    _validation = {
+        "name": {"required": True},
+        "kind": {"required": True},
+    }
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "kind": {"key": "kind", "type": "str"},
+        "ai_services_vision_parameters": {"key": "aiServicesVisionParameters", "type": "AIServicesVisionParameters"},
+    }
+
+    def __init__(
+        self,
+        *,
+        name: str,
+        ai_services_vision_parameters: Optional["_models.AIServicesVisionParameters"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword name: The name to associate with this particular vectorization method. Required.
+        :paramtype name: str
+        :keyword ai_services_vision_parameters: Contains the parameters specific to AI Services Vision
+         embedding vectorization.
+        :paramtype ai_services_vision_parameters:
+         ~azure.search.documents.indexes.models.AIServicesVisionParameters
+        """
+        super().__init__(name=name, **kwargs)
+        self.kind: str = "aiServicesVision"
+        self.ai_services_vision_parameters = ai_services_vision_parameters
+
+
 class AnalyzedTokenInfo(_serialization.Model):
     """Information about a token returned by an analyzer.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to server.
 
@@ -345,23 +500,110 @@
         :paramtype application_secret: str
         """
         super().__init__(**kwargs)
         self.application_id = application_id
         self.application_secret = application_secret
 
 
+class AzureMachineLearningParameters(_serialization.Model):
+    """Specifies the properties for connecting to an AML vectorizer.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar scoring_uri: (Required for no authentication or key authentication) The scoring URI of
+     the AML service to which the JSON payload will be sent. Only the https URI scheme is allowed.
+     Required.
+    :vartype scoring_uri: str
+    :ivar authentication_key: (Required for key authentication) The key for the AML service.
+    :vartype authentication_key: str
+    :ivar resource_id: (Required for token authentication). The Azure Resource Manager resource ID
+     of the AML service. It should be in the format
+     subscriptions/{guid}/resourceGroups/{resource-group-name}/Microsoft.MachineLearningServices/workspaces/{workspace-name}/services/{service_name}.  # pylint: disable=line-too-long
+    :vartype resource_id: str
+    :ivar timeout: (Optional) When specified, indicates the timeout for the http client making the
+     API call.
+    :vartype timeout: ~datetime.timedelta
+    :ivar region: (Optional for token authentication). The region the AML service is deployed in.
+    :vartype region: str
+    :ivar model_name: The name of the embedding model from the Azure AI Studio Catalog that is
+     deployed at the provided endpoint. Known values are:
+     "OpenAI-CLIP-Image-Text-Embeddings-vit-base-patch32",
+     "OpenAI-CLIP-Image-Text-Embeddings-ViT-Large-Patch14-336",
+     "Facebook-DinoV2-Image-Embeddings-ViT-Base", "Facebook-DinoV2-Image-Embeddings-ViT-Giant",
+     "Cohere-embed-v3-english", and "Cohere-embed-v3-multilingual".
+    :vartype model_name: str or ~azure.search.documents.indexes.models.AIStudioModelCatalogName
+    """
+
+    _validation = {
+        "scoring_uri": {"required": True},
+    }
+
+    _attribute_map = {
+        "scoring_uri": {"key": "uri", "type": "str"},
+        "authentication_key": {"key": "key", "type": "str"},
+        "resource_id": {"key": "resourceId", "type": "str"},
+        "timeout": {"key": "timeout", "type": "duration"},
+        "region": {"key": "region", "type": "str"},
+        "model_name": {"key": "modelName", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        scoring_uri: str,
+        authentication_key: Optional[str] = None,
+        resource_id: Optional[str] = None,
+        timeout: Optional[datetime.timedelta] = None,
+        region: Optional[str] = None,
+        model_name: Optional[Union[str, "_models.AIStudioModelCatalogName"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword scoring_uri: (Required for no authentication or key authentication) The scoring URI of
+         the AML service to which the JSON payload will be sent. Only the https URI scheme is allowed.
+         Required.
+        :paramtype scoring_uri: str
+        :keyword authentication_key: (Required for key authentication) The key for the AML service.
+        :paramtype authentication_key: str
+        :keyword resource_id: (Required for token authentication). The Azure Resource Manager resource
+         ID of the AML service. It should be in the format
+         subscriptions/{guid}/resourceGroups/{resource-group-name}/Microsoft.MachineLearningServices/workspaces/{workspace-name}/services/{service_name}.  # pylint: disable=line-too-long
+        :paramtype resource_id: str
+        :keyword timeout: (Optional) When specified, indicates the timeout for the http client making
+         the API call.
+        :paramtype timeout: ~datetime.timedelta
+        :keyword region: (Optional for token authentication). The region the AML service is deployed
+         in.
+        :paramtype region: str
+        :keyword model_name: The name of the embedding model from the Azure AI Studio Catalog that is
+         deployed at the provided endpoint. Known values are:
+         "OpenAI-CLIP-Image-Text-Embeddings-vit-base-patch32",
+         "OpenAI-CLIP-Image-Text-Embeddings-ViT-Large-Patch14-336",
+         "Facebook-DinoV2-Image-Embeddings-ViT-Base", "Facebook-DinoV2-Image-Embeddings-ViT-Giant",
+         "Cohere-embed-v3-english", and "Cohere-embed-v3-multilingual".
+        :paramtype model_name: str or ~azure.search.documents.indexes.models.AIStudioModelCatalogName
+        """
+        super().__init__(**kwargs)
+        self.scoring_uri = scoring_uri
+        self.authentication_key = authentication_key
+        self.resource_id = resource_id
+        self.timeout = timeout
+        self.region = region
+        self.model_name = model_name
+
+
 class SearchIndexerSkill(_serialization.Model):
     """Base type for skills.
 
     You probably want to use the sub-classes and not this class directly. Known sub-classes are:
     AzureMachineLearningSkill, WebApiSkill, AzureOpenAIEmbeddingSkill, CustomEntityLookupSkill,
     EntityRecognitionSkill, KeyPhraseExtractionSkill, LanguageDetectionSkill, MergeSkill,
     PIIDetectionSkill, SentimentSkill, SplitSkill, TextTranslationSkill, EntityLinkingSkill,
     EntityRecognitionSkillV3, SentimentSkillV3, ConditionalSkill, DocumentExtractionSkill,
-    ShaperSkill, ImageAnalysisSkill, OcrSkill
+    ShaperSkill, ImageAnalysisSkill, OcrSkill, VisionVectorizeSkill
 
     All required parameters must be populated in order to send to server.
 
     :ivar odata_type: A URI fragment specifying the type of skill. Required.
     :vartype odata_type: str
     :ivar name: The name of the skill which uniquely identifies it within the skillset. A skill
      with no name defined will be given a default name of its 1-based index in the skills array,
@@ -414,14 +656,15 @@
             "#Microsoft.Skills.Text.V3.EntityRecognitionSkill": "EntityRecognitionSkillV3",
             "#Microsoft.Skills.Text.V3.SentimentSkill": "SentimentSkillV3",
             "#Microsoft.Skills.Util.ConditionalSkill": "ConditionalSkill",
             "#Microsoft.Skills.Util.DocumentExtractionSkill": "DocumentExtractionSkill",
             "#Microsoft.Skills.Util.ShaperSkill": "ShaperSkill",
             "#Microsoft.Skills.Vision.ImageAnalysisSkill": "ImageAnalysisSkill",
             "#Microsoft.Skills.Vision.OcrSkill": "OcrSkill",
+            "#Microsoft.Skills.Vision.VectorizeSkill": "VisionVectorizeSkill",
         }
     }
 
     def __init__(
         self,
         *,
         inputs: List["_models.InputFieldMappingEntry"],
@@ -591,208 +834,264 @@
         self.authentication_key = authentication_key
         self.resource_id = resource_id
         self.timeout = timeout
         self.region = region
         self.degree_of_parallelism = degree_of_parallelism
 
 
-class AzureOpenAIEmbeddingSkill(SearchIndexerSkill):
-    """Allows you to generate a vector embedding for a given text input using the Azure OpenAI
-    resource.
+class AzureMachineLearningVectorizer(VectorSearchVectorizer):
+    """Specifies an Azure Machine Learning endpoint deployed via the Azure AI Studio Model Catalog for
+    generating the vector embedding of a query string.
 
     All required parameters must be populated in order to send to server.
 
-    :ivar odata_type: A URI fragment specifying the type of skill. Required.
-    :vartype odata_type: str
-    :ivar name: The name of the skill which uniquely identifies it within the skillset. A skill
-     with no name defined will be given a default name of its 1-based index in the skills array,
-     prefixed with the character '#'.
+    :ivar name: The name to associate with this particular vectorization method. Required.
     :vartype name: str
-    :ivar description: The description of the skill which describes the inputs, outputs, and usage
-     of the skill.
-    :vartype description: str
-    :ivar context: Represents the level at which operations take place, such as the document root
-     or document content (for example, /document or /document/content). The default is /document.
-    :vartype context: str
-    :ivar inputs: Inputs of the skills could be a column in the source data set, or the output of
-     an upstream skill. Required.
-    :vartype inputs: list[~azure.search.documents.indexes.models.InputFieldMappingEntry]
-    :ivar outputs: The output of a skill is either a field in a search index, or a value that can
-     be consumed as an input by another skill. Required.
-    :vartype outputs: list[~azure.search.documents.indexes.models.OutputFieldMappingEntry]
-    :ivar resource_uri: The resource URI for your Azure OpenAI resource.
-    :vartype resource_uri: str
-    :ivar deployment_id: ID of your Azure OpenAI model deployment on the designated resource.
-    :vartype deployment_id: str
-    :ivar api_key: API key for the designated Azure OpenAI resource.
-    :vartype api_key: str
-    :ivar auth_identity: The user-assigned managed identity used for outbound connections.
-    :vartype auth_identity: ~azure.search.documents.indexes.models.SearchIndexerDataIdentity
+    :ivar kind: The name of the kind of vectorization method being configured for use with vector
+     search. Required. Known values are: "azureOpenAI", "customWebApi", "aiServicesVision", and
+     "aml".
+    :vartype kind: str or ~azure.search.documents.indexes.models.VectorSearchVectorizerKind
+    :ivar aml_parameters: Specifies the properties of the AML vectorizer.
+    :vartype aml_parameters: ~azure.search.documents.indexes.models.AzureMachineLearningParameters
     """
 
     _validation = {
-        "odata_type": {"required": True},
-        "inputs": {"required": True},
-        "outputs": {"required": True},
+        "name": {"required": True},
+        "kind": {"required": True},
     }
 
     _attribute_map = {
-        "odata_type": {"key": "@odata\\.type", "type": "str"},
         "name": {"key": "name", "type": "str"},
-        "description": {"key": "description", "type": "str"},
-        "context": {"key": "context", "type": "str"},
-        "inputs": {"key": "inputs", "type": "[InputFieldMappingEntry]"},
-        "outputs": {"key": "outputs", "type": "[OutputFieldMappingEntry]"},
-        "resource_uri": {"key": "resourceUri", "type": "str"},
-        "deployment_id": {"key": "deploymentId", "type": "str"},
-        "api_key": {"key": "apiKey", "type": "str"},
-        "auth_identity": {"key": "authIdentity", "type": "SearchIndexerDataIdentity"},
+        "kind": {"key": "kind", "type": "str"},
+        "aml_parameters": {"key": "amlParameters", "type": "AzureMachineLearningParameters"},
     }
 
     def __init__(
-        self,
-        *,
-        inputs: List["_models.InputFieldMappingEntry"],
-        outputs: List["_models.OutputFieldMappingEntry"],
-        name: Optional[str] = None,
-        description: Optional[str] = None,
-        context: Optional[str] = None,
-        resource_uri: Optional[str] = None,
-        deployment_id: Optional[str] = None,
-        api_key: Optional[str] = None,
-        auth_identity: Optional["_models.SearchIndexerDataIdentity"] = None,
-        **kwargs: Any
+        self, *, name: str, aml_parameters: Optional["_models.AzureMachineLearningParameters"] = None, **kwargs: Any
     ) -> None:
         """
-        :keyword name: The name of the skill which uniquely identifies it within the skillset. A skill
-         with no name defined will be given a default name of its 1-based index in the skills array,
-         prefixed with the character '#'.
+        :keyword name: The name to associate with this particular vectorization method. Required.
         :paramtype name: str
-        :keyword description: The description of the skill which describes the inputs, outputs, and
-         usage of the skill.
-        :paramtype description: str
-        :keyword context: Represents the level at which operations take place, such as the document
-         root or document content (for example, /document or /document/content). The default is
-         /document.
-        :paramtype context: str
-        :keyword inputs: Inputs of the skills could be a column in the source data set, or the output
-         of an upstream skill. Required.
-        :paramtype inputs: list[~azure.search.documents.indexes.models.InputFieldMappingEntry]
-        :keyword outputs: The output of a skill is either a field in a search index, or a value that
-         can be consumed as an input by another skill. Required.
-        :paramtype outputs: list[~azure.search.documents.indexes.models.OutputFieldMappingEntry]
-        :keyword resource_uri: The resource URI for your Azure OpenAI resource.
-        :paramtype resource_uri: str
-        :keyword deployment_id: ID of your Azure OpenAI model deployment on the designated resource.
-        :paramtype deployment_id: str
-        :keyword api_key: API key for the designated Azure OpenAI resource.
-        :paramtype api_key: str
-        :keyword auth_identity: The user-assigned managed identity used for outbound connections.
-        :paramtype auth_identity: ~azure.search.documents.indexes.models.SearchIndexerDataIdentity
+        :keyword aml_parameters: Specifies the properties of the AML vectorizer.
+        :paramtype aml_parameters:
+         ~azure.search.documents.indexes.models.AzureMachineLearningParameters
         """
-        super().__init__(name=name, description=description, context=context, inputs=inputs, outputs=outputs, **kwargs)
-        self.odata_type: str = "#Microsoft.Skills.Text.AzureOpenAIEmbeddingSkill"
-        self.resource_uri = resource_uri
-        self.deployment_id = deployment_id
-        self.api_key = api_key
-        self.auth_identity = auth_identity
+        super().__init__(name=name, **kwargs)
+        self.kind: str = "aml"
+        self.aml_parameters = aml_parameters
 
 
 class AzureOpenAIParameters(_serialization.Model):
     """Specifies the parameters for connecting to the Azure OpenAI resource.
 
     :ivar resource_uri: The resource URI of the Azure OpenAI resource.
     :vartype resource_uri: str
     :ivar deployment_id: ID of the Azure OpenAI model deployment on the designated resource.
     :vartype deployment_id: str
     :ivar api_key: API key of the designated Azure OpenAI resource.
     :vartype api_key: str
     :ivar auth_identity: The user-assigned managed identity used for outbound connections.
     :vartype auth_identity: ~azure.search.documents.indexes.models.SearchIndexerDataIdentity
+    :ivar model_name: The name of the embedding model that is deployed at the provided deploymentId
+     path. Known values are: "text-embedding-ada-002", "text-embedding-3-large",
+     "text-embedding-3-small", and "experimental".
+    :vartype model_name: str or ~azure.search.documents.indexes.models.AzureOpenAIModelName
     """
 
     _attribute_map = {
         "resource_uri": {"key": "resourceUri", "type": "str"},
         "deployment_id": {"key": "deploymentId", "type": "str"},
         "api_key": {"key": "apiKey", "type": "str"},
         "auth_identity": {"key": "authIdentity", "type": "SearchIndexerDataIdentity"},
+        "model_name": {"key": "modelName", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         resource_uri: Optional[str] = None,
         deployment_id: Optional[str] = None,
         api_key: Optional[str] = None,
         auth_identity: Optional["_models.SearchIndexerDataIdentity"] = None,
+        model_name: Optional[Union[str, "_models.AzureOpenAIModelName"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword resource_uri: The resource URI of the Azure OpenAI resource.
         :paramtype resource_uri: str
         :keyword deployment_id: ID of the Azure OpenAI model deployment on the designated resource.
         :paramtype deployment_id: str
         :keyword api_key: API key of the designated Azure OpenAI resource.
         :paramtype api_key: str
         :keyword auth_identity: The user-assigned managed identity used for outbound connections.
         :paramtype auth_identity: ~azure.search.documents.indexes.models.SearchIndexerDataIdentity
+        :keyword model_name: The name of the embedding model that is deployed at the provided
+         deploymentId path. Known values are: "text-embedding-ada-002", "text-embedding-3-large",
+         "text-embedding-3-small", and "experimental".
+        :paramtype model_name: str or ~azure.search.documents.indexes.models.AzureOpenAIModelName
         """
         super().__init__(**kwargs)
         self.resource_uri = resource_uri
         self.deployment_id = deployment_id
         self.api_key = api_key
         self.auth_identity = auth_identity
+        self.model_name = model_name
 
 
-class VectorSearchVectorizer(_serialization.Model):
-    """Specifies the vectorization method to be used during query time.
-
-    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
-    AzureOpenAIVectorizer, CustomVectorizer
+class AzureOpenAIEmbeddingSkill(
+    SearchIndexerSkill, AzureOpenAIParameters
+):  # pylint: disable=too-many-instance-attributes
+    """Allows you to generate a vector embedding for a given text input using the Azure OpenAI
+    resource.
 
     All required parameters must be populated in order to send to server.
 
-    :ivar name: The name to associate with this particular vectorization method. Required.
+    :ivar resource_uri: The resource URI of the Azure OpenAI resource.
+    :vartype resource_uri: str
+    :ivar deployment_id: ID of the Azure OpenAI model deployment on the designated resource.
+    :vartype deployment_id: str
+    :ivar api_key: API key of the designated Azure OpenAI resource.
+    :vartype api_key: str
+    :ivar auth_identity: The user-assigned managed identity used for outbound connections.
+    :vartype auth_identity: ~azure.search.documents.indexes.models.SearchIndexerDataIdentity
+    :ivar model_name: The name of the embedding model that is deployed at the provided deploymentId
+     path. Known values are: "text-embedding-ada-002", "text-embedding-3-large",
+     "text-embedding-3-small", and "experimental".
+    :vartype model_name: str or ~azure.search.documents.indexes.models.AzureOpenAIModelName
+    :ivar odata_type: A URI fragment specifying the type of skill. Required.
+    :vartype odata_type: str
+    :ivar name: The name of the skill which uniquely identifies it within the skillset. A skill
+     with no name defined will be given a default name of its 1-based index in the skills array,
+     prefixed with the character '#'.
     :vartype name: str
-    :ivar kind: The name of the kind of vectorization method being configured for use with vector
-     search. Required. Known values are: "azureOpenAI" and "customWebApi".
-    :vartype kind: str or ~azure.search.documents.indexes.models.VectorSearchVectorizerKind
+    :ivar description: The description of the skill which describes the inputs, outputs, and usage
+     of the skill.
+    :vartype description: str
+    :ivar context: Represents the level at which operations take place, such as the document root
+     or document content (for example, /document or /document/content). The default is /document.
+    :vartype context: str
+    :ivar inputs: Inputs of the skills could be a column in the source data set, or the output of
+     an upstream skill. Required.
+    :vartype inputs: list[~azure.search.documents.indexes.models.InputFieldMappingEntry]
+    :ivar outputs: The output of a skill is either a field in a search index, or a value that can
+     be consumed as an input by another skill. Required.
+    :vartype outputs: list[~azure.search.documents.indexes.models.OutputFieldMappingEntry]
+    :ivar dimensions: The number of dimensions the resulting output embeddings should have. Only
+     supported in text-embedding-3 and later models.
+    :vartype dimensions: int
     """
 
     _validation = {
-        "name": {"required": True},
-        "kind": {"required": True},
+        "odata_type": {"required": True},
+        "inputs": {"required": True},
+        "outputs": {"required": True},
     }
 
     _attribute_map = {
+        "resource_uri": {"key": "resourceUri", "type": "str"},
+        "deployment_id": {"key": "deploymentId", "type": "str"},
+        "api_key": {"key": "apiKey", "type": "str"},
+        "auth_identity": {"key": "authIdentity", "type": "SearchIndexerDataIdentity"},
+        "model_name": {"key": "modelName", "type": "str"},
+        "odata_type": {"key": "@odata\\.type", "type": "str"},
         "name": {"key": "name", "type": "str"},
-        "kind": {"key": "kind", "type": "str"},
+        "description": {"key": "description", "type": "str"},
+        "context": {"key": "context", "type": "str"},
+        "inputs": {"key": "inputs", "type": "[InputFieldMappingEntry]"},
+        "outputs": {"key": "outputs", "type": "[OutputFieldMappingEntry]"},
+        "dimensions": {"key": "dimensions", "type": "int"},
     }
 
-    _subtype_map = {"kind": {"azureOpenAI": "AzureOpenAIVectorizer", "customWebApi": "CustomVectorizer"}}
-
-    def __init__(self, *, name: str, **kwargs: Any) -> None:
+    def __init__(
+        self,
+        *,
+        inputs: List["_models.InputFieldMappingEntry"],
+        outputs: List["_models.OutputFieldMappingEntry"],
+        resource_uri: Optional[str] = None,
+        deployment_id: Optional[str] = None,
+        api_key: Optional[str] = None,
+        auth_identity: Optional["_models.SearchIndexerDataIdentity"] = None,
+        model_name: Optional[Union[str, "_models.AzureOpenAIModelName"]] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        context: Optional[str] = None,
+        dimensions: Optional[int] = None,
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword name: The name to associate with this particular vectorization method. Required.
+        :keyword resource_uri: The resource URI of the Azure OpenAI resource.
+        :paramtype resource_uri: str
+        :keyword deployment_id: ID of the Azure OpenAI model deployment on the designated resource.
+        :paramtype deployment_id: str
+        :keyword api_key: API key of the designated Azure OpenAI resource.
+        :paramtype api_key: str
+        :keyword auth_identity: The user-assigned managed identity used for outbound connections.
+        :paramtype auth_identity: ~azure.search.documents.indexes.models.SearchIndexerDataIdentity
+        :keyword model_name: The name of the embedding model that is deployed at the provided
+         deploymentId path. Known values are: "text-embedding-ada-002", "text-embedding-3-large",
+         "text-embedding-3-small", and "experimental".
+        :paramtype model_name: str or ~azure.search.documents.indexes.models.AzureOpenAIModelName
+        :keyword name: The name of the skill which uniquely identifies it within the skillset. A skill
+         with no name defined will be given a default name of its 1-based index in the skills array,
+         prefixed with the character '#'.
         :paramtype name: str
+        :keyword description: The description of the skill which describes the inputs, outputs, and
+         usage of the skill.
+        :paramtype description: str
+        :keyword context: Represents the level at which operations take place, such as the document
+         root or document content (for example, /document or /document/content). The default is
+         /document.
+        :paramtype context: str
+        :keyword inputs: Inputs of the skills could be a column in the source data set, or the output
+         of an upstream skill. Required.
+        :paramtype inputs: list[~azure.search.documents.indexes.models.InputFieldMappingEntry]
+        :keyword outputs: The output of a skill is either a field in a search index, or a value that
+         can be consumed as an input by another skill. Required.
+        :paramtype outputs: list[~azure.search.documents.indexes.models.OutputFieldMappingEntry]
+        :keyword dimensions: The number of dimensions the resulting output embeddings should have. Only
+         supported in text-embedding-3 and later models.
+        :paramtype dimensions: int
         """
-        super().__init__(**kwargs)
+        super().__init__(
+            name=name,
+            description=description,
+            context=context,
+            inputs=inputs,
+            outputs=outputs,
+            resource_uri=resource_uri,
+            deployment_id=deployment_id,
+            api_key=api_key,
+            auth_identity=auth_identity,
+            model_name=model_name,
+            **kwargs
+        )
+        self.resource_uri = resource_uri
+        self.deployment_id = deployment_id
+        self.api_key = api_key
+        self.auth_identity = auth_identity
+        self.model_name = model_name
+        self.odata_type: str = "#Microsoft.Skills.Text.AzureOpenAIEmbeddingSkill"
+        self.dimensions = dimensions
         self.name = name
-        self.kind: Optional[str] = None
+        self.description = description
+        self.context = context
+        self.inputs = inputs
+        self.outputs = outputs
 
 
 class AzureOpenAIVectorizer(VectorSearchVectorizer):
     """Specifies the Azure OpenAI resource used to vectorize a query string.
 
     All required parameters must be populated in order to send to server.
 
     :ivar name: The name to associate with this particular vectorization method. Required.
     :vartype name: str
     :ivar kind: The name of the kind of vectorization method being configured for use with vector
-     search. Required. Known values are: "azureOpenAI" and "customWebApi".
+     search. Required. Known values are: "azureOpenAI", "customWebApi", "aiServicesVision", and
+     "aml".
     :vartype kind: str or ~azure.search.documents.indexes.models.VectorSearchVectorizerKind
     :ivar azure_open_ai_parameters: Contains the parameters specific to Azure OpenAI embedding
      vectorization.
     :vartype azure_open_ai_parameters: ~azure.search.documents.indexes.models.AzureOpenAIParameters
     """
 
     _validation = {
@@ -1970,15 +2269,16 @@
     skillset.
 
     All required parameters must be populated in order to send to server.
 
     :ivar name: The name to associate with this particular vectorization method. Required.
     :vartype name: str
     :ivar kind: The name of the kind of vectorization method being configured for use with vector
-     search. Required. Known values are: "azureOpenAI" and "customWebApi".
+     search. Required. Known values are: "azureOpenAI", "customWebApi", "aiServicesVision", and
+     "aml".
     :vartype kind: str or ~azure.search.documents.indexes.models.VectorSearchVectorizerKind
     :ivar custom_web_api_parameters: Specifies the properties of the user-defined vectorizer.
     :vartype custom_web_api_parameters:
      ~azure.search.documents.indexes.models.CustomWebApiParameters
     """
 
     _validation = {
@@ -3334,28 +3634,28 @@
         self.parameters = parameters
 
 
 class ExhaustiveKnnParameters(_serialization.Model):
     """Contains the parameters specific to exhaustive KNN algorithm.
 
     :ivar metric: The similarity metric to use for vector comparisons. Known values are: "cosine",
-     "euclidean", and "dotProduct".
+     "euclidean", "dotProduct", and "hamming".
     :vartype metric: str or ~azure.search.documents.indexes.models.VectorSearchAlgorithmMetric
     """
 
     _attribute_map = {
         "metric": {"key": "metric", "type": "str"},
     }
 
     def __init__(
         self, *, metric: Optional[Union[str, "_models.VectorSearchAlgorithmMetric"]] = None, **kwargs: Any
     ) -> None:
         """
         :keyword metric: The similarity metric to use for vector comparisons. Known values are:
-         "cosine", "euclidean", and "dotProduct".
+         "cosine", "euclidean", "dotProduct", and "hamming".
         :paramtype metric: str or ~azure.search.documents.indexes.models.VectorSearchAlgorithmMetric
         """
         super().__init__(**kwargs)
         self.metric = metric
 
 
 class FieldMapping(_serialization.Model):
@@ -3654,15 +3954,15 @@
      returns.
     :vartype ef_construction: int
     :ivar ef_search: The size of the dynamic list containing the nearest neighbors, which is used
      during search time. Increasing this parameter may improve search results, at the expense of
      slower search. At a certain point, increasing this parameter leads to diminishing returns.
     :vartype ef_search: int
     :ivar metric: The similarity metric to use for vector comparisons. Known values are: "cosine",
-     "euclidean", and "dotProduct".
+     "euclidean", "dotProduct", and "hamming".
     :vartype metric: str or ~azure.search.documents.indexes.models.VectorSearchAlgorithmMetric
     """
 
     _validation = {
         "m": {"maximum": 10, "minimum": 4},
         "ef_construction": {"maximum": 1000, "minimum": 100},
         "ef_search": {"maximum": 1000, "minimum": 100},
@@ -3696,15 +3996,15 @@
          returns.
         :paramtype ef_construction: int
         :keyword ef_search: The size of the dynamic list containing the nearest neighbors, which is
          used during search time. Increasing this parameter may improve search results, at the expense
          of slower search. At a certain point, increasing this parameter leads to diminishing returns.
         :paramtype ef_search: int
         :keyword metric: The similarity metric to use for vector comparisons. Known values are:
-         "cosine", "euclidean", and "dotProduct".
+         "cosine", "euclidean", "dotProduct", and "hamming".
         :paramtype metric: str or ~azure.search.documents.indexes.models.VectorSearchAlgorithmMetric
         """
         super().__init__(**kwargs)
         self.m = m
         self.ef_construction = ef_construction
         self.ef_search = ef_search
         self.metric = metric
@@ -6753,15 +7053,15 @@
     All required parameters must be populated in order to send to server.
 
     :ivar name: The name of the field, which must be unique within the fields collection of the
      index or parent field. Required.
     :vartype name: str
     :ivar type: The data type of the field. Required. Known values are: "Edm.String", "Edm.Int32",
      "Edm.Int64", "Edm.Double", "Edm.Boolean", "Edm.DateTimeOffset", "Edm.GeographyPoint",
-     "Edm.ComplexType", "Edm.Single", "Edm.Half", "Edm.Int16", and "Edm.SByte".
+     "Edm.ComplexType", "Edm.Single", "Edm.Half", "Edm.Int16", "Edm.SByte", and "Edm.Byte".
     :vartype type: str or ~azure.search.documents.indexes.models.SearchFieldDataType
     :ivar key: A value indicating whether the field uniquely identifies documents in the index.
      Exactly one top-level field in each index must be chosen as the key field and it must be of
      type Edm.String. Key fields can be used to look up documents directly and update or delete
      specific documents. Default is false for simple fields and null for complex fields.
     :vartype key: bool
     :ivar retrievable: A value indicating whether the field can be returned in a search result. You
@@ -6889,14 +7189,17 @@
      "asciifolding", "elision", "lowercase", "standard", and "uppercase".
     :vartype normalizer: str or ~azure.search.documents.indexes.models.LexicalNormalizerName
     :ivar vector_search_dimensions: The dimensionality of the vector field.
     :vartype vector_search_dimensions: int
     :ivar vector_search_profile_name: The name of the vector search profile that specifies the
      algorithm and vectorizer to use when searching the vector field.
     :vartype vector_search_profile_name: str
+    :ivar vector_encoding_format: The encoding format to interpret the field contents. "packedBit"
+    :vartype vector_encoding_format: str or
+     ~azure.search.documents.indexes.models.VectorEncodingFormat
     :ivar synonym_maps: A list of the names of synonym maps to associate with this field. This
      option can be used only with searchable fields. Currently only one synonym map per field is
      supported. Assigning a synonym map to a field ensures that query terms targeting that field are
      expanded at query-time using the rules in the synonym map. This attribute can be changed on
      existing fields. Must be null or an empty collection for complex fields.
     :vartype synonym_maps: list[str]
     :ivar fields: A list of sub-fields if this is a field of type Edm.ComplexType or
@@ -6922,14 +7225,15 @@
         "facetable": {"key": "facetable", "type": "bool"},
         "analyzer": {"key": "analyzer", "type": "str"},
         "search_analyzer": {"key": "searchAnalyzer", "type": "str"},
         "index_analyzer": {"key": "indexAnalyzer", "type": "str"},
         "normalizer": {"key": "normalizer", "type": "str"},
         "vector_search_dimensions": {"key": "dimensions", "type": "int"},
         "vector_search_profile_name": {"key": "vectorSearchProfile", "type": "str"},
+        "vector_encoding_format": {"key": "vectorEncoding", "type": "str"},
         "synonym_maps": {"key": "synonymMaps", "type": "[str]"},
         "fields": {"key": "fields", "type": "[SearchField]"},
     }
 
     def __init__(
         self,
         *,
@@ -6944,26 +7248,27 @@
         facetable: Optional[bool] = None,
         analyzer: Optional[Union[str, "_models.LexicalAnalyzerName"]] = None,
         search_analyzer: Optional[Union[str, "_models.LexicalAnalyzerName"]] = None,
         index_analyzer: Optional[Union[str, "_models.LexicalAnalyzerName"]] = None,
         normalizer: Optional[Union[str, "_models.LexicalNormalizerName"]] = None,
         vector_search_dimensions: Optional[int] = None,
         vector_search_profile_name: Optional[str] = None,
+        vector_encoding_format: Optional[Union[str, "_models.VectorEncodingFormat"]] = None,
         synonym_maps: Optional[List[str]] = None,
         fields: Optional[List["_models.SearchField"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword name: The name of the field, which must be unique within the fields collection of the
          index or parent field. Required.
         :paramtype name: str
         :keyword type: The data type of the field. Required. Known values are: "Edm.String",
          "Edm.Int32", "Edm.Int64", "Edm.Double", "Edm.Boolean", "Edm.DateTimeOffset",
-         "Edm.GeographyPoint", "Edm.ComplexType", "Edm.Single", "Edm.Half", "Edm.Int16", and
-         "Edm.SByte".
+         "Edm.GeographyPoint", "Edm.ComplexType", "Edm.Single", "Edm.Half", "Edm.Int16", "Edm.SByte",
+         and "Edm.Byte".
         :paramtype type: str or ~azure.search.documents.indexes.models.SearchFieldDataType
         :keyword key: A value indicating whether the field uniquely identifies documents in the index.
          Exactly one top-level field in each index must be chosen as the key field and it must be of
          type Edm.String. Key fields can be used to look up documents directly and update or delete
          specific documents. Default is false for simple fields and null for complex fields.
         :paramtype key: bool
         :keyword retrievable: A value indicating whether the field can be returned in a search result.
@@ -7091,14 +7396,18 @@
          "asciifolding", "elision", "lowercase", "standard", and "uppercase".
         :paramtype normalizer: str or ~azure.search.documents.indexes.models.LexicalNormalizerName
         :keyword vector_search_dimensions: The dimensionality of the vector field.
         :paramtype vector_search_dimensions: int
         :keyword vector_search_profile_name: The name of the vector search profile that specifies the
          algorithm and vectorizer to use when searching the vector field.
         :paramtype vector_search_profile_name: str
+        :keyword vector_encoding_format: The encoding format to interpret the field contents.
+         "packedBit"
+        :paramtype vector_encoding_format: str or
+         ~azure.search.documents.indexes.models.VectorEncodingFormat
         :keyword synonym_maps: A list of the names of synonym maps to associate with this field. This
          option can be used only with searchable fields. Currently only one synonym map per field is
          supported. Assigning a synonym map to a field ensures that query terms targeting that field are
          expanded at query-time using the rules in the synonym map. This attribute can be changed on
          existing fields. Must be null or an empty collection for complex fields.
         :paramtype synonym_maps: list[str]
         :keyword fields: A list of sub-fields if this is a field of type Edm.ComplexType or
@@ -7117,14 +7426,15 @@
         self.facetable = facetable
         self.analyzer = analyzer
         self.search_analyzer = search_analyzer
         self.index_analyzer = index_analyzer
         self.normalizer = normalizer
         self.vector_search_dimensions = vector_search_dimensions
         self.vector_search_profile_name = vector_search_profile_name
+        self.vector_encoding_format = vector_encoding_format
         self.synonym_maps = synonym_maps
         self.fields = fields
 
 
 class SearchIndex(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """Represents a search index definition, which describes the fields and search behavior of an
     index.
@@ -7578,15 +7888,15 @@
     All required parameters must be populated in order to send to server.
 
     :ivar name: The name of the datasource. Required.
     :vartype name: str
     :ivar description: The description of the datasource.
     :vartype description: str
     :ivar type: The type of the datasource. Required. Known values are: "azuresql", "cosmosdb",
-     "azureblob", "azuretable", "mysql", and "adlsgen2".
+     "azureblob", "azuretable", "mysql", "adlsgen2", and "onelake".
     :vartype type: str or ~azure.search.documents.indexes.models.SearchIndexerDataSourceType
     :ivar credentials: Credentials for the datasource. Required.
     :vartype credentials: ~azure.search.documents.indexes.models.DataSourceCredentials
     :ivar container: The data container for the datasource. Required.
     :vartype container: ~azure.search.documents.indexes.models.SearchIndexerDataContainer
     :ivar identity: An explicit managed identity to use for this datasource. If not specified and
      the connection string is a managed identity, the system-assigned managed identity is used. If
@@ -7649,15 +7959,15 @@
     ) -> None:
         """
         :keyword name: The name of the datasource. Required.
         :paramtype name: str
         :keyword description: The description of the datasource.
         :paramtype description: str
         :keyword type: The type of the datasource. Required. Known values are: "azuresql", "cosmosdb",
-         "azureblob", "azuretable", "mysql", and "adlsgen2".
+         "azureblob", "azuretable", "mysql", "adlsgen2", and "onelake".
         :paramtype type: str or ~azure.search.documents.indexes.models.SearchIndexerDataSourceType
         :keyword credentials: Credentials for the datasource. Required.
         :paramtype credentials: ~azure.search.documents.indexes.models.DataSourceCredentials
         :keyword container: The data container for the datasource. Required.
         :paramtype container: ~azure.search.documents.indexes.models.SearchIndexerDataContainer
         :keyword identity: An explicit managed identity to use for this datasource. If not specified
          and the connection string is a managed identity, the system-assigned managed identity is used.
@@ -8742,53 +9052,60 @@
     :vartype max_field_nesting_depth_per_index: int
     :ivar max_complex_collection_fields_per_index: The maximum number of fields of type
      Collection(Edm.ComplexType) allowed in an index.
     :vartype max_complex_collection_fields_per_index: int
     :ivar max_complex_objects_in_collections_per_document: The maximum number of objects in complex
      collections allowed per document.
     :vartype max_complex_objects_in_collections_per_document: int
+    :ivar max_storage_per_index: The maximum amount of storage in bytes allowed per index.
+    :vartype max_storage_per_index: int
     """
 
     _attribute_map = {
         "max_fields_per_index": {"key": "maxFieldsPerIndex", "type": "int"},
         "max_field_nesting_depth_per_index": {"key": "maxFieldNestingDepthPerIndex", "type": "int"},
         "max_complex_collection_fields_per_index": {"key": "maxComplexCollectionFieldsPerIndex", "type": "int"},
         "max_complex_objects_in_collections_per_document": {
             "key": "maxComplexObjectsInCollectionsPerDocument",
             "type": "int",
         },
+        "max_storage_per_index": {"key": "maxStoragePerIndex", "type": "int"},
     }
 
     def __init__(
         self,
         *,
         max_fields_per_index: Optional[int] = None,
         max_field_nesting_depth_per_index: Optional[int] = None,
         max_complex_collection_fields_per_index: Optional[int] = None,
         max_complex_objects_in_collections_per_document: Optional[int] = None,
+        max_storage_per_index: Optional[int] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword max_fields_per_index: The maximum allowed fields per index.
         :paramtype max_fields_per_index: int
         :keyword max_field_nesting_depth_per_index: The maximum depth which you can nest sub-fields in
          an index, including the top-level complex field. For example, a/b/c has a nesting depth of 3.
         :paramtype max_field_nesting_depth_per_index: int
         :keyword max_complex_collection_fields_per_index: The maximum number of fields of type
          Collection(Edm.ComplexType) allowed in an index.
         :paramtype max_complex_collection_fields_per_index: int
         :keyword max_complex_objects_in_collections_per_document: The maximum number of objects in
          complex collections allowed per document.
         :paramtype max_complex_objects_in_collections_per_document: int
+        :keyword max_storage_per_index: The maximum amount of storage in bytes allowed per index.
+        :paramtype max_storage_per_index: int
         """
         super().__init__(**kwargs)
         self.max_fields_per_index = max_fields_per_index
         self.max_field_nesting_depth_per_index = max_field_nesting_depth_per_index
         self.max_complex_collection_fields_per_index = max_complex_collection_fields_per_index
         self.max_complex_objects_in_collections_per_document = max_complex_objects_in_collections_per_document
+        self.max_storage_per_index = max_storage_per_index
 
 
 class SearchServiceStatistics(_serialization.Model):
     """Response from a get service statistics request. If successful, it includes service level
     counters and limits.
 
     All required parameters must be populated in order to send to server.
@@ -10525,14 +10842,98 @@
         super().__init__(**kwargs)
         self.name = name
         self.algorithm_configuration_name = algorithm_configuration_name
         self.vectorizer = vectorizer
         self.compression_configuration_name = compression_configuration_name
 
 
+class VisionVectorizeSkill(SearchIndexerSkill):
+    """Allows you to generate a vector embedding for a given image or text input using the Azure AI
+    Services Vision Vectorize API.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar odata_type: A URI fragment specifying the type of skill. Required.
+    :vartype odata_type: str
+    :ivar name: The name of the skill which uniquely identifies it within the skillset. A skill
+     with no name defined will be given a default name of its 1-based index in the skills array,
+     prefixed with the character '#'.
+    :vartype name: str
+    :ivar description: The description of the skill which describes the inputs, outputs, and usage
+     of the skill.
+    :vartype description: str
+    :ivar context: Represents the level at which operations take place, such as the document root
+     or document content (for example, /document or /document/content). The default is /document.
+    :vartype context: str
+    :ivar inputs: Inputs of the skills could be a column in the source data set, or the output of
+     an upstream skill. Required.
+    :vartype inputs: list[~azure.search.documents.indexes.models.InputFieldMappingEntry]
+    :ivar outputs: The output of a skill is either a field in a search index, or a value that can
+     be consumed as an input by another skill. Required.
+    :vartype outputs: list[~azure.search.documents.indexes.models.OutputFieldMappingEntry]
+    :ivar model_version: The version of the model to use when calling the AI Services Vision
+     service. It will default to the latest available when not specified. Required.
+    :vartype model_version: str
+    """
+
+    _validation = {
+        "odata_type": {"required": True},
+        "inputs": {"required": True},
+        "outputs": {"required": True},
+        "model_version": {"required": True},
+    }
+
+    _attribute_map = {
+        "odata_type": {"key": "@odata\\.type", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "description": {"key": "description", "type": "str"},
+        "context": {"key": "context", "type": "str"},
+        "inputs": {"key": "inputs", "type": "[InputFieldMappingEntry]"},
+        "outputs": {"key": "outputs", "type": "[OutputFieldMappingEntry]"},
+        "model_version": {"key": "modelVersion", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        inputs: List["_models.InputFieldMappingEntry"],
+        outputs: List["_models.OutputFieldMappingEntry"],
+        model_version: str,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        context: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword name: The name of the skill which uniquely identifies it within the skillset. A skill
+         with no name defined will be given a default name of its 1-based index in the skills array,
+         prefixed with the character '#'.
+        :paramtype name: str
+        :keyword description: The description of the skill which describes the inputs, outputs, and
+         usage of the skill.
+        :paramtype description: str
+        :keyword context: Represents the level at which operations take place, such as the document
+         root or document content (for example, /document or /document/content). The default is
+         /document.
+        :paramtype context: str
+        :keyword inputs: Inputs of the skills could be a column in the source data set, or the output
+         of an upstream skill. Required.
+        :paramtype inputs: list[~azure.search.documents.indexes.models.InputFieldMappingEntry]
+        :keyword outputs: The output of a skill is either a field in a search index, or a value that
+         can be consumed as an input by another skill. Required.
+        :paramtype outputs: list[~azure.search.documents.indexes.models.OutputFieldMappingEntry]
+        :keyword model_version: The version of the model to use when calling the AI Services Vision
+         service. It will default to the latest available when not specified. Required.
+        :paramtype model_version: str
+        """
+        super().__init__(name=name, description=description, context=context, inputs=inputs, outputs=outputs, **kwargs)
+        self.odata_type: str = "#Microsoft.Skills.Vision.VectorizeSkill"
+        self.model_version = model_version
+
+
 class WebApiSkill(SearchIndexerSkill):  # pylint: disable=too-many-instance-attributes
     """A skill that can call a Web API endpoint, allowing you to extend a skillset by having it call
     your custom code.
 
     All required parameters must be populated in order to send to server.
 
     :ivar odata_type: A URI fragment specifying the type of skill. Required.
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/_patch.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,39 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
 
 
+class AIStudioModelCatalogName(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The name of the embedding model from the Azure AI Studio Catalog that will be called."""
+
+    OPEN_AI_CLIP_IMAGE_TEXT_EMBEDDINGS_VIT_BASE_PATCH32 = "OpenAI-CLIP-Image-Text-Embeddings-vit-base-patch32"
+    OPEN_AI_CLIP_IMAGE_TEXT_EMBEDDINGS_VI_T_LARGE_PATCH14_336 = (
+        "OpenAI-CLIP-Image-Text-Embeddings-ViT-Large-Patch14-336"
+    )
+    FACEBOOK_DINO_V2_IMAGE_EMBEDDINGS_VI_T_BASE = "Facebook-DinoV2-Image-Embeddings-ViT-Base"
+    FACEBOOK_DINO_V2_IMAGE_EMBEDDINGS_VI_T_GIANT = "Facebook-DinoV2-Image-Embeddings-ViT-Giant"
+    COHERE_EMBED_V3_ENGLISH = "Cohere-embed-v3-english"
+    COHERE_EMBED_V3_MULTILINGUAL = "Cohere-embed-v3-multilingual"
+
+
+class AzureOpenAIModelName(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The Azure Open AI model name that will be called."""
+
+    TEXT_EMBEDDING_ADA002 = "text-embedding-ada-002"
+    TEXT_EMBEDDING3_LARGE = "text-embedding-3-large"
+    TEXT_EMBEDDING3_SMALL = "text-embedding-3-small"
+    EXPERIMENTAL = "experimental"
+
+
 class BlobIndexerDataToExtract(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Specifies the data to extract from Azure blob storage and tells the indexer which data to
     extract from image content when "imageAction" is set to a value other than "none".  This
     applies to embedded image content in a .PDF or other application, or image files such as .jpg
     and .png, in Azure blobs.
     """
 
@@ -1357,14 +1379,17 @@
     used with Collection(Edm.Half)."""
     INT16 = "Edm.Int16"
     """Indicates that a field contains a 16-bit signed integer. This is only valid when used with
     Collection(Edm.Int16)."""
     S_BYTE = "Edm.SByte"
     """Indicates that a field contains a 8-bit signed integer. This is only valid when used with
     Collection(Edm.SByte)."""
+    BYTE = "Edm.Byte"
+    """Indicates that a field contains a 8-bit unsigned integer. This is only valid when used with
+    Collection(Edm.Byte)."""
 
 
 class SearchIndexerDataSourceType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Defines the type of a datasource."""
 
     AZURE_SQL = "azuresql"
     """Indicates an Azure SQL datasource."""
@@ -1374,14 +1399,16 @@
     """Indicates an Azure Blob datasource."""
     AZURE_TABLE = "azuretable"
     """Indicates an Azure Table datasource."""
     MY_SQL = "mysql"
     """Indicates a MySql datasource."""
     ADLS_GEN2 = "adlsgen2"
     """Indicates an ADLS Gen2 datasource."""
+    ONE_LAKE = "onelake"
+    """Indicates a Microsoft Fabric OneLake datasource."""
 
 
 class SentimentSkillLanguage(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Deprecated. The language codes supported for input text by SentimentSkill."""
 
     DA = "da"
     """Danish"""
@@ -2000,29 +2027,47 @@
     UPPERCASE = "uppercase"
     """Normalizes token text to upper case. See
     https://lucene.apache.org/core/6_6_1/analyzers-common/org/apache/lucene/analysis/core/UpperCaseFilter.html"""
     WORD_DELIMITER = "word_delimiter"
     """Splits words into subwords and performs optional transformations on subword groups."""
 
 
+class VectorEncodingFormat(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The encoding format for interpreting vector field contents."""
+
+    PACKED_BIT = "packedBit"
+    """Encoding format representing bits packed into a wider data type."""
+
+
 class VectorSearchAlgorithmKind(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The algorithm used for indexing and querying."""
 
     HNSW = "hnsw"
     """HNSW (Hierarchical Navigable Small World), a type of approximate nearest neighbors algorithm."""
     EXHAUSTIVE_KNN = "exhaustiveKnn"
     """Exhaustive KNN algorithm which will perform brute-force search."""
 
 
 class VectorSearchAlgorithmMetric(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """The similarity metric to use for vector comparisons."""
+    """The similarity metric to use for vector comparisons. It is recommended to choose the same
+    similarity metric as the embedding model was trained on.
+    """
 
     COSINE = "cosine"
+    """Measures the angle between vectors to quantify their similarity, disregarding magnitude. The
+    smaller the angle, the closer the similarity."""
     EUCLIDEAN = "euclidean"
+    """Computes the straight-line distance between vectors in a multi-dimensional space. The smaller
+    the distance, the closer the similarity."""
     DOT_PRODUCT = "dotProduct"
+    """Calculates the sum of element-wise products to gauge alignment and magnitude similarity. The
+    larger and more positive, the closer the similarity."""
+    HAMMING = "hamming"
+    """Only applicable to bit-packed binary data types. Determines dissimilarity by counting differing
+    positions in binary vectors. The fewer differences, the closer the similarity."""
 
 
 class VectorSearchCompressionKind(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The compression method used for indexing and querying."""
 
     SCALAR_QUANTIZATION = "scalarQuantization"
     """Scalar Quantization, a type of compression method. In scalar quantization, the original vectors
@@ -2039,14 +2084,20 @@
 class VectorSearchVectorizerKind(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The vectorization method to be used during query time."""
 
     AZURE_OPEN_AI = "azureOpenAI"
     """Generate embeddings using an Azure OpenAI resource at query time."""
     CUSTOM_WEB_API = "customWebApi"
     """Generate embeddings using a custom web endpoint at query time."""
+    AI_SERVICES_VISION = "aiServicesVision"
+    """Generate embeddings for an image or text input at query time using the Azure AI Services Vision
+    Vectorize API."""
+    AML = "aml"
+    """Generate embeddings using an Azure Machine Learning endpoint deployed via the Azure AI Studio
+    Model Catalog at query time."""
 
 
 class VisualFeature(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The strings indicating what visual feature types to return."""
 
     ADULT = "adult"
     """Visual features recognized as adult persons."""
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._data_sources_operations import DataSourcesOperations
 from ._indexers_operations import IndexersOperations
 from ._skillsets_operations import SkillsetsOperations
 from ._synonym_maps_operations import SynonymMapsOperations
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_aliases_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_aliases_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Iterable, Optional, Type, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -23,26 +24,30 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import SearchServiceClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_create_request(*, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/aliases")
 
     # Construct parameters
@@ -58,15 +63,15 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_request(*, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/aliases")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -87,15 +92,15 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/aliases('{aliasName}')")
     path_format_arguments = {
         "aliasName": _SERIALIZER.url("alias_name", alias_name, "str"),
@@ -128,15 +133,15 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/aliases('{aliasName}')")
     path_format_arguments = {
         "aliasName": _SERIALIZER.url("alias_name", alias_name, "str"),
     }
@@ -158,15 +163,15 @@
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(alias_name: str, *, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/aliases('{aliasName}')")
     path_format_arguments = {
         "aliasName": _SERIALIZER.url("alias_name", alias_name, "str"),
     }
@@ -272,15 +277,15 @@
         :type alias: ~azure.search.documents.indexes.models.SearchAlias or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchAlias or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchAlias
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -353,15 +358,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ListAliasesResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -547,15 +552,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchAlias or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchAlias
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -644,15 +649,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -709,15 +714,15 @@
         :type alias_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchAlias or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchAlias
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -21,14 +22,18 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import SearchServiceClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -41,15 +46,15 @@
     if_none_match: Optional[str] = None,
     skip_indexer_reset_requirement_for_cache: Optional[bool] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/datasources('{dataSourceName}')")
     path_format_arguments = {
         "dataSourceName": _SERIALIZER.url("data_source_name", data_source_name, "str"),
@@ -86,15 +91,15 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/datasources('{dataSourceName}')")
     path_format_arguments = {
         "dataSourceName": _SERIALIZER.url("data_source_name", data_source_name, "str"),
     }
@@ -118,15 +123,15 @@
 
 def build_get_request(
     data_source_name: str, *, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/datasources('{dataSourceName}')")
     path_format_arguments = {
         "dataSourceName": _SERIALIZER.url("data_source_name", data_source_name, "str"),
     }
@@ -146,15 +151,15 @@
 
 def build_list_request(
     *, select: Optional[str] = None, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/datasources")
 
     # Construct parameters
     if select is not None:
@@ -169,15 +174,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_create_request(*, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/datasources")
 
     # Construct parameters
@@ -338,15 +343,15 @@
         :type skip_indexer_reset_requirement_for_cache: bool
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerDataSource or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerDataSource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -435,15 +440,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -500,15 +505,15 @@
         :type data_source_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerDataSource or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerDataSource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -569,15 +574,15 @@
         :type select: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: ListDataSourcesResult or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.ListDataSourcesResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -692,15 +697,15 @@
         :type data_source: ~azure.search.documents.indexes.models.SearchIndexerDataSource or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerDataSource or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerDataSource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_indexers_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_indexers_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -21,28 +22,32 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import SearchServiceClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_reset_request(
     indexer_name: str, *, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')/search.reset")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
     }
@@ -62,15 +67,15 @@
 
 def build_reset_docs_request(
     indexer_name: str, *, overwrite: bool = False, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')/search.resetdocs")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
@@ -93,15 +98,15 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_run_request(indexer_name: str, *, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')/search.run")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
     }
@@ -129,15 +134,15 @@
     skip_indexer_reset_requirement_for_cache: Optional[bool] = None,
     disable_cache_reprocessing_change_detection: Optional[bool] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
@@ -178,15 +183,15 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
     }
@@ -208,15 +213,15 @@
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(indexer_name: str, *, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
     }
@@ -236,15 +241,15 @@
 
 def build_list_request(
     *, select: Optional[str] = None, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers")
 
     # Construct parameters
     if select is not None:
@@ -259,15 +264,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_create_request(*, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers")
 
     # Construct parameters
@@ -285,15 +290,15 @@
 
 def build_get_status_request(
     indexer_name: str, *, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')/search.status")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
     }
@@ -343,15 +348,15 @@
         :type indexer_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -483,15 +488,15 @@
         :param keys_or_ids: Is either a DocumentKeysOrIds type or a IO[bytes] type. Default value is
          None.
         :type keys_or_ids: ~azure.search.documents.indexes.models.DocumentKeysOrIds or IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -561,15 +566,15 @@
         :type indexer_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -749,15 +754,15 @@
         :type disable_cache_reprocessing_change_detection: bool
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexer or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexer
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -847,15 +852,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -912,15 +917,15 @@
         :type indexer_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexer or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexer
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -981,15 +986,15 @@
         :type select: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: ListIndexersResult or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.ListIndexersResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1104,15 +1109,15 @@
         :type indexer: ~azure.search.documents.indexes.models.SearchIndexer or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexer or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexer
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1181,15 +1186,15 @@
         :type indexer_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerStatus or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerStatus
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_indexes_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_indexes_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Iterable, Optional, Type, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -23,26 +24,30 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import SearchServiceClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_create_request(*, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexes")
 
     # Construct parameters
@@ -60,15 +65,15 @@
 
 def build_list_request(
     *, select: Optional[str] = None, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexes")
 
     # Construct parameters
     if select is not None:
@@ -92,15 +97,15 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexes('{indexName}')")
     path_format_arguments = {
         "indexName": _SERIALIZER.url("index_name", index_name, "str"),
@@ -135,15 +140,15 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexes('{indexName}')")
     path_format_arguments = {
         "indexName": _SERIALIZER.url("index_name", index_name, "str"),
     }
@@ -165,15 +170,15 @@
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(index_name: str, *, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexes('{indexName}')")
     path_format_arguments = {
         "indexName": _SERIALIZER.url("index_name", index_name, "str"),
     }
@@ -193,15 +198,15 @@
 
 def build_get_statistics_request(
     index_name: str, *, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexes('{indexName}')/search.stats")
     path_format_arguments = {
         "indexName": _SERIALIZER.url("index_name", index_name, "str"),
     }
@@ -221,15 +226,15 @@
 
 def build_analyze_request(
     index_name: str, *, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexes('{indexName}')/search.analyze")
     path_format_arguments = {
         "indexName": _SERIALIZER.url("index_name", index_name, "str"),
@@ -338,15 +343,15 @@
         :type index: ~azure.search.documents.indexes.models.SearchIndex or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndex or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndex
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -423,15 +428,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ListIndexesResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -639,15 +644,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndex or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndex
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -738,15 +743,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -803,15 +808,15 @@
         :type index_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndex or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndex
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -870,15 +875,15 @@
         :type index_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: GetIndexStatisticsResult or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.GetIndexStatisticsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1002,15 +1007,15 @@
         :type request: ~azure.search.documents.indexes.models.AnalyzeRequest or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: AnalyzeResult or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.AnalyzeResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_patch.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Optional, TypeVar
+import sys
+from typing import Any, Callable, Dict, Optional, Type, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -20,26 +21,30 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import SearchServiceClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_service_statistics_request(*, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/servicestats")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -49,27 +54,28 @@
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 class SearchServiceClientOperationsMixin(SearchServiceClientMixinABC):
+
     @distributed_trace
     def get_service_statistics(
         self, request_options: Optional[_models.RequestOptions] = None, **kwargs: Any
     ) -> _models.SearchServiceStatistics:
         """Gets service level statistics for a search service.
 
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchServiceStatistics or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchServiceStatistics
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -21,14 +22,18 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import SearchServiceClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -42,15 +47,15 @@
     skip_indexer_reset_requirement_for_cache: Optional[bool] = None,
     disable_cache_reprocessing_change_detection: Optional[bool] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/skillsets('{skillsetName}')")
     path_format_arguments = {
         "skillsetName": _SERIALIZER.url("skillset_name", skillset_name, "str"),
@@ -91,15 +96,15 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/skillsets('{skillsetName}')")
     path_format_arguments = {
         "skillsetName": _SERIALIZER.url("skillset_name", skillset_name, "str"),
     }
@@ -123,15 +128,15 @@
 
 def build_get_request(
     skillset_name: str, *, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/skillsets('{skillsetName}')")
     path_format_arguments = {
         "skillsetName": _SERIALIZER.url("skillset_name", skillset_name, "str"),
     }
@@ -151,15 +156,15 @@
 
 def build_list_request(
     *, select: Optional[str] = None, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/skillsets")
 
     # Construct parameters
     if select is not None:
@@ -174,15 +179,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_create_request(*, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/skillsets")
 
     # Construct parameters
@@ -200,15 +205,15 @@
 
 def build_reset_skills_request(
     skillset_name: str, *, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/skillsets('{skillsetName}')/search.resetskills")
     path_format_arguments = {
         "skillsetName": _SERIALIZER.url("skillset_name", skillset_name, "str"),
@@ -388,15 +393,15 @@
         :type disable_cache_reprocessing_change_detection: bool
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerSkillset or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerSkillset
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -486,15 +491,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -551,15 +556,15 @@
         :type skillset_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerSkillset or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerSkillset
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -620,15 +625,15 @@
         :type select: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: ListSkillsetsResult or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.ListSkillsetsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -745,15 +750,15 @@
         :type skillset: ~azure.search.documents.indexes.models.SearchIndexerSkillset or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SearchIndexerSkillset or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SearchIndexerSkillset
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -887,15 +892,15 @@
         :type skill_names: ~azure.search.documents.indexes.models.SkillNames or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.13)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -21,14 +22,18 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import SearchServiceClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -40,15 +45,15 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/synonymmaps('{synonymMapName}')")
     path_format_arguments = {
         "synonymMapName": _SERIALIZER.url("synonym_map_name", synonym_map_name, "str"),
@@ -81,15 +86,15 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/synonymmaps('{synonymMapName}')")
     path_format_arguments = {
         "synonymMapName": _SERIALIZER.url("synonym_map_name", synonym_map_name, "str"),
     }
@@ -113,15 +118,15 @@
 
 def build_get_request(
     synonym_map_name: str, *, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/synonymmaps('{synonymMapName}')")
     path_format_arguments = {
         "synonymMapName": _SERIALIZER.url("synonym_map_name", synonym_map_name, "str"),
     }
@@ -141,15 +146,15 @@
 
 def build_list_request(
     *, select: Optional[str] = None, x_ms_client_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/synonymmaps")
 
     # Construct parameters
     if select is not None:
@@ -164,15 +169,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_create_request(*, x_ms_client_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-Preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-05-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/synonymmaps")
 
     # Construct parameters
@@ -321,15 +326,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SynonymMap or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SynonymMap
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -417,15 +422,15 @@
         :type if_none_match: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -482,15 +487,15 @@
         :type synonym_map_name: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SynonymMap or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SynonymMap
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -551,15 +556,15 @@
         :type select: str
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: ListSynonymMapsResult or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.ListSynonymMapsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -674,15 +679,15 @@
         :type synonym_map: ~azure.search.documents.indexes.models.SynonymMap or IO[bytes]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
         :return: SynonymMap or the result of cls(response)
         :rtype: ~azure.search.documents.indexes.models.SynonymMap
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_search_index_client.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_search_index_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_search_indexer_client.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_search_indexer_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_utils.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/_search_index_client.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/aio/_search_index_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/_search_indexer_client.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/aio/_search_indexer_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,25 @@
     SimpleField,
     SearchIndex,
 )
 from . import _edm
 from ..._generated.models import SuggestOptions
 from .._generated.models import (
     SearchAlias,
+    AIServicesVisionParameters,
+    AIServicesVisionVectorizer,
+    AIStudioModelCatalogName,
+    AzureMachineLearningParameters,
     AzureMachineLearningSkill,
+    AzureMachineLearningVectorizer,
     AnalyzeResult,
     AnalyzedTokenInfo,
     AsciiFoldingTokenFilter,
     AzureOpenAIEmbeddingSkill,
+    AzureOpenAIModelName,
     AzureOpenAIParameters,
     AzureOpenAIVectorizer,
     BlobIndexerDataToExtract,
     BlobIndexerImageAction,
     BlobIndexerParsingMode,
     BlobIndexerPDFTextRotationAlgorithm,
     BM25SimilarityAlgorithm,
@@ -204,24 +210,26 @@
     TextWeights,
     TokenCharacterKind,
     TokenFilter,
     TokenFilterName,
     TruncateTokenFilter,
     UaxUrlEmailTokenizer,
     UniqueTokenFilter,
+    VectorEncodingFormat,
     VectorSearch,
     VectorSearchAlgorithmConfiguration,
     VectorSearchAlgorithmKind,
     VectorSearchAlgorithmMetric,
     VectorSearchCompressionConfiguration,
     VectorSearchCompressionTargetDataType,
     VectorSearchProfile,
     VectorSearchVectorizer,
     VectorSearchVectorizerKind,
     VisualFeature,
+    VisionVectorizeSkill,
     WebApiSkill,
     WordDelimiterTokenFilter,
 )
 from ._models import (
     AnalyzeTextOptions,
     CustomAnalyzer,
     EntityRecognitionSkill,
@@ -245,22 +253,28 @@
 
 class PathHierarchyTokenizer(PathHierarchyTokenizerV2):
     pass
 
 
 __all__ = (
     "SearchAlias",
+    "AIServicesVisionParameters",
+    "AIServicesVisionVectorizer",
+    "AIStudioModelCatalogName",
     "AnalyzeTextOptions",
     "AnalyzeResult",
     "AnalyzedTokenInfo",
     "AsciiFoldingTokenFilter",
     "AzureOpenAIEmbeddingSkill",
+    "AzureOpenAIModelName",
     "AzureOpenAIParameters",
     "AzureOpenAIVectorizer",
+    "AzureMachineLearningParameters",
     "AzureMachineLearningSkill",
+    "AzureMachineLearningVectorizer",
     "BlobIndexerDataToExtract",
     "BlobIndexerImageAction",
     "BlobIndexerParsingMode",
     "BlobIndexerPDFTextRotationAlgorithm",
     "BM25SimilarityAlgorithm",
     "CharFilter",
     "CharFilterName",
@@ -437,21 +451,23 @@
     "TextWeights",
     "TokenCharacterKind",
     "TokenFilter",
     "TokenFilterName",
     "TruncateTokenFilter",
     "UaxUrlEmailTokenizer",
     "UniqueTokenFilter",
+    "VectorEncodingFormat",
     "VectorSearch",
     "VectorSearchAlgorithmConfiguration",
     "VectorSearchAlgorithmKind",
     "VectorSearchAlgorithmMetric",
     "VectorSearchCompressionConfiguration",
     "VectorSearchCompressionTargetDataType",
     "VectorSearchProfile",
     "VectorSearchVectorizer",
     "VectorSearchVectorizerKind",
     "VisualFeature",
+    "VisionVectorizeSkill",
     "WebApiSkill",
     "WordDelimiterTokenFilter",
     "SearchFieldDataType",
 )
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/_edm.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/models/_edm.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/_index.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/models/_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     All required parameters must be populated in order to send to Azure.
 
     :ivar name: The name of the field, which must be unique within the fields collection of the
         index or parent field. Required.
     :vartype name: str
     :ivar type: The data type of the field. Required. Known values are: "Edm.String", "Edm.Int32",
         "Edm.Int64", "Edm.Double", "Edm.Boolean", "Edm.DateTimeOffset", "Edm.GeographyPoint",
-        "Edm.ComplexType", and "Edm.Single".
+        "Edm.ComplexType", "Edm.Single", "Edm.Half", "Edm.Int16", "Edm.SByte", and "Edm.Byte".
     :vartype type: str or ~azure.search.documents.indexes.models.SearchFieldDataType
     :ivar key: A value indicating whether the field uniquely identifies documents in the index.
         Exactly one top-level field in each index must be chosen as the key field and it must be of
         type Edm.String. Key fields can be used to look up documents directly and update or delete
         specific documents. Default is false for simple fields and null for complex fields.
     :vartype key: bool
     :ivar stored: An immutable value indicating whether the field will be persisted separately on
@@ -167,14 +167,16 @@
         supported. Assigning a synonym map to a field ensures that query terms targeting that field are
         expanded at query-time using the rules in the synonym map. This attribute can be changed on
         existing fields. Must be null or an empty collection for complex fields.
     :vartype synonym_map_names: list[str]
     :ivar fields: A list of sub-fields if this is a field of type Edm.ComplexType or
         Collection(Edm.ComplexType). Must be null or empty for simple fields.
     :vartype fields: list[~azure.search.documents.indexes.models.SearchField]
+    :ivar vector_encoding_format: The encoding format to interpret the field contents. "packedBit"
+    :vartype vector_encoding_format: str or ~azure.search.documents.indexes.models.VectorEncodingFormat
     """
 
     def __init__(self, **kwargs):
         self.name = kwargs["name"]
         self.type = kwargs["type"]
         self.key = kwargs.get("key", None)
         self.hidden = kwargs.get("hidden", None)
@@ -187,14 +189,15 @@
         self.search_analyzer_name = kwargs.get("search_analyzer_name", None)
         self.index_analyzer_name = kwargs.get("index_analyzer_name", None)
         self.normalizer_name = kwargs.get("normalizer_name", None)
         self.synonym_map_names = kwargs.get("synonym_map_names", None)
         self.fields = kwargs.get("fields", None)
         self.vector_search_dimensions = kwargs.get("vector_search_dimensions", None)
         self.vector_search_profile_name = kwargs.get("vector_search_profile_name", None)
+        self.vector_encoding_format = kwargs.get("vector_encoding_format", None)
 
     def _to_generated(self) -> _SearchField:
         fields = [pack_search_field(x) for x in self.fields] if self.fields else None
         retrievable = not self.hidden if self.hidden is not None else None
         return _SearchField(
             name=self.name,
             type=self.type,
@@ -209,14 +212,15 @@
             search_analyzer=self.search_analyzer_name,
             index_analyzer=self.index_analyzer_name,
             normalizer=self.normalizer_name,
             synonym_maps=self.synonym_map_names,
             fields=fields,
             vector_search_dimensions=self.vector_search_dimensions,
             vector_search_profile_name=self.vector_search_profile_name,
+            vector_encoding_format=self.vector_encoding_format,
         )
 
     @classmethod
     def _from_generated(cls, search_field) -> Optional["SearchField"]:
         if not search_field:
             return None
         # pylint:disable=protected-access
@@ -240,14 +244,15 @@
             search_analyzer_name=search_field.search_analyzer,
             index_analyzer_name=search_field.index_analyzer,
             normalizer_name=normalizer,
             synonym_map_names=search_field.synonym_maps,
             fields=fields,
             vector_search_dimensions=search_field.vector_search_dimensions,
             vector_search_profile_name=search_field.vector_search_profile_name,
+            vector_encoding_format=search_field.vector_encoding_format,
         )
 
     def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> MutableMapping[str, Any]:
         """Return the JSON that would be sent to server from this model.
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
@@ -675,17 +680,19 @@
     def _from_generated(cls, search_index) -> "SearchIndex":
         if search_index.analyzers:
             analyzers = [unpack_analyzer(x) for x in search_index.analyzers]  # type: ignore
         else:
             analyzers = None
         if search_index.tokenizers:
             tokenizers = [
-                PatternTokenizer._from_generated(x)  # pylint:disable=protected-access
-                if isinstance(x, _PatternTokenizer)
-                else x
+                (
+                    PatternTokenizer._from_generated(x)  # pylint:disable=protected-access
+                    if isinstance(x, _PatternTokenizer)
+                    else x
+                )
                 for x in search_index.tokenizers
             ]
         else:
             tokenizers = None
         if search_index.fields:
             fields = [SearchField._from_generated(x) for x in search_index.fields]  # pylint:disable=protected-access
         else:
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/_models.py` & `azure-search-documents-11.6.0b4/azure/search/documents/indexes/models/_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -950,17 +950,17 @@
         self.encryption_key = kwargs.get("encryption_key", None)
         self.e_tag = kwargs.get("e_tag", None)
 
     def _to_generated(self):
         return _SynonymMap(
             name=self.name,
             synonyms="\n".join(self.synonyms),
-            encryption_key=self.encryption_key._to_generated()  # pylint:disable=protected-access
-            if self.encryption_key
-            else None,
+            encryption_key=(
+                self.encryption_key._to_generated() if self.encryption_key else None  # pylint:disable=protected-access
+            ),
             e_tag=self.e_tag,
         )
 
     @classmethod
     def _from_generated(cls, synonym_map) -> "SynonymMap":
         return cls(
             name=synonym_map.name,
```

### Comparing `azure-search-documents-11.6.0b3/azure/search/documents/models/__init__.py` & `azure-search-documents-11.6.0b4/azure/search/documents/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,51 +22,67 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # --------------------------------------------------------------------------
 
 from .._generated.models import (
     AutocompleteMode,
+    HybridCountAndFacetMode,
+    HybridSearch,
     IndexAction,
     IndexingResult,
     QueryAnswerResult,
     QueryAnswerType,
     QueryCaptionResult,
     QueryCaptionType,
     QueryDebugMode,
     QueryLanguage,
     QuerySpellerType,
     QueryType,
     ScoringStatistics,
     SearchMode,
+    SearchScoreThreshold,
     SemanticErrorMode,
     SemanticErrorReason,
     SemanticSearchResultsType,
     VectorFilterMode,
+    VectorSimilarityThreshold,
+    VectorThreshold,
+    VectorThresholdKind,
+    VectorizableImageBinaryQuery,
+    VectorizableImageUrlQuery,
     VectorizedQuery,
     VectorizableTextQuery,
     VectorQuery,
 )
 
 
 __all__ = (
     "AutocompleteMode",
+    "HybridCountAndFacetMode",
+    "HybridSearch",
     "IndexAction",
     "IndexingResult",
     "QueryAnswerResult",
     "QueryAnswerType",
     "QueryCaptionResult",
     "QueryCaptionType",
     "QueryDebugMode",
     "QueryLanguage",
     "QuerySpellerType",
     "QueryType",
     "ScoringStatistics",
     "SearchMode",
+    "SearchScoreThreshold",
     "SemanticErrorMode",
     "SemanticErrorReason",
     "SemanticSearchResultsType",
     "VectorFilterMode",
+    "VectorSimilarityThreshold",
+    "VectorThreshold",
+    "VectorThresholdKind",
+    "VectorizableImageBinaryQuery",
+    "VectorizableImageUrlQuery",
     "VectorizedQuery",
     "VectorizableTextQuery",
     "VectorQuery",
 )
```

### Comparing `azure-search-documents-11.6.0b3/azure_search_documents.egg-info/PKG-INFO` & `azure-search-documents-11.6.0b4/azure_search_documents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-search-documents
-Version: 11.6.0b3
+Version: 11.6.0b4
 Summary: Microsoft Azure Cognitive Search Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/search/azure-search-documents
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -16,17 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: azure-core>=1.28.0
-Requires-Dist: azure-common>=1.1
-Requires-Dist: isodate>=0.6.0
 
 # Azure AI Search client library for Python
 
 [Azure AI Search](https://docs.microsoft.com/azure/search/) (formerly known as "Azure Cognitive Search") is an AI-powered information retrieval platform that helps developers build rich search experiences and generative AI apps that combine large language models with enterprise data.
 
 Azure AI Search is well suited for the following application scenarios:
```

### Comparing `azure-search-documents-11.6.0b3/azure_search_documents.egg-info/SOURCES.txt` & `azure-search-documents-11.6.0b4/azure_search_documents.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 azure/search/documents/py.typed
 azure/search/documents/_generated/__init__.py
 azure/search/documents/_generated/_configuration.py
 azure/search/documents/_generated/_patch.py
 azure/search/documents/_generated/_search_index_client.py
 azure/search/documents/_generated/_serialization.py
 azure/search/documents/_generated/_vendor.py
-azure/search/documents/_generated/py.typed
 azure/search/documents/_generated/aio/__init__.py
 azure/search/documents/_generated/aio/_configuration.py
 azure/search/documents/_generated/aio/_patch.py
 azure/search/documents/_generated/aio/_search_index_client.py
 azure/search/documents/_generated/aio/operations/__init__.py
 azure/search/documents/_generated/aio/operations/_documents_operations.py
 azure/search/documents/_generated/aio/operations/_patch.py
@@ -53,15 +52,14 @@
 azure/search/documents/indexes/_utils.py
 azure/search/documents/indexes/_generated/__init__.py
 azure/search/documents/indexes/_generated/_configuration.py
 azure/search/documents/indexes/_generated/_patch.py
 azure/search/documents/indexes/_generated/_search_service_client.py
 azure/search/documents/indexes/_generated/_serialization.py
 azure/search/documents/indexes/_generated/_vendor.py
-azure/search/documents/indexes/_generated/py.typed
 azure/search/documents/indexes/_generated/aio/__init__.py
 azure/search/documents/indexes/_generated/aio/_configuration.py
 azure/search/documents/indexes/_generated/aio/_patch.py
 azure/search/documents/indexes/_generated/aio/_search_service_client.py
 azure/search/documents/indexes/_generated/aio/_vendor.py
 azure/search/documents/indexes/_generated/aio/operations/__init__.py
 azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py
```

### Comparing `azure-search-documents-11.6.0b3/samples/README.md` & `azure-search-documents-11.6.0b4/samples/README.md`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_analyze_text_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_analyze_text_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_authentication_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_authentication_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_autocomplete_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_autocomplete_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_buffered_sender_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_buffered_sender_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_crud_operations_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_crud_operations_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_data_source_operations_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_data_source_operations_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_facet_query_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_facet_query_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_filter_query_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_filter_query_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_get_document_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_get_document_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_index_alias_crud_operations_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_index_alias_crud_operations_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_index_client_send_request_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_index_client_send_request_async.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     index_name = os.environ["AZURE_SEARCH_INDEX_NAME"]
     key = os.environ["AZURE_SEARCH_API_KEY"]
 
     client = SearchIndexClient(endpoint, AzureKeyCredential(key))
 
     # The `send_request` method can send custom HTTP requests that share the client's existing pipeline,
     # while adding convenience for endpoint construction.
-    request = HttpRequest(method="GET", url=f"/indexes('{index_name}')?api-version=2024-03-01-Preview")
+    request = HttpRequest(method="GET", url=f"/indexes('{index_name}')?api-version=2024-05-01-preview")
     async with client:
         response = await client.send_request(request)
     response.raise_for_status()
     response_body = response.json()
     print(response_body)
```

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_index_crud_operations_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_index_crud_operations_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_indexers_operations_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_indexers_operations_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_query_session_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_query_session_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_search_client_send_request_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_search_client_send_request_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     index_name = os.environ["AZURE_SEARCH_INDEX_NAME"]
     key = os.environ["AZURE_SEARCH_API_KEY"]
 
     client = SearchClient(endpoint, index_name, AzureKeyCredential(key))
 
     # The `send_request` method can send custom HTTP requests that share the client's existing pipeline,
     # while adding convenience for endpoint construction.
-    request = HttpRequest(method="GET", url=f"/docs/$count?api-version=2024-03-01-Preview")
+    request = HttpRequest(method="GET", url=f"/docs/$count?api-version=2024-05-01-preview")
     async with client:
         response = await client.send_request(request)
     response.raise_for_status()
     response_body = response.json()
     print(response_body)
```

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_semantic_search_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_semantic_search_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_simple_query_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_simple_query_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_suggestions_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_suggestions_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_synonym_map_operations_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_synonym_map_operations_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/async_samples/sample_vector_search_async.py` & `azure-search-documents-11.6.0b4/samples/async_samples/sample_vector_search_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_analyze_text.py` & `azure-search-documents-11.6.0b4/samples/sample_analyze_text.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_authentication.py` & `azure-search-documents-11.6.0b4/samples/sample_authentication.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_autocomplete.py` & `azure-search-documents-11.6.0b4/samples/sample_autocomplete.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_buffered_sender.py` & `azure-search-documents-11.6.0b4/samples/sample_buffered_sender.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_crud_operations.py` & `azure-search-documents-11.6.0b4/samples/sample_crud_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_data_source_operations.py` & `azure-search-documents-11.6.0b4/samples/sample_data_source_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_facet_query.py` & `azure-search-documents-11.6.0b4/samples/sample_facet_query.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_filter_query.py` & `azure-search-documents-11.6.0b4/samples/sample_filter_query.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_get_document.py` & `azure-search-documents-11.6.0b4/samples/sample_get_document.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_index_alias_crud_operations.py` & `azure-search-documents-11.6.0b4/samples/sample_index_alias_crud_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_index_client_send_request.py` & `azure-search-documents-11.6.0b4/samples/sample_index_client_send_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     index_name = os.environ["AZURE_SEARCH_INDEX_NAME"]
     key = os.environ["AZURE_SEARCH_API_KEY"]
 
     client = SearchIndexClient(endpoint, AzureKeyCredential(key))
 
     # The `send_request` method can send custom HTTP requests that share the client's existing pipeline,
     # while adding convenience for endpoint construction.
-    request = HttpRequest(method="GET", url=f"/indexes('{index_name}')?api-version=2024-03-01-Preview")
+    request = HttpRequest(method="GET", url=f"/indexes('{index_name}')?api-version=2024-05-01-preview")
     response = client.send_request(request)
     response.raise_for_status()
     response_body = response.json()
     print(response_body)
 
 
 if __name__ == "__main__":
```

### Comparing `azure-search-documents-11.6.0b3/samples/sample_index_crud_operations.py` & `azure-search-documents-11.6.0b4/samples/sample_index_crud_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_indexer_datasource_skillset.py` & `azure-search-documents-11.6.0b4/samples/sample_indexer_datasource_skillset.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_indexers_operations.py` & `azure-search-documents-11.6.0b4/samples/sample_indexers_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_query_session.py` & `azure-search-documents-11.6.0b4/samples/sample_query_session.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_search_client_send_request.py` & `azure-search-documents-11.6.0b4/samples/sample_search_client_send_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     index_name = os.environ["AZURE_SEARCH_INDEX_NAME"]
     key = os.environ["AZURE_SEARCH_API_KEY"]
 
     client = SearchClient(endpoint, index_name, AzureKeyCredential(key))
 
     # The `send_request` method can send custom HTTP requests that share the client's existing pipeline,
     # while adding convenience for endpoint construction.
-    request = HttpRequest(method="GET", url=f"/docs/$count?api-version=2024-03-01-Preview")
+    request = HttpRequest(method="GET", url=f"/docs/$count?api-version=2024-05-01-preview")
     response = client.send_request(request)
     response.raise_for_status()
     response_body = response.json()
     print(response_body)
 
 
 if __name__ == "__main__":
```

### Comparing `azure-search-documents-11.6.0b3/samples/sample_semantic_search.py` & `azure-search-documents-11.6.0b4/samples/sample_semantic_search.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_simple_query.py` & `azure-search-documents-11.6.0b4/samples/sample_simple_query.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_suggestions.py` & `azure-search-documents-11.6.0b4/samples/sample_suggestions.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_synonym_map_operations.py` & `azure-search-documents-11.6.0b4/samples/sample_synonym_map_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/samples/sample_vector_search.py` & `azure-search-documents-11.6.0b4/samples/sample_vector_search.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/setup.py` & `azure-search-documents-11.6.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/async_tests/test_buffered_sender_async.py` & `azure-search-documents-11.6.0b4/tests/test_buffered_sender.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,149 +1,154 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 from unittest import mock
 import pytest
-from azure.search.documents.aio import (
+from azure.search.documents import (
     SearchIndexingBufferedSender,
 )
 from azure.core.credentials import AzureKeyCredential
 from azure.core.exceptions import HttpResponseError, ServiceResponseTimeoutError
 from azure.search.documents.models import IndexingResult
 
 CREDENTIAL = AzureKeyCredential(key="test_api_key")
 
 
-class TestSearchBatchingClientAsync:
-    async def test_search_indexing_buffered_sender_kwargs(self):
-        async with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, window=100) as client:
+class TestSearchBatchingClient:
+    def test_search_indexing_buffered_sender_kwargs(self):
+        with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, window=100) as client:
             assert client._batch_action_count == 512
             assert client._max_retries_per_action == 3
             assert client._auto_flush_interval == 60
             assert client._auto_flush
 
-    async def test_batch_queue(self):
-        async with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
+    def test_batch_queue(self):
+        with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
             assert client._index_documents_batch
-            await client.upload_documents(["upload1"])
-            await client.delete_documents(["delete1", "delete2"])
-            await client.merge_documents(["merge1", "merge2", "merge3"])
-            await client.merge_or_upload_documents(["merge_or_upload1"])
+            client.upload_documents(["upload1"])
+            client.delete_documents(["delete1", "delete2"])
+            client.merge_documents(["merge1", "merge2", "merge3"])
+            client.merge_or_upload_documents(["merge_or_upload1"])
             assert len(client.actions) == 7
-            actions = await client._index_documents_batch.dequeue_actions()
+            actions = client._index_documents_batch.dequeue_actions()
             assert len(client.actions) == 0
-            await client._index_documents_batch.enqueue_actions(actions)
+            client._index_documents_batch.enqueue_actions(actions)
+            assert len(client.actions) == 7
+            actions = client._index_documents_batch.dequeue_actions()
+            assert len(client.actions) == 0
+            for action in actions:
+                client._index_documents_batch.enqueue_actions(action)
             assert len(client.actions) == 7
 
     @mock.patch(
-        "azure.search.documents.aio._search_indexing_buffered_sender_async.SearchIndexingBufferedSender._process_if_needed"
+        "azure.search.documents._search_indexing_buffered_sender.SearchIndexingBufferedSender._process_if_needed"
     )
-    async def test_process_if_needed(self, mock_process_if_needed):
-        async with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL) as client:
-            await client.upload_documents(["upload1"])
-            await client.delete_documents(["delete1", "delete2"])
+    def test_process_if_needed(self, mock_process_if_needed):
+        with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL) as client:
+            client.upload_documents(["upload1"])
+            client.delete_documents(["delete1", "delete2"])
         assert mock_process_if_needed.called
 
-    @mock.patch(
-        "azure.search.documents.aio._search_indexing_buffered_sender_async.SearchIndexingBufferedSender._cleanup"
-    )
-    async def test_context_manager(self, mock_cleanup):
-        async with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
-            await client.upload_documents(["upload1"])
-            await client.delete_documents(["delete1", "delete2"])
+    @mock.patch("azure.search.documents._search_indexing_buffered_sender.SearchIndexingBufferedSender._cleanup")
+    def test_context_manager(self, mock_cleanup):
+        with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
+            client.upload_documents(["upload1"])
+            client.delete_documents(["delete1", "delete2"])
         assert mock_cleanup.called
 
-    async def test_flush(self):
+    def test_flush(self):
         DOCUMENT = {
             "category": "Hotel",
             "hotelId": "1000",
             "rating": 4.0,
             "rooms": [],
             "hotelName": "Azure Inn",
         }
         with mock.patch.object(
             SearchIndexingBufferedSender,
             "_index_documents_actions",
             side_effect=HttpResponseError("Error"),
         ):
-            async with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
+            with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
                 client._index_key = "hotelId"
-                await client.upload_documents([DOCUMENT])
-                await client.flush()
+                client.upload_documents([DOCUMENT])
+                client.flush()
                 assert len(client.actions) == 0
 
-    async def test_callback_new(self):
-        on_new = mock.AsyncMock()
-        async with SearchIndexingBufferedSender(
+    def test_callback_new(self):
+        on_new = mock.Mock()
+        with SearchIndexingBufferedSender(
             "endpoint", "index name", CREDENTIAL, auto_flush=False, on_new=on_new
         ) as client:
-            await client.upload_documents(["upload1"])
+            client.upload_documents(["upload1"])
             assert on_new.called
 
-    async def test_callback_error(self):
-        async def mock_fail_index_documents(actions, timeout=86400):
+    def test_callback_error(self):
+        def mock_fail_index_documents(actions, timeout=86400):
             if len(actions) > 0:
                 result = IndexingResult()
                 result.key = actions[0].additional_properties.get("id")
                 result.status_code = 400
                 result.succeeded = False
                 self.uploaded = self.uploaded + len(actions) - 1
                 return [result]
 
-        on_error = mock.AsyncMock()
-        async with SearchIndexingBufferedSender(
+        on_error = mock.Mock()
+        with SearchIndexingBufferedSender(
             "endpoint", "index name", CREDENTIAL, auto_flush=False, on_error=on_error
         ) as client:
             client._index_documents_actions = mock_fail_index_documents
             client._index_key = "id"
-            await client.upload_documents({"id": 0})
-            await client.flush()
+            client.upload_documents({"id": 0})
+            client.flush()
             assert on_error.called
 
-    async def test_callback_error_on_timeout(self):
-        async def mock_fail_index_documents(actions, timeout=86400):
+    def test_callback_error_on_timeout(self):
+        def mock_fail_index_documents(actions, timeout=86400):
+            import time
+
             if len(actions) > 0:
                 result = IndexingResult()
                 result.key = actions[0].additional_properties.get("id")
                 result.status_code = 400
                 result.succeeded = False
                 self.uploaded = self.uploaded + len(actions) - 1
                 time.sleep(1)
                 return [result]
 
-        on_error = mock.AsyncMock()
-        async with SearchIndexingBufferedSender(
+        on_error = mock.Mock()
+        with SearchIndexingBufferedSender(
             "endpoint", "index name", CREDENTIAL, auto_flush=False, on_error=on_error
         ) as client:
             client._index_documents_actions = mock_fail_index_documents
             client._index_key = "id"
-            await client.upload_documents([{"id": 0}, {"id": 1}])
+            client.upload_documents([{"id": 0}, {"id": 1}])
             with pytest.raises(ServiceResponseTimeoutError):
-                await client.flush(timeout=-1)
+                client.flush(timeout=-1)
             assert on_error.call_count == 2
 
-    async def test_callback_progress(self):
-        async def mock_successful_index_documents(actions, timeout=86400):
+    def test_callback_progress(self):
+        def mock_successful_index_documents(actions, timeout=86400):
             if len(actions) > 0:
                 result = IndexingResult()
                 result.key = actions[0].additional_properties.get("id")
                 result.status_code = 200
                 result.succeeded = True
                 return [result]
 
-        on_progress = mock.AsyncMock()
-        on_remove = mock.AsyncMock()
-        async with SearchIndexingBufferedSender(
+        on_progress = mock.Mock()
+        on_remove = mock.Mock()
+        with SearchIndexingBufferedSender(
             "endpoint",
             "index name",
             CREDENTIAL,
             auto_flush=False,
             on_progress=on_progress,
             on_remove=on_remove,
         ) as client:
             client._index_documents_actions = mock_successful_index_documents
             client._index_key = "id"
-            await client.upload_documents({"id": 0})
-            await client.flush()
+            client.upload_documents({"id": 0})
+            client.flush()
             assert on_progress.called
             assert on_remove.called
```

### Comparing `azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_async.py` & `azure-search-documents-11.6.0b4/tests/async_tests/test_search_client_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 # Licensed under the MIT License.
 # ------------------------------------
 from unittest import mock
 from azure.core.credentials import AzureKeyCredential
 from azure.search.documents._generated.models import SearchDocumentsResult, SearchResult
 from azure.search.documents.aio import SearchClient
 from azure.search.documents.aio._search_client_async import AsyncSearchPageIterator
+from test_search_index_client_async import await_prepared_test
 
 CREDENTIAL = AzureKeyCredential(key="test_api_key")
 
 
 class TestSearchClientAsync:
+    @await_prepared_test
     @mock.patch(
         "azure.search.documents._generated.aio.operations._documents_operations.DocumentsOperations.search_post"
     )
     async def test_get_count_reset_continuation_token(self, mock_search_post):
         client = SearchClient("endpoint", "index name", CREDENTIAL)
         result = await client.search(search_text="search text")
         assert result._page_iterator_class is AsyncSearchPageIterator
```

### Comparing `azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_basic_live_async.py` & `azure-search-documents-11.6.0b4/tests/async_tests/test_search_client_basic_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_buffered_sender_live_async.py` & `azure-search-documents-11.6.0b4/tests/async_tests/test_search_client_buffered_sender_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_index_document_live_async.py` & `azure-search-documents-11.6.0b4/tests/async_tests/test_search_client_index_document_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_search_live_async.py` & `azure-search-documents-11.6.0b4/tests/async_tests/test_search_client_search_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_alias_live_async.py` & `azure-search-documents-11.6.0b4/tests/async_tests/test_search_index_client_alias_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_async.py` & `azure-search-documents-11.6.0b4/tests/async_tests/test_search_index_client_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_data_source_live_async.py` & `azure-search-documents-11.6.0b4/tests/async_tests/test_search_index_client_data_source_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_live_async.py` & `azure-search-documents-11.6.0b4/tests/async_tests/test_search_index_client_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_skillset_live_async.py` & `azure-search-documents-11.6.0b4/tests/async_tests/test_search_index_client_skillset_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_synonym_map_live_async.py` & `azure-search-documents-11.6.0b4/tests/async_tests/test_search_index_client_synonym_map_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/async_tests/test_search_indexer_client_live_async.py` & `azure-search-documents-11.6.0b4/tests/async_tests/test_search_indexer_client_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/conftest.py` & `azure-search-documents-11.6.0b4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/perfstress_tests/autocomplete.py` & `azure-search-documents-11.6.0b4/tests/perfstress_tests/autocomplete.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/perfstress_tests/search_documents.py` & `azure-search-documents-11.6.0b4/tests/perfstress_tests/search_documents.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/perfstress_tests/suggest.py` & `azure-search-documents-11.6.0b4/tests/perfstress_tests/suggest.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/search_service_preparer.py` & `azure-search-documents-11.6.0b4/tests/search_service_preparer.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_buffered_sender.py` & `azure-search-documents-11.6.0b4/tests/async_tests/test_buffered_sender_async.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,154 +1,159 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 from unittest import mock
 import pytest
-from azure.search.documents import (
+from azure.search.documents.aio import (
     SearchIndexingBufferedSender,
 )
 from azure.core.credentials import AzureKeyCredential
 from azure.core.exceptions import HttpResponseError, ServiceResponseTimeoutError
 from azure.search.documents.models import IndexingResult
+from test_search_index_client_async import await_prepared_test
 
 CREDENTIAL = AzureKeyCredential(key="test_api_key")
 
 
-class TestSearchBatchingClient:
-    def test_search_indexing_buffered_sender_kwargs(self):
-        with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, window=100) as client:
+class TestSearchBatchingClientAsync:
+    @await_prepared_test
+    async def test_search_indexing_buffered_sender_kwargs(self):
+        async with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, window=100) as client:
             assert client._batch_action_count == 512
             assert client._max_retries_per_action == 3
             assert client._auto_flush_interval == 60
             assert client._auto_flush
 
-    def test_batch_queue(self):
-        with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
+    @await_prepared_test
+    async def test_batch_queue(self):
+        async with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
             assert client._index_documents_batch
-            client.upload_documents(["upload1"])
-            client.delete_documents(["delete1", "delete2"])
-            client.merge_documents(["merge1", "merge2", "merge3"])
-            client.merge_or_upload_documents(["merge_or_upload1"])
+            await client.upload_documents(["upload1"])
+            await client.delete_documents(["delete1", "delete2"])
+            await client.merge_documents(["merge1", "merge2", "merge3"])
+            await client.merge_or_upload_documents(["merge_or_upload1"])
             assert len(client.actions) == 7
-            actions = client._index_documents_batch.dequeue_actions()
+            actions = await client._index_documents_batch.dequeue_actions()
             assert len(client.actions) == 0
-            client._index_documents_batch.enqueue_actions(actions)
-            assert len(client.actions) == 7
-            actions = client._index_documents_batch.dequeue_actions()
-            assert len(client.actions) == 0
-            for action in actions:
-                client._index_documents_batch.enqueue_actions(action)
+            await client._index_documents_batch.enqueue_actions(actions)
             assert len(client.actions) == 7
 
+    @await_prepared_test
     @mock.patch(
-        "azure.search.documents._search_indexing_buffered_sender.SearchIndexingBufferedSender._process_if_needed"
+        "azure.search.documents.aio._search_indexing_buffered_sender_async.SearchIndexingBufferedSender._process_if_needed"
     )
-    def test_process_if_needed(self, mock_process_if_needed):
-        with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL) as client:
-            client.upload_documents(["upload1"])
-            client.delete_documents(["delete1", "delete2"])
+    async def test_process_if_needed(self, mock_process_if_needed):
+        async with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL) as client:
+            await client.upload_documents(["upload1"])
+            await client.delete_documents(["delete1", "delete2"])
         assert mock_process_if_needed.called
 
-    @mock.patch("azure.search.documents._search_indexing_buffered_sender.SearchIndexingBufferedSender._cleanup")
-    def test_context_manager(self, mock_cleanup):
-        with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
-            client.upload_documents(["upload1"])
-            client.delete_documents(["delete1", "delete2"])
+    @await_prepared_test
+    @mock.patch(
+        "azure.search.documents.aio._search_indexing_buffered_sender_async.SearchIndexingBufferedSender._cleanup"
+    )
+    async def test_context_manager(self, mock_cleanup):
+        async with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
+            await client.upload_documents(["upload1"])
+            await client.delete_documents(["delete1", "delete2"])
         assert mock_cleanup.called
 
-    def test_flush(self):
+    @await_prepared_test
+    async def test_flush(self):
         DOCUMENT = {
             "category": "Hotel",
             "hotelId": "1000",
             "rating": 4.0,
             "rooms": [],
             "hotelName": "Azure Inn",
         }
         with mock.patch.object(
             SearchIndexingBufferedSender,
             "_index_documents_actions",
             side_effect=HttpResponseError("Error"),
         ):
-            with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
+            async with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
                 client._index_key = "hotelId"
-                client.upload_documents([DOCUMENT])
-                client.flush()
+                await client.upload_documents([DOCUMENT])
+                await client.flush()
                 assert len(client.actions) == 0
 
-    def test_callback_new(self):
-        on_new = mock.Mock()
-        with SearchIndexingBufferedSender(
+    @await_prepared_test
+    async def test_callback_new(self):
+        on_new = mock.AsyncMock()
+        async with SearchIndexingBufferedSender(
             "endpoint", "index name", CREDENTIAL, auto_flush=False, on_new=on_new
         ) as client:
-            client.upload_documents(["upload1"])
+            await client.upload_documents(["upload1"])
             assert on_new.called
 
-    def test_callback_error(self):
-        def mock_fail_index_documents(actions, timeout=86400):
+    @await_prepared_test
+    async def test_callback_error(self):
+        async def mock_fail_index_documents(actions, timeout=86400):
             if len(actions) > 0:
                 result = IndexingResult()
                 result.key = actions[0].additional_properties.get("id")
                 result.status_code = 400
                 result.succeeded = False
                 self.uploaded = self.uploaded + len(actions) - 1
                 return [result]
 
-        on_error = mock.Mock()
-        with SearchIndexingBufferedSender(
+        on_error = mock.AsyncMock()
+        async with SearchIndexingBufferedSender(
             "endpoint", "index name", CREDENTIAL, auto_flush=False, on_error=on_error
         ) as client:
             client._index_documents_actions = mock_fail_index_documents
             client._index_key = "id"
-            client.upload_documents({"id": 0})
-            client.flush()
+            await client.upload_documents({"id": 0})
+            await client.flush()
             assert on_error.called
 
-    def test_callback_error_on_timeout(self):
-        def mock_fail_index_documents(actions, timeout=86400):
-            import time
-
+    @await_prepared_test
+    async def test_callback_error_on_timeout(self):
+        async def mock_fail_index_documents(actions, timeout=86400):
             if len(actions) > 0:
                 result = IndexingResult()
                 result.key = actions[0].additional_properties.get("id")
                 result.status_code = 400
                 result.succeeded = False
                 self.uploaded = self.uploaded + len(actions) - 1
                 time.sleep(1)
                 return [result]
 
-        on_error = mock.Mock()
-        with SearchIndexingBufferedSender(
+        on_error = mock.AsyncMock()
+        async with SearchIndexingBufferedSender(
             "endpoint", "index name", CREDENTIAL, auto_flush=False, on_error=on_error
         ) as client:
             client._index_documents_actions = mock_fail_index_documents
             client._index_key = "id"
-            client.upload_documents([{"id": 0}, {"id": 1}])
+            await client.upload_documents([{"id": 0}, {"id": 1}])
             with pytest.raises(ServiceResponseTimeoutError):
-                client.flush(timeout=-1)
+                await client.flush(timeout=-1)
             assert on_error.call_count == 2
 
-    def test_callback_progress(self):
-        def mock_successful_index_documents(actions, timeout=86400):
+    @await_prepared_test
+    async def test_callback_progress(self):
+        async def mock_successful_index_documents(actions, timeout=86400):
             if len(actions) > 0:
                 result = IndexingResult()
                 result.key = actions[0].additional_properties.get("id")
                 result.status_code = 200
                 result.succeeded = True
                 return [result]
 
-        on_progress = mock.Mock()
-        on_remove = mock.Mock()
-        with SearchIndexingBufferedSender(
+        on_progress = mock.AsyncMock()
+        on_remove = mock.AsyncMock()
+        async with SearchIndexingBufferedSender(
             "endpoint",
             "index name",
             CREDENTIAL,
             auto_flush=False,
             on_progress=on_progress,
             on_remove=on_remove,
         ) as client:
             client._index_documents_actions = mock_successful_index_documents
             client._index_key = "id"
-            client.upload_documents({"id": 0})
-            client.flush()
+            await client.upload_documents({"id": 0})
+            await client.flush()
             assert on_progress.called
             assert on_remove.called
```

### Comparing `azure-search-documents-11.6.0b3/tests/test_index_documents_batch.py` & `azure-search-documents-11.6.0b4/tests/test_index_documents_batch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_index_field_helpers.py` & `azure-search-documents-11.6.0b4/tests/test_index_field_helpers.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_queries.py` & `azure-search-documents-11.6.0b4/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_regex_flags.py` & `azure-search-documents-11.6.0b4/tests/test_regex_flags.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_search_client.py` & `azure-search-documents-11.6.0b4/tests/test_search_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from azure.search.documents import (
     IndexDocumentsBatch,
     SearchClient,
     RequestEntityTooLargeError,
     ApiVersion,
 )
-from azure.search.documents._utils import odata
+from azure.search.documents._utils import odata, get_answer_query
 
 CREDENTIAL = AzureKeyCredential(key="test_api_key")
 
 CRUD_METHOD_NAMES = [
     "upload_documents",
     "delete_documents",
     "merge_documents",
@@ -52,14 +52,31 @@
     def test_escape_single_quote(self):
         assert odata("foo eq {foo}", foo="a '' str'ing") == "foo eq 'a '''' str''ing'"
 
     def test_prevent_double_quoting(self):
         assert odata("foo eq '{foo}'", foo="a string") == "foo eq 'a string'"
 
 
+class TestAnswerQuery:
+    def test_no_args(self):
+        assert get_answer_query() is None
+
+    def test_query_answer(self):
+        assert get_answer_query("query") == "query"
+
+    def test_query_answer_count(self):
+        assert get_answer_query("query", 5) == "query|count-5"
+
+    def test_query_answer_threshold(self):
+        assert get_answer_query("query", query_answer_threshold=0.5) == "query|threshold-0.5"
+
+    def test_query_answer_count_threshold(self):
+        assert get_answer_query("query", 5, 0.5) == "query|count-5,threshold-0.5"
+
+
 class TestSearchClient:
     def test_init(self):
         client = SearchClient("endpoint", "index name", CREDENTIAL)
         assert client._headers == {
             "api-key": "test_api_key",
             "Accept": "application/json;odata.metadata=none",
         }
```

### Comparing `azure-search-documents-11.6.0b3/tests/test_search_client_basic_live.py` & `azure-search-documents-11.6.0b4/tests/test_search_client_basic_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_search_client_buffered_sender_live.py` & `azure-search-documents-11.6.0b4/tests/test_search_client_buffered_sender_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_search_client_index_document_live.py` & `azure-search-documents-11.6.0b4/tests/test_search_client_index_document_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_search_client_search_live.py` & `azure-search-documents-11.6.0b4/tests/test_search_client_search_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_search_index_client.py` & `azure-search-documents-11.6.0b4/tests/test_search_index_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_search_index_client_alias_live.py` & `azure-search-documents-11.6.0b4/tests/test_search_index_client_alias_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_search_index_client_data_source_live.py` & `azure-search-documents-11.6.0b4/tests/test_search_index_client_data_source_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_search_index_client_live.py` & `azure-search-documents-11.6.0b4/tests/test_search_index_client_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_search_index_client_skillset_live.py` & `azure-search-documents-11.6.0b4/tests/test_search_index_client_skillset_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_search_index_client_synonym_map_live.py` & `azure-search-documents-11.6.0b4/tests/test_search_index_client_synonym_map_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_search_indexer_client_live.py` & `azure-search-documents-11.6.0b4/tests/test_search_indexer_client_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b3/tests/test_serialization.py` & `azure-search-documents-11.6.0b4/tests/test_serialization.py`

 * *Files identical despite different names*

