# Comparing `tmp/internetarchive-4.0.1.tar.gz` & `tmp/internetarchive-4.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetarchive-4.0.1.tar", last modified: Mon Apr 15 16:02:50 2024, max compression
+gzip compressed data, was "internetarchive-4.1.0.dev1.tar", last modified: Tue May  7 15:50:05 2024, max compression
```

## Comparing `internetarchive-4.0.1.tar` & `internetarchive-4.1.0.dev1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 jake       (501) staff       (20)        0 2024-04-15 16:02:50.059755 internetarchive-4.0.1/
--rw-r--r--   0 jake       (501) staff       (20)      427 2022-08-15 17:17:53.000000 internetarchive-4.0.1/AUTHORS.rst
--rw-r--r--   0 jake       (501) staff       (20)    33924 2024-04-15 16:00:28.000000 internetarchive-4.0.1/HISTORY.rst
--rw-r--r--   0 jake       (501) staff       (20)    34520 2021-12-09 01:11:21.000000 internetarchive-4.0.1/LICENSE
--rw-r--r--   0 jake       (501) staff       (20)       69 2021-12-09 01:11:21.000000 internetarchive-4.0.1/MANIFEST.in
--rw-r--r--   0 jake       (501) staff       (20)     4865 2024-04-15 16:02:50.059673 internetarchive-4.0.1/PKG-INFO
--rw-r--r--   0 jake       (501) staff       (20)     1777 2024-03-25 21:42:55.000000 internetarchive-4.0.1/README.rst
-drwxr-xr-x   0 jake       (501) staff       (20)        0 2024-04-15 16:02:50.048505 internetarchive-4.0.1/internetarchive/
--rw-r--r--   0 jake       (501) staff       (20)     2237 2022-06-15 19:17:01.000000 internetarchive-4.0.1/internetarchive/__init__.py
--rw-r--r--   0 jake       (501) staff       (20)       22 2024-04-12 19:54:31.000000 internetarchive-4.0.1/internetarchive/__version__.py
--rw-r--r--   0 jake       (501) staff       (20)    20034 2023-05-01 17:00:08.000000 internetarchive-4.0.1/internetarchive/api.py
--rw-r--r--   0 jake       (501) staff       (20)     2641 2022-05-09 19:53:33.000000 internetarchive-4.0.1/internetarchive/auth.py
--rw-r--r--   0 jake       (501) staff       (20)    11922 2022-05-25 17:26:41.000000 internetarchive-4.0.1/internetarchive/catalog.py
-drwxr-xr-x   0 jake       (501) staff       (20)        0 2024-04-15 16:02:50.052807 internetarchive-4.0.1/internetarchive/cli/
--rw-r--r--   0 jake       (501) staff       (20)     1297 2022-05-25 17:26:41.000000 internetarchive-4.0.1/internetarchive/cli/__init__.py
--rw-r--r--   0 jake       (501) staff       (20)     2528 2022-05-25 17:26:41.000000 internetarchive-4.0.1/internetarchive/cli/argparser.py
--rwxr-xr-x   0 jake       (501) staff       (20)     6139 2024-03-25 21:42:55.000000 internetarchive-4.0.1/internetarchive/cli/ia.py
--rw-r--r--   0 jake       (501) staff       (20)     4133 2024-01-25 16:46:02.000000 internetarchive-4.0.1/internetarchive/cli/ia_configure.py
--rw-r--r--   0 jake       (501) staff       (20)     6307 2022-05-25 17:26:41.000000 internetarchive-4.0.1/internetarchive/cli/ia_copy.py
--rw-r--r--   0 jake       (501) staff       (20)     5652 2022-05-25 17:26:41.000000 internetarchive-4.0.1/internetarchive/cli/ia_delete.py
--rw-r--r--   0 jake       (501) staff       (20)     9850 2023-04-05 19:41:25.000000 internetarchive-4.0.1/internetarchive/cli/ia_download.py
--rw-r--r--   0 jake       (501) staff       (20)     3002 2022-05-25 17:26:41.000000 internetarchive-4.0.1/internetarchive/cli/ia_list.py
--rw-r--r--   0 jake       (501) staff       (20)    13180 2024-03-25 21:42:55.000000 internetarchive-4.0.1/internetarchive/cli/ia_metadata.py
--rw-r--r--   0 jake       (501) staff       (20)     3225 2022-05-25 17:26:41.000000 internetarchive-4.0.1/internetarchive/cli/ia_move.py
--rw-r--r--   0 jake       (501) staff       (20)     3428 2024-03-25 21:42:55.000000 internetarchive-4.0.1/internetarchive/cli/ia_reviews.py
--rw-r--r--   0 jake       (501) staff       (20)     4859 2023-04-04 17:42:58.000000 internetarchive-4.0.1/internetarchive/cli/ia_search.py
--rw-r--r--   0 jake       (501) staff       (20)     6838 2023-04-04 17:42:58.000000 internetarchive-4.0.1/internetarchive/cli/ia_tasks.py
--rw-r--r--   0 jake       (501) staff       (20)    14533 2024-04-11 22:25:15.000000 internetarchive-4.0.1/internetarchive/cli/ia_upload.py
--rw-r--r--   0 jake       (501) staff       (20)        0 2022-05-25 17:26:41.000000 internetarchive-4.0.1/internetarchive/cli/py.typed
--rw-r--r--   0 jake       (501) staff       (20)     6727 2023-05-01 17:00:08.000000 internetarchive-4.0.1/internetarchive/config.py
--rw-r--r--   0 jake       (501) staff       (20)     1586 2024-04-12 17:22:00.000000 internetarchive-4.0.1/internetarchive/exceptions.py
--rw-r--r--   0 jake       (501) staff       (20)    18203 2024-04-12 19:53:45.000000 internetarchive-4.0.1/internetarchive/files.py
--rw-r--r--   0 jake       (501) staff       (20)    21055 2024-03-25 21:42:55.000000 internetarchive-4.0.1/internetarchive/iarequest.py
--rw-r--r--   0 jake       (501) staff       (20)    53850 2024-03-25 21:43:54.000000 internetarchive-4.0.1/internetarchive/item.py
--rw-r--r--   0 jake       (501) staff       (20)        0 2022-05-25 17:26:41.000000 internetarchive-4.0.1/internetarchive/py.typed
--rw-r--r--   0 jake       (501) staff       (20)     9958 2024-03-25 21:42:55.000000 internetarchive-4.0.1/internetarchive/search.py
--rw-r--r--   0 jake       (501) staff       (20)    22967 2024-02-02 21:31:14.000000 internetarchive-4.0.1/internetarchive/session.py
--rw-r--r--   0 jake       (501) staff       (20)    14322 2024-03-25 21:42:55.000000 internetarchive-4.0.1/internetarchive/utils.py
-drwxr-xr-x   0 jake       (501) staff       (20)        0 2024-04-15 16:02:50.057049 internetarchive-4.0.1/internetarchive.egg-info/
--rw-r--r--   0 jake       (501) staff       (20)     4865 2024-04-15 16:02:50.000000 internetarchive-4.0.1/internetarchive.egg-info/PKG-INFO
--rw-r--r--   0 jake       (501) staff       (20)     1591 2024-04-15 16:02:50.000000 internetarchive-4.0.1/internetarchive.egg-info/SOURCES.txt
--rw-r--r--   0 jake       (501) staff       (20)        1 2024-04-15 16:02:50.000000 internetarchive-4.0.1/internetarchive.egg-info/dependency_links.txt
--rw-r--r--   0 jake       (501) staff       (20)       51 2024-04-15 16:02:50.000000 internetarchive-4.0.1/internetarchive.egg-info/entry_points.txt
--rw-r--r--   0 jake       (501) staff       (20)        1 2021-12-09 02:36:16.000000 internetarchive-4.0.1/internetarchive.egg-info/not-zip-safe
--rw-r--r--   0 jake       (501) staff       (20)      839 2024-04-15 16:02:50.000000 internetarchive-4.0.1/internetarchive.egg-info/requires.txt
--rw-r--r--   0 jake       (501) staff       (20)       16 2024-04-15 16:02:50.000000 internetarchive-4.0.1/internetarchive.egg-info/top_level.txt
--rw-r--r--   0 jake       (501) staff       (20)     1916 2024-03-25 21:19:38.000000 internetarchive-4.0.1/pyproject.toml
--rw-r--r--   0 jake       (501) staff       (20)     2033 2024-04-15 16:02:50.060117 internetarchive-4.0.1/setup.cfg
--rw-r--r--   0 jake       (501) staff       (20)       38 2022-05-25 17:26:41.000000 internetarchive-4.0.1/setup.py
-drwxr-xr-x   0 jake       (501) staff       (20)        0 2024-04-15 16:02:50.055079 internetarchive-4.0.1/tests/
--rw-r--r--   0 jake       (501) staff       (20)        0 2021-12-09 01:11:21.000000 internetarchive-4.0.1/tests/__init__.py
-drwxr-xr-x   0 jake       (501) staff       (20)        0 2024-04-15 16:02:50.056739 internetarchive-4.0.1/tests/cli/
--rw-r--r--   0 jake       (501) staff       (20)     1047 2022-05-24 22:31:00.000000 internetarchive-4.0.1/tests/cli/test_argparser.py
--rw-r--r--   0 jake       (501) staff       (20)      541 2021-12-09 01:11:21.000000 internetarchive-4.0.1/tests/cli/test_ia.py
--rw-r--r--   0 jake       (501) staff       (20)     3972 2022-12-05 19:47:24.000000 internetarchive-4.0.1/tests/cli/test_ia_download.py
--rw-r--r--   0 jake       (501) staff       (20)     2759 2022-02-03 22:48:23.000000 internetarchive-4.0.1/tests/cli/test_ia_list.py
--rw-r--r--   0 jake       (501) staff       (20)     1563 2022-03-07 19:43:12.000000 internetarchive-4.0.1/tests/cli/test_ia_metadata.py
--rw-r--r--   0 jake       (501) staff       (20)     1490 2023-01-30 18:36:38.000000 internetarchive-4.0.1/tests/cli/test_ia_search.py
--rw-r--r--   0 jake       (501) staff       (20)    15221 2024-03-25 21:42:55.000000 internetarchive-4.0.1/tests/cli/test_ia_upload.py
--rw-r--r--   0 jake       (501) staff       (20)     3489 2024-03-25 21:19:38.000000 internetarchive-4.0.1/tests/conftest.py
--rw-r--r--   0 jake       (501) staff       (20)    14514 2024-04-03 17:27:47.000000 internetarchive-4.0.1/tests/test_api.py
--rw-r--r--   0 jake       (501) staff       (20)      418 2021-12-09 01:11:21.000000 internetarchive-4.0.1/tests/test_bad_data.py
--rw-r--r--   0 jake       (501) staff       (20)    14898 2022-04-26 18:19:02.000000 internetarchive-4.0.1/tests/test_config.py
--rw-r--r--   0 jake       (501) staff       (20)      243 2022-02-03 22:48:23.000000 internetarchive-4.0.1/tests/test_exceptions.py
--rw-r--r--   0 jake       (501) staff       (20)    29248 2024-04-12 17:22:00.000000 internetarchive-4.0.1/tests/test_item.py
--rw-r--r--   0 jake       (501) staff       (20)     4477 2022-05-06 00:42:03.000000 internetarchive-4.0.1/tests/test_session.py
--rw-r--r--   0 jake       (501) staff       (20)     3493 2022-05-06 00:42:03.000000 internetarchive-4.0.1/tests/test_utils.py
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2024-05-07 15:50:05.883959 internetarchive-4.1.0.dev1/
+-rw-r--r--   0 jake       (501) staff       (20)      427 2022-08-15 17:17:53.000000 internetarchive-4.1.0.dev1/AUTHORS.rst
+-rw-r--r--   0 jake       (501) staff       (20)    34063 2024-05-07 15:48:57.000000 internetarchive-4.1.0.dev1/HISTORY.rst
+-rw-r--r--   0 jake       (501) staff       (20)    34520 2021-12-09 01:11:21.000000 internetarchive-4.1.0.dev1/LICENSE
+-rw-r--r--   0 jake       (501) staff       (20)       69 2021-12-09 01:11:21.000000 internetarchive-4.1.0.dev1/MANIFEST.in
+-rw-r--r--   0 jake       (501) staff       (20)     4870 2024-05-07 15:50:05.883890 internetarchive-4.1.0.dev1/PKG-INFO
+-rw-r--r--   0 jake       (501) staff       (20)     1777 2024-03-25 21:42:55.000000 internetarchive-4.1.0.dev1/README.rst
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2024-05-07 15:50:05.872629 internetarchive-4.1.0.dev1/internetarchive/
+-rw-r--r--   0 jake       (501) staff       (20)     2237 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/__init__.py
+-rw-r--r--   0 jake       (501) staff       (20)       27 2024-05-07 15:26:45.000000 internetarchive-4.1.0.dev1/internetarchive/__version__.py
+-rw-r--r--   0 jake       (501) staff       (20)    20056 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/api.py
+-rw-r--r--   0 jake       (501) staff       (20)     2641 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/auth.py
+-rw-r--r--   0 jake       (501) staff       (20)    11922 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/catalog.py
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2024-05-07 15:50:05.877309 internetarchive-4.1.0.dev1/internetarchive/cli/
+-rw-r--r--   0 jake       (501) staff       (20)     1297 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/__init__.py
+-rw-r--r--   0 jake       (501) staff       (20)     2528 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/argparser.py
+-rwxr-xr-x   0 jake       (501) staff       (20)     6139 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/ia.py
+-rw-r--r--   0 jake       (501) staff       (20)     4133 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/ia_configure.py
+-rw-r--r--   0 jake       (501) staff       (20)     6307 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/ia_copy.py
+-rw-r--r--   0 jake       (501) staff       (20)     5652 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/ia_delete.py
+-rw-r--r--   0 jake       (501) staff       (20)     9850 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/ia_download.py
+-rw-r--r--   0 jake       (501) staff       (20)     3002 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/ia_list.py
+-rw-r--r--   0 jake       (501) staff       (20)    13195 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/ia_metadata.py
+-rw-r--r--   0 jake       (501) staff       (20)     3225 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/ia_move.py
+-rw-r--r--   0 jake       (501) staff       (20)     3428 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/ia_reviews.py
+-rw-r--r--   0 jake       (501) staff       (20)     4859 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/ia_search.py
+-rw-r--r--   0 jake       (501) staff       (20)     6838 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/ia_tasks.py
+-rw-r--r--   0 jake       (501) staff       (20)    14533 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/cli/ia_upload.py
+-rw-r--r--   0 jake       (501) staff       (20)        0 2022-05-25 17:26:41.000000 internetarchive-4.1.0.dev1/internetarchive/cli/py.typed
+-rw-r--r--   0 jake       (501) staff       (20)     6727 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/config.py
+-rw-r--r--   0 jake       (501) staff       (20)     1586 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/exceptions.py
+-rw-r--r--   0 jake       (501) staff       (20)    18212 2024-05-07 15:26:26.000000 internetarchive-4.1.0.dev1/internetarchive/files.py
+-rw-r--r--   0 jake       (501) staff       (20)    21055 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/iarequest.py
+-rw-r--r--   0 jake       (501) staff       (20)    53990 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/item.py
+-rw-r--r--   0 jake       (501) staff       (20)        0 2022-05-25 17:26:41.000000 internetarchive-4.1.0.dev1/internetarchive/py.typed
+-rw-r--r--   0 jake       (501) staff       (20)     9958 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/search.py
+-rw-r--r--   0 jake       (501) staff       (20)    22967 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/session.py
+-rw-r--r--   0 jake       (501) staff       (20)    14322 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/internetarchive/utils.py
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2024-05-07 15:50:05.881321 internetarchive-4.1.0.dev1/internetarchive.egg-info/
+-rw-r--r--   0 jake       (501) staff       (20)     4870 2024-05-07 15:50:05.000000 internetarchive-4.1.0.dev1/internetarchive.egg-info/PKG-INFO
+-rw-r--r--   0 jake       (501) staff       (20)     1591 2024-05-07 15:50:05.000000 internetarchive-4.1.0.dev1/internetarchive.egg-info/SOURCES.txt
+-rw-r--r--   0 jake       (501) staff       (20)        1 2024-05-07 15:50:05.000000 internetarchive-4.1.0.dev1/internetarchive.egg-info/dependency_links.txt
+-rw-r--r--   0 jake       (501) staff       (20)       51 2024-05-07 15:50:05.000000 internetarchive-4.1.0.dev1/internetarchive.egg-info/entry_points.txt
+-rw-r--r--   0 jake       (501) staff       (20)        1 2021-12-09 02:36:16.000000 internetarchive-4.1.0.dev1/internetarchive.egg-info/not-zip-safe
+-rw-r--r--   0 jake       (501) staff       (20)      839 2024-05-07 15:50:05.000000 internetarchive-4.1.0.dev1/internetarchive.egg-info/requires.txt
+-rw-r--r--   0 jake       (501) staff       (20)       16 2024-05-07 15:50:05.000000 internetarchive-4.1.0.dev1/internetarchive.egg-info/top_level.txt
+-rw-r--r--   0 jake       (501) staff       (20)     1916 2024-03-25 21:19:38.000000 internetarchive-4.1.0.dev1/pyproject.toml
+-rw-r--r--   0 jake       (501) staff       (20)     2033 2024-05-07 15:50:05.884324 internetarchive-4.1.0.dev1/setup.cfg
+-rw-r--r--   0 jake       (501) staff       (20)       38 2022-05-25 17:26:41.000000 internetarchive-4.1.0.dev1/setup.py
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2024-05-07 15:50:05.879527 internetarchive-4.1.0.dev1/tests/
+-rw-r--r--   0 jake       (501) staff       (20)        0 2021-12-09 01:11:21.000000 internetarchive-4.1.0.dev1/tests/__init__.py
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2024-05-07 15:50:05.881003 internetarchive-4.1.0.dev1/tests/cli/
+-rw-r--r--   0 jake       (501) staff       (20)     1047 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/tests/cli/test_argparser.py
+-rw-r--r--   0 jake       (501) staff       (20)      541 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/tests/cli/test_ia.py
+-rw-r--r--   0 jake       (501) staff       (20)     3972 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/tests/cli/test_ia_download.py
+-rw-r--r--   0 jake       (501) staff       (20)     2759 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/tests/cli/test_ia_list.py
+-rw-r--r--   0 jake       (501) staff       (20)     1546 2024-05-02 22:12:00.000000 internetarchive-4.1.0.dev1/tests/cli/test_ia_metadata.py
+-rw-r--r--   0 jake       (501) staff       (20)     1490 2024-05-01 22:04:40.000000 internetarchive-4.1.0.dev1/tests/cli/test_ia_search.py
+-rw-r--r--   0 jake       (501) staff       (20)    15221 2024-05-06 23:46:38.000000 internetarchive-4.1.0.dev1/tests/cli/test_ia_upload.py
+-rw-r--r--   0 jake       (501) staff       (20)     3489 2024-05-01 18:39:26.000000 internetarchive-4.1.0.dev1/tests/conftest.py
+-rw-r--r--   0 jake       (501) staff       (20)    14514 2024-04-25 18:11:41.000000 internetarchive-4.1.0.dev1/tests/test_api.py
+-rw-r--r--   0 jake       (501) staff       (20)      418 2021-12-09 01:11:21.000000 internetarchive-4.1.0.dev1/tests/test_bad_data.py
+-rw-r--r--   0 jake       (501) staff       (20)    14898 2022-04-26 18:19:02.000000 internetarchive-4.1.0.dev1/tests/test_config.py
+-rw-r--r--   0 jake       (501) staff       (20)      243 2022-02-03 22:48:23.000000 internetarchive-4.1.0.dev1/tests/test_exceptions.py
+-rw-r--r--   0 jake       (501) staff       (20)    29248 2024-04-25 18:11:57.000000 internetarchive-4.1.0.dev1/tests/test_item.py
+-rw-r--r--   0 jake       (501) staff       (20)     4477 2022-05-06 00:42:03.000000 internetarchive-4.1.0.dev1/tests/test_session.py
+-rw-r--r--   0 jake       (501) staff       (20)     3493 2022-05-06 00:42:03.000000 internetarchive-4.1.0.dev1/tests/test_utils.py
```

### Comparing `internetarchive-4.0.1/HISTORY.rst` & `internetarchive-4.1.0.dev1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 .. :changelog:
 
 Release History
 ---------------
 
+4.1.0 (2024-05-07)
+++++++++++++++++++
+
+**Bugfixes**
+
+- Use mtime from files.xml if no Last-Modified header is available (e.g. VTT files).
+
 4.0.1 (2024-04-15)
 ++++++++++++++++++
 
 **Features and Improvements**
 
 - Partially downloaded files will now automatically resume where they left off when retried.
 - Use ``Last-Modified`` header to set all mtimes (this includes files.xml now).
```

### Comparing `internetarchive-4.0.1/LICENSE` & `internetarchive-4.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/PKG-INFO` & `internetarchive-4.1.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetarchive
-Version: 4.0.1
+Version: 4.1.0.dev1
 Summary: A Python interface to archive.org.
 Home-page: https://github.com/jjjake/internetarchive
 Author: Jacob M. Johnson
 Author-email: jake@archive.org
 License: AGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `internetarchive-4.0.1/README.rst` & `internetarchive-4.1.0.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/__init__.py` & `internetarchive-4.1.0.dev1/internetarchive/__init__.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/api.py` & `internetarchive-4.1.0.dev1/internetarchive/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,14 +205,15 @@
         append=append,
         append_list=append_list,
         priority=priority,
         access_key=access_key,
         secret_key=secret_key,
         debug=debug,
         request_kwargs=request_kwargs,
+        refresh=False
     )
 
 
 def upload(
     identifier: str,
     files,
     metadata: Mapping | None = None,
```

### Comparing `internetarchive-4.0.1/internetarchive/auth.py` & `internetarchive-4.1.0.dev1/internetarchive/auth.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/catalog.py` & `internetarchive-4.1.0.dev1/internetarchive/catalog.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/cli/__init__.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/cli/argparser.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/argparser.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/cli/ia.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/ia.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/cli/ia_configure.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/ia_configure.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/cli/ia_copy.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/ia_copy.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/cli/ia_delete.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/ia_delete.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/cli/ia_download.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/ia_download.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/cli/ia_list.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/ia_list.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/cli/ia_metadata.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/ia_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     expect = get_args_dict(args['--expect'])
     append_list = bool(args['--append-list'])
     insert = bool(args['--insert'])
     try:
         r = item.modify_metadata(metadata, target=args['--target'], append=append,
                                  expect=expect, priority=args['--priority'],
                                  append_list=append_list, headers=args['--header'],
-                                 insert=insert, timeout=args['--timeout'])
+                                 insert=insert, timeout=args['--timeout'], refresh=False)
         assert isinstance(r, Response)  # mypy: modify_metadata() -> Request | Response
     except ItemLocateError as exc:
         print(f'{item.identifier} - error: {exc}', file=sys.stderr)
         sys.exit(1)
     if not r.json()['success']:
         error_msg = r.json()['error']
         etype = 'warning' if 'no changes' in r.text else 'error'
```

### Comparing `internetarchive-4.0.1/internetarchive/cli/ia_move.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/ia_move.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/cli/ia_reviews.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/ia_reviews.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/cli/ia_search.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/ia_search.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/cli/ia_tasks.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/ia_tasks.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/cli/ia_upload.py` & `internetarchive-4.1.0.dev1/internetarchive/cli/ia_upload.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/config.py` & `internetarchive-4.1.0.dev1/internetarchive/config.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/exceptions.py` & `internetarchive-4.1.0.dev1/internetarchive/exceptions.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/files.py` & `internetarchive-4.1.0.dev1/internetarchive/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
                                                  headers=headers)
                 # Get timestamp from Last-Modified header
                 last_mod_header = response.headers.get('Last-Modified')
                 if last_mod_header:
                     dt = parsedate_to_datetime(last_mod_header)
                     last_mod_mtime = dt.timestamp()
                 else:
-                    last_mod_mtime = 0
+                    last_mod_mtime = self.mtime
 
                 response.raise_for_status()
 
                 # Check if we should skip...
                 if not return_responses and os.path.exists(file_path.encode('utf-8')):
                     if ignore_existing:
                         msg = f'skipping {file_path}, file already exists.'
```

### Comparing `internetarchive-4.0.1/internetarchive/iarequest.py` & `internetarchive-4.1.0.dev1/internetarchive/iarequest.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/item.py` & `internetarchive-4.1.0.dev1/internetarchive/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -775,15 +775,16 @@
                         insert: bool = False,
                         priority: int = 0,
                         access_key: str | None = None,
                         secret_key: str | None = None,
                         debug: bool = False,
                         headers: Mapping | None = None,
                         request_kwargs: Mapping | None = None,
-                        timeout: int | float | None = None) -> Request | Response:
+                        timeout: int | float | None = None,
+                        refresh: bool = True) -> Request | Response:
         """Modify the metadata of an existing item on Archive.org.
 
         Note: The Metadata Write API does not yet comply with the
         latest Json-Patch standard. It currently complies with `version 02
         <https://tools.ietf.org/html/draft-ietf-appsawg-json-patch-02>`__.
 
         :param metadata: Metadata used to update the item.
@@ -797,14 +798,16 @@
 
         :param expect: Provide a dict of expectations to be tested
                        server-side before applying patch to item metadata.
 
         :param append_list: Append values to an existing multi-value
                             metadata field. No duplicate values will be added.
 
+        :param refresh: Refresh the item metadata after the request.
+
         :returns: A Request if debug else a Response.
 
         Usage::
 
             >>> import internetarchive
             >>> item = internetarchive.Item('mapi_test_item1')
             >>> md = {'new_key': 'new_value', 'foo': ['bar', 'bar2']}
@@ -846,15 +849,16 @@
         # Must use Session.prepare_request to make sure session settings
         # are used on request!
         prepared_request = request.prepare()
         if debug:
             return prepared_request
         resp = self.session.send(prepared_request, **request_kwargs)
         # Re-initialize the Item object with the updated metadata.
-        self.refresh()
+        if refresh:
+            self.refresh()
         return resp
 
     # TODO: `list` parameter name shadows the Python builtin
     def remove_from_simplelist(self, parent, list) -> Response:
         """Remove item from a simplelist.
 
         :returns: :class:`requests.Response`
```

### Comparing `internetarchive-4.0.1/internetarchive/search.py` & `internetarchive-4.1.0.dev1/internetarchive/search.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/session.py` & `internetarchive-4.1.0.dev1/internetarchive/session.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive/utils.py` & `internetarchive-4.1.0.dev1/internetarchive/utils.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive.egg-info/PKG-INFO` & `internetarchive-4.1.0.dev1/internetarchive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetarchive
-Version: 4.0.1
+Version: 4.1.0.dev1
 Summary: A Python interface to archive.org.
 Home-page: https://github.com/jjjake/internetarchive
 Author: Jacob M. Johnson
 Author-email: jake@archive.org
 License: AGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `internetarchive-4.0.1/internetarchive.egg-info/SOURCES.txt` & `internetarchive-4.1.0.dev1/internetarchive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/internetarchive.egg-info/requires.txt` & `internetarchive-4.1.0.dev1/internetarchive.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/pyproject.toml` & `internetarchive-4.1.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/setup.cfg` & `internetarchive-4.1.0.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/tests/cli/test_argparser.py` & `internetarchive-4.1.0.dev1/tests/cli/test_argparser.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/tests/cli/test_ia.py` & `internetarchive-4.1.0.dev1/tests/cli/test_ia.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/tests/cli/test_ia_download.py` & `internetarchive-4.1.0.dev1/tests/cli/test_ia_download.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/tests/cli/test_ia_list.py` & `internetarchive-4.1.0.dev1/tests/cli/test_ia_list.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/tests/cli/test_ia_metadata.py` & `internetarchive-4.1.0.dev1/tests/cli/test_ia_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,13 @@
     assert set(out.split('\n')) == expected_formats
 
 
 def test_ia_metadata_modify(capsys):
     md_rsp = ('{"success":true,"task_id":447613301,'
               '"log":"https://catalogd.archive.org/log/447613301"}')
     with IaRequestsMock() as rsps:
-        rsps.add_metadata_mock('nasa')
+        rsps.add_metadata_mock('nasa', method=responses.GET)
         rsps.add_metadata_mock('nasa', body=md_rsp, method=responses.POST)
-        rsps.add_metadata_mock('nasa')
         valid_key = f'foo-{int(time())}'
         ia_call(['ia', 'metadata', '--modify', f'{valid_key}:test_value', 'nasa'])
         out, err = capsys.readouterr()
         assert err == 'nasa - success: https://catalogd.archive.org/log/447613301\n'
```

### Comparing `internetarchive-4.0.1/tests/cli/test_ia_search.py` & `internetarchive-4.1.0.dev1/tests/cli/test_ia_search.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/tests/cli/test_ia_upload.py` & `internetarchive-4.1.0.dev1/tests/cli/test_ia_upload.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/tests/conftest.py` & `internetarchive-4.1.0.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/tests/test_api.py` & `internetarchive-4.1.0.dev1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/tests/test_config.py` & `internetarchive-4.1.0.dev1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/tests/test_item.py` & `internetarchive-4.1.0.dev1/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/tests/test_session.py` & `internetarchive-4.1.0.dev1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `internetarchive-4.0.1/tests/test_utils.py` & `internetarchive-4.1.0.dev1/tests/test_utils.py`

 * *Files identical despite different names*

