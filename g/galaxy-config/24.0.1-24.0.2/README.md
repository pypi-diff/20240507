# Comparing `tmp/galaxy_config-24.0.1.tar.gz` & `tmp/galaxy_config-24.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_config-24.0.1.tar", last modified: Thu May  2 13:47:12 2024, max compression
+gzip compressed data, was "galaxy_config-24.0.2.tar", last modified: Tue May  7 14:32:16 2024, max compression
```

## Comparing `galaxy_config-24.0.1.tar` & `galaxy_config-24.0.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:12.629356 galaxy_config-24.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    16004 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17449 2024-05-02 13:47:12.629356 galaxy_config-24.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:12.617356 galaxy_config-24.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:12.617356 galaxy_config-24.0.1/galaxy/config/
--rw-r--r--   0 runner    (1001) docker     (127)    65685 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20242 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/config_manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:12.625356 galaxy_config-24.0.1/galaxy/config/sample/
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/auth_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/build_sites.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/container_resolvers.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/data_manager_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)   121212 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/datatypes_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/disposable_email_blocklist.conf.sample
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/environment_modules_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/error_report.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/file_sources_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)   133915 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/galaxy.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)    53508 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/job_conf.sample.yml
--rw-r--r--   0 runner    (1001) docker     (127)    79501 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/job_conf.xml.sample_advanced
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/job_conf.xml.sample_basic
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/job_resource_params_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/lmod_modules_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/local_conda_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/object_store_conf.sample.yml
--rw-r--r--   0 runner    (1001) docker     (127)    20971 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/object_store_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/oidc_backends_config.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/oidc_config.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/reports.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/themes_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/tool_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/tool_data_table_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/tool_destinations.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/tool_recommendations_overwrite.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)    17943 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/tool_shed.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/tool_sheds_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/trs_servers_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/user_preferences_extra_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/workflow_resource_mapper_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/workflow_resource_params_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/workflow_schedulers_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:12.625356 galaxy_config-24.0.1/galaxy/config/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   158599 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/schemas/config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/schemas/job_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/schemas/reports_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)    25120 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/schemas/tool_shed_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:12.629356 galaxy_config-24.0.1/galaxy_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17449 2024-05-02 13:47:12.000000 galaxy_config-24.0.1/galaxy_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-02 13:47:12.000000 galaxy_config-24.0.1/galaxy_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:47:12.000000 galaxy_config-24.0.1/galaxy_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 13:47:12.000000 galaxy_config-24.0.1/galaxy_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 13:47:12.000000 galaxy_config-24.0.1/galaxy_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:47:12.000000 galaxy_config-24.0.1/galaxy_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-02 13:47:12.629356 galaxy_config-24.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:16.801421 galaxy_config-24.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-07 14:31:49.000000 galaxy_config-24.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17550 2024-05-07 14:32:16.801421 galaxy_config-24.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:16.793421 galaxy_config-24.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:16.793421 galaxy_config-24.0.2/galaxy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    65685 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20242 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/config_manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:16.801421 galaxy_config-24.0.2/galaxy/config/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/auth_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/build_sites.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/container_resolvers.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/data_manager_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)   121212 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/datatypes_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/disposable_email_blocklist.conf.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/environment_modules_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/error_report.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/file_sources_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)   133915 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/galaxy.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    53508 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/job_conf.sample.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    79501 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/job_conf.xml.sample_advanced
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/job_conf.xml.sample_basic
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/job_resource_params_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/lmod_modules_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/local_conda_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/object_store_conf.sample.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    20971 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/object_store_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/oidc_backends_config.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/oidc_config.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/reports.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/themes_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/tool_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/tool_data_table_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/tool_destinations.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/tool_recommendations_overwrite.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    17943 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/tool_shed.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/tool_sheds_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/trs_servers_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/user_preferences_extra_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/workflow_resource_mapper_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/workflow_resource_params_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/sample/workflow_schedulers_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:16.801421 galaxy_config-24.0.2/galaxy/config/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   158599 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/schemas/config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/schemas/job_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/schemas/reports_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    25120 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/schemas/tool_shed_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/config/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:16.801421 galaxy_config-24.0.2/galaxy_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17550 2024-05-07 14:32:16.000000 galaxy_config-24.0.2/galaxy_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-07 14:32:16.000000 galaxy_config-24.0.2/galaxy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:32:16.000000 galaxy_config-24.0.2/galaxy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 14:32:16.000000 galaxy_config-24.0.2/galaxy_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 14:32:16.000000 galaxy_config-24.0.2/galaxy_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:32:16.000000 galaxy_config-24.0.2/galaxy_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-07 14:32:16.801421 galaxy_config-24.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 14:31:50.000000 galaxy_config-24.0.2/test-requirements.txt
```

### Comparing `galaxy_config-24.0.1/HISTORY.rst` & `galaxy_config-24.0.2/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_config-24.0.1/LICENSE` & `galaxy_config-24.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/PKG-INFO` & `galaxy_config-24.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-config
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy configuration
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,14 +47,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_config-24.0.1/galaxy/config/__init__.py` & `galaxy_config-24.0.2/galaxy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/config_manage.py` & `galaxy_config-24.0.2/galaxy/config/config_manage.py`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/auth_conf.xml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/auth_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/build_sites.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/build_sites.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/container_resolvers.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/container_resolvers.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/datatypes_conf.xml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/datatypes_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/environment_modules_mapping.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/environment_modules_mapping.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/error_report.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/error_report.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/file_sources_conf.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/file_sources_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/galaxy.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/galaxy.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/job_conf.sample.yml` & `galaxy_config-24.0.2/galaxy/config/sample/job_conf.sample.yml`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/job_conf.xml.sample_advanced` & `galaxy_config-24.0.2/galaxy/config/sample/job_conf.xml.sample_advanced`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/job_resource_params_conf.xml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/job_resource_params_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/lmod_modules_mapping.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/lmod_modules_mapping.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/object_store_conf.sample.yml` & `galaxy_config-24.0.2/galaxy/config/sample/object_store_conf.sample.yml`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/object_store_conf.xml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/object_store_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/oidc_backends_config.xml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/oidc_backends_config.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/oidc_config.xml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/oidc_config.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/reports.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/reports.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/themes_conf.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/themes_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/tool_conf.xml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/tool_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/tool_data_table_conf.xml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/tool_data_table_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/tool_destinations.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/tool_destinations.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/tool_recommendations_overwrite.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/tool_recommendations_overwrite.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/tool_shed.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/tool_shed.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/trs_servers_conf.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/trs_servers_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/user_preferences_extra_conf.yml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/user_preferences_extra_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/workflow_resource_params_conf.xml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/workflow_resource_params_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/sample/workflow_schedulers_conf.xml.sample` & `galaxy_config-24.0.2/galaxy/config/sample/workflow_schedulers_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/schema.py` & `galaxy_config-24.0.2/galaxy/config/schema.py`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/schemas/config_schema.yml` & `galaxy_config-24.0.2/galaxy/config/schemas/config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/schemas/job_config_schema.yml` & `galaxy_config-24.0.2/galaxy/config/schemas/job_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/schemas/reports_config_schema.yml` & `galaxy_config-24.0.2/galaxy/config/schemas/reports_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/schemas/tool_shed_config_schema.yml` & `galaxy_config-24.0.2/galaxy/config/schemas/tool_shed_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/script.py` & `galaxy_config-24.0.2/galaxy/config/script.py`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy/config/templates.py` & `galaxy_config-24.0.2/galaxy/config/templates.py`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/galaxy_config.egg-info/PKG-INFO` & `galaxy_config-24.0.2/galaxy_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-config
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy configuration
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,14 +47,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_config-24.0.1/galaxy_config.egg-info/SOURCES.txt` & `galaxy_config-24.0.2/galaxy_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy_config-24.0.1/setup.cfg` & `galaxy_config-24.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-config
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.1
+version = 24.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	boltons
 	jinja2
```

