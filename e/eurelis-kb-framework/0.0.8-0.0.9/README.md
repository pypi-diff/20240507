# Comparing `tmp/eurelis_kb_framework-0.0.8.tar.gz` & `tmp/eurelis_kb_framework-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurelis_kb_framework-0.0.8.tar", last modified: Thu Dec 21 08:50:27 2023, max compression
+gzip compressed data, was "eurelis_kb_framework-0.0.9.tar", last modified: Thu Jan 11 10:16:38 2024, max compression
```

## Comparing `eurelis_kb_framework-0.0.8.tar` & `eurelis_kb_framework-0.0.9.tar`

### file list

```diff
@@ -1,98 +1,105 @@
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.603295 eurelis_kb_framework-0.0.8/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1064 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.8/LICENSE
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2032 2023-12-21 08:50:27.602789 eurelis_kb_framework-0.0.8/PKG-INFO
--rw-r--r--   0 vincentlambert   (501) staff       (20)      322 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.8/README.md
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1448 2023-12-21 08:49:37.000000 eurelis_kb_framework-0.0.8/pyproject.toml
--rw-r--r--   0 vincentlambert   (501) staff       (20)       38 2023-12-21 08:50:27.603395 eurelis_kb_framework-0.0.8/setup.cfg
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.447333 eurelis_kb_framework-0.0.8/src/
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.467125 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3850 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.473986 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/acronyms/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1379 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/acronyms/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1987 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/acronyms/acronyms_chain_wrapper.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1849 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/acronyms/acronyms_document_transformer.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)      645 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/acronyms/acronyms_text_transformer.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.448436 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/addons/
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.475994 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/addons/output/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1616 2023-12-20 17:46:02.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/addons/output/markdown_html_callback.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     6485 2023-12-21 08:49:37.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/base_factory.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.477395 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/chains/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      601 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/chains/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.478078 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/chains/conversational_retrieval/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     4855 2023-12-21 08:49:37.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/chains/conversational_retrieval/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     8600 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/class_loader.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.480883 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/dataset/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     6220 2023-12-14 18:51:05.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/dataset/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)    11376 2023-12-14 18:51:05.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/dataset/dataset.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.481657 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      581 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.482401 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/fs/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2441 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/fs/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.484489 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/list/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2549 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/list/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2293 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/list/list_loader.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.505959 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/sitemap/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3030 2023-12-21 08:49:37.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/sitemap/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.514369 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/url/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1989 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/url/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.537677 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_transformers/
--rw-r--r--   0 vincentlambert   (501) staff       (20)        0 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_transformers/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.561252 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_transformers/html2text/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      782 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_transformers/html2text/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.582832 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_transformers/urloutput/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3155 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_transformers/urloutput/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.583451 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/embeddings/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      657 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/embeddings/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.583923 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/embeddings/huggingface/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      822 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/embeddings/huggingface/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.584507 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/embeddings/openai/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1295 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/embeddings/openai/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1813 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/gradiochat.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)    27646 2023-12-14 18:51:05.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/langchain_wrapper.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.585253 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/llms/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      396 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/llms/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.585826 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/llms/huggingface/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      982 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/llms/huggingface/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.586305 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/llms/openai/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1894 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/llms/openai/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     4914 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/main.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.587470 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/memory/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      534 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/memory/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)      848 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/memory/conversation_buffer_memory.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.591505 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/output/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2591 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/output/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3423 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/output/base_console_output.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3635 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/output/logging_console_output.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)      755 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/output/output.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1385 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/output/verbose_console_output.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.593090 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/parsers/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1234 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/parsers/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1172 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/parsers/pdf.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.593713 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/retrievers/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      493 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/retrievers/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.594227 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/retrievers/selfquery/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1753 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/retrievers/selfquery/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.595285 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/retrievers/vectorstore/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      738 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/retrievers/vectorstore/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.595740 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/text_splitter/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3900 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/text_splitter/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.596931 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/text_transformers/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      366 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/text_transformers/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)      475 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/types.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1352 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/utils.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.597442 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/vectorstores/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      547 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/vectorstores/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.597836 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/vectorstores/chroma/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3056 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/vectorstores/chroma/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.599329 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/vectorstores/mongodb/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2749 2023-12-14 18:51:05.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/vectorstores/mongodb/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1507 2023-12-14 18:51:05.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/vectorstores/mongodb/mongodb_similarity_atlas_vector_store_search.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.599966 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/vectorstores/solr/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      938 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/vectorstores/solr/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-12-21 08:50:27.600463 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework.egg-info/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2032 2023-12-21 08:50:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework.egg-info/PKG-INFO
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3021 2023-12-21 08:50:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vincentlambert   (501) staff       (20)        1 2023-12-21 08:50:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vincentlambert   (501) staff       (20)       59 2023-12-21 08:50:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework.egg-info/entry_points.txt
--rw-r--r--   0 vincentlambert   (501) staff       (20)      459 2023-12-21 08:50:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework.egg-info/requires.txt
--rw-r--r--   0 vincentlambert   (501) staff       (20)       21 2023-12-21 08:50:27.000000 eurelis_kb_framework-0.0.8/src/eurelis_kb_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.864878 eurelis_kb_framework-0.0.9/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1064 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.9/LICENSE
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2089 2024-01-11 10:16:38.864198 eurelis_kb_framework-0.0.9/PKG-INFO
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      322 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.9/README.md
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1475 2024-01-11 10:11:39.000000 eurelis_kb_framework-0.0.9/pyproject.toml
+-rw-r--r--   0 vincentlambert   (501) staff       (20)       38 2024-01-11 10:16:38.865014 eurelis_kb_framework-0.0.9/setup.cfg
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.813785 eurelis_kb_framework-0.0.9/src/
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.827512 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3850 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.833274 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/acronyms/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1379 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/acronyms/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1987 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/acronyms/acronyms_chain_wrapper.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1849 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/acronyms/acronyms_document_transformer.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      645 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/acronyms/acronyms_text_transformer.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.833793 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/addons/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:11:39.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/addons/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.836669 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/addons/checker/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      198 2024-01-11 10:11:39.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/addons/checker/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2012 2024-01-11 10:11:39.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/addons/checker/chat_checker.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      394 2024-01-11 10:11:39.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/addons/checker/check_input.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1388 2024-01-11 10:11:39.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/addons/checker/check_input_callback.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:11:39.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/addons/checker/method.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.837215 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/addons/output/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1616 2023-12-20 17:46:02.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/addons/output/markdown_html_callback.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     6485 2023-12-21 08:49:37.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/base_factory.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.837782 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/chains/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      601 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/chains/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.838140 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/chains/conversational_retrieval/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     5858 2024-01-11 10:11:39.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/chains/conversational_retrieval/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     8600 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/class_loader.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.839091 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/dataset/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     6220 2023-12-14 18:51:05.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/dataset/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)    11376 2023-12-14 18:51:05.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/dataset/dataset.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.839486 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      581 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.840010 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/fs/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2441 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/fs/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.840913 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/list/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2549 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/list/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2293 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/list/list_loader.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.841290 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/sitemap/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3030 2023-12-21 08:49:37.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/sitemap/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.841711 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/url/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1989 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/url/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.842344 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_transformers/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)        0 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_transformers/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.842872 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_transformers/html2text/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      782 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_transformers/html2text/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.843474 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_transformers/urloutput/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3155 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_transformers/urloutput/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.843946 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/embeddings/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      657 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/embeddings/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.844405 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/embeddings/huggingface/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      822 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/embeddings/huggingface/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.845040 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/embeddings/openai/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1295 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/embeddings/openai/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2598 2024-01-11 10:11:39.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/gradiochat.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)    27646 2023-12-14 18:51:05.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/langchain_wrapper.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.845828 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/llms/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      396 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/llms/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.846339 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/llms/huggingface/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      982 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/llms/huggingface/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.846884 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/llms/openai/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1894 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/llms/openai/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     5001 2024-01-11 10:11:39.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/main.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.847676 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/memory/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      534 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/memory/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      848 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/memory/conversation_buffer_memory.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.850638 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/output/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2591 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/output/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3423 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/output/base_console_output.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3635 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/output/logging_console_output.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      755 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/output/output.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1385 2023-11-14 16:17:51.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/output/verbose_console_output.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.851957 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/parsers/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1234 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/parsers/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1172 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/parsers/pdf.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.852479 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/retrievers/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      493 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/retrievers/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.852988 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/retrievers/selfquery/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1753 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/retrievers/selfquery/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.853507 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/retrievers/vectorstore/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      738 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/retrievers/vectorstore/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.854667 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/text_splitter/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3900 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/text_splitter/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.856251 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/text_transformers/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      366 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/text_transformers/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      475 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/types.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1352 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/utils.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.856984 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/vectorstores/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      547 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/vectorstores/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.857508 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/vectorstores/chroma/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3056 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/vectorstores/chroma/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.858726 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/vectorstores/mongodb/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2749 2023-12-14 18:51:05.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/vectorstores/mongodb/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3111 2024-01-11 10:11:39.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/vectorstores/mongodb/mongodb_similarity_atlas_vector_store_search.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.859311 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/vectorstores/solr/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      938 2023-12-11 09:26:27.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/vectorstores/solr/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-01-11 10:16:38.859960 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework.egg-info/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2089 2024-01-11 10:16:38.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3342 2024-01-11 10:16:38.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vincentlambert   (501) staff       (20)        1 2024-01-11 10:16:38.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vincentlambert   (501) staff       (20)       59 2024-01-11 10:16:38.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework.egg-info/entry_points.txt
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      479 2024-01-11 10:16:38.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework.egg-info/requires.txt
+-rw-r--r--   0 vincentlambert   (501) staff       (20)       21 2024-01-11 10:16:38.000000 eurelis_kb_framework-0.0.9/src/eurelis_kb_framework.egg-info/top_level.txt
```

### Comparing `eurelis_kb_framework-0.0.8/LICENSE` & `eurelis_kb_framework-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/PKG-INFO` & `eurelis_kb_framework-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eurelis_kb_framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: Framework to build and manage knowledge base. Based on Langchain under the hood.
 Author-email: Jérôme DIAZ <j.diaz@eurelis.com>, Vincent LAMBERT <v.lambert@eurelis.com>
 Project-URL: Homepage, https://github.com/Eurelis/Eurelis-KB-Framework
 Project-URL: Bug Tracker, https://github.com/Eurelis/Eurelis-KB-Framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -29,20 +29,21 @@
 Requires-Dist: lxml==4.9.3; extra == "sitemap"
 Requires-Dist: beautifulsoup4==4.12.2; extra == "sitemap"
 Provides-Extra: chatbot
 Requires-Dist: gradio==3.47.1; extra == "chatbot"
 Provides-Extra: pdf
 Requires-Dist: pypdf==3.16.4; extra == "pdf"
 Requires-Dist: cryptography==41.0.7; extra == "pdf"
-Provides-Extra: selfcheck
-Requires-Dist: lark==1.1.8; extra == "selfcheck"
 Provides-Extra: mongodb
 Requires-Dist: pymongo==4.6.1; extra == "mongodb"
 Provides-Extra: markdown
 Requires-Dist: markdown==3.5.1; extra == "markdown"
+Provides-Extra: selfcheck
+Requires-Dist: selfcheckgpt==0.1.4; extra == "selfcheck"
+Requires-Dist: lark==1.1.8; extra == "selfcheck"
 
 # Eurelis-KB-Framework
 
 ![Python : 11](https://img.shields.io/badge/Python-=3.11-green)
 ![Code style : black](https://img.shields.io/badge/Code_style-black-black)
 ![Linting : pylint](https://img.shields.io/badge/Linting-pylint-yellowgreen)
```

### Comparing `eurelis_kb_framework-0.0.8/pyproject.toml` & `eurelis_kb_framework-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eurelis_kb_framework"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Jérôme DIAZ", email="j.diaz@eurelis.com" },
   { name="Vincent LAMBERT", email="v.lambert@eurelis.com" }
 ]
 description = "Framework to build and manage knowledge base. Based on Langchain under the hood."
 readme = "README.md"
 requires-python = ">=3.11"
@@ -46,23 +46,24 @@
 chatbot = [
     "gradio==3.47.1"
 ]
 pdf = [
     "pypdf==3.16.4",
     "cryptography==41.0.7"
 ]
-selfcheck = [
-    "lark==1.1.8"
-]
 mongodb = [
     "pymongo==4.6.1"
 ]
 markdown = [
     "markdown==3.5.1"
 ]
+selfcheck = [
+    "selfcheckgpt==0.1.4",
+    "lark==1.1.8"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/Eurelis/Eurelis-KB-Framework"
 "Bug Tracker" = "https://github.com/Eurelis/Eurelis-KB-Framework/issues"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
```

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/acronyms/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/acronyms/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/acronyms/acronyms_chain_wrapper.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/acronyms/acronyms_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/acronyms/acronyms_document_transformer.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/acronyms/acronyms_document_transformer.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/acronyms/acronyms_text_transformer.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/acronyms/acronyms_text_transformer.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/addons/output/markdown_html_callback.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/addons/output/markdown_html_callback.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/base_factory.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/base_factory.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/chains/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/chains/conversational_retrieval/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/chains/conversational_retrieval/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from typing import Union
 
 from langchain.chains.base import Chain
+
 from langchain.prompts import (
     PromptTemplate,
     ChatPromptTemplate,
     SystemMessagePromptTemplate,
     HumanMessagePromptTemplate,
 )
+
 from langchain.schema import BaseMemory
 
+
 from eurelis_kb_framework.base_factory import (
     ParamsDictFactory,
     DefaultFactories,
 )
 from eurelis_kb_framework.types import FACTORY
 
 
@@ -26,17 +29,25 @@
         super().__init__()
         self.retriever_kwargs = {}
         self.memory = None
 
         self.condense_question_prompt = None
 
         self.combine_docs_chain_kwargs = None
+        self.condense_question_llm_factory = None
         self.output_format = None
         self.output_field = None
 
+    def set_condense_question_llm(self, value: FACTORY):
+        if not isinstance(value, (str, dict)):
+            raise ValueError(
+                "condense_question_llm parameter is expected to be a factory (str ou dict)"
+            )
+        self.condense_question_llm_factory = value.copy()
+
     def set_condense_question_prompt(self, value: str):
         if not isinstance(value, str):
             raise ValueError(
                 "Bad condensed_question_prompt value given, expected str got {type(str)}"
             )
         if not value or "{question}" not in value or "{chat_history}" not in value:
             raise ValueError(
@@ -57,23 +68,31 @@
             if not isinstance(prompt_value, dict):
                 raise ValueError(
                     f"Bad combine_docs_chain_kwargs prompt value, expecting a dict, got {type(value)}"
                 )
             system = prompt_value.get("system")
             human = prompt_value.get("human")
 
+            if isinstance(system, list) and all(
+                isinstance(item, str) for item in system
+            ):
+                system = " ".join(system)
+
+            if isinstance(human, list) and all(isinstance(item, str) for item in human):
+                human = " ".join(human)
+
             if not system or not isinstance(system, str) or "{context}" not in system:
                 raise ValueError(
                     "Bad combine_docs_chain_kwargs prompt value, "
-                    + "should have contain a system key with an associated text containing {context}"
+                    + "should have contain a system key with an associated text (or a list) containing {context}"
                 )
             if not human or not isinstance(human, str) or "{question}" not in human:
                 raise ValueError(
                     "Bad combine_docs_chain_kwargs prompt value, "
-                    + "should have contain a human key with an associated text containing {question}"
+                    + "should have contain a human key with an associated text (or a list) containing {question}"
                 )
 
             self.combine_docs_chain_kwargs["prompt"] = ChatPromptTemplate.from_messages(
                 [
                     SystemMessagePromptTemplate.from_template(system),
                     HumanMessagePromptTemplate.from_template(human),
                 ]
@@ -124,14 +143,23 @@
         )
 
         other_args = {}
         if self.condense_question_prompt:
             other_args["condense_question_prompt"] = self.condense_question_prompt
         if self.combine_docs_chain_kwargs:
             other_args["combine_docs_chain_kwargs"] = self.combine_docs_chain_kwargs
+        if self.condense_question_llm_factory:
+            other_args[
+                "condense_question_llm"
+            ] = context.__class__.get_instance_from_factory(
+                context,
+                DefaultFactories.LLM,
+                self.condense_question_llm_factory,
+                mandatory=True,
+            )
 
         # build and return the chain
         return ConversationalRetrievalChain.from_llm(
             context.lazy_get_llm(),
             retriever=retriever,
             return_source_documents=True,
             memory=memory,
```

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/class_loader.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/class_loader.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/dataset/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/dataset/dataset.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/fs/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/list/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/list/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/list/list_loader.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/list/list_loader.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/sitemap/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/sitemap/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_loaders/url/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_loaders/url/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_transformers/html2text/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_transformers/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/document_transformers/urloutput/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/document_transformers/urloutput/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/embeddings/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/embeddings/huggingface/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/embeddings/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/embeddings/openai/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/embeddings/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/langchain_wrapper.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/langchain_wrapper.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/llms/huggingface/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/llms/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/llms/openai/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/llms/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/main.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,21 +202,22 @@
         filter_args = None
 
     wrapper = ctx.obj["singleton"]()
     wrapper.search_documents(query, for_print=True, search_filter=filter_args)
 
 
 @cli.command()
+@click.option("--selfcheck/--no-selfcheck", default=False)
 @click.pass_context
-def gradio(ctx):
+def gradio(ctx, selfcheck: bool):
     wrapper = ctx.obj["singleton"]()
 
     from eurelis_kb_framework import gradiochat
 
-    gradiochat.define_chatbot(wrapper).launch()
+    gradiochat.define_chatbot(wrapper, selfcheck).launch()
 
 
 # enable the dataset and search commands
 if __name__ == "__main__":
     cli(obj={})
```

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/memory/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/memory/conversation_buffer_memory.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/memory/conversation_buffer_memory.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/output/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/output/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/output/base_console_output.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/output/base_console_output.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/output/logging_console_output.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/output/logging_console_output.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/output/output.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/output/output.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/output/verbose_console_output.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/output/verbose_console_output.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/parsers/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/parsers/pdf.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/parsers/pdf.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/retrievers/selfquery/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/retrievers/selfquery/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/retrievers/vectorstore/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/retrievers/vectorstore/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/text_splitter/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/text_splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/utils.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/utils.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/vectorstores/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/vectorstores/chroma/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/vectorstores/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/vectorstores/mongodb/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/vectorstores/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework/vectorstores/solr/__init__.py` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework/vectorstores/solr/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework.egg-info/PKG-INFO` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eurelis-kb-framework
-Version: 0.0.8
+Name: eurelis_kb_framework
+Version: 0.0.9
 Summary: Framework to build and manage knowledge base. Based on Langchain under the hood.
 Author-email: Jérôme DIAZ <j.diaz@eurelis.com>, Vincent LAMBERT <v.lambert@eurelis.com>
 Project-URL: Homepage, https://github.com/Eurelis/Eurelis-KB-Framework
 Project-URL: Bug Tracker, https://github.com/Eurelis/Eurelis-KB-Framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -29,20 +29,21 @@
 Requires-Dist: lxml==4.9.3; extra == "sitemap"
 Requires-Dist: beautifulsoup4==4.12.2; extra == "sitemap"
 Provides-Extra: chatbot
 Requires-Dist: gradio==3.47.1; extra == "chatbot"
 Provides-Extra: pdf
 Requires-Dist: pypdf==3.16.4; extra == "pdf"
 Requires-Dist: cryptography==41.0.7; extra == "pdf"
-Provides-Extra: selfcheck
-Requires-Dist: lark==1.1.8; extra == "selfcheck"
 Provides-Extra: mongodb
 Requires-Dist: pymongo==4.6.1; extra == "mongodb"
 Provides-Extra: markdown
 Requires-Dist: markdown==3.5.1; extra == "markdown"
+Provides-Extra: selfcheck
+Requires-Dist: selfcheckgpt==0.1.4; extra == "selfcheck"
+Requires-Dist: lark==1.1.8; extra == "selfcheck"
 
 # Eurelis-KB-Framework
 
 ![Python : 11](https://img.shields.io/badge/Python-=3.11-green)
 ![Code style : black](https://img.shields.io/badge/Code_style-black-black)
 ![Linting : pylint](https://img.shields.io/badge/Linting-pylint-yellowgreen)
```

### Comparing `eurelis_kb_framework-0.0.8/src/eurelis_kb_framework.egg-info/SOURCES.txt` & `eurelis_kb_framework-0.0.9/src/eurelis_kb_framework.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 src/eurelis_kb_framework.egg-info/entry_points.txt
 src/eurelis_kb_framework.egg-info/requires.txt
 src/eurelis_kb_framework.egg-info/top_level.txt
 src/eurelis_kb_framework/acronyms/__init__.py
 src/eurelis_kb_framework/acronyms/acronyms_chain_wrapper.py
 src/eurelis_kb_framework/acronyms/acronyms_document_transformer.py
 src/eurelis_kb_framework/acronyms/acronyms_text_transformer.py
+src/eurelis_kb_framework/addons/__init__.py
+src/eurelis_kb_framework/addons/checker/__init__.py
+src/eurelis_kb_framework/addons/checker/chat_checker.py
+src/eurelis_kb_framework/addons/checker/check_input.py
+src/eurelis_kb_framework/addons/checker/check_input_callback.py
+src/eurelis_kb_framework/addons/checker/method.py
 src/eurelis_kb_framework/addons/output/markdown_html_callback.py
 src/eurelis_kb_framework/chains/__init__.py
 src/eurelis_kb_framework/chains/conversational_retrieval/__init__.py
 src/eurelis_kb_framework/dataset/__init__.py
 src/eurelis_kb_framework/dataset/dataset.py
 src/eurelis_kb_framework/document_loaders/__init__.py
 src/eurelis_kb_framework/document_loaders/fs/__init__.py
```

