# Comparing `tmp/cldfviz-1.0.2.tar.gz` & `tmp/cldfviz-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cldfviz-1.0.2.tar", last modified: Tue Dec  5 14:13:38 2023, max compression
+gzip compressed data, was "cldfviz-1.1.0.tar", last modified: Tue May  7 14:26:30 2024, max compression
```

## Comparing `cldfviz-1.0.2.tar` & `cldfviz-1.1.0.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-12-05 14:13:38.834249 cldfviz-1.0.2/
--rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2022-12-22 10:06:37.000000 cldfviz-1.0.2/LICENSE
--rw-rw-r--   0 robert    (1000) robert    (1000)       50 2022-12-22 10:06:37.000000 cldfviz-1.0.2/MANIFEST.in
--rw-rw-r--   0 robert    (1000) robert    (1000)     7507 2023-12-05 14:13:38.834249 cldfviz-1.0.2/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)     6435 2023-12-01 07:39:52.000000 cldfviz-1.0.2/README.md
--rw-rw-r--   0 robert    (1000) robert    (1000)       81 2022-12-22 10:06:37.000000 cldfviz-1.0.2/pyproject.toml
--rw-rw-r--   0 robert    (1000) robert    (1000)     2104 2023-12-05 14:13:38.838249 cldfviz-1.0.2/setup.cfg
--rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2022-12-22 10:06:37.000000 cldfviz-1.0.2/setup.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-12-05 14:13:38.834249 cldfviz-1.0.2/src/
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-12-05 14:13:38.834249 cldfviz-1.0.2/src/cldfviz/
--rw-rw-r--   0 robert    (1000) robert    (1000)       78 2023-12-05 14:12:30.000000 cldfviz-1.0.2/src/cldfviz/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    11824 2023-12-01 08:06:14.000000 cldfviz-1.0.2/src/cldfviz/cli_util.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     4969 2023-02-04 12:07:55.000000 cldfviz-1.0.2/src/cldfviz/colormap.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-12-05 14:13:38.834249 cldfviz-1.0.2/src/cldfviz/commands/
--rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/commands/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2841 2023-01-31 15:05:03.000000 cldfviz-1.0.2/src/cldfviz/commands/audiowordlist.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3389 2023-08-11 06:24:14.000000 cldfviz-1.0.2/src/cldfviz/commands/erd.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     1224 2023-01-31 14:56:29.000000 cldfviz-1.0.2/src/cldfviz/commands/examples.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     4320 2023-02-03 08:00:56.000000 cldfviz-1.0.2/src/cldfviz/commands/map.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     5453 2023-12-01 09:31:49.000000 cldfviz-1.0.2/src/cldfviz/commands/text.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     4840 2023-02-03 15:25:31.000000 cldfviz-1.0.2/src/cldfviz/commands/tree.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     7790 2023-08-12 05:31:33.000000 cldfviz-1.0.2/src/cldfviz/commands/treemap.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2987 2023-01-27 09:26:51.000000 cldfviz-1.0.2/src/cldfviz/glottolog.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-12-05 14:13:38.834249 cldfviz-1.0.2/src/cldfviz/map/
--rw-rw-r--   0 robert    (1000) robert    (1000)     2047 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/map/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     1811 2023-02-03 15:41:05.000000 cldfviz-1.0.2/src/cldfviz/map/base.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     9936 2023-02-06 12:48:51.000000 cldfviz-1.0.2/src/cldfviz/map/leaflet.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    15859 2023-08-12 10:45:49.000000 cldfviz-1.0.2/src/cldfviz/map/mpl.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2136 2023-01-31 15:23:17.000000 cldfviz-1.0.2/src/cldfviz/media.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    10189 2023-11-30 13:03:32.000000 cldfviz-1.0.2/src/cldfviz/multiparameter.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      924 2023-01-30 09:33:14.000000 cldfviz-1.0.2/src/cldfviz/pdutils.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      383 2023-01-31 07:56:07.000000 cldfviz-1.0.2/src/cldfviz/template.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-12-05 14:13:38.834249 cldfviz-1.0.2/src/cldfviz/templates/
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-12-05 14:13:38.834249 cldfviz-1.0.2/src/cldfviz/templates/audiowordlist/
--rw-rw-r--   0 robert    (1000) robert    (1000)     1730 2023-01-31 08:05:08.000000 cldfviz-1.0.2/src/cldfviz/templates/audiowordlist/audiowordlist.html
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-12-05 14:13:38.834249 cldfviz-1.0.2/src/cldfviz/templates/examples/
--rw-rw-r--   0 robert    (1000) robert    (1000)     2950 2023-01-31 14:54:36.000000 cldfviz-1.0.2/src/cldfviz/templates/examples/examples.html
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-12-05 14:13:38.834249 cldfviz-1.0.2/src/cldfviz/templates/map/
--rw-rw-r--   0 robert    (1000) robert    (1000)      459 2023-02-06 12:00:46.000000 cldfviz-1.0.2/src/cldfviz/templates/map/README.md
--rw-rw-r--   0 robert    (1000) robert    (1000)  1876729 2023-02-04 15:20:32.000000 cldfviz-1.0.2/src/cldfviz/templates/map/ecoregions.geojson.zip
--rw-rw-r--   0 robert    (1000) robert    (1000)     1984 2023-02-04 15:33:21.000000 cldfviz-1.0.2/src/cldfviz/templates/map/ecoregions.js
--rw-rw-r--   0 robert    (1000) robert    (1000)     4145 2023-02-04 15:06:13.000000 cldfviz-1.0.2/src/cldfviz/templates/map/leaflet.html
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-12-05 14:13:38.834249 cldfviz-1.0.2/src/cldfviz/templates/text/
--rw-rw-r--   0 robert    (1000) robert    (1000)      489 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/BorrowingTable_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      149 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/CodeTable_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      141 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/CognateTable_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      404 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/CognateTable_index.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      407 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/CognatesetTable_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      285 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/ContributionTable_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      192 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/ContributionTable_index.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      344 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/EntryTable_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)     1379 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/ExampleTable_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      157 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/FormTable_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      333 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/LanguageTable_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      625 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/LanguageTable_index.md
--rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/MediaTable_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)        9 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/Metadata_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      360 2023-12-05 12:03:04.000000 cldfviz-1.0.2/src/cldfviz/templates/text/ParameterTable_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      110 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/ParameterTable_index.md
--rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/SenseTable_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      679 2023-12-05 07:30:32.000000 cldfviz-1.0.2/src/cldfviz/templates/text/Source_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      356 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/Source_index.md
--rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-22 10:06:37.000000 cldfviz-1.0.2/src/cldfviz/templates/text/ValueTable_detail.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      214 2023-12-05 12:02:50.000000 cldfviz-1.0.2/src/cldfviz/templates/text/property.md
--rw-rw-r--   0 robert    (1000) robert    (1000)     2678 2023-12-05 07:10:08.000000 cldfviz-1.0.2/src/cldfviz/templates/text/util.md
--rw-rw-r--   0 robert    (1000) robert    (1000)     6924 2023-12-05 12:18:09.000000 cldfviz-1.0.2/src/cldfviz/text.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     9461 2023-10-09 04:57:41.000000 cldfviz-1.0.2/src/cldfviz/tree.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-12-05 14:13:38.834249 cldfviz-1.0.2/src/cldfviz.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     7507 2023-12-05 14:13:38.000000 cldfviz-1.0.2/src/cldfviz.egg-info/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)     2393 2023-12-05 14:13:38.000000 cldfviz-1.0.2/src/cldfviz.egg-info/SOURCES.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-12-05 14:13:38.000000 cldfviz-1.0.2/src/cldfviz.egg-info/dependency_links.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)       49 2023-12-05 14:13:38.000000 cldfviz-1.0.2/src/cldfviz.egg-info/entry_points.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-12-22 10:13:08.000000 cldfviz-1.0.2/src/cldfviz.egg-info/not-zip-safe
--rw-rw-r--   0 robert    (1000) robert    (1000)      328 2023-12-05 14:13:38.000000 cldfviz-1.0.2/src/cldfviz.egg-info/requires.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        8 2023-12-05 14:13:38.000000 cldfviz-1.0.2/src/cldfviz.egg-info/top_level.txt
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-12-05 14:13:38.834249 cldfviz-1.0.2/tests/
--rw-rw-r--   0 robert    (1000) robert    (1000)    15377 2023-12-01 09:33:53.000000 cldfviz-1.0.2/tests/test_cli.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      323 2023-02-04 14:26:30.000000 cldfviz-1.0.2/tests/test_cli_util.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2553 2023-02-03 06:55:26.000000 cldfviz-1.0.2/tests/test_colormap.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     1402 2023-01-27 13:59:26.000000 cldfviz-1.0.2/tests/test_glottolog.py
--rw-rw-r--   0 robert    (1000) robert    (1000)        2 2023-02-03 06:55:26.000000 cldfviz-1.0.2/tests/test_map.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2208 2023-12-01 08:06:14.000000 cldfviz-1.0.2/tests/test_multiparameter.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     5116 2023-12-05 12:15:42.000000 cldfviz-1.0.2/tests/test_text.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     1537 2023-10-09 04:55:51.000000 cldfviz-1.0.2/tests/test_tree.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-07 14:26:30.866493 cldfviz-1.1.0/
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2022-12-22 10:06:37.000000 cldfviz-1.1.0/LICENSE
+-rw-rw-r--   0 robert    (1000) robert    (1000)       50 2022-12-22 10:06:37.000000 cldfviz-1.1.0/MANIFEST.in
+-rw-rw-r--   0 robert    (1000) robert    (1000)     8517 2024-05-07 14:26:30.866493 cldfviz-1.1.0/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     7421 2024-05-07 14:14:06.000000 cldfviz-1.1.0/README.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)       81 2022-12-22 10:06:37.000000 cldfviz-1.1.0/pyproject.toml
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2135 2024-05-07 14:26:30.866493 cldfviz-1.1.0/setup.cfg
+-rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2022-12-22 10:06:37.000000 cldfviz-1.1.0/setup.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-07 14:26:30.862493 cldfviz-1.1.0/src/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-07 14:26:30.862493 cldfviz-1.1.0/src/cldfviz/
+-rw-rw-r--   0 robert    (1000) robert    (1000)       78 2024-05-07 14:24:33.000000 cldfviz-1.1.0/src/cldfviz/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11824 2024-03-05 11:07:42.000000 cldfviz-1.1.0/src/cldfviz/cli_util.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4969 2023-02-04 12:07:55.000000 cldfviz-1.1.0/src/cldfviz/colormap.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-07 14:26:30.862493 cldfviz-1.1.0/src/cldfviz/commands/
+-rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/commands/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2841 2023-01-31 15:05:03.000000 cldfviz-1.1.0/src/cldfviz/commands/audiowordlist.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3389 2023-08-11 06:24:14.000000 cldfviz-1.1.0/src/cldfviz/commands/erd.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1224 2023-01-31 14:56:29.000000 cldfviz-1.1.0/src/cldfviz/commands/examples.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4320 2023-02-03 08:00:56.000000 cldfviz-1.1.0/src/cldfviz/commands/map.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     8647 2024-05-06 16:55:52.000000 cldfviz-1.1.0/src/cldfviz/commands/network.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     5453 2023-12-01 09:31:49.000000 cldfviz-1.1.0/src/cldfviz/commands/text.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4840 2023-02-03 15:25:31.000000 cldfviz-1.1.0/src/cldfviz/commands/tree.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     7790 2023-08-12 05:31:33.000000 cldfviz-1.1.0/src/cldfviz/commands/treemap.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2987 2023-01-27 09:26:51.000000 cldfviz-1.1.0/src/cldfviz/glottolog.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-07 14:26:30.862493 cldfviz-1.1.0/src/cldfviz/map/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2047 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/map/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1811 2023-02-03 15:41:05.000000 cldfviz-1.1.0/src/cldfviz/map/base.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     9936 2023-02-06 12:48:51.000000 cldfviz-1.1.0/src/cldfviz/map/leaflet.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    15859 2023-08-12 10:45:49.000000 cldfviz-1.1.0/src/cldfviz/map/mpl.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2136 2023-01-31 15:23:17.000000 cldfviz-1.1.0/src/cldfviz/media.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    10431 2024-05-06 16:55:52.000000 cldfviz-1.1.0/src/cldfviz/multiparameter.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      924 2023-01-30 09:33:14.000000 cldfviz-1.1.0/src/cldfviz/pdutils.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      383 2023-01-31 07:56:07.000000 cldfviz-1.1.0/src/cldfviz/template.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-07 14:26:30.862493 cldfviz-1.1.0/src/cldfviz/templates/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-07 14:26:30.862493 cldfviz-1.1.0/src/cldfviz/templates/audiowordlist/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1730 2023-01-31 08:05:08.000000 cldfviz-1.1.0/src/cldfviz/templates/audiowordlist/audiowordlist.html
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-07 14:26:30.862493 cldfviz-1.1.0/src/cldfviz/templates/examples/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2950 2023-01-31 14:54:36.000000 cldfviz-1.1.0/src/cldfviz/templates/examples/examples.html
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-07 14:26:30.862493 cldfviz-1.1.0/src/cldfviz/templates/map/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      459 2023-02-06 12:00:46.000000 cldfviz-1.1.0/src/cldfviz/templates/map/README.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)  1876729 2023-02-04 15:20:32.000000 cldfviz-1.1.0/src/cldfviz/templates/map/ecoregions.geojson.zip
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1984 2023-02-04 15:33:21.000000 cldfviz-1.1.0/src/cldfviz/templates/map/ecoregions.js
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4145 2023-02-04 15:06:13.000000 cldfviz-1.1.0/src/cldfviz/templates/map/leaflet.html
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-07 14:26:30.866493 cldfviz-1.1.0/src/cldfviz/templates/text/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      489 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/BorrowingTable_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      149 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/CodeTable_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      141 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/CognateTable_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      404 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/CognateTable_index.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      407 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/CognatesetTable_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      285 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/ContributionTable_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      192 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/ContributionTable_index.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      344 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/EntryTable_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1379 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/ExampleTable_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      157 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/FormTable_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      333 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/LanguageTable_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      625 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/LanguageTable_index.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/MediaTable_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)        9 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/Metadata_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      360 2023-12-05 12:03:04.000000 cldfviz-1.1.0/src/cldfviz/templates/text/ParameterTable_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      110 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/ParameterTable_index.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/SenseTable_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      679 2023-12-05 07:30:32.000000 cldfviz-1.1.0/src/cldfviz/templates/text/Source_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      356 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/Source_index.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-22 10:06:37.000000 cldfviz-1.1.0/src/cldfviz/templates/text/ValueTable_detail.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      214 2023-12-05 12:02:50.000000 cldfviz-1.1.0/src/cldfviz/templates/text/property.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2678 2023-12-05 07:10:08.000000 cldfviz-1.1.0/src/cldfviz/templates/text/util.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)     6924 2023-12-05 12:18:09.000000 cldfviz-1.1.0/src/cldfviz/text.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     9461 2023-10-09 04:57:41.000000 cldfviz-1.1.0/src/cldfviz/tree.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-07 14:26:30.862493 cldfviz-1.1.0/src/cldfviz.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     8517 2024-05-07 14:26:30.000000 cldfviz-1.1.0/src/cldfviz.egg-info/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2425 2024-05-07 14:26:30.000000 cldfviz-1.1.0/src/cldfviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2024-05-07 14:26:30.000000 cldfviz-1.1.0/src/cldfviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       49 2024-05-07 14:26:30.000000 cldfviz-1.1.0/src/cldfviz.egg-info/entry_points.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-12-22 10:13:08.000000 cldfviz-1.1.0/src/cldfviz.egg-info/not-zip-safe
+-rw-rw-r--   0 robert    (1000) robert    (1000)      357 2024-05-07 14:26:30.000000 cldfviz-1.1.0/src/cldfviz.egg-info/requires.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        8 2024-05-07 14:26:30.000000 cldfviz-1.1.0/src/cldfviz.egg-info/top_level.txt
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-07 14:26:30.866493 cldfviz-1.1.0/tests/
+-rw-rw-r--   0 robert    (1000) robert    (1000)    17157 2024-05-06 15:57:35.000000 cldfviz-1.1.0/tests/test_cli.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      323 2023-02-04 14:26:30.000000 cldfviz-1.1.0/tests/test_cli_util.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2553 2023-02-03 06:55:26.000000 cldfviz-1.1.0/tests/test_colormap.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1402 2023-01-27 13:59:26.000000 cldfviz-1.1.0/tests/test_glottolog.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)        2 2023-02-03 06:55:26.000000 cldfviz-1.1.0/tests/test_map.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2208 2023-12-01 08:06:14.000000 cldfviz-1.1.0/tests/test_multiparameter.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     5116 2023-12-05 12:15:42.000000 cldfviz-1.1.0/tests/test_text.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1537 2023-10-09 04:55:51.000000 cldfviz-1.1.0/tests/test_tree.py
```

### Comparing `cldfviz-1.0.2/LICENSE` & `cldfviz-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/PKG-INFO` & `cldfviz-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cldfviz
-Version: 1.0.2
+Version: 1.1.0
 Summary: A cldfbench plugin to create vizualisations of CLDF datasets
 Home-page: https://github.com/cldf/cldfviz
 Author: Robert Forkel
 Author-email: dlce.rdm@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/cldf/cldfviz/issues
 Keywords: cldfbench
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cartopy
 Provides-Extra: dev
 Provides-Extra: lingtreemaps
+Provides-Extra: network
 Provides-Extra: test
 License-File: LICENSE
 
 # cldfviz
 
 [![Build Status](https://github.com/cldf/cldfviz/workflows/tests/badge.svg)](https://github.com/cldf/cldfviz/actions?query=workflow%3Atests)
 [![PyPI](https://img.shields.io/pypi/v/cldfviz.svg)](https://pypi.org/project/cldfviz)
@@ -170,14 +171,29 @@
 are "entity-relationship diagrams", i.e. diagramy of the [entitty-relationship model](https://en.wikipedia.org/wiki/Entity%E2%80%93relationship_model)
 of the dataset. Such a diagram can be created via `cldfviz.erd` (if a Java runtime is installed).
 For details see [docs/erd.md](docs/erd.md).
 
 [<img alt="details" width="350" src="docs/output/wacl.svg" />](docs/erd.md)
 
 
+### `cldfviz.network`
+
+A [ParameterNetwork component](https://github.com/cldf/cldf/tree/master/components/parameternetworks)
+was added to CLDF with version 1.3, acknowledging that in datasets like [CLICS](https://clics.clld.org/)
+a network of parameters (established through colexifications in CLICS) acted as both, output of the
+colexification algorithm, but also as input for various cluster methods. Since there are many tools
+for network analysis available, the main task for a CLDF-based tool is to convert (filtered) parts
+of a `ParameterNetwork` to a format that can serve as input for other tools. This is what `cldfviz.network`
+does and since [Graphviz' DOT format](https://graphviz.org/doc/info/lang.html) is one of the target
+formats supported by `cldfviz.network`, exploratory analysis is supported by just piping the output
+into the `dot` program to create a network visualization.
+
+[<img alt="details" width="350" src="docs/output/partof_neck2.svg" />](docs/network.md)
+
+
 ## Related
 
 Other tools to convert CLDF data to "human-readable" formats:
 - [cldfofflinebrowser](https://github.com/cldf/cldfofflinebrowser)
 - [clld](https://github.com/clld/clld)
```

### Comparing `cldfviz-1.0.2/README.md` & `cldfviz-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -140,12 +140,27 @@
 are "entity-relationship diagrams", i.e. diagramy of the [entitty-relationship model](https://en.wikipedia.org/wiki/Entity%E2%80%93relationship_model)
 of the dataset. Such a diagram can be created via `cldfviz.erd` (if a Java runtime is installed).
 For details see [docs/erd.md](docs/erd.md).
 
 [<img alt="details" width="350" src="docs/output/wacl.svg" />](docs/erd.md)
 
 
+### `cldfviz.network`
+
+A [ParameterNetwork component](https://github.com/cldf/cldf/tree/master/components/parameternetworks)
+was added to CLDF with version 1.3, acknowledging that in datasets like [CLICS](https://clics.clld.org/)
+a network of parameters (established through colexifications in CLICS) acted as both, output of the
+colexification algorithm, but also as input for various cluster methods. Since there are many tools
+for network analysis available, the main task for a CLDF-based tool is to convert (filtered) parts
+of a `ParameterNetwork` to a format that can serve as input for other tools. This is what `cldfviz.network`
+does and since [Graphviz' DOT format](https://graphviz.org/doc/info/lang.html) is one of the target
+formats supported by `cldfviz.network`, exploratory analysis is supported by just piping the output
+into the `dot` program to create a network visualization.
+
+[<img alt="details" width="350" src="docs/output/partof_neck2.svg" />](docs/network.md)
+
+
 ## Related
 
 Other tools to convert CLDF data to "human-readable" formats:
 - [cldfofflinebrowser](https://github.com/cldf/cldfofflinebrowser)
 - [clld](https://github.com/clld/clld)
```

### Comparing `cldfviz-1.0.2/setup.cfg` & `cldfviz-1.1.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cldfviz
-version = 1.0.2
+version = 1.1.0
 author = Robert Forkel
 author_email = dlce.rdm@eva.mpg.de
 description = A cldfbench plugin to create vizualisations of CLDF datasets
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = cldfbench
 license = Apache 2.0
@@ -71,15 +71,18 @@
 	biopython
 	pyyaml
 dev = 
 	flake8
 	wheel
 	build
 	twine
+network = 
+	networkx
 test = 
+	networkx
 	pytest>=5
 	pytest-mock
 	pytest-cov
 	coverage>=4.2
 	requests-mock
 
 [bdist_wheel]
```

### Comparing `cldfviz-1.0.2/src/cldfviz/cli_util.py` & `cldfviz-1.1.0/src/cldfviz/cli_util.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/colormap.py` & `cldfviz-1.1.0/src/cldfviz/colormap.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/commands/audiowordlist.py` & `cldfviz-1.1.0/src/cldfviz/commands/audiowordlist.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/commands/erd.py` & `cldfviz-1.1.0/src/cldfviz/commands/erd.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/commands/examples.py` & `cldfviz-1.1.0/src/cldfviz/commands/examples.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/commands/map.py` & `cldfviz-1.1.0/src/cldfviz/commands/map.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/commands/text.py` & `cldfviz-1.1.0/src/cldfviz/commands/text.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/commands/tree.py` & `cldfviz-1.1.0/src/cldfviz/commands/tree.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/commands/treemap.py` & `cldfviz-1.1.0/src/cldfviz/commands/treemap.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/glottolog.py` & `cldfviz-1.1.0/src/cldfviz/glottolog.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/map/__init__.py` & `cldfviz-1.1.0/src/cldfviz/map/__init__.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/map/base.py` & `cldfviz-1.1.0/src/cldfviz/map/base.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/map/leaflet.py` & `cldfviz-1.1.0/src/cldfviz/map/leaflet.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/map/mpl.py` & `cldfviz-1.1.0/src/cldfviz/map/mpl.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/media.py` & `cldfviz-1.1.0/src/cldfviz/media.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/multiparameter.py` & `cldfviz-1.1.0/src/cldfviz/multiparameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,18 +142,20 @@
         for i, language_property in enumerate(language_properties):
             if i == 0:
                 language_rows = [
                     r for r in ds.iter_rows('LanguageTable', 'id', 'name')
                     if r['id'] in langs]
             if not all(isinstance(v[language_property], (int, float, decimal.Decimal))
                        for v in language_rows if v[language_property] is not None):
+                counts = collections.Counter([r[language_property] for r in language_rows])
                 codes[language_property] = collections.OrderedDict([
                     (p, p) for p in sorted(
                         set(r[language_property] for r in language_rows
-                            if r[language_property] is not None))
+                            if r[language_property] is not None),
+                        key=lambda x: -counts[x])
                 ])
         self.languages = collections.OrderedDict()
         self.values = []
         colmap = ['languageReference', 'parameterReference', 'value']
         if codes:
             colmap.append('codeReference')
         if pids:
@@ -209,16 +211,18 @@
                 vals = [v for v in self.values if v.pid == p.id]
                 if all(v.float is not None for v in vals) and \
                         (len(set(v.v for v in vals)) > 8 or  # noqa: W504
                          (datatypes and datatypes[i] == 'number')):
                     p.type = CONTINUOUS
                     p.domain = (min(v.float for v in vals), max(v.float for v in vals))
                 else:
+                    counts = collections.Counter([vv.v for vv in vals])
                     p.domain = collections.OrderedDict([
-                        (v, v) for v in sorted(set(vv.v for vv in vals), key=lambda vv: str(vv))])
+                        (v, v)
+                        for v in sorted(set(vv.v for vv in vals), key=lambda vv: -counts[vv])])
 
     def __str__(self):  # pragma: no cover
         return str(self.parameters)
 
     def iter_languages(self) \
             -> typing.Iterator[typing.Tuple[Language, typing.Dict[str, typing.List[Value]]]]:
         for lid, values in itertools.groupby(sorted(self.values), lambda v: v.lid):
```

### Comparing `cldfviz-1.0.2/src/cldfviz/pdutils.py` & `cldfviz-1.1.0/src/cldfviz/pdutils.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/templates/audiowordlist/audiowordlist.html` & `cldfviz-1.1.0/src/cldfviz/templates/audiowordlist/audiowordlist.html`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/templates/examples/examples.html` & `cldfviz-1.1.0/src/cldfviz/templates/examples/examples.html`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/templates/map/ecoregions.geojson.zip` & `cldfviz-1.1.0/src/cldfviz/templates/map/ecoregions.geojson.zip`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/templates/map/ecoregions.js` & `cldfviz-1.1.0/src/cldfviz/templates/map/ecoregions.js`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/templates/map/leaflet.html` & `cldfviz-1.1.0/src/cldfviz/templates/map/leaflet.html`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/templates/text/ExampleTable_detail.md` & `cldfviz-1.1.0/src/cldfviz/templates/text/ExampleTable_detail.md`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/templates/text/LanguageTable_index.md` & `cldfviz-1.1.0/src/cldfviz/templates/text/LanguageTable_index.md`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/templates/text/Source_detail.md` & `cldfviz-1.1.0/src/cldfviz/templates/text/Source_detail.md`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/templates/text/util.md` & `cldfviz-1.1.0/src/cldfviz/templates/text/util.md`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/text.py` & `cldfviz-1.1.0/src/cldfviz/text.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz/tree.py` & `cldfviz-1.1.0/src/cldfviz/tree.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/src/cldfviz.egg-info/PKG-INFO` & `cldfviz-1.1.0/src/cldfviz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cldfviz
-Version: 1.0.2
+Version: 1.1.0
 Summary: A cldfbench plugin to create vizualisations of CLDF datasets
 Home-page: https://github.com/cldf/cldfviz
 Author: Robert Forkel
 Author-email: dlce.rdm@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/cldf/cldfviz/issues
 Keywords: cldfbench
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cartopy
 Provides-Extra: dev
 Provides-Extra: lingtreemaps
+Provides-Extra: network
 Provides-Extra: test
 License-File: LICENSE
 
 # cldfviz
 
 [![Build Status](https://github.com/cldf/cldfviz/workflows/tests/badge.svg)](https://github.com/cldf/cldfviz/actions?query=workflow%3Atests)
 [![PyPI](https://img.shields.io/pypi/v/cldfviz.svg)](https://pypi.org/project/cldfviz)
@@ -170,14 +171,29 @@
 are "entity-relationship diagrams", i.e. diagramy of the [entitty-relationship model](https://en.wikipedia.org/wiki/Entity%E2%80%93relationship_model)
 of the dataset. Such a diagram can be created via `cldfviz.erd` (if a Java runtime is installed).
 For details see [docs/erd.md](docs/erd.md).
 
 [<img alt="details" width="350" src="docs/output/wacl.svg" />](docs/erd.md)
 
 
+### `cldfviz.network`
+
+A [ParameterNetwork component](https://github.com/cldf/cldf/tree/master/components/parameternetworks)
+was added to CLDF with version 1.3, acknowledging that in datasets like [CLICS](https://clics.clld.org/)
+a network of parameters (established through colexifications in CLICS) acted as both, output of the
+colexification algorithm, but also as input for various cluster methods. Since there are many tools
+for network analysis available, the main task for a CLDF-based tool is to convert (filtered) parts
+of a `ParameterNetwork` to a format that can serve as input for other tools. This is what `cldfviz.network`
+does and since [Graphviz' DOT format](https://graphviz.org/doc/info/lang.html) is one of the target
+formats supported by `cldfviz.network`, exploratory analysis is supported by just piping the output
+into the `dot` program to create a network visualization.
+
+[<img alt="details" width="350" src="docs/output/partof_neck2.svg" />](docs/network.md)
+
+
 ## Related
 
 Other tools to convert CLDF data to "human-readable" formats:
 - [cldfofflinebrowser](https://github.com/cldf/cldfofflinebrowser)
 - [clld](https://github.com/clld/clld)
```

### Comparing `cldfviz-1.0.2/src/cldfviz.egg-info/SOURCES.txt` & `cldfviz-1.1.0/src/cldfviz.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 src/cldfviz.egg-info/requires.txt
 src/cldfviz.egg-info/top_level.txt
 src/cldfviz/commands/__init__.py
 src/cldfviz/commands/audiowordlist.py
 src/cldfviz/commands/erd.py
 src/cldfviz/commands/examples.py
 src/cldfviz/commands/map.py
+src/cldfviz/commands/network.py
 src/cldfviz/commands/text.py
 src/cldfviz/commands/tree.py
 src/cldfviz/commands/treemap.py
 src/cldfviz/map/__init__.py
 src/cldfviz/map/base.py
 src/cldfviz/map/leaflet.py
 src/cldfviz/map/mpl.py
```

### Comparing `cldfviz-1.0.2/tests/test_cli.py` & `cldfviz-1.1.0/tests/test_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -200,14 +200,72 @@
         jar.write_text('abc', encoding='utf8')
         o = tmp_path / 'res.svg'
         m.get(requests_mock.ANY, text='abc')
         main(['cldfviz.erd', ds_arg, '--output', str(o), '--test', '--sqlite-jar', str(jar)])
         assert o.exists()
 
 
+def test_network(capsys, StructureDataset, tmp_path):
+    eattrs = tmp_path / 'e.py'
+    eattrs.write_text(
+        """dict(
+    drop=lambda e: e.id == "2",
+    color=lambda e: "red" if e.id == "1" else "blue",
+    integer=lambda e: 1,
+    float=lambda e: 2.1,
+    boolean=True,
+)""",
+        encoding='utf8')
+
+    nattrs = tmp_path / 'n.py'
+    nattrs.write_text('dict(color=lambda n: "black" if n.id == "B" else None)', encoding='utf8')
+
+    runcli(
+        'cldfviz.network',
+        '{} --edge-attributes {} --node-attributes {} --format graphml'.format(
+            StructureDataset.directory,
+            eattrs,
+            nattrs,
+        ))
+    assert '<node ' in capsys.readouterr()[0]
+
+    runcli('cldfviz.network', '{} --edge-attributes {}'.format(
+        StructureDataset.directory,
+        eattrs,
+    ))
+    assert 'digraph' in capsys.readouterr()[0]
+
+    runcli('cldfviz.network', """{} --edge-filters '{}'""".format(
+        StructureDataset.directory,
+        '{"Description": "a"}'
+    ))
+    assert capsys.readouterr()[0].count('->') == 3
+
+    runcli('cldfviz.network', """{} --edge-filters '{}'""".format(
+        StructureDataset.directory,
+        '{"Description": ["a"]}'
+    ))
+    assert capsys.readouterr()[0].count('->') == 3
+
+    runcli('cldfviz.network', """{} --edge-filters '{}'""".format(
+        StructureDataset.directory,
+        '{"Description": "a|b"}'
+    ))
+    assert capsys.readouterr()[0].count('->') == 4
+
+    runcli('cldfviz.network', """{} --edge-filters '{}'""".format(
+        StructureDataset.directory,
+        '{"iattr": 4}'
+    ))
+    assert capsys.readouterr()[0].count('->') == 1
+
+    runcli('cldfviz.network', """{} --parameter 'H'""".format(StructureDataset.directory))
+    assert capsys.readouterr()[0].count('->') == 2
+
+
 @pytest.mark.parametrize(
     'ds,opts,expect',
     [
         (
             'StructureDataset',
             '--text-string "[](Source?with_the_works=false#cldf:__all__)"',
             lambda out: 'Peterson, John' in out),
```

### Comparing `cldfviz-1.0.2/tests/test_colormap.py` & `cldfviz-1.1.0/tests/test_colormap.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/tests/test_glottolog.py` & `cldfviz-1.1.0/tests/test_glottolog.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/tests/test_multiparameter.py` & `cldfviz-1.1.0/tests/test_multiparameter.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/tests/test_text.py` & `cldfviz-1.1.0/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `cldfviz-1.0.2/tests/test_tree.py` & `cldfviz-1.1.0/tests/test_tree.py`

 * *Files identical despite different names*

