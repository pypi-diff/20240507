# Comparing `tmp/galaxy_test_api-24.0.1.tar.gz` & `tmp/galaxy_test_api-24.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_test_api-24.0.1.tar", last modified: Thu May  2 13:49:13 2024, max compression
+gzip compressed data, was "galaxy_test_api-24.0.2.tar", last modified: Tue May  7 14:34:19 2024, max compression
```

## Comparing `galaxy_test_api-24.0.1.tar` & `galaxy_test_api-24.0.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:13.242053 galaxy_test_api-24.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18782 2024-05-02 13:49:13.242053 galaxy_test_api-24.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:13.230053 galaxy_test_api-24.0.1/galaxy_test/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:13.238053 galaxy_test_api-24.0.1/galaxy_test/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:13.238053 galaxy_test_api-24.0.1/galaxy_test/api/cwl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/cwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/embed_test_1.gxwf.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/embed_test_1_tool.gxtool.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/sharable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_container_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    33522 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_dataset_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    39575 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_display_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_drs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19567 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_folder_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_group_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    51434 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_histories.py
--rw-r--r--   0 runner    (1001) docker     (127)    78797 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_history_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_history_contents_provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_item_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    54283 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29503 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_page_revisions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23420 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_short_term_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_tool_data.py
--rw-r--r--   0 runner    (1001) docker     (127)   148621 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    46383 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_tools_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_tours.py
--rw-r--r--   0 runner    (1001) docker     (127)    16370 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_visualizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    27526 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_workflow_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)   292809 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_workflows_cwl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_workflows_from_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:13.238053 galaxy_test_api-24.0.1/galaxy_test_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18782 2024-05-02 13:49:13.000000 galaxy_test_api-24.0.1/galaxy_test_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-02 13:49:13.000000 galaxy_test_api-24.0.1/galaxy_test_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:49:13.000000 galaxy_test_api-24.0.1/galaxy_test_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 13:49:13.000000 galaxy_test_api-24.0.1/galaxy_test_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 13:49:13.000000 galaxy_test_api-24.0.1/galaxy_test_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-02 13:49:13.242053 galaxy_test_api-24.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:19.684628 galaxy_test_api-24.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-07 14:31:49.000000 galaxy_test_api-24.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19039 2024-05-07 14:34:19.684628 galaxy_test_api-24.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:19.672628 galaxy_test_api-24.0.2/galaxy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:19.680628 galaxy_test_api-24.0.2/galaxy_test/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:19.680628 galaxy_test_api-24.0.2/galaxy_test/api/cwl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/cwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/embed_test_1.gxwf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/embed_test_1_tool.gxtool.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/sharable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_container_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33522 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_dataset_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39575 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_display_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_drs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19567 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_folder_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51434 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_histories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78797 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_history_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_history_contents_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_item_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54283 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29503 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_page_revisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23420 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_short_term_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_tool_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   149661 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46383 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_tools_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_tours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16370 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27526 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_workflow_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)   292809 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_workflows_cwl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/api/test_workflows_from_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/galaxy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:19.680628 galaxy_test_api-24.0.2/galaxy_test_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19039 2024-05-07 14:34:19.000000 galaxy_test_api-24.0.2/galaxy_test_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-07 14:34:19.000000 galaxy_test_api-24.0.2/galaxy_test_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:34:19.000000 galaxy_test_api-24.0.2/galaxy_test_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 14:34:19.000000 galaxy_test_api-24.0.2/galaxy_test_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 14:34:19.000000 galaxy_test_api-24.0.2/galaxy_test_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-07 14:34:19.684628 galaxy_test_api-24.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:31:50.000000 galaxy_test_api-24.0.2/test-requirements.txt
```

### Comparing `galaxy_test_api-24.0.1/HISTORY.rst` & `galaxy_test_api-24.0.2/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Improve error message for ``Extract dataset`` tool by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18078 <https://github.com/galaxyproject/galaxy/pull/18078>`_
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_test_api-24.0.1/LICENSE` & `galaxy_test_api-24.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/PKG-INFO` & `galaxy_test_api-24.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-api
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy API tests
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -50,14 +50,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Improve error message for ``Extract dataset`` tool by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18078 <https://github.com/galaxyproject/galaxy/pull/18078>`_
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/_framework.py` & `galaxy_test_api-24.0.2/galaxy_test/api/_framework.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/sharable.py` & `galaxy_test_api-24.0.2/galaxy_test/api/sharable.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_authenticate.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_authenticate.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_configuration.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_configuration.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_container_resolution.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_container_resolution.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_dataset_collections.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_dataset_collections.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_datasets.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_datasets.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_datatypes.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_display_applications.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_display_applications.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_drs.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_drs.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_folder_contents.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_folder_contents.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_folders.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_folders.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_framework.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_framework.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_group_roles.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_group_roles.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_group_users.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_group_users.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_groups.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_groups.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_histories.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_histories.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_history_contents.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_history_contents.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_history_contents_provenance.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_history_contents_provenance.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_item_tags.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_item_tags.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_jobs.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_jobs.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_libraries.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_libraries.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_licenses.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_licenses.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_page_revisions.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_page_revisions.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_pages.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_pages.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_roles.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_roles.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_short_term_storage.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_short_term_storage.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_tags.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_tool_data.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_tool_data.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_tools.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -697,31 +697,50 @@
     @skip_without_tool("__EXTRACT_DATASET__")
     @skip_without_tool("cat_data_and_sleep")
     def test_database_operation_tool_with_pending_inputs(self):
         with self.dataset_populator.test_history(require_new=False) as history_id:
             hdca1_id = self.dataset_collection_populator.create_list_in_history(
                 history_id, contents=["a\nb\nc\nd", "e\nf\ng\nh"], wait=True
             ).json()["outputs"][0]["id"]
-            self.dataset_populator.run_tool(
+            run_response = self.dataset_populator.run_tool(
                 tool_id="cat_data_and_sleep",
                 inputs={
                     "sleep_time": 15,
                     "input1": {"batch": True, "values": [{"src": "hdca", "id": hdca1_id}]},
                 },
                 history_id=history_id,
             )
+            output_hdca_id = run_response["implicit_collections"][0]["id"]
             run_response = self.dataset_populator.run_tool(
                 tool_id="__EXTRACT_DATASET__",
                 inputs={
-                    "data_collection": {"src": "hdca", "id": hdca1_id},
+                    "data_collection": {"src": "hdca", "id": output_hdca_id},
                 },
                 history_id=history_id,
             )
             assert run_response["outputs"][0]["state"] != "ok"
 
+    @skip_without_tool("__EXTRACT_DATASET__")
+    def test_extract_dataset_invalid_element_identifier(self):
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            hdca1_id = self.dataset_collection_populator.create_list_in_history(
+                history_id, contents=["a\nb\nc\nd", "e\nf\ng\nh"], wait=True
+            ).json()["outputs"][0]["id"]
+            run_response = self.dataset_populator.run_tool_raw(
+                tool_id="__EXTRACT_DATASET__",
+                inputs={
+                    "data_collection": {"src": "hdca", "id": hdca1_id},
+                    "which": {"which_dataset": "by_index", "index": 100},
+                },
+                history_id=history_id,
+                input_format="21.01",
+            )
+            assert run_response.status_code == 400
+            assert run_response.json()["err_msg"] == "Dataset collection has no element_index with key 100."
+
     @skip_without_tool("__FILTER_FAILED_DATASETS__")
     def test_filter_failed_list(self):
         with self.dataset_populator.test_history(require_new=False) as history_id:
             ok_hdca_id = self.dataset_collection_populator.create_list_in_history(
                 history_id, contents=["0", "1", "0", "1"], wait=True
             ).json()["outputs"][0]["id"]
             response = self.dataset_populator.run_exit_code_from_file(history_id, ok_hdca_id)
```

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_tools_upload.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_tools_upload.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_tours.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_tours.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_users.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_users.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_visualizations.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_webhooks.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_workflow_extraction.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_workflow_extraction.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_workflows.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test/api/test_workflows_from_yaml.py` & `galaxy_test_api-24.0.2/galaxy_test/api/test_workflows_from_yaml.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/galaxy_test_api.egg-info/PKG-INFO` & `galaxy_test_api-24.0.2/galaxy_test_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-api
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy API tests
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -50,14 +50,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Improve error message for ``Extract dataset`` tool by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18078 <https://github.com/galaxyproject/galaxy/pull/18078>`_
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_test_api-24.0.1/galaxy_test_api.egg-info/SOURCES.txt` & `galaxy_test_api-24.0.2/galaxy_test_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy_test_api-24.0.1/setup.cfg` & `galaxy_test_api-24.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-test-api
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.1
+version = 24.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-test-base
 	pytest
 	python-dateutil
```

