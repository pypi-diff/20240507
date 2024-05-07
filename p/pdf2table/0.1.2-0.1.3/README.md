# Comparing `tmp/pdf2table-0.1.2.tar.gz` & `tmp/pdf2table-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf2table-0.1.2.tar", last modified: Wed Apr 24 15:55:26 2024, max compression
+gzip compressed data, was "pdf2table-0.1.3.tar", last modified: Tue May  7 03:21:18 2024, max compression
```

## Comparing `pdf2table-0.1.2.tar` & `pdf2table-0.1.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.972113 pdf2table-0.1.2/
--rw-r--r--   0 lirongzhi   (501) staff       (20)     1067 2024-04-22 17:13:14.000000 pdf2table-0.1.2/LICENSE
--rw-r--r--   0 lirongzhi   (501) staff       (20)     2806 2024-04-24 15:55:26.972053 pdf2table-0.1.2/PKG-INFO
--rw-r--r--   0 lirongzhi   (501) staff       (20)     2076 2024-04-24 12:39:38.000000 pdf2table-0.1.2/README.md
--rw-r--r--   0 lirongzhi   (501) staff       (20)       89 2024-04-24 12:58:11.000000 pdf2table-0.1.2/pyproject.toml
--rw-r--r--   0 lirongzhi   (501) staff       (20)      689 2024-04-24 15:55:26.972380 pdf2table-0.1.2/setup.cfg
--rw-r--r--   0 lirongzhi   (501) staff       (20)      909 2024-04-24 15:54:38.000000 pdf2table-0.1.2/setup.py
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.957105 pdf2table-0.1.2/src/
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.959411 pdf2table-0.1.2/src/pdf2table/
--rw-r--r--   0 lirongzhi   (501) staff       (20)       26 2024-04-24 07:05:41.000000 pdf2table-0.1.2/src/pdf2table/__init__.py
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.961695 pdf2table-0.1.2/src/pdf2table/document/
--rw-r--r--   0 lirongzhi   (501) staff       (20)       68 2024-04-24 06:53:50.000000 pdf2table-0.1.2/src/pdf2table/document/__init__.py
--rw-r--r--   0 lirongzhi   (501) staff       (20)     4173 2024-04-23 15:47:40.000000 pdf2table-0.1.2/src/pdf2table/document/image.py
--rw-r--r--   0 lirongzhi   (501) staff       (20)     2493 2024-04-23 15:52:43.000000 pdf2table-0.1.2/src/pdf2table/document/page.py
--rw-r--r--   0 lirongzhi   (501) staff       (20)     5097 2024-04-24 14:19:02.000000 pdf2table-0.1.2/src/pdf2table/document/pdf.py
--rw-r--r--   0 lirongzhi   (501) staff       (20)     2822 2024-04-24 12:38:16.000000 pdf2table-0.1.2/src/pdf2table/driver.py
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.962580 pdf2table-0.1.2/src/pdf2table/table/
--rw-r--r--   0 lirongzhi   (501) staff       (20)     5449 2024-04-23 13:52:16.000000 pdf2table-0.1.2/src/pdf2table/table/__init__.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)    13363 2024-04-23 02:51:26.000000 pdf2table-0.1.2/src/pdf2table/table/metrics.py
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.963068 pdf2table-0.1.2/src/pdf2table/table/processing/
--rw-r--r--   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:27:10.000000 pdf2table-0.1.2/src/pdf2table/table/processing/__init__.py
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.963960 pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/
--rw-r--r--   0 lirongzhi   (501) staff       (20)        0 2024-04-23 02:56:13.000000 pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.964908 pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/cells/
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     1197 2024-04-23 08:38:52.000000 pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/cells/__init__.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     4767 2024-04-23 08:33:44.000000 pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/cells/deduplication.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     6421 2024-04-23 13:56:23.000000 pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/cells/identification.py
--rw-r--r--   0 lirongzhi   (501) staff       (20)     9420 2024-04-23 02:59:15.000000 pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/line.py
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.966277 pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/tables/
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     1611 2024-04-23 13:47:40.000000 pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/tables/__init__.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     3315 2024-04-23 09:33:15.000000 pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/tables/cell_clustering.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     6600 2024-04-23 03:23:59.000000 pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/tables/implicit_rows.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     4188 2024-04-23 13:48:33.000000 pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/tables/semi_bordered.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     8246 2024-04-23 03:25:08.000000 pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/tables/table_creation.py
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.967619 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     3825 2024-04-23 09:21:26.000000 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/__init__.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     9296 2024-04-23 09:23:55.000000 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/columns.py
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.969075 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/layout/
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     2585 2024-04-23 09:25:54.000000 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/layout/__init__.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)    14402 2024-04-23 09:31:53.000000 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/layout/column_segments.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     1111 2024-04-23 09:31:20.000000 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/layout/image_elements.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)    10952 2024-04-23 09:31:37.000000 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/layout/rlsa.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)    10793 2024-04-23 13:10:06.000000 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/layout/table_segments.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     7885 2024-04-23 09:22:12.000000 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/model.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     7050 2024-04-23 09:22:38.000000 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/rows.py
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.969878 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/table/
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     1324 2024-04-23 09:24:29.000000 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/table/__init__.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     2091 2024-04-23 09:24:44.000000 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/table/coherency.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     1606 2024-04-23 09:25:11.000000 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/table/table_creation.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)    10291 2024-04-23 09:23:43.000000 pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/whitespaces.py
--rw-rw-r--   0 lirongzhi   (501) staff       (20)     7434 2024-04-23 03:23:45.000000 pdf2table-0.1.2/src/pdf2table/table/processing/common.py
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.970926 pdf2table-0.1.2/src/pdf2table/table/structure/
--rw-r--r--   0 lirongzhi   (501) staff       (20)      100 2024-04-23 02:35:43.000000 pdf2table-0.1.2/src/pdf2table/table/structure/__init__.py
--rw-r--r--   0 lirongzhi   (501) staff       (20)     2789 2024-04-23 02:42:20.000000 pdf2table-0.1.2/src/pdf2table/table/structure/models.py
--rw-r--r--   0 lirongzhi   (501) staff       (20)    10923 2024-04-23 05:33:21.000000 pdf2table-0.1.2/src/pdf2table/table/structure/table_object.py
--rw-r--r--   0 lirongzhi   (501) staff       (20)     5256 2024-04-23 15:53:59.000000 pdf2table-0.1.2/src/pdf2table/table/utils.py
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.971191 pdf2table-0.1.2/src/pdf2table/tatr/
--rw-r--r--   0 lirongzhi   (501) staff       (20)     6499 2024-04-24 09:51:14.000000 pdf2table-0.1.2/src/pdf2table/tatr/__init__.py
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.971807 pdf2table-0.1.2/src/pdf2table.egg-info/
--rw-r--r--   0 lirongzhi   (501) staff       (20)     2806 2024-04-24 15:55:26.000000 pdf2table-0.1.2/src/pdf2table.egg-info/PKG-INFO
--rw-r--r--   0 lirongzhi   (501) staff       (20)     2305 2024-04-24 15:55:26.000000 pdf2table-0.1.2/src/pdf2table.egg-info/SOURCES.txt
--rw-r--r--   0 lirongzhi   (501) staff       (20)        1 2024-04-24 15:55:26.000000 pdf2table-0.1.2/src/pdf2table.egg-info/dependency_links.txt
--rw-r--r--   0 lirongzhi   (501) staff       (20)      105 2024-04-24 15:55:26.000000 pdf2table-0.1.2/src/pdf2table.egg-info/requires.txt
--rw-r--r--   0 lirongzhi   (501) staff       (20)       10 2024-04-24 15:55:26.000000 pdf2table-0.1.2/src/pdf2table.egg-info/top_level.txt
-drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:55:26.971425 pdf2table-0.1.2/tests/
--rw-r--r--   0 lirongzhi   (501) staff       (20)     1183 2024-04-24 14:16:48.000000 pdf2table-0.1.2/tests/test_driver.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.532259 pdf2table-0.1.3/
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     1067 2024-04-22 17:13:14.000000 pdf2table-0.1.3/LICENSE
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     3146 2024-05-07 03:21:18.532177 pdf2table-0.1.3/PKG-INFO
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     2416 2024-05-07 03:11:54.000000 pdf2table-0.1.3/README.md
+-rw-r--r--   0 lirongzhi   (501) staff       (20)       89 2024-04-24 12:58:11.000000 pdf2table-0.1.3/pyproject.toml
+-rw-r--r--   0 lirongzhi   (501) staff       (20)      689 2024-05-07 03:21:18.532884 pdf2table-0.1.3/setup.cfg
+-rw-r--r--   0 lirongzhi   (501) staff       (20)      909 2024-05-07 03:21:06.000000 pdf2table-0.1.3/setup.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.511819 pdf2table-0.1.3/src/
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.517047 pdf2table-0.1.3/src/pdf2table/
+-rw-r--r--   0 lirongzhi   (501) staff       (20)       26 2024-04-24 07:05:41.000000 pdf2table-0.1.3/src/pdf2table/__init__.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.520226 pdf2table-0.1.3/src/pdf2table/document/
+-rw-r--r--   0 lirongzhi   (501) staff       (20)       68 2024-04-24 06:53:50.000000 pdf2table-0.1.3/src/pdf2table/document/__init__.py
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     4173 2024-04-23 15:47:40.000000 pdf2table-0.1.3/src/pdf2table/document/image.py
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     2493 2024-04-23 15:52:43.000000 pdf2table-0.1.3/src/pdf2table/document/page.py
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     5097 2024-04-24 14:19:02.000000 pdf2table-0.1.3/src/pdf2table/document/pdf.py
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     2922 2024-05-07 03:01:45.000000 pdf2table-0.1.3/src/pdf2table/driver.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.522441 pdf2table-0.1.3/src/pdf2table/table/
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     5521 2024-05-07 02:46:35.000000 pdf2table-0.1.3/src/pdf2table/table/__init__.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)    13363 2024-04-23 02:51:26.000000 pdf2table-0.1.3/src/pdf2table/table/metrics.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.522863 pdf2table-0.1.3/src/pdf2table/table/processing/
+-rw-r--r--   0 lirongzhi   (501) staff       (20)        0 2024-04-24 15:27:10.000000 pdf2table-0.1.3/src/pdf2table/table/processing/__init__.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.523317 pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/
+-rw-r--r--   0 lirongzhi   (501) staff       (20)        0 2024-04-23 02:56:13.000000 pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.524239 pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/cells/
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     1197 2024-04-23 08:38:52.000000 pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/cells/__init__.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     4767 2024-04-23 08:33:44.000000 pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/cells/deduplication.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     6421 2024-04-23 13:56:23.000000 pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/cells/identification.py
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     9420 2024-04-23 02:59:15.000000 pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/line.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.525984 pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/tables/
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     1611 2024-04-23 13:47:40.000000 pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/tables/__init__.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     3315 2024-04-23 09:33:15.000000 pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/tables/cell_clustering.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     6600 2024-04-23 03:23:59.000000 pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/tables/implicit_rows.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     4188 2024-04-23 13:48:33.000000 pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/tables/semi_bordered.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     8246 2024-04-23 03:25:08.000000 pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/tables/table_creation.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.527424 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     3825 2024-04-23 09:21:26.000000 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/__init__.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     9296 2024-04-23 09:23:55.000000 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/columns.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.528790 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/layout/
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     2585 2024-04-23 09:25:54.000000 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/layout/__init__.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)    14402 2024-04-23 09:31:53.000000 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/layout/column_segments.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     1111 2024-04-23 09:31:20.000000 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/layout/image_elements.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)    10952 2024-04-23 09:31:37.000000 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/layout/rlsa.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)    10793 2024-04-23 13:10:06.000000 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/layout/table_segments.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     7885 2024-04-23 09:22:12.000000 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/model.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     7050 2024-04-23 09:22:38.000000 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/rows.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.529692 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/table/
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     1324 2024-04-23 09:24:29.000000 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/table/__init__.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     2091 2024-04-23 09:24:44.000000 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/table/coherency.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     1606 2024-04-23 09:25:11.000000 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/table/table_creation.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)    10291 2024-04-23 09:23:43.000000 pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/whitespaces.py
+-rw-rw-r--   0 lirongzhi   (501) staff       (20)     7434 2024-04-23 03:23:45.000000 pdf2table-0.1.3/src/pdf2table/table/processing/common.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.530782 pdf2table-0.1.3/src/pdf2table/table/structure/
+-rw-r--r--   0 lirongzhi   (501) staff       (20)      100 2024-04-23 02:35:43.000000 pdf2table-0.1.3/src/pdf2table/table/structure/__init__.py
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     2789 2024-04-23 02:42:20.000000 pdf2table-0.1.3/src/pdf2table/table/structure/models.py
+-rw-r--r--   0 lirongzhi   (501) staff       (20)    10959 2024-05-07 02:47:18.000000 pdf2table-0.1.3/src/pdf2table/table/structure/table_object.py
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     5256 2024-04-23 15:53:59.000000 pdf2table-0.1.3/src/pdf2table/table/utils.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.531278 pdf2table-0.1.3/src/pdf2table/tatr/
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     6767 2024-05-07 03:15:26.000000 pdf2table-0.1.3/src/pdf2table/tatr/__init__.py
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.531883 pdf2table-0.1.3/src/pdf2table.egg-info/
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     3146 2024-05-07 03:21:18.000000 pdf2table-0.1.3/src/pdf2table.egg-info/PKG-INFO
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     2305 2024-05-07 03:21:18.000000 pdf2table-0.1.3/src/pdf2table.egg-info/SOURCES.txt
+-rw-r--r--   0 lirongzhi   (501) staff       (20)        1 2024-05-07 03:21:18.000000 pdf2table-0.1.3/src/pdf2table.egg-info/dependency_links.txt
+-rw-r--r--   0 lirongzhi   (501) staff       (20)      105 2024-05-07 03:21:18.000000 pdf2table-0.1.3/src/pdf2table.egg-info/requires.txt
+-rw-r--r--   0 lirongzhi   (501) staff       (20)       10 2024-05-07 03:21:18.000000 pdf2table-0.1.3/src/pdf2table.egg-info/top_level.txt
+drwxr-xr-x   0 lirongzhi   (501) staff       (20)        0 2024-05-07 03:21:18.531529 pdf2table-0.1.3/tests/
+-rw-r--r--   0 lirongzhi   (501) staff       (20)     1183 2024-04-24 14:16:48.000000 pdf2table-0.1.3/tests/test_driver.py
```

### Comparing `pdf2table-0.1.2/LICENSE` & `pdf2table-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/PKG-INFO` & `pdf2table-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf2table
-Version: 0.1.2
+Version: 0.1.3
 Summary: pdf2table is a powerful Python tool designed to streamline the extraction of tabular data from PDF documents.
 Home-page: https://github.com/li-rongzhi/pdf2table
 Author: rngzhi
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,17 @@
 Requires-Dist: torch
 Requires-Dist: transformers
 Requires-Dist: pandas
 Requires-Dist: pypdf
 Requires-Dist: poppler-utils
 
 # pdf2table
+[![PyPI](https://img.shields.io/pypi/v/pdf2table.svg)](https://pypi.org/project/pdf2table/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pdf2table)](https://img.shields.io/pypi/dm/pdf2table)
+![GitHub](https://img.shields.io/github/license/li-rongzhi/pdf2table.svg)
 
 pdf2table is a Python library designed to extract tabular data from PDF files and images efficiently and accurately. It leverages an enhanced algorithm of `img2table` library for table detection and the TATR model from Microsoft's Table Transformer for precise table structure recognition and content extraction.
 
 ## Features
 - **High Precision of Detection**: Compared to Table Transformer's DETR model, rule-based algorithm is less likely to identify text blocks as table regions.
 - **Maintenance Structural Information**: Utilizes state-of-the-art models for table structure recognition to maintain structural information of tables.
 - **Flexible Input**: Supports both PDF files and image formats for table extraction. (More file format will be available later)
@@ -64,13 +67,13 @@
 # which returns a list of Table objects
 img_tables = img.extract_tables()
 
 # Initialize an PDF object
 pdf = PDF("sample.jpg")
 pdf_tables = pdf.extract_tables()
 ```
-
+You may refer to [tutorial](samples/tutorial.ipynb) for more details
 ## License
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgements
 Thanks to the creators of the [img2table](https://github.com/xavctn/img2table) library and Microsoft's [Table Transformer](https://github.com/microsoft/table-transformer) model for providing the robust foundations for this tool.
```

### Comparing `pdf2table-0.1.2/README.md` & `pdf2table-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # pdf2table
+[![PyPI](https://img.shields.io/pypi/v/pdf2table.svg)](https://pypi.org/project/pdf2table/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pdf2table)](https://img.shields.io/pypi/dm/pdf2table)
+![GitHub](https://img.shields.io/github/license/li-rongzhi/pdf2table.svg)
 
 pdf2table is a Python library designed to extract tabular data from PDF files and images efficiently and accurately. It leverages an enhanced algorithm of `img2table` library for table detection and the TATR model from Microsoft's Table Transformer for precise table structure recognition and content extraction.
 
 ## Features
 - **High Precision of Detection**: Compared to Table Transformer's DETR model, rule-based algorithm is less likely to identify text blocks as table regions.
 - **Maintenance Structural Information**: Utilizes state-of-the-art models for table structure recognition to maintain structural information of tables.
 - **Flexible Input**: Supports both PDF files and image formats for table extraction. (More file format will be available later)
@@ -40,13 +43,13 @@
 # which returns a list of Table objects
 img_tables = img.extract_tables()
 
 # Initialize an PDF object
 pdf = PDF("sample.jpg")
 pdf_tables = pdf.extract_tables()
 ```
-
+You may refer to [tutorial](samples/tutorial.ipynb) for more details
 ## License
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgements
 Thanks to the creators of the [img2table](https://github.com/xavctn/img2table) library and Microsoft's [Table Transformer](https://github.com/microsoft/table-transformer) model for providing the robust foundations for this tool.
```

### Comparing `pdf2table-0.1.2/setup.cfg` & `pdf2table-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pdf2table
-version = 0.1.2
+version = 0.1.3
 author = rngzhi
 description = pdf2table is a powerful Python tool designed to streamline the extraction of tabular data from PDF documents.
 long_description = file: README.md, LICENSE
 long_description_content_type = 'text/markdown'
 url = https://github.com/li-rongzhi/pdf2table
 license = MIT
 classifiers =
```

### Comparing `pdf2table-0.1.2/setup.py` & `pdf2table-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pdf2table',
-    version='0.1.2',
+    version='0.1.3',
     author='rngzhi',
     description='pdf2table is a powerful Python tool designed to streamline the extraction of tabular data from PDF documents.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/li-rongzhi/pdf2table',
     license='MIT',
     classifiers=[
```

### Comparing `pdf2table-0.1.2/src/pdf2table/document/image.py` & `pdf2table-0.1.3/src/pdf2table/document/image.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/document/page.py` & `pdf2table-0.1.3/src/pdf2table/document/page.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/document/pdf.py` & `pdf2table-0.1.3/src/pdf2table/document/pdf.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/driver.py` & `pdf2table-0.1.3/src/pdf2table/driver.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,26 +28,27 @@
 
     def extract_tables(self, filepath, implicit_rows=False, borderless_tables=False, min_confidence=50):
         """Determine the file type and invoke the extract_tables method of the appropriate object."""
         filetype = self.check_file_type(filepath)
         if filetype == 'image':
             file_object = Image(path=filepath)
             table_images = file_object.extract_and_crop_tables(implicit_rows=implicit_rows, borderless_tables=borderless_tables, min_confidence=min_confidence)
-            tables = []
-            for tb in table_images:
-                tables.append(self.tatr.process_table_image([PILImage.fromarray(tb)]))
+            tables = self.tatr.get_tables(table_images)
+            # for tb in table_images:
+            #     tables.append(self.tatr.process_table_image([PILImage.fromarray(tb)]))
             return tables
         elif filetype == 'pdf':
             file_object = PDF(filepath)
             table_images = file_object.extract_and_crop_tables(implicit_rows=implicit_rows, borderless_tables=borderless_tables, min_confidence=min_confidence)
             tables = {}
             for page_num, value in table_images.items():
-                tables_in_page = []
-                for tb in value:
-                    tables_in_page.append(self.tatr.process_table_image([PILImage.fromarray(tb)]))
+                tables_in_page = self.tatr.get_tables(value)
+                # tables_in_page = []
+                # for tb in value:
+                #     tables_in_page.append(self.tatr.get_table_contents(PILImage.fromarray(tb)))
                 tables[page_num] = tables_in_page
             return tables
         else:
             raise ValueError("Unsupported file type")
 
     def detect_tables(self, filepath, implicit_rows=False, borderless_tables=False, min_confidence=50):
         filetype = self.check_file_type(filepath)
```

### Comparing `pdf2table-0.1.2/src/pdf2table/table/__init__.py` & `pdf2table-0.1.3/src/pdf2table/table/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import copy
 from functools import cached_property
 import cv2
 import numpy as np
 from dataclasses import dataclass, field
 from typing import List, Optional
 
+import pandas as pd
+
 from pdf2table.table.processing.bordered_tables.cells import get_cells
 from pdf2table.table.processing.bordered_tables.line import detect_lines
 from pdf2table.table.processing.bordered_tables.tables import get_tables
 from pdf2table.table.processing.bordered_tables.tables.implicit_rows import handle_implicit_rows
 from pdf2table.table.metrics import compute_img_metrics
 from pdf2table.table.processing.borderless_tables import identify_borderless_tables
 from pdf2table.table.structure.models import Line
+from pdf2table.table.structure.table_object import Table
 
 from .utils import threshold_dark_areas
 
 from .structure import TableObject
 # from .utils import preprocess_image, detect_lines, detect_tables
 
 @dataclass
@@ -23,15 +26,15 @@
     img_array: np.ndarray
     min_confidence: int = 50
     char_length: Optional[float] = None
     median_line_sep: Optional[float] = None
     thresh: Optional[np.ndarray] = None
     contours: List[any] = field(default_factory=list)
     lines: List[Line] = field(default_factory=list)
-    tables: List[TableObject] = field(default_factory=list)
+    tables: List[Table] = field(default_factory=list)
     grayscale_img: np.ndarray = field(init=False)
 
     def __post_init__(self):
         """Initialize the image processing."""
         self.convert_to_grayscale()
         self.char_length, self.median_line_sep, self.contours = compute_img_metrics(self.grayscale_img)
```

### Comparing `pdf2table-0.1.2/src/pdf2table/table/metrics.py` & `pdf2table-0.1.3/src/pdf2table/table/metrics.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/cells/__init__.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/cells/__init__.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/cells/deduplication.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/cells/deduplication.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/cells/identification.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/cells/identification.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/line.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/line.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/tables/__init__.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/tables/cell_clustering.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/tables/cell_clustering.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/tables/implicit_rows.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/tables/implicit_rows.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/tables/semi_bordered.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/tables/semi_bordered.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/bordered_tables/tables/table_creation.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/bordered_tables/tables/table_creation.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/__init__.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/columns.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/columns.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/layout/__init__.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/layout/column_segments.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/layout/column_segments.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/layout/image_elements.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/layout/image_elements.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/layout/rlsa.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/layout/rlsa.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/layout/table_segments.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/layout/table_segments.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/model.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/model.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/rows.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/rows.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/table/__init__.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/table/__init__.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/table/coherency.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/table/coherency.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/table/table_creation.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/table/table_creation.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/borderless_tables/whitespaces.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/borderless_tables/whitespaces.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/processing/common.py` & `pdf2table-0.1.3/src/pdf2table/table/processing/common.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/structure/models.py` & `pdf2table-0.1.3/src/pdf2table/table/structure/models.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/table/structure/table_object.py` & `pdf2table-0.1.3/src/pdf2table/table/structure/table_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from functools import cached_property
 from dataclasses import dataclass
 
 import numpy as np
+import pandas as pd
 from .models import TableCell, BBox
-from typing import Union, List
+from typing import Optional, OrderedDict, Union, List
 from dataclasses import dataclass, field
 import copy
 
 class TableObject:
     """A super class for all table related elements."""
     @cached_property
     def height(self) -> int:
@@ -145,29 +146,28 @@
                 assert self.items == other.items
                 return True
             except AssertionError:
                 return False
         return False
 
 
-# # coding: utf-8
-# import typing
-# from collections import OrderedDict
-# from typing import Union, List
-
-# import numpy as np
-
-# from img2table.tables.objects import TableObject
-# from img2table.tables.objects.cell import Cell
-# from img2table.tables.objects.extraction import ExtractedTable, BBox
-# from img2table.tables.objects.row import Row
-
-# if typing.TYPE_CHECKING:
-#     from img2table.ocr.data import OCRDataframe
+@dataclass
+class ExtractedTable:
+    bbox: BBox
+    title: Optional[str]
+    content: OrderedDict[int, List[TableCell]]
 
+    @property
+    def df(self) -> pd.DataFrame:
+        """
+        Create pandas DataFrame representation of the table
+        :return: pandas DataFrame containing table data
+        """
+        values = [[cell.value for cell in row] for k, row in self.content.items()]
+        return pd.DataFrame(values)
 
 class Table(TableObject):
     def __init__(self, rows: Union[Row, List[Row]], borderless: bool = False):
         if rows is None:
             self._items = []
         elif isinstance(rows, Row):
             self._items = [rows]
@@ -297,19 +297,19 @@
     #     # Check for uniqueness of content
     #     unique_cells = set([cell for row in self.items for cell in row.items])
     #     if len(unique_cells) == 1:
     #         self._items = [Row(cells=self.items[0].items[0])]
 
     #     return self
 
-    # @property
-    # def extracted_table(self) -> ExtractedTable:
-    #     bbox = BBox(x1=self.x1, x2=self.x2, y1=self.y1, y2=self.y2)
-    #     content = OrderedDict({idx: [cell.table_cell for cell in row.items] for idx, row in enumerate(self.items)})
-    #     return ExtractedTable(bbox=bbox, title=self.title, content=content)
+    @property
+    def extracted_table(self) -> ExtractedTable:
+        bbox = BBox(x1=self.x1, x2=self.x2, y1=self.y1, y2=self.y2)
+        content = OrderedDict({idx: [cell.table_cell for cell in row.items] for idx, row in enumerate(self.items)})
+        return ExtractedTable(bbox=bbox, title=self.title, content=content)
 
     def __eq__(self, other) -> bool:
         if isinstance(other, self.__class__):
             try:
                 assert self.items == other.items
                 if self.title is not None:
                     assert self.title == other.title
```

### Comparing `pdf2table-0.1.2/src/pdf2table/table/utils.py` & `pdf2table-0.1.3/src/pdf2table/table/utils.py`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/src/pdf2table/tatr/__init__.py` & `pdf2table-0.1.3/src/pdf2table/tatr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import torch
 from PIL import ImageDraw, Image
 import numpy as np
 import pandas as pd
 import csv
 from torchvision import transforms
+from PIL import Image as PILImage
 
 class MaxResize(object):
         def __init__(self, max_size=800):
             self.max_size = max_size
 
         def __call__(self, image):
             width, height = image.size
@@ -106,15 +107,15 @@
 
         # Sort rows from top to bottom
         cell_coordinates.sort(key=lambda x: x['row'][1])
 
         return cell_coordinates
 
 
-    def apply_ocr(self, cell_coordinates, cropped_table):
+    def apply_ocr(self, cell_coordinates, cropped_table, to_csv=False):
         data = dict()
         max_num_columns = 0
         for idx, row in enumerate(cell_coordinates):
             row_text = []
             for cell in row["cells"]:
                 # crop cell out of image
                 cell_image = np.array(cropped_table.crop(cell["cell"]))
@@ -139,29 +140,34 @@
 
         # write to csv
         with open('output.csv','w') as result_file:
             wr = csv.writer(result_file, dialect='excel')
             for row, row_text in data.items():
                 wr.writerow(row_text)
         # return as Pandas dataframe
-        try:
-            df = pd.read_csv('output.csv')
-        except pd.errors.EmptyDataError:
-            df = pd.DataFrame()  # Create an empty DataFrame
-            print("Warning: No data found in the CSV file")
+        if to_csv:
+            try:
+                df = pd.read_csv('output.csv')
+            except pd.errors.EmptyDataError:
+                df = pd.DataFrame()  # Create an empty DataFrame
+                print("Warning: No data found in the CSV file")
         # df = pd.read_csv('output.csv')
         return df, data
 
-    def process_table_image(self, images):
+    def process_table_images(self, images):
         # Adjusted implementation of process_pdf to work with table images
         # Multiple tables processing
         results = []
         for cropped_table in images:
-            image_processed, cells = self.recognize_table(cropped_table)
+            image_processed, cells = self.recognize_table(PILImage.fromarray(cropped_table))
             cell_coordinates = self.get_cell_coordinates_by_row(cells)
             df, data = self.apply_ocr(cell_coordinates, image_processed)
             results.append((image_processed, df, data))
         return results
 
+    def get_tables(self, images):
+        table_list = self.process_table_images(images)
+        return [pd.DataFrame(tb_tuple[2]) for tb_tuple in table_list]
+
     def clear_memory(self):
         # Clear memory if needed
         torch.cuda.empty_cache()
```

### Comparing `pdf2table-0.1.2/src/pdf2table.egg-info/PKG-INFO` & `pdf2table-0.1.3/src/pdf2table.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf2table
-Version: 0.1.2
+Version: 0.1.3
 Summary: pdf2table is a powerful Python tool designed to streamline the extraction of tabular data from PDF documents.
 Home-page: https://github.com/li-rongzhi/pdf2table
 Author: rngzhi
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,17 @@
 Requires-Dist: torch
 Requires-Dist: transformers
 Requires-Dist: pandas
 Requires-Dist: pypdf
 Requires-Dist: poppler-utils
 
 # pdf2table
+[![PyPI](https://img.shields.io/pypi/v/pdf2table.svg)](https://pypi.org/project/pdf2table/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pdf2table)](https://img.shields.io/pypi/dm/pdf2table)
+![GitHub](https://img.shields.io/github/license/li-rongzhi/pdf2table.svg)
 
 pdf2table is a Python library designed to extract tabular data from PDF files and images efficiently and accurately. It leverages an enhanced algorithm of `img2table` library for table detection and the TATR model from Microsoft's Table Transformer for precise table structure recognition and content extraction.
 
 ## Features
 - **High Precision of Detection**: Compared to Table Transformer's DETR model, rule-based algorithm is less likely to identify text blocks as table regions.
 - **Maintenance Structural Information**: Utilizes state-of-the-art models for table structure recognition to maintain structural information of tables.
 - **Flexible Input**: Supports both PDF files and image formats for table extraction. (More file format will be available later)
@@ -64,13 +67,13 @@
 # which returns a list of Table objects
 img_tables = img.extract_tables()
 
 # Initialize an PDF object
 pdf = PDF("sample.jpg")
 pdf_tables = pdf.extract_tables()
 ```
-
+You may refer to [tutorial](samples/tutorial.ipynb) for more details
 ## License
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgements
 Thanks to the creators of the [img2table](https://github.com/xavctn/img2table) library and Microsoft's [Table Transformer](https://github.com/microsoft/table-transformer) model for providing the robust foundations for this tool.
```

### Comparing `pdf2table-0.1.2/src/pdf2table.egg-info/SOURCES.txt` & `pdf2table-0.1.3/src/pdf2table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdf2table-0.1.2/tests/test_driver.py` & `pdf2table-0.1.3/tests/test_driver.py`

 * *Files identical despite different names*

