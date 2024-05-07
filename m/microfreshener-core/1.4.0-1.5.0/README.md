# Comparing `tmp/microfreshener-core-1.4.0.tar.gz` & `tmp/microfreshener-core-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microfreshener-core-1.4.0.tar", last modified: Thu Sep  5 15:03:45 2019, max compression
+gzip compressed data, was "microfreshener-core-1.5.0.tar", last modified: Tue May  7 10:21:23 2024, max compression
```

## Comparing `microfreshener-core-1.4.0.tar` & `microfreshener-core-1.5.0.tar`

### file list

```diff
@@ -1,104 +1,113 @@
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener/
--rw-r--r--   0 dido      (1000) dido      (1000)     1575 2019-07-05 11:23:42.000000 microfreshener-core-1.4.0/microfreshener/command_line.py
--rw-r--r--   0 dido      (1000) dido      (1000)      134 2019-09-05 15:02:31.000000 microfreshener-core-1.4.0/microfreshener/__init__.py
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener/core/
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener/core/helper/
--rw-r--r--   0 dido      (1000) dido      (1000)      989 2019-05-30 17:08:10.000000 microfreshener-core-1.4.0/microfreshener/core/helper/decorator.py
--rw-r--r--   0 dido      (1000) dido      (1000)        0 2019-06-03 10:00:32.000000 microfreshener-core-1.4.0/microfreshener/core/helper/__init__.py
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener/core/importer/
--rw-r--r--   0 dido      (1000) dido      (1000)      179 2019-05-30 17:08:10.000000 microfreshener-core-1.4.0/microfreshener/core/importer/iimporter.py
--rw-r--r--   0 dido      (1000) dido      (1000)      494 2019-08-30 11:25:07.000000 microfreshener-core-1.4.0/microfreshener/core/importer/jsontype.py
--rw-r--r--   0 dido      (1000) dido      (1000)     8117 2019-08-30 11:24:10.000000 microfreshener-core-1.4.0/microfreshener/core/importer/ymlimporter.py
--rw-r--r--   0 dido      (1000) dido      (1000)       75 2019-05-30 17:08:10.000000 microfreshener-core-1.4.0/microfreshener/core/importer/__init__.py
--rw-r--r--   0 dido      (1000) dido      (1000)      358 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/microfreshener/core/importer/ymltype.py
--rw-r--r--   0 dido      (1000) dido      (1000)     8390 2019-08-30 11:32:03.000000 microfreshener-core-1.4.0/microfreshener/core/importer/jsonimporter.py
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener/core/refiner/
--rw-r--r--   0 dido      (1000) dido      (1000)      199 2019-09-04 10:35:13.000000 microfreshener-core-1.4.0/microfreshener/core/refiner/irefiner.py
--rw-r--r--   0 dido      (1000) dido      (1000)       89 2019-09-04 11:08:59.000000 microfreshener-core-1.4.0/microfreshener/core/refiner/__init__.py
--rw-r--r--   0 dido      (1000) dido      (1000)     3258 2019-09-04 15:04:02.000000 microfreshener-core-1.4.0/microfreshener/core/refiner/istiorefiner.py
--rw-r--r--   0 dido      (1000) dido      (1000)     5835 2019-09-04 14:22:28.000000 microfreshener-core-1.4.0/microfreshener/core/refiner/kubernetesrefiner.py
--rw-r--r--   0 dido      (1000) dido      (1000)     1539 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/microfreshener/core/logging.py
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener/core/analyser/
--rw-r--r--   0 dido      (1000) dido      (1000)     4072 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/microfreshener/core/analyser/analyser.py
--rw-r--r--   0 dido      (1000) dido      (1000)      315 2019-05-30 17:08:10.000000 microfreshener-core-1.4.0/microfreshener/core/analyser/constant.py
--rw-r--r--   0 dido      (1000) dido      (1000)     1016 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/microfreshener/core/analyser/costants.py
--rw-r--r--   0 dido      (1000) dido      (1000)     5514 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/microfreshener/core/analyser/smell.py
--rw-r--r--   0 dido      (1000) dido      (1000)     3234 2019-06-03 14:52:57.000000 microfreshener-core-1.4.0/microfreshener/core/analyser/builder.py
--rw-r--r--   0 dido      (1000) dido      (1000)     4148 2019-08-30 11:12:09.000000 microfreshener-core-1.4.0/microfreshener/core/analyser/sniffer.py
--rw-r--r--   0 dido      (1000) dido      (1000)      344 2019-05-30 17:08:10.000000 microfreshener-core-1.4.0/microfreshener/core/analyser/refactorings.py
--rw-r--r--   0 dido      (1000) dido      (1000)      247 2019-05-30 17:08:10.000000 microfreshener-core-1.4.0/microfreshener/core/analyser/__init__.py
--rw-r--r--   0 dido      (1000) dido      (1000)     2119 2019-09-03 17:33:11.000000 microfreshener-core-1.4.0/microfreshener/core/errors.py
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener/core/model/
--rw-r--r--   0 dido      (1000) dido      (1000)     1047 2019-09-05 15:02:19.000000 microfreshener-core-1.4.0/microfreshener/core/model/type.py
--rw-r--r--   0 dido      (1000) dido      (1000)     4434 2019-09-03 17:47:20.000000 microfreshener-core-1.4.0/microfreshener/core/model/nodes.py
--rw-r--r--   0 dido      (1000) dido      (1000)     6227 2019-09-04 14:17:15.000000 microfreshener-core-1.4.0/microfreshener/core/model/microtosca.py
--rw-r--r--   0 dido      (1000) dido      (1000)     4891 2019-09-04 14:53:41.000000 microfreshener-core-1.4.0/microfreshener/core/model/relationships.py
--rw-r--r--   0 dido      (1000) dido      (1000)     1651 2019-09-03 17:33:04.000000 microfreshener-core-1.4.0/microfreshener/core/model/groups.py
--rw-r--r--   0 dido      (1000) dido      (1000)      296 2019-08-30 11:15:51.000000 microfreshener-core-1.4.0/microfreshener/core/model/__init__.py
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener/core/exporter/
--rw-r--r--   0 dido      (1000) dido      (1000)     3913 2019-08-30 17:55:50.000000 microfreshener-core-1.4.0/microfreshener/core/exporter/jsonexporter.py
--rw-r--r--   0 dido      (1000) dido      (1000)      181 2019-05-30 17:08:10.000000 microfreshener-core-1.4.0/microfreshener/core/exporter/iexporter.py
--rw-r--r--   0 dido      (1000) dido      (1000)     7308 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/microfreshener/core/exporter/ymlexporter.py
--rw-r--r--   0 dido      (1000) dido      (1000)       75 2019-05-30 17:08:10.000000 microfreshener-core-1.4.0/microfreshener/core/exporter/__init__.py
--rw-r--r--   0 dido      (1000) dido      (1000)        0 2019-05-30 17:08:10.000000 microfreshener-core-1.4.0/microfreshener/core/__init__.py
--rw-r--r--   0 dido      (1000) dido      (1000)        0 2018-11-28 14:38:48.000000 microfreshener-core-1.4.0/README.rst
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener_core.egg-info/
--rw-r--r--   0 dido      (1000) dido      (1000)       68 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener_core.egg-info/entry_points.txt
--rw-r--r--   0 dido      (1000) dido      (1000)        1 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener_core.egg-info/dependency_links.txt
--rw-r--r--   0 dido      (1000) dido      (1000)       25 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener_core.egg-info/requires.txt
--rw-r--r--   0 dido      (1000) dido      (1000)       21 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener_core.egg-info/top_level.txt
--rw-r--r--   0 dido      (1000) dido      (1000)     3401 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener_core.egg-info/SOURCES.txt
--rw-r--r--   0 dido      (1000) dido      (1000)        1 2019-05-30 16:40:13.000000 microfreshener-core-1.4.0/microfreshener_core.egg-info/not-zip-safe
--rw-r--r--   0 dido      (1000) dido      (1000)      382 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/microfreshener_core.egg-info/PKG-INFO
--rw-r--r--   0 dido      (1000) dido      (1000)      555 2019-09-05 15:03:22.000000 microfreshener-core-1.4.0/HISTORY.rst
--rw-r--r--   0 dido      (1000) dido      (1000)      167 2019-05-30 17:08:10.000000 microfreshener-core-1.4.0/MANIFEST.in
--rw-r--r--   0 dido      (1000) dido      (1000)       38 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/setup.cfg
--rw-r--r--   0 dido      (1000) dido      (1000)     1273 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/setup.py
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/tests/
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/tests/test_analyser/
--rw-r--r--   0 dido      (1000) dido      (1000)     5716 2019-05-30 17:08:10.000000 microfreshener-core-1.4.0/tests/test_analyser/test_sniffer_wbsi.py
--rw-r--r--   0 dido      (1000) dido      (1000)     1061 2019-08-09 16:39:20.000000 microfreshener-core-1.4.0/tests/test_analyser/test_sniffer_ctdm.py
--rw-r--r--   0 dido      (1000) dido      (1000)     3396 2019-09-03 10:55:17.000000 microfreshener-core-1.4.0/tests/test_analyser/test_sniffer_nagw.py
--rw-r--r--   0 dido      (1000) dido      (1000)     4807 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_analyser/test_sniffer_ebsi.py
--rw-r--r--   0 dido      (1000) dido      (1000)     1348 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_analyser/test_sniffer_shpr.py
--rw-r--r--   0 dido      (1000) dido      (1000)     2282 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_analyser/test_analyser.py
--rw-r--r--   0 dido      (1000) dido      (1000)     2135 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_analyser/test_builder.py
--rw-r--r--   0 dido      (1000) dido      (1000)        0 2019-05-15 15:19:46.000000 microfreshener-core-1.4.0/tests/test_analyser/__init__.py
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/tests/test_exporter/
--rw-r--r--   0 dido      (1000) dido      (1000)     1518 2019-05-30 17:08:10.000000 microfreshener-core-1.4.0/tests/test_exporter/test_export_yml_groups.py
--rw-r--r--   0 dido      (1000) dido      (1000)     1535 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_exporter/test_export_json.py
--rw-r--r--   0 dido      (1000) dido      (1000)     7100 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_exporter/test_export_yml_relationships_properties.py
--rw-r--r--   0 dido      (1000) dido      (1000)     1446 2019-08-30 11:23:00.000000 microfreshener-core-1.4.0/tests/test_exporter/test_export_yml_nodes.py
--rw-r--r--   0 dido      (1000) dido      (1000)     4787 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_exporter/test_export_json_relationships_properties.py
--rw-r--r--   0 dido      (1000) dido      (1000)        0 2019-05-15 15:19:46.000000 microfreshener-core-1.4.0/tests/test_exporter/__init__.py
--rw-r--r--   0 dido      (1000) dido      (1000)     1876 2019-08-30 11:23:00.000000 microfreshener-core-1.4.0/tests/test_exporter/test_export_json_nodes.py
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/tests/test_importer/
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/tests/test_importer/yml_importer/
--rw-r--r--   0 dido      (1000) dido      (1000)     1051 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_importer/yml_importer/test_import_yml_groups.py
--rw-r--r--   0 dido      (1000) dido      (1000)     4049 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_importer/yml_importer/test_import_yml.py
--rw-r--r--   0 dido      (1000) dido      (1000)     6820 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_importer/yml_importer/test_import_yml_relationships_properties.py
--rw-r--r--   0 dido      (1000) dido      (1000)     1704 2019-08-30 11:23:39.000000 microfreshener-core-1.4.0/tests/test_importer/yml_importer/test_import_yml_nodes.py
--rw-r--r--   0 dido      (1000) dido      (1000)        0 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_importer/yml_importer/__init__.py
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/tests/test_importer/json_importer/
--rw-r--r--   0 dido      (1000) dido      (1000)     2400 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_importer/json_importer/test_import_json_relationships.py
--rw-r--r--   0 dido      (1000) dido      (1000)     7596 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_importer/json_importer/test_import_json.py
--rw-r--r--   0 dido      (1000) dido      (1000)     4379 2019-08-30 11:32:38.000000 microfreshener-core-1.4.0/tests/test_importer/json_importer/test_import_json_nodes.py
--rw-r--r--   0 dido      (1000) dido      (1000)     2957 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_importer/json_importer/test_import_json_relationships_properties.py
--rw-r--r--   0 dido      (1000) dido      (1000)        0 2019-08-30 10:54:17.000000 microfreshener-core-1.4.0/tests/test_importer/json_importer/__init__.py
--rw-r--r--   0 dido      (1000) dido      (1000)        0 2019-05-15 15:19:46.000000 microfreshener-core-1.4.0/tests/test_importer/__init__.py
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/tests/test_model/
--rw-r--r--   0 dido      (1000) dido      (1000)     6392 2019-09-04 14:53:51.000000 microfreshener-core-1.4.0/tests/test_model/test_relationships.py
--rw-r--r--   0 dido      (1000) dido      (1000)     9091 2019-09-04 14:21:32.000000 microfreshener-core-1.4.0/tests/test_model/test_microtosca.py
--rw-r--r--   0 dido      (1000) dido      (1000)        0 2019-08-07 13:37:02.000000 microfreshener-core-1.4.0/tests/test_model/__init__.py
--rw-r--r--   0 dido      (1000) dido      (1000)     2564 2019-09-03 17:33:21.000000 microfreshener-core-1.4.0/tests/test_model/test_group.py
-drwxr-xr-x   0 dido      (1000) dido      (1000)        0 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/tests/test_refiner/
--rw-r--r--   0 dido      (1000) dido      (1000)      368 2019-09-02 12:04:10.000000 microfreshener-core-1.4.0/tests/test_refiner/test_load_kdeployment.py
--rw-r--r--   0 dido      (1000) dido      (1000)     1453 2019-09-04 11:40:33.000000 microfreshener-core-1.4.0/tests/test_refiner/test_istio_refiner_destination_rule.py
--rw-r--r--   0 dido      (1000) dido      (1000)      365 2019-09-02 12:09:45.000000 microfreshener-core-1.4.0/tests/test_refiner/test_load_kingress.py
--rw-r--r--   0 dido      (1000) dido      (1000)      888 2019-09-02 11:42:54.000000 microfreshener-core-1.4.0/tests/test_refiner/test_kubernetes_refiner.py
--rw-r--r--   0 dido      (1000) dido      (1000)        0 2019-08-30 11:57:03.000000 microfreshener-core-1.4.0/tests/test_refiner/__init__.py
--rw-r--r--   0 dido      (1000) dido      (1000)       38 2018-11-28 14:29:30.000000 microfreshener-core-1.4.0/tests/__init__.py
--rw-r--r--   0 dido      (1000) dido      (1000)        0 2019-05-30 17:08:10.000000 microfreshener-core-1.4.0/DESCRIPTION.rst
--rw-r--r--   0 dido      (1000) dido      (1000)     1068 2019-01-17 16:57:16.000000 microfreshener-core-1.4.0/LICENSE
--rw-r--r--   0 dido      (1000) dido      (1000)      382 2019-09-05 15:03:45.000000 microfreshener-core-1.4.0/PKG-INFO
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.488001 microfreshener-core-1.5.0/
+-rw-r--r--   0 meek      (1000) meek      (1000)        0 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/DESCRIPTION.rst
+-rw-r--r--   0 meek      (1000) meek      (1000)      657 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/HISTORY.rst
+-rw-r--r--   0 meek      (1000) meek      (1000)     1068 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/LICENSE
+-rw-r--r--   0 meek      (1000) meek      (1000)      167 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/MANIFEST.in
+-rw-r--r--   0 meek      (1000) meek      (1000)      358 2024-05-07 10:21:23.488001 microfreshener-core-1.5.0/PKG-INFO
+-rw-r--r--   0 meek      (1000) meek      (1000)        0 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/README.rst
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.476001 microfreshener-core-1.5.0/microfreshener/
+-rw-r--r--   0 meek      (1000) meek      (1000)      134 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/__init__.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     1575 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/command_line.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.477001 microfreshener-core-1.5.0/microfreshener/core/
+-rw-r--r--   0 meek      (1000) meek      (1000)        0 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/__init__.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.478001 microfreshener-core-1.5.0/microfreshener/core/analyser/
+-rw-r--r--   0 meek      (1000) meek      (1000)      247 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/analyser/__init__.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     4280 2023-10-26 00:10:46.000000 microfreshener-core-1.5.0/microfreshener/core/analyser/analyser.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     4627 2023-12-30 22:09:59.000000 microfreshener-core-1.5.0/microfreshener/core/analyser/builder.py
+-rw-r--r--   0 meek      (1000) meek      (1000)      315 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/analyser/constant.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     1385 2024-04-05 21:22:47.000000 microfreshener-core-1.5.0/microfreshener/core/analyser/costants.py
+-rw-r--r--   0 meek      (1000) meek      (1000)      344 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/analyser/refactorings.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     7800 2024-04-05 21:22:47.000000 microfreshener-core-1.5.0/microfreshener/core/analyser/smell.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     7683 2024-05-06 15:55:23.000000 microfreshener-core-1.5.0/microfreshener/core/analyser/sniffer.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     2119 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/errors.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.478001 microfreshener-core-1.5.0/microfreshener/core/exporter/
+-rw-r--r--   0 meek      (1000) meek      (1000)       75 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/exporter/__init__.py
+-rw-r--r--   0 meek      (1000) meek      (1000)      181 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/exporter/iexporter.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     4201 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/exporter/jsonexporter.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     7701 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/exporter/ymlexporter.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.479001 microfreshener-core-1.5.0/microfreshener/core/helper/
+-rw-r--r--   0 meek      (1000) meek      (1000)        0 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/helper/__init__.py
+-rw-r--r--   0 meek      (1000) meek      (1000)      989 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/helper/decorator.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.480001 microfreshener-core-1.5.0/microfreshener/core/importer/
+-rw-r--r--   0 meek      (1000) meek      (1000)       75 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/importer/__init__.py
+-rw-r--r--   0 meek      (1000) meek      (1000)      179 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/importer/iimporter.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     8779 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/importer/jsonimporter.py
+-rw-r--r--   0 meek      (1000) meek      (1000)      570 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/importer/jsontype.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     8189 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/importer/ymlimporter.py
+-rw-r--r--   0 meek      (1000) meek      (1000)      391 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/importer/ymltype.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     1539 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/logging.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.480001 microfreshener-core-1.5.0/microfreshener/core/model/
+-rw-r--r--   0 meek      (1000) meek      (1000)      324 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/model/__init__.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     1651 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/model/groups.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     7745 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/model/microtosca.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     5857 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/model/nodes.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     5771 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/model/relationships.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     1168 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/model/type.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.481001 microfreshener-core-1.5.0/microfreshener/core/refiner/
+-rw-r--r--   0 meek      (1000) meek      (1000)       89 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/refiner/__init__.py
+-rw-r--r--   0 meek      (1000) meek      (1000)      199 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/refiner/irefiner.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     3258 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/refiner/istiorefiner.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     5835 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/microfreshener/core/refiner/kubernetesrefiner.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.482001 microfreshener-core-1.5.0/microfreshener_core.egg-info/
+-rw-r--r--   0 meek      (1000) meek      (1000)      358 2024-05-07 10:21:22.000000 microfreshener-core-1.5.0/microfreshener_core.egg-info/PKG-INFO
+-rw-r--r--   0 meek      (1000) meek      (1000)     3713 2024-05-07 10:21:23.000000 microfreshener-core-1.5.0/microfreshener_core.egg-info/SOURCES.txt
+-rw-r--r--   0 meek      (1000) meek      (1000)        1 2024-05-07 10:21:22.000000 microfreshener-core-1.5.0/microfreshener_core.egg-info/dependency_links.txt
+-rw-r--r--   0 meek      (1000) meek      (1000)       67 2024-05-07 10:21:23.000000 microfreshener-core-1.5.0/microfreshener_core.egg-info/entry_points.txt
+-rw-r--r--   0 meek      (1000) meek      (1000)        1 2023-10-21 16:25:46.000000 microfreshener-core-1.5.0/microfreshener_core.egg-info/not-zip-safe
+-rw-r--r--   0 meek      (1000) meek      (1000)       25 2024-05-07 10:21:23.000000 microfreshener-core-1.5.0/microfreshener_core.egg-info/requires.txt
+-rw-r--r--   0 meek      (1000) meek      (1000)       21 2024-05-07 10:21:23.000000 microfreshener-core-1.5.0/microfreshener_core.egg-info/top_level.txt
+-rw-r--r--   0 meek      (1000) meek      (1000)       38 2024-05-07 10:21:23.488001 microfreshener-core-1.5.0/setup.cfg
+-rw-r--r--   0 meek      (1000) meek      (1000)     1273 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/setup.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.482001 microfreshener-core-1.5.0/tests/
+-rw-r--r--   0 meek      (1000) meek      (1000)       38 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/__init__.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.482001 microfreshener-core-1.5.0/tests/log/
+-rw-r--r--   0 meek      (1000) meek      (1000)     1668 2023-10-21 06:22:11.000000 microfreshener-core-1.5.0/tests/log/log_2023-10-21.log
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.484001 microfreshener-core-1.5.0/tests/test_analyser/
+-rw-r--r--   0 meek      (1000) meek      (1000)        0 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_analyser/__init__.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.484001 microfreshener-core-1.5.0/tests/test_analyser/log/
+-rw-r--r--   0 meek      (1000) meek      (1000)      959 2024-04-05 16:32:07.000000 microfreshener-core-1.5.0/tests/test_analyser/log/log_2024-04-05.log
+-rw-r--r--   0 meek      (1000) meek      (1000)     2807 2023-10-25 12:47:25.000000 microfreshener-core-1.5.0/tests/test_analyser/test_analyser.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     2128 2023-10-25 12:47:25.000000 microfreshener-core-1.5.0/tests/test_analyser/test_builder.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     4807 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_analyser/test_sniffer_ebsi.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     2168 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_analyser/test_sniffer_msioc.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     3396 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_analyser/test_sniffer_nagw.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     2542 2024-04-05 21:22:47.000000 microfreshener-core-1.5.0/tests/test_analyser/test_sniffer_sbc.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     1348 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_analyser/test_sniffer_shpr.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     3885 2024-04-05 21:22:47.000000 microfreshener-core-1.5.0/tests/test_analyser/test_sniffer_slt.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     4072 2024-04-05 21:22:47.000000 microfreshener-core-1.5.0/tests/test_analyser/test_sniffer_tct.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     5716 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_analyser/test_sniffer_wbsi.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.485001 microfreshener-core-1.5.0/tests/test_exporter/
+-rw-r--r--   0 meek      (1000) meek      (1000)        0 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_exporter/__init__.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     1529 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_exporter/test_export_json.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     2167 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_exporter/test_export_json_nodes.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     1237 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_exporter/test_export_json_relationship.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     4787 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_exporter/test_export_json_relationships_properties.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     1518 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_exporter/test_export_yml_groups.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     1691 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_exporter/test_export_yml_nodes.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     7100 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_exporter/test_export_yml_relationships_properties.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.485001 microfreshener-core-1.5.0/tests/test_importer/
+-rw-r--r--   0 meek      (1000) meek      (1000)        0 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_importer/__init__.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.486001 microfreshener-core-1.5.0/tests/test_importer/json_importer/
+-rw-r--r--   0 meek      (1000) meek      (1000)        0 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_importer/json_importer/__init__.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     9062 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_importer/json_importer/test_import_json.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     4822 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_importer/json_importer/test_import_json_nodes.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     2400 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_importer/json_importer/test_import_json_relationships.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     2957 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_importer/json_importer/test_import_json_relationships_properties.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.487001 microfreshener-core-1.5.0/tests/test_importer/yml_importer/
+-rw-r--r--   0 meek      (1000) meek      (1000)        0 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_importer/yml_importer/__init__.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     4497 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_importer/yml_importer/test_import_yml.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     1051 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_importer/yml_importer/test_import_yml_groups.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     1879 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_importer/yml_importer/test_import_yml_nodes.py
+-rw-r--r--   0 meek      (1000) meek      (1000)      703 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_importer/yml_importer/test_import_yml_relationships.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     6820 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_importer/yml_importer/test_import_yml_relationships_properties.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.487001 microfreshener-core-1.5.0/tests/test_model/
+-rw-r--r--   0 meek      (1000) meek      (1000)        0 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_model/__init__.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     2564 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_model/test_group.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     9091 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_model/test_microtosca.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     6392 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_model/test_relationships.py
+drwxr-xr-x   0 meek      (1000) meek      (1000)        0 2024-05-07 10:21:23.488001 microfreshener-core-1.5.0/tests/test_refiner/
+-rw-r--r--   0 meek      (1000) meek      (1000)        0 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_refiner/__init__.py
+-rw-r--r--   0 meek      (1000) meek      (1000)     1453 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_refiner/test_istio_refiner_destination_rule.py
+-rw-r--r--   0 meek      (1000) meek      (1000)      888 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_refiner/test_kubernetes_refiner.py
+-rw-r--r--   0 meek      (1000) meek      (1000)      368 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_refiner/test_load_kdeployment.py
+-rw-r--r--   0 meek      (1000) meek      (1000)      365 2023-10-21 05:56:14.000000 microfreshener-core-1.5.0/tests/test_refiner/test_load_kingress.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `microfreshener-core-1.4.0/microfreshener/command_line.py` & `microfreshener-core-1.5.0/microfreshener/command_line.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/microfreshener/core/helper/decorator.py` & `microfreshener-core-1.5.0/microfreshener/core/helper/decorator.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/microfreshener/core/importer/ymlimporter.py` & `microfreshener-core-1.5.0/microfreshener/core/importer/ymlimporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-import ruamel.yaml
 from pathlib import Path
-from ..model import MicroToscaModel
-from ..model import Service, Datastore, CommunicationPattern, MessageBroker, MessageRouter
-from ..model import KProxy, KService, KIngress
-from ..model.groups import Team, Edge
-from .iimporter import Importer
 
-from ..model.type import MICROTOSCA_NODES_SERVICE, MICROTOSCA_NODES_COMMUNICATIONPATTERN, MICROTOSCA_NODES_DATABASE, MICROTOSCA_NODES_MESSAGE_BROKER, MICROTOSCA_NODES_MESSAGE_ROUTER
-from ..model.type import MICROTOSCA_NODES_MESSAGE_ROUTER_KINGRESS, MICROTOSCA_NODES_MESSAGE_ROUTER_KPROXY, MICROTOSCA_NODES_MESSAGE_ROUTER_KSERVICE
-from ..model.type import MICROTOSCA_GROUPS_TEAM, MICROTOSCA_GROUPS_EDGE
-from ..model.type import MICROTOSCA_RELATIONSHIPS_INTERACT_WITH
-from ..model.type import MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_TIMEOUT_PROPERTY, MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_DYNAMIC_DISCOVEY_PROPERTY, MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_CIRCUIT_BREAKER_PROPERTY
-from .ymltype import YML_INTERACTION
-from .ymltype import YML_RELATIONSHIP_T, YML_RELATIONSHIP_D, YML_RELATIONSHIP_C, YML_RELATIONSHIP_CD, YML_RELATIONSHIP_TC, YML_RELATIONSHIP_TD, YML_RELATIONSHIP_TCD
+import ruamel.yaml
+
+from .iimporter import Importer
+from .ymltype import YML_INTERACTION, YML_DEPLOYED_ON
 from .ymltype import YML_RELATIONSHIP_TEMPLATE
 from ..errors import YMLImporterError
 from ..logging import MyLogger
+from ..model import KProxy, KService, KIngress, Compute
+from ..model import MicroToscaModel
+from ..model import Service, Datastore, MessageBroker, MessageRouter
+from ..model.groups import Team, Edge
+from ..model.type import MICROTOSCA_GROUPS_TEAM, MICROTOSCA_GROUPS_EDGE, MICROTOSCA_NODES_COMPUTE
+from ..model.type import MICROTOSCA_NODES_MESSAGE_ROUTER_KINGRESS, MICROTOSCA_NODES_MESSAGE_ROUTER_KPROXY, \
+    MICROTOSCA_NODES_MESSAGE_ROUTER_KSERVICE
+from ..model.type import MICROTOSCA_NODES_SERVICE, MICROTOSCA_NODES_COMMUNICATIONPATTERN, MICROTOSCA_NODES_DATABASE, \
+    MICROTOSCA_NODES_MESSAGE_BROKER, MICROTOSCA_NODES_MESSAGE_ROUTER
+from ..model.type import MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_TIMEOUT_PROPERTY, \
+    MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_DYNAMIC_DISCOVEY_PROPERTY, \
+    MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_CIRCUIT_BREAKER_PROPERTY
 
 logger = MyLogger().get_logger()
 
+
 class YMLImporter(Importer):
 
     def __init__(self):
         self.micro_model = None
 
-    def Import(self, path_to_yml)->MicroToscaModel:
+    def Import(self, path_to_yml) -> MicroToscaModel:
         self.micro_model = MicroToscaModel('micro.tosca')
         yaml = ruamel.yaml.YAML()  # default  type='rt'
         logger.info("Loading YML file: {}".format(path_to_yml))
         self.micro_yml = yaml.load(Path(path_to_yml))
 
         self.relationship_templates = self._parse_relationship_templates()
         self._add_nodes()
@@ -53,15 +57,16 @@
     def _get_relationship_property_values(self, relationship):
         is_timeout = False
         is_circuit_breaker = False
         is_dynamic_discovery = False
         if MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_TIMEOUT_PROPERTY in relationship['properties']:
             is_timeout = relationship['properties'][MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_TIMEOUT_PROPERTY]
         if MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_CIRCUIT_BREAKER_PROPERTY in relationship['properties']:
-            is_circuit_breaker = relationship['properties'][MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_CIRCUIT_BREAKER_PROPERTY]
+            is_circuit_breaker = relationship['properties'][
+                MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_CIRCUIT_BREAKER_PROPERTY]
         if MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_DYNAMIC_DISCOVEY_PROPERTY in relationship['properties']:
             is_dynamic_discovery = relationship['properties'][
                 MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_DYNAMIC_DISCOVEY_PROPERTY]
         return (is_timeout, is_circuit_breaker, is_dynamic_discovery)
 
     def _add_nodes(self):
         nodes_ruamel = self.micro_yml.get(
@@ -72,14 +77,16 @@
                 el = Service(node_name)
             elif node_type == MICROTOSCA_NODES_DATABASE:
                 el = Datastore(node_name)
             elif node_type == MICROTOSCA_NODES_MESSAGE_BROKER:
                 el = MessageBroker(node_name)
             elif node_type == MICROTOSCA_NODES_MESSAGE_ROUTER:
                 el = MessageRouter(node_name)
+            elif node_type == MICROTOSCA_NODES_COMPUTE:
+                el = Compute(node_name)
             elif node_type == MICROTOSCA_NODES_MESSAGE_ROUTER_KINGRESS:
                 el = KIngress(node_name)
             elif node_type == MICROTOSCA_NODES_MESSAGE_ROUTER_KPROXY:
                 el = KProxy(node_name)
             elif node_type == MICROTOSCA_NODES_MESSAGE_ROUTER_KSERVICE:
                 el = KService(node_name)
             elif node_type == MICROTOSCA_NODES_COMMUNICATIONPATTERN:
@@ -97,34 +104,36 @@
             source_node = self.micro_model[node_name]
             for req in self.get_requirements(commented_map):
                 for interaction_type, target_type in req.items():
                     # [('run_time', ordereddict([('node', 'shipping'), ('relationship', 't'| 'c'| 'd')]))]
                     is_timeout = False
                     is_circuit_breaker = False
                     is_dynamic_discovery = False
-                    if(isinstance(target_type, str)):
+                    if (isinstance(target_type, str)):
                         target_node = self.micro_model[target_type]
                     elif isinstance(target_type, ruamel.yaml.comments.CommentedMap):
                         for key, value in target_type.items():
-                            if(key == "relationship"):
+                            if (key == "relationship"):
                                 rel = self._get_relationship_template_by_name(
                                     value)
                                 (is_timeout, is_circuit_breaker,
                                  is_dynamic_discovery) = self._get_relationship_property_values(rel)
                             elif key == "node":
                                 target_node = self.micro_model[value]
                             else:
                                 raise YMLImporterError(
                                     "Relationship {} not recognized ".format(key))
                     else:
                         raise YMLImporterError(
                             "Target type {} of relatinoship {} not recognized ".format(target_type, req))
-                    if(interaction_type == YML_INTERACTION):
+                    if (interaction_type == YML_INTERACTION):
                         source_node.add_interaction(
                             target_node, is_timeout, is_circuit_breaker, is_dynamic_discovery)
+                    elif interaction_type == YML_DEPLOYED_ON:
+                        source_node.add_deployed_on(target_node)
                     else:
                         raise YMLImporterError(
                             f"Type of interaction {interaction_type} not recognied")
 
     def _add_groups(self):
         if 'groups' in self.micro_yml.get('topology_template'):
             groups_ruamel = self.micro_yml.get(
```

### Comparing `microfreshener-core-1.4.0/microfreshener/core/importer/jsonimporter.py` & `microfreshener-core-1.5.0/microfreshener/core/importer/jsonimporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 
 import json
-from ..model import MicroToscaModel
+from ..model import MicroToscaModel, Compute
 from ..model import Service, Datastore, CommunicationPattern, MessageBroker, MessageRouter
 
 from ..model import KProxy, KService, KIngress
 from ..model.groups import Edge, Team
 from ..model.relationships import InteractsWith, DeploymentTimeInteraction, RunTimeInteraction
 
 from ..logging import MyLogger
 from .iimporter import Importer
 from ..model.type import MICROTOSCA_NODES_MESSAGE_BROKER, MICROTOSCA_NODES_MESSAGE_ROUTER, MICROTOSCA_GROUPS_TEAM, MICROTOSCA_GROUPS_EDGE, MICROTOSCA_RELATIONSHIPS_INTERACT_WITH
 
 from ..model.type import MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_TIMEOUT_PROPERTY, MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_DYNAMIC_DISCOVEY_PROPERTY, MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_CIRCUIT_BREAKER_PROPERTY
-from .jsontype import JSON_RELATIONSHIP_INTERACT_WITH, JSON_RUN_TIME, JSON_DEPLOYMENT_TIME, JSON_NODE_SERVICE, JSON_NODE_DATABASE, JSON_NODE_MESSAGE_BROKER, JSON_NODE_MESSAGE_ROUTER
+from .jsontype import JSON_RELATIONSHIP_INTERACT_WITH, JSON_RUN_TIME, JSON_DEPLOYMENT_TIME, JSON_NODE_SERVICE, \
+    JSON_NODE_DATABASE, JSON_NODE_MESSAGE_BROKER, JSON_NODE_MESSAGE_ROUTER, JSON_NODE_COMPUTE, \
+    JSON_RELATIONSHIP_DEPLOYED_ON
 from .jsontype import JSON_NODE_MESSAGE_ROUTER_KINGRESS, JSON_NODE_MESSAGE_ROUTER_KPROXY, JSON_NODE_MESSAGE_ROUTER_KSERVICE
 from .jsontype import JSON_GROUPS_EDGE, JSON_GROUPS_TEAM
 import os
 
 from ..errors import ImporterError
 logger = MyLogger().get_logger()
 
@@ -62,14 +64,16 @@
             el = Service(name_node)
         elif(type_node == JSON_NODE_MESSAGE_BROKER):
             el = MessageBroker(name_node)
         elif(type_node == JSON_NODE_MESSAGE_ROUTER):
             el = MessageRouter(name_node)
         elif(type_node == JSON_NODE_DATABASE):
             el = Datastore(name_node)
+        elif type_node == JSON_NODE_COMPUTE:
+            el = Compute(name_node)
         elif(type_node == JSON_NODE_MESSAGE_ROUTER_KSERVICE):
             el = KService(name_node)
         elif(type_node == JSON_NODE_MESSAGE_ROUTER_KPROXY):
             el = KProxy(name_node)
         elif(type_node == JSON_NODE_MESSAGE_ROUTER_KINGRESS):
             el = KIngress(name_node)
         else:
@@ -84,14 +88,18 @@
 
     def import_link_from_json(self, link_json):
         type_rel = self.load_type_relationship_from_json(link_json)
         if(type_rel == JSON_RELATIONSHIP_INTERACT_WITH):
             interaction = self.load_interaction_from_json(link_json)
             source = self.load_source_node_from_json(link_json)
             return source.add_interaction(interaction)
+        elif type_rel == JSON_RELATIONSHIP_DEPLOYED_ON:
+            source = self.load_source_node_from_json(link_json)
+            target_node = self.load_target_node_from_json(link_json)
+            source.add_deployed_on(target_node)
         else:
             raise ImporterError(f"Link type {type_rel} not recognized")
 
     def load_interaction_from_json(self, link_json):
         source_node = self.load_source_node_from_json(link_json)
         target_node = self.load_target_node_from_json(link_json)
         (with_timeout, with_circuit_breaker,
```

### Comparing `microfreshener-core-1.4.0/microfreshener/core/refiner/istiorefiner.py` & `microfreshener-core-1.5.0/microfreshener/core/refiner/istiorefiner.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/microfreshener/core/refiner/kubernetesrefiner.py` & `microfreshener-core-1.5.0/microfreshener/core/refiner/kubernetesrefiner.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/microfreshener/core/logging.py` & `microfreshener-core-1.5.0/microfreshener/core/logging.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/microfreshener/core/analyser/analyser.py` & `microfreshener-core-1.5.0/microfreshener/core/analyser/analyser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from ..model import Service, Datastore, CommunicationPattern, MessageBroker, MessageRouter
+from ..model import Service, Datastore, CommunicationPattern, MessageBroker, MessageRouter, Compute
 from ..analyser.sniffer import NodeSmellSniffer, GroupSmellSniffer
 from ..logging import MyLogger
 
 logger = MyLogger().get_logger()
 
 from microfreshener.core.analyser.smell import WobblyServiceInteractionSmell, EndpointBasedServiceInteractionSmell
 
@@ -37,24 +37,26 @@
         return self.node_smell_sniffers
 
     def add_group_smell_sniffer(self, sniffer):
         assert isinstance(sniffer, GroupSmellSniffer)
         logger.info("Group Sniffer {} added".format(sniffer))
         self.group_smell_sniffers.append(sniffer)
 
-    def run(self):
+    def run(self, smell_as_dict: bool = True):
         logger.debug("Running analysis")
         # Return a dictionary with two fields of types: ANodes:[], AGroups:[]
         result = {}
         nodes = []
         for node in self.micro_model.nodes:
             #  TODO: creare una classe ANode che identifica il nodo analizzato.
             anode = {'name': node.name}
             if(isinstance(node, Service)):
                 anode["type"] = "software"
+            if(isinstance(node, Compute)):
+                anode["type"] = "compute"
             if(isinstance(node, Datastore)):
                 anode["type"] = "datastore"
             if(isinstance(node, MessageBroker)):
                 anode["type"] = "communicationpattern"
                 # TODO: remove concrete type
                 anode['concrete_type'] = "messageBroker"
             if(isinstance(node, MessageRouter)):
@@ -63,15 +65,15 @@
                 anode['concrete_type'] = "messageRouter"
 
             smells = []
             for sniffer in self.node_smell_sniffers:
                 # if self.get_ignore_smells_for_node(node) or sniffer not in self.get_ignore_smells_for_node(node):
                 smell = sniffer.snif(node)
                 if(smell and not smell.isEmpty()):
-                    smells.append(smell.to_dict())
+                    smells.append(smell.to_dict() if smell_as_dict else smell)
             if(smells):  # add only nodes that has at least one smell
                 anode['smells'] = smells
                 nodes.append(anode)
         result['nodes'] = nodes
 
         groups = []
         for group in self.micro_model.groups:
@@ -81,17 +83,17 @@
             for gsniffer in self.group_smell_sniffers:
                 gsmells = gsniffer.snif(group)
                 if(gsmells):
                     # NoApiGatewaysmellSniffer returns a list of node-based noApiGatewaySmellSniffer
                     if isinstance(gsmells, list):
                         for smell in gsmells:
                             if(not smell.isEmpty()):
-                                smells.append(smell.to_dict())
+                                smells.append(smell.to_dict() if smell_as_dict else smell)
                     else:
                         if(not gsmells.isEmpty()):
-                            smells.append(gsmells.to_dict())
+                            smells.append(gsmells.to_dict() if smell_as_dict else gsmells)
             if(smells):
                 agroup['smells'] = smells
                 groups.append(agroup)
         result['groups'] = groups
 
         return result
```

### Comparing `microfreshener-core-1.4.0/microfreshener/core/analyser/costants.py` & `microfreshener-core-1.5.0/microfreshener/core/analyser/costants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,5 +1,5 @@
-SMELLS_NAME = SMELL_ENDPOINT_BASED_SERVICE_INTERACTION, SMELL_WOBBLY_SERVICE_INTERACTION_SMELL, SMELL_SHARED_PERSITENCY, SMELL_NO_API_GATEWAY, SMELL_CROSS_TEAM_DATA_MANAGEMENT=\
-            "Endpoint-based-service-interaction", "Wobbly-service-interaction", "Shared-persistency", "No-api-gateway", "Cross-team-data-management"
+SMELLS_NAME = SMELL_ENDPOINT_BASED_SERVICE_INTERACTION, SMELL_WOBBLY_SERVICE_INTERACTION_SMELL, SMELL_SHARED_PERSISTENCY, SMELL_NO_API_GATEWAY, SMELL_SINGLE_LAYER_TEAMS, SMELL_MULTIPLE_SERVICES_IN_ONE_CONTAINER, SMELL_ESB_MISUSE, SMELL_TIGHTLY_COUPLED_TEAMS, SMELL_SHARED_BOUNDED_CONTEXT =\
+            "Endpoint-based-service-interaction", "Wobbly-service-interaction", "Shared-persistency", "No-api-gateway", "Single-layer-teams", "Multiple-services-in-one-container", "ESB-misuse", "Tightly-coupled-teams", "Shared-bounded-context"
 
-REFACTORING_NAMES = REFACTORING_ADD_SERVICE_DISCOVERY, REFACTORING_ADD_MESSAGE_ROUTER, REFACTORING_ADD_MESSAGE_BROKER, REFACTORING_ADD_CIRCUIT_BREAKER, REFACTORING_USE_TIMEOUT, REFACTORING_MERGE_SERVICES, REFACTORING_SPLIT_DATABASE, REFACTORING_ADD_DATA_MANAGER, REFACTORING_ADD_API_GATEWAY, REFACTORING_ADD_TEAM_DATA_MANAGER, REFACTORING_CHANGE_DATABASE_OWENRSHIP, REFACTORING_CHANGE_SERVICE_OWENRSHIP =\
-             'Add-service-discovery', 'Add-message-router',  'Add-message-broker', 'Add-circuit-breaker', "Use-timeout", "Merge-service", "Split-Datastore", "Add-data-manager", "Add-api-gateway", "Add-data-team-data-manager", "Change-Datastore-ownership","Change-service-ownership"
+REFACTORING_NAMES = REFACTORING_ADD_SERVICE_DISCOVERY, REFACTORING_ADD_MESSAGE_ROUTER, REFACTORING_ADD_MESSAGE_BROKER, REFACTORING_ADD_CIRCUIT_BREAKER, REFACTORING_USE_TIMEOUT, REFACTORING_MERGE_SERVICES, REFACTORING_SPLIT_DATABASE, REFACTORING_ADD_DATA_MANAGER, REFACTORING_ADD_API_GATEWAY, REFACTORING_SPLIT_SERVICES, REFACTORING_SPLIT_TEAMS_BY_MICROSERVICE, REFACTORING_SPLIT_TEAMS_BY_COUPLING, REFACTORING_REORGANIZE_TEAMS_BY_BOUNDED_CONTEXT, REFACTORING_SPLIT_BOUNDED_CONTEXT_BY_TEAMS =\
+             "Add-service-discovery", "Add-message-router",  "Add-message-broker", "Add-circuit-breaker", "Use-timeout", "Merge-service", "Split-Datastore", "Add-data-manager", "Add-api-gateway", "Split-service-in-two-pods", "Split-teams-by-microservice", "Split-teams-by-coupling", "Reorganize-teams-by-bounded-contexts", "Split-bounded-context-by-teams"
```

### Comparing `microfreshener-core-1.4.0/microfreshener/core/analyser/smell.py` & `microfreshener-core-1.5.0/microfreshener/core/model/nodes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,139 +1,212 @@
-from typing import List
-from ..model import Root
-from ..model import Relationship
-from .costants import SMELL_ENDPOINT_BASED_SERVICE_INTERACTION, SMELL_NO_API_GATEWAY, SMELL_SHARED_PERSITENCY, SMELL_WOBBLY_SERVICE_INTERACTION_SMELL, SMELL_CROSS_TEAM_DATA_MANAGEMENT
-from .costants import REFACTORING_ADD_SERVICE_DISCOVERY, REFACTORING_ADD_MESSAGE_ROUTER, REFACTORING_ADD_MESSAGE_BROKER, REFACTORING_ADD_CIRCUIT_BREAKER, REFACTORING_USE_TIMEOUT, REFACTORING_MERGE_SERVICES, REFACTORING_SPLIT_DATABASE, REFACTORING_ADD_DATA_MANAGER, REFACTORING_ADD_API_GATEWAY, REFACTORING_ADD_TEAM_DATA_MANAGER, REFACTORING_CHANGE_DATABASE_OWENRSHIP, REFACTORING_CHANGE_SERVICE_OWENRSHIP
-class Smell(object):
+'''
+nodes module
+'''
+
+from .relationships import DeploymentTimeInteraction, RunTimeInteraction, InteractsWith, DeployedOn
+from ..logging import MyLogger
+from ..errors import MicroToscaModelError
+
+logger = MyLogger().get_logger()
+
+
+class Root(object):
 
     def __init__(self, name):
-        self.nodes_cause = []
-        self.links_cause = []
         self.name = name
 
-    def addNodeCause(self, node: Root):
-        self.nodes_cause.append(node)
+        # Requirements
+        self._interactions = []
 
-    def getNodeCause(self):
-        return self.nodes_cause
+        # Incoming interaction of a node
+        self.up_interactions = []
 
-    def addLinkCause(self, link: Relationship):
-        self.links_cause.append(link)
 
-    def getLinkCause(self):
-        return self.links_cause
+        # Outcoming DeployedOn relations
+        self._deployed_on = []
 
-    def to_dict(self):
-        return {"name": self.name,
-                "nodes": [node.name for node in self.getNodeCause()],
-                "links": [interation.to_dict() for interation in self.getLinkCause()]}
+    @property
+    def interactions(self):
+        return self._interactions
 
-    def isEmpty(self):
-        return len(self.getLinkCause()) == 0 and len(self.getNodeCause()) == 0
+    @property
+    def incoming_interactions(self):
+        return self.up_interactions
+
+    @property
+    def deployed_on(self):
+        return self._deployed_on
+
+    def add_incoming_interaction(self, interaction):
+        self.up_interactions.append(interaction)
+
+    # Add a interactWith interaction from source node to target node.
+    # Only Service and MessagRoouter can be source of a relation (checkd in the InteractWith costructor)
+    def add_interaction(self, item, with_timeout=False, with_circuit_breaker=False, with_dynamic_discovery=False):
+        if not isinstance(item, InteractsWith):
+            item = InteractsWith(self, item, with_timeout=with_timeout,
+                                 with_circuit_breaker=with_circuit_breaker,
+                                 with_dynamic_discovery=with_dynamic_discovery)
+        if (item in self._interactions):
+            raise MicroToscaModelError(
+                f"Interaction {item} from {self} to {item.target} already exist")
+        self._interactions.append(item)
+        if not isinstance(item.target, str):
+            item.target.add_incoming_interaction(item)
+        return item
+
+    def remove_interaction(self, interaction):
+        if interaction in self._interactions:
+            self._interactions.remove(interaction)
+        interaction.target.remove_incoming_interaction(interaction)
+
+    def remove_incoming_interaction(self, interaction):
+        if interaction in self.up_interactions:
+            self.up_interactions.remove(interaction)
+
+    # Adds a deployedOn interaction from source node (self) to target node. Only Service can be source of the relation
+    # and only Compute can be the target
+    def add_deployed_on(self, item):
+        if not isinstance(item, DeployedOn):
+            item = DeployedOn(source=self, target=item)
+
+        if item in self._deployed_on:
+            raise MicroToscaModelError(f"Interaction {item} from {self} to {item.target} already exist")
+
+        self._deployed_on.append(item)
+        if not isinstance(item.target, str):
+            item.target.add_deploy(item)
+        return item
+
+    def remove_deployed_on(self, link):
+        if link in self._deployed_on:
+            self._deployed_on.remove(link)
+        link.target.remove_deploy(link)
+
+    def __str__(self):
+        return self.name
+
+    def __eq__(self, other):
+        return self.name == other.name  # and type(self) == type(other)
 
     def __hash__(self):
         return hash(self.name)
 
+    def to_dict(self):
+        return {'name': self.name}
 
-class NodeSmell(Smell):
 
-    def __init__(self, name, node):
-        super(NodeSmell, self).__init__(name)
-        self._node = node
+class Software(Root):
 
-    @property
-    def node(self):
-        return self._node
+    def __init__(self, name):
+        super(Software, self).__init__(name)
 
 
-class GroupSmell(Smell):
+class Service(Software):
 
-    def __init__(self, name, group):
-        super(GroupSmell, self).__init__(name)
-        self._group = group
+    def __init__(self, name):
+        super(Service, self).__init__(name)
+
+    def __str__(self):
+        return '{} ({})'.format(self.name, 'service')
 
-    @property
-    def group(self):
-        return self._group
 
+class Compute(Root):
 
-class EndpointBasedServiceInteractionSmell(NodeSmell):
-    name: str = SMELL_ENDPOINT_BASED_SERVICE_INTERACTION
+    def __init__(self, name):
+        super(Compute, self).__init__(name)
 
-    def __init__(self, node):
-        super(EndpointBasedServiceInteractionSmell,
-              self).__init__(self.name, node)
+        # Incoming DeployedOn relations
+        self._deploys: list = []
 
     def __str__(self):
-        return 'EndpointBasedServiceInteractionSmell({})'.format(super(NodeSmell, self).__str__())
+        return '{} ({})'.format(self.name, 'compute')
 
-    def to_dict(self):
-        sup_dict = super(EndpointBasedServiceInteractionSmell, self).to_dict()
-        return {**sup_dict, **{"refactorings": [
-            {"name": REFACTORING_ADD_SERVICE_DISCOVERY, "description": "Add Service discovery"},
-            {"name": REFACTORING_ADD_MESSAGE_ROUTER, "description": "Add a message router"},
-            {"name": REFACTORING_ADD_MESSAGE_BROKER, "description": " Add message broker"}
-        ]}}
+    @property
+    def deploys(self):
+        return self._deploys
+
+    def add_deploy(self, relation):
+        self._deploys.append(relation)
 
+    def remove_deploy(self, deploys):
+        if deploys in self._deploys:
+            self._deploys.remove(deploys)
 
-class WobblyServiceInteractionSmell(NodeSmell):
-    name: str = SMELL_WOBBLY_SERVICE_INTERACTION_SMELL
 
-    def __init__(self, node):
-        super(WobblyServiceInteractionSmell, self).__init__(self.name, node)
+class CommunicationPattern(Software):
+
+    def __init__(self, name, short_name="CP"):
+        super(CommunicationPattern, self).__init__(name)
+        self.short_name = short_name
 
     def __str__(self):
-        return 'WobblyServiceInteractionSmell({})'.format(super(NodeSmell, self).__str__())
+        return '{} ({})'.format(self.name, self.short_name)
 
-    def to_dict(self):
-        sup_dict = super(WobblyServiceInteractionSmell, self).to_dict()
-        return {**sup_dict, **{"refactorings": [
-            {"name": REFACTORING_ADD_MESSAGE_BROKER, "description": "Add Message broker"},
-            {"name": REFACTORING_ADD_CIRCUIT_BREAKER, "description": " Add Circuit breaker"},
-            {"name": REFACTORING_USE_TIMEOUT, "description": "Use timeouts in the interaction"}]}}
 
-class SharedPersistencySmell(NodeSmell):
-    name: str = SMELL_SHARED_PERSITENCY
+class MessageBroker(CommunicationPattern):
 
-    def __init__(self, node):
-        super(SharedPersistencySmell, self).__init__(self.name, node)
+    def __init__(self, name):
+        super(MessageBroker, self).__init__(name, "MB")
 
     def __str__(self):
-        return 'SharedPersistencySmell({})'.format(super(NodeSmell, self).__str__())
+        return '{} ({})'.format(self.name, self.short_name)
 
-    def to_dict(self):
-        sup_dict = super(SharedPersistencySmell, self).to_dict()
-        return {**sup_dict, **{"refactorings": [
-            {"name": REFACTORING_MERGE_SERVICES,"description": "Merge services accesing the same Datastore"},
-            {"name": REFACTORING_SPLIT_DATABASE, "description": "Split the Datastore."},
-            {"name": REFACTORING_ADD_DATA_MANAGER, "description": " Add Data manager"}]}}
 
-class NoApiGatewaySmell(NodeSmell):
-    name: str = SMELL_NO_API_GATEWAY
+class Datastore(Root):
 
-    def __init__(self, node):
-        super(NoApiGatewaySmell, self).__init__(self.name, node)
+    def __init__(self, name):
+        super(Datastore, self).__init__(name)
 
     def __str__(self):
-        return 'NoApiGateway({})'.format(super(NoApiGatewaySmell, self).__str__())
+        return '{} ({})'.format(self.name, 'Datastore')
 
-    def to_dict(self):
-        sup_dict = super(NoApiGatewaySmell, self).to_dict()
-        return {**sup_dict, **{"refactorings": [{
-            "name": REFACTORING_ADD_API_GATEWAY, "description": "Add an Api Gateway between the external user"}]}}
 
-class CrossTeamDataManagementSmell(GroupSmell):
-    name: str = SMELL_CROSS_TEAM_DATA_MANAGEMENT
+class MessageRouter(CommunicationPattern):
+
+    def __init__(self, name, label="MR"):
+        self.label = label
+        super(MessageRouter, self).__init__(name, label)
 
-    def __init__(self, group):
-        super(CrossTeamDataManagementSmell, self).__init__(self.name, group)
+
+class KService(MessageRouter):
+
+    def __init__(self, name, selector=None, stype=None):
+        self._selector = selector  # {<key>:<value>}
+        # LoadBalancer | NodePort :for knowing if the service is acessed by external
+        self._type = stype
+
+        super(KService, self).__init__(name, "KS")
+
+    @property
+    def service_type(self):
+        return self._type
+
+    @property
+    def selector(self):
+        return self._selector
+
+    def is_external_accessed(self):
+        return self.service_type == "LoadBalancer" or self.service_type == "NodePort"
 
     def __str__(self):
-        return 'CrossTeamDataManagement({})'.format(super(CrossTeamDataManagementSmell, self).__str__())
+        return '{} ({})'.format(self.name, 'Kservice')
 
-    def to_dict(self):
-        sup_dict = super(CrossTeamDataManagementSmell, self).to_dict()
-        return {**sup_dict, **{"refactorings": [
-            {"name": REFACTORING_ADD_TEAM_DATA_MANAGER, "description": "Move the Datastore to another team"},
-            {"name": REFACTORING_CHANGE_DATABASE_OWENRSHIP, "description": "Move the Datastore to another team"},
-            {"name": REFACTORING_CHANGE_SERVICE_OWENRSHIP, "description": "Move the service to another team"},
-            ]}}
+
+class KIngress(MessageRouter):
+
+    def __init__(self, name, backends=[]):
+        self.backend_services = backends
+        super(KIngress, self).__init__(name, "KIngress")
+
+    @property
+    def backends(self):
+        return self.backend_services
+
+    def add_service_name(self, name):
+        self.backend_services.append(name)
+
+
+class KProxy(MessageRouter):
+
+    def __init__(self, name):
+        super(KProxy, self).__init__(name, "KProxy")
```

### Comparing `microfreshener-core-1.4.0/microfreshener/core/errors.py` & `microfreshener-core-1.5.0/microfreshener/core/errors.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/microfreshener/core/model/type.py` & `microfreshener-core-1.5.0/microfreshener/core/model/type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # MicroTosca types
 
 # MicroTOSCA node types
 MICROTOSCA_NODES_SERVICE = 'micro.nodes.Service'
+MICROTOSCA_NODES_COMPUTE = "micro.nodes.Compute"
 MICROTOSCA_NODES_DATABASE = 'micro.nodes.Datastore'
 
 MICROTOSCA_NODES_COMMUNICATIONPATTERN = 'micro.nodes.CommunicationPattern'
 MICROTOSCA_NODES_MESSAGE_BROKER = 'micro.nodes.MessageBroker'
 MICROTOSCA_NODES_MESSAGE_ROUTER = 'micro.nodes.MessageRouter'
 
 MICROTOSCA_NODES_MESSAGE_ROUTER_KINGRESS = 'micro.nodes.MessageRouter.KIngress'
 MICROTOSCA_NODES_MESSAGE_ROUTER_KSERVICE = 'micro.nodes.MessageRouter.KService'
 MICROTOSCA_NODES_MESSAGE_ROUTER_KPROXY = 'micro.nodes.MessageRouter.KProxy'
 
 # MicroTOSCA relationship types
 MICROTOSCA_RELATIONSHIPS_INTERACT_WITH = 'micro.relationships.InteractsWith'
+MICROTOSCA_RELATIONSHIPS_DEPLOYED_ON = 'micro.relationships.DeployedOn'
 MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_TIMEOUT_PROPERTY = "timeout"
 MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_CIRCUIT_BREAKER_PROPERTY = "circuit_breaker"
 MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_DYNAMIC_DISCOVEY_PROPERTY = "dynamic_discovery"
 
 # MicroTOSCA group types
 MICROTOSCA_GROUPS_TEAM = 'micro.groups.Team'
 MICROTOSCA_GROUPS_EDGE = 'micro.groups.Edge'
```

### Comparing `microfreshener-core-1.4.0/microfreshener/core/model/microtosca.py` & `microfreshener-core-1.5.0/microfreshener/core/model/microtosca.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 MicroModelModel module
 '''
+import re
+
 import six
-from .type import MICROTOSCA_RELATIONSHIPS_INTERACT_WITH
-from .nodes import Root, Service, Datastore, CommunicationPattern, MessageRouter, MessageBroker
-from .relationships import InteractsWith, DeploymentTimeInteraction, RunTimeInteraction
+from .nodes import Root, Service, Datastore, CommunicationPattern, MessageRouter, MessageBroker, Compute
 from .groups import Team, Edge
 from ..errors import MicroToscaModelError, MultipleEdgeGroupsError
 from ..logging import MyLogger
 from ..errors import RelationshipNotFoundError, GroupNotFoundError
 logger = MyLogger().get_logger()
 
 
@@ -24,14 +24,18 @@
         return (v for k, v in self._nodes.items())
 
     @property
     def services(self):
         return (v for k, v in self._nodes.items() if isinstance(v, Service))
 
     @property
+    def computes(self):
+        return (v for k, v in self._nodes.items() if isinstance(v, Compute))
+
+    @property
     def datastores(self):
         return (v for k, v in self._nodes.items() if isinstance(v, Datastore))
 
     @property
     def communication_patterns(self):
         return (v for k, v in self._nodes.items() if isinstance(v, CommunicationPattern))
 
@@ -63,14 +67,28 @@
                 return v
         raise GroupNotFoundError("Edge group is missing")
 
     def add_node(self, node):
         self._nodes[node.name] = node
         logger.debug("Added node {}".format(node))
         return node
+    
+    def rename_node(self, node, new_name):
+        old_name = node.name
+        self._nodes[new_name] = self._nodes.pop(node.name)
+
+        logger.debug(f"Renamed node {node.name} to {new_name}")
+        node.name = new_name
+
+        for name, group in self._groups.items():
+            for name in list(group._members.keys()):
+                if name == old_name:
+                    del group._members[name]
+                    group.add_member(node)
+
 
     def relink_incoming(self, current_node, target_node, source_nodes_to_be_discarded=[]):
         
         incoming_interactions = list(current_node.incoming_interactions)
         for incoming in incoming_interactions:
             if incoming.source not in source_nodes_to_be_discarded:
                 incoming.source.remove_interaction(incoming)
@@ -82,26 +100,34 @@
         # return target_node.add_interaction(current_node)
 
     def delete_node(self, node):
         for rel in node.interactions:
             rel.target.remove_incoming_interaction(rel)
         for up_rel in node.incoming_interactions:
             up_rel.source.remove_interaction(up_rel)
+
+        if isinstance(node, Service):
+            for dep in node.deployed_on:
+                node.remove_deployed_on(dep)
+
         logger.debug(f"Deleted node {node}")
         del self._nodes[node.name]
 
     def add_interaction(self, source_node, target_node,
                         with_timeout=False,
                         with_circuit_breaker=False,
                         with_dynamic_discovery=False):
         return source_node.add_interaction(target_node,
                                            with_timeout,
                                            with_circuit_breaker,
                                            with_dynamic_discovery)
 
+    def add_deployed_on(self, source_node, target_node):
+        return source_node.add_deployed_on(item=target_node)
+
     def get_relationship(self, id):
         for node in self.nodes:
             for interaction in node.interactions:
                 if(interaction.id == id):
                     return interaction
         raise RelationshipNotFoundError(f"Relationship with id {id} not found")
 
@@ -152,14 +178,33 @@
                         subMicroToscaModel.add_group(team_of_node)
                     else:
                         subMicroToscaModel.get_group(
                             team_of_node.name).add_member(node)
 
         return subMicroToscaModel
 
+    def get_node_by_name(self, name: str, type = None):
+        nodes_to_consider = [n for n in self.nodes if isinstance(n, type)] if type else self.nodes
+
+        # Case: node.name == name
+        for node in nodes_to_consider:
+            if node.name == name:
+                return node
+
+        for node in nodes_to_consider:
+            # Case: name is FQDN (name.ns.svc, name.ns.svc.cluster, name.ns.svc.cluster.local)
+            match = re.match(name+r"([.][a-zA-Z]*){1,3}", node.name)
+            if match and match.string == node.name:
+                return node
+
+            # Case: node.name is FQDN (name.ns.svc, name.ns.svc.cluster, name.ns.svc.cluster.local)
+            match = re.match(node.name + r"([.][a-zA-Z]*){1,3}", name)
+            if match and match.string == name:
+                return node
+
     def __getitem__(self, name):
         node = self._nodes.get(name, None)
         if node is None:
             raise MicroToscaModelError(f"Node {name} does not exist")
         else:
             return node
         # return self._nodes.get(name, None)
```

### Comparing `microfreshener-core-1.4.0/microfreshener/core/model/relationships.py` & `microfreshener-core-1.5.0/microfreshener/core/model/relationships.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 '''
 Relationships module
 '''
 import six
 import uuid
 
-
 from ..errors import MicroToscaModelError, SelfLoopMicroToscaModelError
 
 
 def _get_str_name(obj):
     return obj if isinstance(obj, six.string_types) else obj.name
 
 
@@ -133,7 +132,29 @@
         return 'RunTimeInteraction({})'.format(super(RunTimeInteraction, self).__str__())
 
     def __repr__(self):
         return 'RunTimeInteraction({})'.format(super(RunTimeInteraction, self).__repr__())
 
     def to_dict(self):
         return {'source': self.source.name, 'target': self.target.name, "type": "runtime"}
+
+
+class DeployedOn(Relationship):
+
+    def __init__(self, source, target, id=None):
+        from .nodes import Service, Compute, Datastore
+        from microfreshener.core.model import MessageBroker
+
+        if (isinstance(source, Service) or isinstance(source, Datastore) or isinstance(source, MessageBroker)) and isinstance(target, Compute):
+            super().__init__(source, target, id)
+        else:
+            raise MicroToscaModelError(
+                f"DeployedOn relationship cannot be created from {source} to {target}. {type(source).__name__}")
+
+    def __str__(self):
+        return 'DeployedOn({})'.format(super(InteractsWith, self).__str__())
+
+    def __repr__(self):
+        return 'DeployedOn({})'.format(super(InteractsWith, self).__repr__())
+
+    def to_dict(self):
+        return {'source': self.source.name, 'target': self.target.name, "type": "deployment"}
```

### Comparing `microfreshener-core-1.4.0/microfreshener/core/model/groups.py` & `microfreshener-core-1.5.0/microfreshener/core/model/groups.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/microfreshener/core/exporter/jsonexporter.py` & `microfreshener-core-1.5.0/microfreshener/core/exporter/jsonexporter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import json
-
+from .iexporter import Exporter
+from ..errors import ExporterError
+from ..importer.jsontype import JSON_GROUPS_EDGE, JSON_GROUPS_TEAM, JSON_NODE_COMPUTE, JSON_RELATIONSHIP_DEPLOYED_ON
+from ..importer.jsontype import JSON_NODE_DATABASE, JSON_NODE_MESSAGE_BROKER, JSON_NODE_MESSAGE_ROUTER, \
+    JSON_NODE_SERVICE
+from ..importer.jsontype import JSON_RELATIONSHIP_INTERACT_WITH
+from ..model import InteractsWith, Compute, DeployedOn
 from ..model import MicroToscaModel
-from ..model  import RunTimeInteraction, DeploymentTimeInteraction, InteractsWith
-from ..model import Root, Service, Datastore, CommunicationPattern, MessageBroker, MessageRouter
+from ..model import Service, Datastore, MessageBroker, MessageRouter
 from ..model.groups import Edge, Team
+from ..model.type import MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_TIMEOUT_PROPERTY, \
+    MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_CIRCUIT_BREAKER_PROPERTY, \
+    MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_DYNAMIC_DISCOVEY_PROPERTY
 
-from ..model.type import  MICROTOSCA_NODES_MESSAGE_BROKER
-from ..model.type import MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_TIMEOUT_PROPERTY, MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_CIRCUIT_BREAKER_PROPERTY, MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_DYNAMIC_DISCOVEY_PROPERTY
-from ..errors import ExporterError
-from .iexporter import Exporter
-from ..importer.jsontype import JSON_NODE_DATABASE, JSON_NODE_MESSAGE_BROKER, JSON_NODE_MESSAGE_ROUTER, JSON_NODE_SERVICE
-from ..importer.jsontype import JSON_DEPLOYMENT_TIME, JSON_RUN_TIME, JSON_RELATIONSHIP_INTERACT_WITH
-from ..importer.jsontype import JSON_GROUPS_EDGE, JSON_GROUPS_TEAM
 
 class JSONExporter(Exporter):
 
     def __init__(self):
         pass
 
     # Transform a microModel Oject to a Dicionary format.
@@ -34,14 +34,17 @@
             d['nodes'] = []      # nodes
             d['links'] = []      # links
             d['groups'] = []     # groups
             for node in obj.nodes:
                 d['nodes'].append(self.transform_node_to_json(node))
                 for rel in node.interactions:
                     d['links'].append(self.export_link_to_json(rel))
+                if hasattr(node, "deployed_on"):
+                    for rel in node.deployed_on:
+                        d['links'].append(self.export_link_to_json(rel))
             for group in obj.groups:
                 d['groups'].append(self.export_group_to_json(group))
         return d
 
     def transform_node_to_json(self, node):
         dict_node = {}
         dict_node['name'] = node.name
@@ -49,28 +52,33 @@
             dict_node['type'] = JSON_NODE_SERVICE
         elif(isinstance(node, Datastore)):
             dict_node['type'] = JSON_NODE_DATABASE
         elif(isinstance(node, MessageBroker)):
             dict_node['type'] = JSON_NODE_MESSAGE_BROKER
         elif(isinstance(node, MessageRouter)):
             dict_node['type'] = JSON_NODE_MESSAGE_ROUTER
+        elif(isinstance(node, Compute)):
+            dict_node['type'] = JSON_NODE_COMPUTE
         else:
             raise ExporterError(f"Node {n} not recognized")
         return dict_node
 
     def export_link_to_json(self, relationship):
         nrel = {}
         nrel['id'] = relationship.id
         nrel['target'] = relationship.target.name
         nrel['source'] = relationship.source.name
-        nrel[MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_TIMEOUT_PROPERTY] = relationship.timeout
-        nrel[MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_CIRCUIT_BREAKER_PROPERTY] = relationship.circuit_breaker
-        nrel[MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_DYNAMIC_DISCOVEY_PROPERTY] = relationship.dynamic_discovery
+
         if(isinstance(relationship, InteractsWith)):
             nrel['type'] = JSON_RELATIONSHIP_INTERACT_WITH
+            nrel[MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_TIMEOUT_PROPERTY] = relationship.timeout
+            nrel[MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_CIRCUIT_BREAKER_PROPERTY] = relationship.circuit_breaker
+            nrel[MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_DYNAMIC_DISCOVEY_PROPERTY] = relationship.dynamic_discovery
+        elif isinstance(relationship, DeployedOn):
+            nrel['type'] = JSON_RELATIONSHIP_DEPLOYED_ON
         else:
             raise ExporterError("{} Relationship not recognized.".format(relationship))
         return nrel
 
     def export_group_to_json(self, group):
         g_dict = {}
         g_dict['name'] = group.name
```

### Comparing `microfreshener-core-1.4.0/microfreshener/core/exporter/ymlexporter.py` & `microfreshener-core-1.5.0/microfreshener/core/exporter/ymlexporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import sys
 from ruamel.yaml import YAML
 from ruamel.yaml.compat import StringIO
 
 from ..model import MicroToscaModel
-from ..model  import InteractsWith
-from ..model import Root, Service, Datastore, CommunicationPattern, MessageBroker, MessageRouter
+from ..model import InteractsWith
+from ..model import Root, Service, Datastore, CommunicationPattern, MessageBroker, MessageRouter, Compute
 from ..model.groups import RootGroup, Edge, Team
+from ..model.relationships import DeployedOn
 from ..model.type import MICROTOSCA_RELATIONSHIPS_INTERACT_WITH, MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_TIMEOUT_PROPERTY, MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_CIRCUIT_BREAKER_PROPERTY, MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_DYNAMIC_DISCOVEY_PROPERTY
-from ..model.type import MICROTOSCA_NODES_SERVICE, MICROTOSCA_NODES_DATABASE, MICROTOSCA_NODES_MESSAGE_BROKER, MICROTOSCA_NODES_MESSAGE_ROUTER
-from ..model.type import  MICROTOSCA_GROUPS_EDGE, MICROTOSCA_GROUPS_TEAM
-from ..importer.ymltype import  YML_INTERACTION
+from ..model.type import MICROTOSCA_NODES_SERVICE, MICROTOSCA_NODES_DATABASE, MICROTOSCA_NODES_MESSAGE_BROKER, MICROTOSCA_NODES_MESSAGE_ROUTER, MICROTOSCA_NODES_COMPUTE
+from ..model.type import MICROTOSCA_GROUPS_EDGE, MICROTOSCA_GROUPS_TEAM
+from ..importer.ymltype import YML_INTERACTION, YML_DEPLOYED_ON
 from ..importer.ymltype import YML_RELATIONSHIP_T, YML_RELATIONSHIP_D, YML_RELATIONSHIP_C, YML_RELATIONSHIP_CD, YML_RELATIONSHIP_TC, YML_RELATIONSHIP_TD, YML_RELATIONSHIP_TCD
 from .iexporter import Exporter
 from ..errors import ExporterError
 
 class MyYAML(YAML):
     def dump(self, data, stream=None, **kw):
         inefficient = False
@@ -96,21 +97,25 @@
             node_type = MICROTOSCA_NODES_SERVICE
         elif(isinstance(node, Datastore)):
             node_type = MICROTOSCA_NODES_DATABASE
         elif(isinstance(node, MessageBroker)):
             node_type = MICROTOSCA_NODES_MESSAGE_BROKER
         elif(isinstance(node, MessageRouter)):
             node_type = MICROTOSCA_NODES_MESSAGE_ROUTER
+        elif(isinstance(node, Compute)):
+            node_type = MICROTOSCA_NODES_COMPUTE
         else:
             raise ExporterError(f"Node {node} not recognized")
         d_node['type'] = node_type
 
         requirements = []
         for rel in node.interactions:
             requirements.append(self._transform_relationship(rel))
+        for dep in node.deployed_on:
+            requirements.append(self._transform_relationship(dep))
         if(requirements):
             d_node['requirements'] = requirements
         return d_node
 
     def _transform_relationship(self, rel):
         d_rel = {}
         if(isinstance(rel, InteractsWith)):
@@ -126,10 +131,12 @@
                 d_rel[YML_INTERACTION] = {"node": rel.target.name, "relationship": YML_RELATIONSHIP_TD}
             elif(not rel.timeout and rel.circuit_breaker and rel.dynamic_discovery):
                 d_rel[YML_INTERACTION] = {"node": rel.target.name, "relationship": YML_RELATIONSHIP_CD}
             elif(rel.timeout and rel.circuit_breaker and rel.dynamic_discovery):
                 d_rel[YML_INTERACTION] = {"node": rel.target.name, "relationship": YML_RELATIONSHIP_TCD}
             else:
                 d_rel[YML_INTERACTION] = rel.target.name
+        elif isinstance(rel, DeployedOn):
+            d_rel[YML_DEPLOYED_ON] = {"node": rel.target.name}
         else:
             raise ExporterError('{} relationship not recognized.'.format(rel))
         return d_rel
```

### Comparing `microfreshener-core-1.4.0/microfreshener_core.egg-info/SOURCES.txt` & `microfreshener-core-1.5.0/microfreshener_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,39 +43,46 @@
 microfreshener_core.egg-info/SOURCES.txt
 microfreshener_core.egg-info/dependency_links.txt
 microfreshener_core.egg-info/entry_points.txt
 microfreshener_core.egg-info/not-zip-safe
 microfreshener_core.egg-info/requires.txt
 microfreshener_core.egg-info/top_level.txt
 tests/__init__.py
+tests/log/log_2023-10-21.log
 tests/test_analyser/__init__.py
 tests/test_analyser/test_analyser.py
 tests/test_analyser/test_builder.py
-tests/test_analyser/test_sniffer_ctdm.py
 tests/test_analyser/test_sniffer_ebsi.py
+tests/test_analyser/test_sniffer_msioc.py
 tests/test_analyser/test_sniffer_nagw.py
+tests/test_analyser/test_sniffer_sbc.py
 tests/test_analyser/test_sniffer_shpr.py
+tests/test_analyser/test_sniffer_slt.py
+tests/test_analyser/test_sniffer_tct.py
 tests/test_analyser/test_sniffer_wbsi.py
+tests/test_analyser/log/log_2024-04-05.log
 tests/test_exporter/__init__.py
 tests/test_exporter/test_export_json.py
 tests/test_exporter/test_export_json_nodes.py
+tests/test_exporter/test_export_json_relationship.py
 tests/test_exporter/test_export_json_relationships_properties.py
 tests/test_exporter/test_export_yml_groups.py
 tests/test_exporter/test_export_yml_nodes.py
 tests/test_exporter/test_export_yml_relationships_properties.py
 tests/test_importer/__init__.py
 tests/test_importer/json_importer/__init__.py
 tests/test_importer/json_importer/test_import_json.py
 tests/test_importer/json_importer/test_import_json_nodes.py
 tests/test_importer/json_importer/test_import_json_relationships.py
 tests/test_importer/json_importer/test_import_json_relationships_properties.py
 tests/test_importer/yml_importer/__init__.py
 tests/test_importer/yml_importer/test_import_yml.py
 tests/test_importer/yml_importer/test_import_yml_groups.py
 tests/test_importer/yml_importer/test_import_yml_nodes.py
+tests/test_importer/yml_importer/test_import_yml_relationships.py
 tests/test_importer/yml_importer/test_import_yml_relationships_properties.py
 tests/test_model/__init__.py
 tests/test_model/test_group.py
 tests/test_model/test_microtosca.py
 tests/test_model/test_relationships.py
 tests/test_refiner/__init__.py
 tests/test_refiner/test_istio_refiner_destination_rule.py
```

### Comparing `microfreshener-core-1.4.0/setup.py` & `microfreshener-core-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_analyser/test_sniffer_wbsi.py` & `microfreshener-core-1.5.0/tests/test_analyser/test_sniffer_wbsi.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_analyser/test_sniffer_nagw.py` & `microfreshener-core-1.5.0/tests/test_analyser/test_sniffer_nagw.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_analyser/test_sniffer_ebsi.py` & `microfreshener-core-1.5.0/tests/test_analyser/test_sniffer_ebsi.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_analyser/test_sniffer_shpr.py` & `microfreshener-core-1.5.0/tests/test_analyser/test_sniffer_shpr.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_analyser/test_analyser.py` & `microfreshener-core-1.5.0/tests/test_analyser/test_analyser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import TestCase
 
 from microfreshener.core.importer import YMLImporter
 from microfreshener.core.analyser import MicroToscaAnalyser
 
-from microfreshener.core.analyser.sniffer import NoApiGatewaySmellSniffer, WobblyServiceInteractionSmellSniffer, SharedPersistencySmellSniffer, CrossTeamDataManagementSmellSniffer
+from microfreshener.core.analyser.sniffer import NoApiGatewaySmellSniffer, WobblyServiceInteractionSmellSniffer, SharedPersistencySmellSniffer, SingleLayerTeamsSmellSniffer, MultipleServicesInOneContainerSmellSniffer
 
 
 class TestAnalyser(TestCase):
 
     @classmethod
     def setUpClass(self):
         file = 'data/examples/hello-world/helloworld.yml'
@@ -41,15 +41,24 @@
         d = res['nodes'][0]['smells'][0]['links']
         my_res = [{'source': 'order', 'target': 'order_db',  "type": "interaction"}, {'source': 'shipping', 'target': 'order_db',  "type": "interaction"}]
         self.assertEqual(d, my_res)
 
 
     def test_SingleLayerTeamSniffer(self):
         analyser = MicroToscaAnalyser(self.microtosca)
-        sltm = CrossTeamDataManagementSmellSniffer(self.microtosca)
+        sltm = SingleLayerTeamsSmellSniffer(self.microtosca)
         analyser.add_group_smell_sniffer(sltm)
         res = analyser.run()
         actual_res = res['groups'][0]['smells'][0]['links']
         expected_res = [{'source': 'shipping', 'target': 'order_db',  "type": "interaction"}]
         self.assertEqual(actual_res, expected_res)
         self.assertEqual(res['groups'][0]['smells'][0]['nodes'], [])
 
+    def test_MultipleServicesInOneContainerSniffer(self):
+        analyser = MicroToscaAnalyser(self.microtosca)
+        analyser.add_node_smell_sniffer(MultipleServicesInOneContainerSmellSniffer())
+        res = analyser.run()
+
+        d = res['nodes'][0]['smells'][0]['links']
+        my_res = [{'source': 'order', 'target': 'order-shipping-compute', 'type': 'deployment'}, {'source': 'shipping', 'target': 'order-shipping-compute', 'type': 'deployment'}]
+        self.assertEqual(d, my_res)
+
```

### Comparing `microfreshener-core-1.4.0/tests/test_analyser/test_builder.py` & `microfreshener-core-1.5.0/tests/test_analyser/test_builder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 from microfreshener.core.importer import YMLImporter
 from microfreshener.core.analyser.builder import MicroToscaAnalyserBuilder
 from microfreshener.core.analyser.smell import WobblyServiceInteractionSmell
-from microfreshener.core.analyser.sniffer import NoApiGatewaySmellSniffer, EndpointBasedServiceInteractionSmellSniffer, WobblyServiceInteractionSmellSniffer, SharedPersistencySmellSniffer, CrossTeamDataManagementSmellSniffer
+from microfreshener.core.analyser.sniffer import NoApiGatewaySmellSniffer, EndpointBasedServiceInteractionSmellSniffer, WobblyServiceInteractionSmellSniffer, SharedPersistencySmellSniffer, SingleLayerTeamsSmellSniffer
 
 
 class TestAnalyserBUilder(unittest.TestCase):
 
     @classmethod
     def setUpClass(self):
         file = 'data/examples/hello-world/helloworld.yml'
```

### Comparing `microfreshener-core-1.4.0/tests/test_exporter/test_export_yml_groups.py` & `microfreshener-core-1.5.0/tests/test_exporter/test_export_yml_groups.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_exporter/test_export_json.py` & `microfreshener-core-1.5.0/tests/test_exporter/test_export_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
     def test_team2(self):
         squad2 =  self.microtosca.get_group("team2")
         squad_dict = self.tranformer.export_group_to_json(squad2)
         self.assertEqual('name' in squad_dict, True)
         self.assertEqual(squad_dict['name'], "team2")
         self.assertEqual("type" in squad_dict, True)
         self.assertEqual(squad_dict['type'], JSON_GROUPS_TEAM)
-      
+
```

### Comparing `microfreshener-core-1.4.0/tests/test_exporter/test_export_yml_relationships_properties.py` & `microfreshener-core-1.5.0/tests/test_exporter/test_export_yml_relationships_properties.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_exporter/test_export_yml_nodes.py` & `microfreshener-core-1.5.0/tests/test_exporter/test_export_yml_nodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from unittest import TestCase
 
 from microfreshener.core.importer import YMLImporter
 from microfreshener.core.exporter import YMLExporter
-from microfreshener.core.model.type import MICROTOSCA_NODES_SERVICE, MICROTOSCA_NODES_DATABASE, MICROTOSCA_NODES_MESSAGE_BROKER, MICROTOSCA_NODES_MESSAGE_ROUTER
+from microfreshener.core.model.type import MICROTOSCA_NODES_SERVICE, MICROTOSCA_NODES_DATABASE, \
+    MICROTOSCA_NODES_MESSAGE_BROKER, MICROTOSCA_NODES_MESSAGE_ROUTER, MICROTOSCA_NODES_COMPUTE
 
 
 class TestYMLTranformer(TestCase):
 
     @classmethod
     def setUpClass(self):
         file = 'data/tests/test_nodes.yml'
@@ -29,7 +30,12 @@
         dict_mb = self.tranformer._transform_node_template(mb)
         self.assertEqual(dict_mb["type"], MICROTOSCA_NODES_MESSAGE_BROKER)
 
     def test_transform_router(self):
         mr = self.microtosca['my_messagerouter']
         dict_mr = self.tranformer._transform_node_template(mr)
         self.assertEqual(dict_mr["type"], MICROTOSCA_NODES_MESSAGE_ROUTER)
+
+    def test_transform_compute(self):
+        mr = self.microtosca['my_compute']
+        dict_mr = self.tranformer._transform_node_template(mr)
+        self.assertEqual(dict_mr["type"], MICROTOSCA_NODES_COMPUTE)
```

### Comparing `microfreshener-core-1.4.0/tests/test_exporter/test_export_json_relationships_properties.py` & `microfreshener-core-1.5.0/tests/test_exporter/test_export_json_relationships_properties.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_exporter/test_export_json_nodes.py` & `microfreshener-core-1.5.0/tests/test_exporter/test_export_json_nodes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from unittest import TestCase
 
 from microfreshener.core.importer import JSONImporter, YMLImporter
 from microfreshener.core.exporter import JSONExporter
 from microfreshener.core.model.type import MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_TIMEOUT_PROPERTY, MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_DYNAMIC_DISCOVEY_PROPERTY,MICROTOSCA_RELATIONSHIPS_INTERACT_WITH_CIRCUIT_BREAKER_PROPERTY
 
-from microfreshener.core.importer.jsontype import JSON_NODE_DATABASE, JSON_NODE_MESSAGE_BROKER, JSON_NODE_MESSAGE_ROUTER, JSON_NODE_SERVICE
+from microfreshener.core.importer.jsontype import JSON_NODE_DATABASE, JSON_NODE_MESSAGE_BROKER, \
+    JSON_NODE_MESSAGE_ROUTER, JSON_NODE_SERVICE, JSON_NODE_COMPUTE
+
 
 class TestJSONTranformer(TestCase):
 
     @classmethod
     def setUpClass(self):
         file = 'data/tests/test_nodes.json'
         self.importer = JSONImporter()
@@ -33,8 +35,14 @@
         self.assertEqual(dict_mb["type"],JSON_NODE_MESSAGE_BROKER)
         self.assertEqual(dict_mb["name"], "my_messagebroker")
     
     def test_transform_router(self):
         mr = self.microtosca['my_messagerouter']
         dict_mr = self.tranformer.transform_node_to_json(mr)
         self.assertEqual(dict_mr["type"],JSON_NODE_MESSAGE_ROUTER)
-        self.assertEqual(dict_mr["name"], "my_messagerouter")
+        self.assertEqual(dict_mr["name"], "my_messagerouter")
+
+    def test_transform_compute(self):
+        cmp = self.microtosca['my_compute']
+        dict_cmp = self.tranformer.transform_node_to_json(cmp)
+        self.assertEqual(dict_cmp["type"], JSON_NODE_COMPUTE)
+        self.assertEqual(dict_cmp["name"], "my_compute")
```

### Comparing `microfreshener-core-1.4.0/tests/test_importer/yml_importer/test_import_yml_groups.py` & `microfreshener-core-1.5.0/tests/test_importer/yml_importer/test_import_yml_groups.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_importer/yml_importer/test_import_yml.py` & `microfreshener-core-1.5.0/tests/test_importer/yml_importer/test_import_yml.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,57 @@
 from unittest import TestCase
 
 from microfreshener.core.importer import YMLImporter 
-from microfreshener.core.model import Service, Datastore, CommunicationPattern, MessageBroker, MessageRouter
+from microfreshener.core.model import Service
 
 class TestYMLImporter(TestCase):
 
     @classmethod
     def setUpClass(self):
         file = 'data/examples/hello-world/helloworld.yml'
         self.importer = YMLImporter()
         self.microtosca = self.importer.Import(file)
 
     def test_number_nodes(self):
-        self.assertEqual(len(list(self.microtosca.nodes)), 5)
+        self.assertEqual(len(list(self.microtosca.nodes)), 7)
         
     def test_get_node_by_name(self):
-        self.assertEqual(self.microtosca['shipping'].name, "shipping" )
+        self.assertEqual(self.microtosca['shipping'].name, "shipping")
 
     def test_get_services(self):
         self.assertEqual(len(list(self.microtosca.services)), 2)
     
     def test_database(self):
         db = self.microtosca['shipping']
         self.assertIsInstance(db, Service)
-    
+
+    def test_compute(self):
+        self.assertEqual(len(list(self.microtosca.computes)), 2)
+
+    def test_shipping_deployed_on(self):
+        shipping = self.microtosca["shipping"]
+        self.assertEqual(len(shipping.deployed_on), 1)
+
+    def test_order_deployed_on(self):
+        order = self.microtosca["order"]
+        self.assertEqual(len(order.deployed_on), 1)
+
+    def test_order_db_deployed_on(self):
+        order_db = self.microtosca["order_db"]
+        self.assertEqual(len(order_db.deployed_on), 1)
+
     def test_shipping_interactions(self):
         shipping = self.microtosca["shipping"]
         rels = [link.target.name for link in shipping.interactions]       
         self.assertCountEqual(rels, ['rabbitmq', 'order_db'])
 
     def test_order_interactions(self):
         order = self.microtosca["order"]
         rels = [link.target.name for link in order.interactions]       
-        self.assertCountEqual(rels, ['shipping','order_db','rabbitmq', 'shipping'])
+        self.assertCountEqual(rels, ['shipping', 'order_db', 'rabbitmq', 'shipping'])
     
     def test_gateway_interactions(self):
         order = self.microtosca["gateway"]
         rels = [link.target.name for link in order.interactions]       
         self.assertCountEqual(rels, ['shipping'])
 
     def test_shipping_incoming_interactions(self):
```

### Comparing `microfreshener-core-1.4.0/tests/test_importer/yml_importer/test_import_yml_relationships_properties.py` & `microfreshener-core-1.5.0/tests/test_importer/yml_importer/test_import_yml_relationships_properties.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_importer/yml_importer/test_import_yml_nodes.py` & `microfreshener-core-1.5.0/tests/test_importer/yml_importer/test_import_yml_nodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from unittest import TestCase
 
 from microfreshener.core.importer import YMLImporter
-from microfreshener.core.model import Service, Datastore, CommunicationPattern, MessageBroker, MessageRouter, KIngress, KProxy, KService
+from microfreshener.core.model import Service, Datastore, CommunicationPattern, MessageBroker, MessageRouter, KIngress, \
+    KProxy, KService, Compute
+
 
 class TestYMLImporterNodes(TestCase):
 
     @classmethod
     def setUpClass(self):
         file = 'data/tests/test_nodes.yml'
         self.importer = YMLImporter()
         self.microtosca = self.importer.Import(file)
 
     def test_service(self):
         s1 = self.microtosca['my_service']
         self.assertIsInstance(s1, Service)
         self.assertEqual(s1.name, "my_service")
-    
+
+    def test_compute(self):
+        s1 = self.microtosca['my_compute']
+        self.assertIsInstance(s1, Compute)
+        self.assertEqual(s1.name, "my_compute")
+
     def test_database(self):
         db = self.microtosca['my_datastore']
         self.assertIsInstance(db, Datastore)
         self.assertEqual(db.name, "my_datastore")
     
     def test_messagebroker(self):
         mb = self.microtosca['my_messagebroker']
```

### Comparing `microfreshener-core-1.4.0/tests/test_importer/json_importer/test_import_json_relationships.py` & `microfreshener-core-1.5.0/tests/test_importer/json_importer/test_import_json_relationships.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_importer/json_importer/test_import_json.py` & `microfreshener-core-1.5.0/tests/test_importer/json_importer/test_import_json.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class TestJSONImporter(TestCase):
 
     @classmethod
     def setUpClass(self):
         file = 'data/examples/hello-world/helloworld.json'
         self.loader = JSONImporter()
         self.microtosca_template = self.loader.Import(file)
-    
+
     def test_import_json_as_string(self):
         json_string = """
             {
                 "name": "hello-world",
                 "nodes": [
                     {
                         "name": "shipping",
@@ -31,18 +31,41 @@
                     {
                         "name": "rabbitmq",
                         "type": "messagebroker"
                     },
                     {
                         "name": "gateway",
                         "type": "messagerouter"
+                    },
+                    {
+                        "name": "order_db_compute",
+                        "type": "compute"
+                    },
+                    {
+                        "name": "order_shipping_compute",
+                        "type": "compute"
                     }
                 ],
                 "links": [
                     {
+                        "source": "order_db",
+                        "target": "order_db_compute",
+                        "type": "deployment"
+                    },
+                    {
+                        "source": "order",
+                        "target": "order_shipping_compute",
+                        "type": "deployment"
+                    },
+                    {
+                        "source": "shipping",
+                        "target": "order_shipping_compute",
+                        "type": "deployment"
+                    },
+                    {
                         "source": "shipping",
                         "target": "rabbitmq",
                         "type": "interaction"
                     },
                     {
                         "source": "shipping",
                         "target": "order_db",
@@ -101,46 +124,62 @@
                             "order_db"
                         ]
                     }
                 ]
             }
             """
         self.microtosca_template = self.loader.Import(json_string)
-        self.assertEqual(len(list(self.microtosca_template.nodes)), 5)
+        self.assertEqual(len(list(self.microtosca_template.nodes)), 7)
 
 
 
     def test_number_nodes(self):
-        self.assertEqual(len(list(self.microtosca_template.nodes)), 5)
+        self.assertEqual(len(list(self.microtosca_template.nodes)), 7)
 
     def test_get_node_by_id(self):
         self.assertEqual(self.microtosca_template['shipping'].name, "shipping")
 
     def test_get_services(self):
         self.assertEqual(len(list(self.microtosca_template.services)), 2)
 
     def test_get_database(self):
         self.assertEqual(len(list(self.microtosca_template.datastores)), 1)
       
     def test_get_mb(self):
         self.assertEqual(len(list(self.microtosca_template.datastores)), 1)  
 
     def test_get_mr(self):
-        self.assertEqual(len(list(self.microtosca_template.datastores)), 1)  
+        self.assertEqual(len(list(self.microtosca_template.datastores)), 1)
+
+    def test_get_compute(self):
+        self.assertEqual(len(list(self.microtosca_template.computes)), 2)
 
     def test_shipping_interactions(self):
         shipping = self.microtosca_template["shipping"]
         rels = [link.target.name for link in shipping.interactions]
         self.assertCountEqual(rels,  ['order_db','rabbitmq'])
+        self.assertEqual(len(shipping.deployed_on), 1)
 
     def test_order_interactions(self):
         order = self.microtosca_template["order"]
         rels = [link.target.name for link in order.interactions]
         self.assertCountEqual(rels, [ 'order_db', 'rabbitmq', 'shipping', 'shipping'])
 
+    def test_shipping_deployed_on(self):
+        shipping = self.microtosca_template["shipping"]
+        self.assertEqual(len(shipping.deployed_on), 1)
+
+    def test_order_deployed_on(self):
+        order = self.microtosca_template["order"]
+        self.assertEqual(len(order.deployed_on), 1)
+
+    def test_order_db_deployed_on(self):
+        order_db = self.microtosca_template["order_db"]
+        self.assertEqual(len(order_db.deployed_on), 1)
+
     def test_gateway_interactions(self):
         order = self.microtosca_template["gateway"]
         rels = [link.target.name for link in order.interactions]
         self.assertCountEqual(rels, ['shipping'])
 
     def test_shipping_incoming_interactions(self):
         shipping = self.microtosca_template["shipping"]
```

### Comparing `microfreshener-core-1.4.0/tests/test_importer/json_importer/test_import_json_nodes.py` & `microfreshener-core-1.5.0/tests/test_importer/json_importer/test_import_json_nodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from unittest import TestCase
 
 from microfreshener.core.importer import JSONImporter
 from microfreshener.core.errors import ImporterError
-from microfreshener.core.model import Service, Datastore, CommunicationPattern, MessageBroker, MessageRouter, KIngress, KProxy, KService
-from microfreshener.core.importer.jsontype import JSON_NODE_SERVICE, JSON_NODE_DATABASE, JSON_NODE_MESSAGE_BROKER, JSON_NODE_MESSAGE_ROUTER
+from microfreshener.core.model import Service, Datastore, CommunicationPattern, MessageBroker, MessageRouter, KIngress, \
+    KProxy, KService, Compute
+from microfreshener.core.importer.jsontype import JSON_NODE_SERVICE, JSON_NODE_DATABASE, JSON_NODE_MESSAGE_BROKER, \
+    JSON_NODE_MESSAGE_ROUTER, JSON_NODE_COMPUTE
 from microfreshener.core.importer.jsontype import JSON_NODE_MESSAGE_ROUTER_KINGRESS, JSON_NODE_MESSAGE_ROUTER_KPROXY, JSON_NODE_MESSAGE_ROUTER_KSERVICE
 
 class TestJSONImporterNodes(TestCase):
 
     @classmethod
     def setUpClass(self):
         file = 'data/tests/test_nodes.json'
@@ -15,14 +17,19 @@
         self.microtosca = self.importer.Import(file)
 
     def test_service(self):
         s1 = self.microtosca['my_service']
         self.assertIsInstance(s1, Service)
         self.assertEqual(s1.name, "my_service")
 
+    def test_compute(self):
+        cmp = self.microtosca['my_compute']
+        self.assertIsInstance(cmp, Compute)
+        self.assertEqual(cmp.name, "my_compute")
+
     def test_database(self):
         db = self.microtosca['my_datastore']
         self.assertIsInstance(db, Datastore)
         self.assertEqual(db.name, "my_datastore")
 
     def test_messagebroker(self):
         mb = self.microtosca['my_messagebroker']
@@ -61,14 +68,20 @@
 
     def test_load_node_service(self):
         node = self.importer.load_node_from_json(
             {"type": JSON_NODE_SERVICE, "name": "prova"})
         self.assertIsInstance(node, Service)
         self.assertEqual(node.name, "prova")
 
+    def test_load_node_compute(self):
+        node = self.importer.load_node_from_json(
+            {"type": JSON_NODE_COMPUTE, "name": "prova"})
+        self.assertIsInstance(node, Compute)
+        self.assertEqual(node.name, "prova")
+
     def test_load_node_database(self):
         node = self.importer.load_node_from_json(
             {"type": JSON_NODE_DATABASE, "name": "provadb"})
         self.assertIsInstance(node, Datastore)
         self.assertEqual(node.name, "provadb")
 
     def test_load_node_message_broker(self):
```

### Comparing `microfreshener-core-1.4.0/tests/test_importer/json_importer/test_import_json_relationships_properties.py` & `microfreshener-core-1.5.0/tests/test_importer/json_importer/test_import_json_relationships_properties.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_model/test_relationships.py` & `microfreshener-core-1.5.0/tests/test_model/test_relationships.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_model/test_microtosca.py` & `microfreshener-core-1.5.0/tests/test_model/test_microtosca.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_model/test_group.py` & `microfreshener-core-1.5.0/tests/test_model/test_group.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_refiner/test_istio_refiner_destination_rule.py` & `microfreshener-core-1.5.0/tests/test_refiner/test_istio_refiner_destination_rule.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/tests/test_refiner/test_kubernetes_refiner.py` & `microfreshener-core-1.5.0/tests/test_refiner/test_kubernetes_refiner.py`

 * *Files identical despite different names*

### Comparing `microfreshener-core-1.4.0/LICENSE` & `microfreshener-core-1.5.0/LICENSE`

 * *Files identical despite different names*

