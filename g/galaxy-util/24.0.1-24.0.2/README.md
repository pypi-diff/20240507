# Comparing `tmp/galaxy_util-24.0.1.tar.gz` & `tmp/galaxy_util-24.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_util-24.0.1.tar", last modified: Thu May  2 13:47:03 2024, max compression
+gzip compressed data, was "galaxy_util-24.0.2.tar", last modified: Tue May  7 14:32:07 2024, max compression
```

## Comparing `galaxy_util-24.0.1.tar` & `galaxy_util-24.0.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:03.245302 galaxy_util-24.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-05-02 13:47:03.245302 galaxy_util-24.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:03.229302 galaxy_util-24.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:03.233302 galaxy_util-24.0.1/galaxy/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/exceptions/error_codes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/exceptions/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/exceptions/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:03.241302 galaxy_util-24.0.1/galaxy/util/
--rw-r--r--   0 runner    (1001) docker     (127)    63297 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/aliaspickler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/bool_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/bunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/bytesize.py
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/config_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:03.241302 galaxy_util-24.0.1/galaxy/util/custom_logging/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/custom_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/custom_logging/fluent_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/dictifiable.py
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/docutils_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/drs.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/facts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/filelock.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/form_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/hash_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/image_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/inflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/jstree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/lazy_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/monitors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/odict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/oset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:03.241302 galaxy_util-24.0.1/galaxy/util/path/
--rw-r--r--   0 runner    (1001) docker     (127)    16890 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/path/ntpath.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/path/posixpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/permutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/plugin_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/renamed_temporary_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/rst_to_html.py
--rw-r--r--   0 runner    (1001) docker     (127)    18165 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/rules_dsl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11738 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/rules_dsl_spec.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/sanitize_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/simplegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/sleeper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/sockets.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/specs.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/submodules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/themes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:03.241302 galaxy_util-24.0.1/galaxy/util/tool_shed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/tool_shed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/tool_shed/common_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/tool_shed/encoding_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/tool_shed/tool_shed_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/tool_shed/xml_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/tool_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/topsort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/tree_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/ucsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/unittest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:03.241302 galaxy_util-24.0.1/galaxy/util/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/xml_macros.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/yaml_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/util/zipstream.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/galaxy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:03.241302 galaxy_util-24.0.1/galaxy_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-05-02 13:47:03.000000 galaxy_util-24.0.1/galaxy_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-02 13:47:03.000000 galaxy_util-24.0.1/galaxy_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:47:03.000000 galaxy_util-24.0.1/galaxy_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-02 13:47:03.000000 galaxy_util-24.0.1/galaxy_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:47:03.000000 galaxy_util-24.0.1/galaxy_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-02 13:47:03.245302 galaxy_util-24.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 13:46:45.000000 galaxy_util-24.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:07.277464 galaxy_util-24.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-07 14:31:49.000000 galaxy_util-24.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-05-07 14:32:07.277464 galaxy_util-24.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:07.261464 galaxy_util-24.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:07.261464 galaxy_util-24.0.2/galaxy/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     8490 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/exceptions/error_codes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/exceptions/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/exceptions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:07.273464 galaxy_util-24.0.2/galaxy/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    63297 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/aliaspickler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/bool_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/bytesize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/config_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:07.273464 galaxy_util-24.0.2/galaxy/util/custom_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/custom_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/custom_logging/fluent_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/dictifiable.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/docutils_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/drs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/facts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/form_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/hash_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/image_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/inflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/jstree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/lazy_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/odict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/oset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:07.273464 galaxy_util-24.0.2/galaxy/util/path/
+-rw-r--r--   0 runner    (1001) docker     (127)    16890 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/path/ntpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/path/posixpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/permutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/plugin_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/renamed_temporary_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/rst_to_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18165 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/rules_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11738 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/rules_dsl_spec.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/sanitize_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/simplegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/sleeper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/submodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/themes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:07.277464 galaxy_util-24.0.2/galaxy/util/tool_shed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/tool_shed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/tool_shed/common_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/tool_shed/encoding_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/tool_shed/tool_shed_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/tool_shed/xml_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/tool_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/topsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/tree_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/ucsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:07.277464 galaxy_util-24.0.2/galaxy/util/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/xml_macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/yaml_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/util/zipstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/galaxy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:07.277464 galaxy_util-24.0.2/galaxy_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-05-07 14:32:07.000000 galaxy_util-24.0.2/galaxy_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-07 14:32:07.000000 galaxy_util-24.0.2/galaxy_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:32:07.000000 galaxy_util-24.0.2/galaxy_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-07 14:32:07.000000 galaxy_util-24.0.2/galaxy_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:32:07.000000 galaxy_util-24.0.2/galaxy_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-07 14:32:07.277464 galaxy_util-24.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 14:31:50.000000 galaxy_util-24.0.2/test-requirements.txt
```

### Comparing `galaxy_util-24.0.1/HISTORY.rst` & `galaxy_util-24.0.2/HISTORY.rst`

 * *Files 1% similar despite different names*

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
+* Adds logging of messageExceptions in the fastapi exception handler. by `@dannon <https://github.com/dannon>`_ in `#18041 <https://github.com/galaxyproject/galaxy/pull/18041>`_
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_util-24.0.1/LICENSE` & `galaxy_util-24.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/PKG-INFO` & `galaxy_util-24.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-util
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy generic utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,14 +59,25 @@
 
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
+* Adds logging of messageExceptions in the fastapi exception handler. by `@dannon <https://github.com/dannon>`_ in `#18041 <https://github.com/galaxyproject/galaxy/pull/18041>`_
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_util-24.0.1/galaxy/exceptions/__init__.py` & `galaxy_util-24.0.2/galaxy/exceptions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,31 @@
 
 Reflecting Galaxy's origins as a web application, these exceptions tend to be a
 bit web-oriented. However this module is a dependency of modules and tools that
 have nothing to do with the web - keep this in mind when defining exception names
 and messages.
 """
 
+from typing import Optional
+
 from .error_codes import (
     error_codes_by_name,
     ErrorCode,
 )
 
 
 class MessageException(Exception):
     """Most generic Galaxy exception - indicates merely that some exceptional condition happened."""
 
     # status code to be set when used with API.
     status_code: int = 400
     # Error code information embedded into API json responses.
     err_code: ErrorCode = error_codes_by_name["UNKNOWN"]
 
-    def __init__(self, err_msg=None, type="info", **extra_error_info):
+    def __init__(self, err_msg: Optional[str] = None, type="info", **extra_error_info):
         self.err_msg = err_msg or self.err_code.default_error_message
         self.type = type
         self.extra_error_info = extra_error_info
 
     @staticmethod
     def from_code(status_code, message):
         exception_class = MessageException
@@ -60,15 +62,15 @@
 
 
 class AcceptedRetryLater(MessageException):
     status_code = 202
     err_code = error_codes_by_name["ACCEPTED_RETRY_LATER"]
     retry_after: int
 
-    def __init__(self, msg, retry_after=60):
+    def __init__(self, msg: Optional[str] = None, retry_after=60):
         super().__init__(msg)
         self.retry_after = retry_after
 
 
 class NoContentException(MessageException):
     status_code = 204
     err_code = error_codes_by_name["NO_CONTENT_GENERIC"]
@@ -132,15 +134,15 @@
     err_code = error_codes_by_name["USER_TOOL_META_PARAMETER_PROBLEM"]
 
 
 class ToolMissingException(MessageException):
     status_code = 400
     err_code = error_codes_by_name["USER_TOOL_MISSING_PROBLEM"]
 
-    def __init__(self, err_msg=None, type="info", tool_id=None, **extra_error_info):
+    def __init__(self, err_msg: Optional[str] = None, type="info", tool_id=None, **extra_error_info):
         super().__init__(err_msg, type, **extra_error_info)
         self.tool_id = tool_id
 
 
 class RequestParameterInvalidException(MessageException):
     status_code = 400
     err_code = error_codes_by_name["USER_REQUEST_INVALID_PARAMETER"]
@@ -148,15 +150,15 @@
 
 class ToolInputsNotReadyException(MessageException):
     status_code = 400
     error_code = error_codes_by_name["TOOL_INPUTS_NOT_READY"]
 
 
 class ToolInputsNotOKException(MessageException):
-    def __init__(self, err_msg=None, type="info", *, src: str, id: int, **extra_error_info):
+    def __init__(self, err_msg: Optional[str] = None, type="info", *, src: str, id: int, **extra_error_info):
         super().__init__(err_msg, type, **extra_error_info)
         self.src = src
         self.id = id
 
     status_code = 400
     error_code = error_codes_by_name["TOOL_INPUTS_NOT_OK"]
```

### Comparing `galaxy_util-24.0.1/galaxy/exceptions/error_codes.json` & `galaxy_util-24.0.2/galaxy/exceptions/error_codes.json`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/exceptions/error_codes.py` & `galaxy_util-24.0.2/galaxy/exceptions/error_codes.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/exceptions/utils.py` & `galaxy_util-24.0.2/galaxy/exceptions/utils.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/__init__.py` & `galaxy_util-24.0.2/galaxy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/aliaspickler.py` & `galaxy_util-24.0.2/galaxy/util/aliaspickler.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/bool_expressions.py` & `galaxy_util-24.0.2/galaxy/util/bool_expressions.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/bunch.py` & `galaxy_util-24.0.2/galaxy/util/bunch.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/bytesize.py` & `galaxy_util-24.0.2/galaxy/util/bytesize.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/checkers.py` & `galaxy_util-24.0.2/galaxy/util/checkers.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/commands.py` & `galaxy_util-24.0.2/galaxy/util/commands.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/compression_utils.py` & `galaxy_util-24.0.2/galaxy/util/compression_utils.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/config_parsers.py` & `galaxy_util-24.0.2/galaxy/util/config_parsers.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/custom_logging/fluent_log.py` & `galaxy_util-24.0.2/galaxy/util/custom_logging/fluent_log.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/dictifiable.py` & `galaxy_util-24.0.2/galaxy/util/dictifiable.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/drs.py` & `galaxy_util-24.0.2/galaxy/util/drs.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/expressions.py` & `galaxy_util-24.0.2/galaxy/util/expressions.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/facts.py` & `galaxy_util-24.0.2/galaxy/util/facts.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/filelock.py` & `galaxy_util-24.0.2/galaxy/util/filelock.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/form_builder.py` & `galaxy_util-24.0.2/galaxy/util/form_builder.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/hash_util.py` & `galaxy_util-24.0.2/galaxy/util/hash_util.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/heartbeat.py` & `galaxy_util-24.0.2/galaxy/util/heartbeat.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/image_util.py` & `galaxy_util-24.0.2/galaxy/util/image_util.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/inflection.py` & `galaxy_util-24.0.2/galaxy/util/inflection.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/json.py` & `galaxy_util-24.0.2/galaxy/util/json.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/jstree.py` & `galaxy_util-24.0.2/galaxy/util/jstree.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/lazy_process.py` & `galaxy_util-24.0.2/galaxy/util/lazy_process.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/monitors.py` & `galaxy_util-24.0.2/galaxy/util/monitors.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/odict.py` & `galaxy_util-24.0.2/galaxy/util/odict.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/oset.py` & `galaxy_util-24.0.2/galaxy/util/oset.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/path/__init__.py` & `galaxy_util-24.0.2/galaxy/util/path/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/permutations.py` & `galaxy_util-24.0.2/galaxy/util/permutations.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/plugin_config.py` & `galaxy_util-24.0.2/galaxy/util/plugin_config.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/properties.py` & `galaxy_util-24.0.2/galaxy/util/properties.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/renamed_temporary_file.py` & `galaxy_util-24.0.2/galaxy/util/renamed_temporary_file.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/resources.py` & `galaxy_util-24.0.2/galaxy/util/resources.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/rst_to_html.py` & `galaxy_util-24.0.2/galaxy/util/rst_to_html.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/rules_dsl.py` & `galaxy_util-24.0.2/galaxy/util/rules_dsl.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/rules_dsl_spec.yml` & `galaxy_util-24.0.2/galaxy/util/rules_dsl_spec.yml`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/sanitize_html.py` & `galaxy_util-24.0.2/galaxy/util/sanitize_html.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/script.py` & `galaxy_util-24.0.2/galaxy/util/script.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/search.py` & `galaxy_util-24.0.2/galaxy/util/search.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/simplegraph.py` & `galaxy_util-24.0.2/galaxy/util/simplegraph.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/sleeper.py` & `galaxy_util-24.0.2/galaxy/util/sleeper.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/sockets.py` & `galaxy_util-24.0.2/galaxy/util/sockets.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/specs.py` & `galaxy_util-24.0.2/galaxy/util/specs.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/sqlite.py` & `galaxy_util-24.0.2/galaxy/util/sqlite.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/submodules.py` & `galaxy_util-24.0.2/galaxy/util/submodules.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/task.py` & `galaxy_util-24.0.2/galaxy/util/task.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/template.py` & `galaxy_util-24.0.2/galaxy/util/template.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/themes.py` & `galaxy_util-24.0.2/galaxy/util/themes.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/tool_shed/common_util.py` & `galaxy_util-24.0.2/galaxy/util/tool_shed/common_util.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/tool_shed/encoding_util.py` & `galaxy_util-24.0.2/galaxy/util/tool_shed/encoding_util.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/tool_shed/tool_shed_registry.py` & `galaxy_util-24.0.2/galaxy/util/tool_shed/tool_shed_registry.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/tool_shed/xml_util.py` & `galaxy_util-24.0.2/galaxy/util/tool_shed/xml_util.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/topsort.py` & `galaxy_util-24.0.2/galaxy/util/topsort.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/tree_dict.py` & `galaxy_util-24.0.2/galaxy/util/tree_dict.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/ucsc.py` & `galaxy_util-24.0.2/galaxy/util/ucsc.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/unittest.py` & `galaxy_util-24.0.2/galaxy/util/unittest.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/unittest_utils/__init__.py` & `galaxy_util-24.0.2/galaxy/util/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/validation.py` & `galaxy_util-24.0.2/galaxy/util/validation.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/watcher.py` & `galaxy_util-24.0.2/galaxy/util/watcher.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/xml_macros.py` & `galaxy_util-24.0.2/galaxy/util/xml_macros.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/yaml_util.py` & `galaxy_util-24.0.2/galaxy/util/yaml_util.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy/util/zipstream.py` & `galaxy_util-24.0.2/galaxy/util/zipstream.py`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/galaxy_util.egg-info/PKG-INFO` & `galaxy_util-24.0.2/galaxy_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-util
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy generic utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,14 +59,25 @@
 
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
+* Adds logging of messageExceptions in the fastapi exception handler. by `@dannon <https://github.com/dannon>`_ in `#18041 <https://github.com/galaxyproject/galaxy/pull/18041>`_
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_util-24.0.1/galaxy_util.egg-info/SOURCES.txt` & `galaxy_util-24.0.2/galaxy_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy_util-24.0.1/setup.cfg` & `galaxy_util-24.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-util
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.1
+version = 24.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	bleach
 	boltons
 	docutils!=0.17,!=0.17.1
```

