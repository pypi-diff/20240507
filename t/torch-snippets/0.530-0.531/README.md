# Comparing `tmp/torch_snippets-0.530.tar.gz` & `tmp/torch_snippets-0.531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_snippets-0.530.tar", last modified: Sun May  5 12:48:50 2024, max compression
+gzip compressed data, was "torch_snippets-0.531.tar", last modified: Tue May  7 08:15:31 2024, max compression
```

## Comparing `torch_snippets-0.530.tar` & `torch_snippets-0.531.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-05 12:48:50.756183 torch_snippets-0.530/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.530/LICENSE
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1062 2023-01-17 16:58:23.000000 torch_snippets-0.530/LICENSE.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.530/MANIFEST.in
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5711 2024-05-05 12:48:50.756642 torch_snippets-0.530/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4999 2023-01-17 16:58:23.000000 torch_snippets-0.530/README.md
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      871 2024-04-25 12:13:34.000000 torch_snippets-0.530/settings.ini
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2024-05-05 12:48:50.758336 torch_snippets-0.530/setup.cfg
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2024-01-08 09:24:32.000000 torch_snippets-0.530/setup.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-05 12:48:50.740661 torch_snippets-0.530/torch_snippets/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      401 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    57057 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/_modidx.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4482 2023-01-17 16:58:25.000000 torch_snippets-0.530/torch_snippets/_nbdev.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8846 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/adapters.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    17079 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/bb_utils.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2026 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/bokeh_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    19042 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/charts.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1866 2023-12-28 06:40:32.000000 torch_snippets-0.530/torch_snippets/dates.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2056 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/decorators.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.530/torch_snippets/fastcores.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11427 2023-11-28 11:52:35.000000 torch_snippets-0.530/torch_snippets/icecream.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8479 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/imgaug_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3429 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/inspector.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8386 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/interactive_show.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5727 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/ipython.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      597 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/load_defaults.py
--rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    23434 2024-05-05 12:47:54.000000 torch_snippets-0.530/torch_snippets/loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8480 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/logger.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14432 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/markup.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    17441 2024-05-05 12:47:53.000000 torch_snippets-0.530/torch_snippets/markup2.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2054 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/misc.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11039 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/paths.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1465 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/pdf_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      822 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/registry.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3234 2024-05-05 12:47:53.000000 torch_snippets-0.530/torch_snippets/scp.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/sklegos.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14202 2024-03-28 08:34:42.000000 torch_snippets-0.530/torch_snippets/text_utils.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-05 12:48:50.750918 torch_snippets-0.530/torch_snippets/thinc_parser/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/thinc_parser/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.530/torch_snippets/thinc_parser/parser.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    31250 2024-02-29 09:58:55.000000 torch_snippets-0.530/torch_snippets/torch_loader.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-05 12:48:50.754964 torch_snippets-0.530/torch_snippets/trainer/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/trainer/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6882 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/trainer/capsule.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2432 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/trainer/config.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5801 2024-04-24 06:16:19.000000 torch_snippets-0.530/torch_snippets/trainer/hooks.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2137 2024-02-14 10:01:57.000000 torch_snippets-0.530/torch_snippets/video.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-05 12:48:50.749344 torch_snippets-0.530/torch_snippets.egg-info/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5711 2024-05-05 12:48:50.000000 torch_snippets-0.530/torch_snippets.egg-info/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1337 2024-05-05 12:48:50.000000 torch_snippets-0.530/torch_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2024-05-05 12:48:50.000000 torch_snippets-0.530/torch_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       20 2024-05-05 12:48:50.000000 torch_snippets-0.530/torch_snippets.egg-info/entry_points.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-01-17 16:58:23.000000 torch_snippets-0.530/torch_snippets.egg-info/not-zip-safe
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      281 2024-05-05 12:48:50.000000 torch_snippets-0.530/torch_snippets.egg-info/requires.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2024-05-05 12:48:50.000000 torch_snippets-0.530/torch_snippets.egg-info/top_level.txt
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-07 08:15:31.334568 torch_snippets-0.531/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.531/LICENSE
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1062 2023-01-17 16:58:23.000000 torch_snippets-0.531/LICENSE.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.531/MANIFEST.in
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5711 2024-05-07 08:15:31.334918 torch_snippets-0.531/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4999 2023-01-17 16:58:23.000000 torch_snippets-0.531/README.md
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      871 2024-05-07 08:12:44.000000 torch_snippets-0.531/settings.ini
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2024-05-07 08:15:31.337021 torch_snippets-0.531/setup.cfg
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2024-01-08 09:24:32.000000 torch_snippets-0.531/setup.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-07 08:15:31.319326 torch_snippets-0.531/torch_snippets/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      401 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    57057 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/_modidx.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4482 2023-01-17 16:58:25.000000 torch_snippets-0.531/torch_snippets/_nbdev.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8846 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/adapters.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    17079 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/bb_utils.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2026 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/bokeh_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    19042 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/charts.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1866 2023-12-28 06:40:32.000000 torch_snippets-0.531/torch_snippets/dates.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2056 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/decorators.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.531/torch_snippets/fastcores.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11427 2023-11-28 11:52:35.000000 torch_snippets-0.531/torch_snippets/icecream.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8479 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/imgaug_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3429 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/inspector.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8386 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/interactive_show.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5727 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/ipython.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      597 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/load_defaults.py
+-rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    23434 2024-05-05 12:47:54.000000 torch_snippets-0.531/torch_snippets/loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8480 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/logger.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14683 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/markup.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    17692 2024-05-07 08:11:34.000000 torch_snippets-0.531/torch_snippets/markup2.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2054 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/misc.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11039 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/paths.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1465 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/pdf_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      822 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/registry.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3234 2024-05-05 12:47:53.000000 torch_snippets-0.531/torch_snippets/scp.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/sklegos.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14202 2024-03-28 08:34:42.000000 torch_snippets-0.531/torch_snippets/text_utils.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-07 08:15:31.326416 torch_snippets-0.531/torch_snippets/thinc_parser/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/thinc_parser/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.531/torch_snippets/thinc_parser/parser.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    31250 2024-02-29 09:58:55.000000 torch_snippets-0.531/torch_snippets/torch_loader.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-07 08:15:31.333427 torch_snippets-0.531/torch_snippets/trainer/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/trainer/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6882 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/trainer/capsule.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2432 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/trainer/config.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5801 2024-04-24 06:16:19.000000 torch_snippets-0.531/torch_snippets/trainer/hooks.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2137 2024-02-14 10:01:57.000000 torch_snippets-0.531/torch_snippets/video.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-07 08:15:31.325037 torch_snippets-0.531/torch_snippets.egg-info/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5711 2024-05-07 08:15:31.000000 torch_snippets-0.531/torch_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1337 2024-05-07 08:15:31.000000 torch_snippets-0.531/torch_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2024-05-07 08:15:31.000000 torch_snippets-0.531/torch_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       20 2024-05-07 08:15:31.000000 torch_snippets-0.531/torch_snippets.egg-info/entry_points.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-01-17 16:58:23.000000 torch_snippets-0.531/torch_snippets.egg-info/not-zip-safe
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      281 2024-05-07 08:15:31.000000 torch_snippets-0.531/torch_snippets.egg-info/requires.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2024-05-07 08:15:31.000000 torch_snippets-0.531/torch_snippets.egg-info/top_level.txt
```

### Comparing `torch_snippets-0.530/LICENSE` & `torch_snippets-0.531/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/LICENSE.txt` & `torch_snippets-0.531/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/PKG-INFO` & `torch_snippets-0.531/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_snippets
-Version: 0.530
+Version: 0.531
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
 Platform: UNKNOWN
```

### Comparing `torch_snippets-0.530/README.md` & `torch_snippets-0.531/README.md`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/settings.ini` & `torch_snippets-0.531/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = sizhky
 description = One line functions for common tasks
 keywords = snippets, torch
 author = Yeshwanth Reddy
 author_email = 1992chinna@gmail.com
 copyright = sizhky
 branch = master
-version = 0.530
+version = 0.531
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 requirements = fastcore matplotlib Pillow altair dill ipython loguru numpy pandas tqdm rich PyYAML catalogue confection pydantic typing srsly typing_extensions wasabi jsonlines imgaug>=0.4.0 xmltodict fuzzywuzzy scikit-learn nltk python-Levenshtein pre-commit pymupdf nbconvert nbformat icecream
```

### Comparing `torch_snippets-0.530/setup.py` & `torch_snippets-0.531/setup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/_modidx.py` & `torch_snippets-0.531/torch_snippets/_modidx.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/_nbdev.py` & `torch_snippets-0.531/torch_snippets/_nbdev.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/adapters.py` & `torch_snippets-0.531/torch_snippets/adapters.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/bb_utils.py` & `torch_snippets-0.531/torch_snippets/bb_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/bokeh_loader.py` & `torch_snippets-0.531/torch_snippets/bokeh_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/charts.py` & `torch_snippets-0.531/torch_snippets/charts.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/dates.py` & `torch_snippets-0.531/torch_snippets/dates.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/decorators.py` & `torch_snippets-0.531/torch_snippets/decorators.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/icecream.py` & `torch_snippets-0.531/torch_snippets/icecream.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/imgaug_loader.py` & `torch_snippets-0.531/torch_snippets/imgaug_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/inspector.py` & `torch_snippets-0.531/torch_snippets/inspector.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/interactive_show.py` & `torch_snippets-0.531/torch_snippets/interactive_show.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/ipython.py` & `torch_snippets-0.531/torch_snippets/ipython.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/load_defaults.py` & `torch_snippets-0.531/torch_snippets/load_defaults.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/loader.py` & `torch_snippets-0.531/torch_snippets/loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/logger.py` & `torch_snippets-0.531/torch_snippets/logger.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/markup.py` & `torch_snippets-0.531/torch_snippets/markup.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,24 @@
         )
 
     def __dir__(self):
         return self.__dict__.keys()
 
     def __contains__(self, key):
         key = str(key)
-        return key in self.__dict__.keys()
+        if "." not in key:
+            return key in self.__dict__.keys()
+        else:
+            d = self
+            for _k in key.split("."):
+                try:
+                    d = d[_k]
+                except AttributeError:
+                    return False
+            return True
 
     def __delitem__(self, key):
         key = str(key)
         del self.__dict__[key]
 
     def map(self, func):
         for k in dir(self):
```

### Comparing `torch_snippets-0.530/torch_snippets/markup2.py` & `torch_snippets-0.531/torch_snippets/markup2.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,24 @@
         return f"\n```↯ AttrDict ↯\n{self.summary()}\n```\n"
 
     def __dir__(self):
         return self.__dict__.keys()
 
     def __contains__(self, key):
         key = str(key)
-        return key in self.__dict__.keys()
+        if "." not in key:
+            return key in self.__dict__.keys()
+        else:
+            d = self
+            for _k in key.split("."):
+                try:
+                    d = d[_k]
+                except AttributeError:
+                    return False
+            return True
 
     def __delitem__(self, key):
         key = str(key)
         del self.__dict__[key]
 
     def map(self, func):
         for k in dir(self):
```

### Comparing `torch_snippets-0.530/torch_snippets/misc.py` & `torch_snippets-0.531/torch_snippets/misc.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/paths.py` & `torch_snippets-0.531/torch_snippets/paths.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/pdf_loader.py` & `torch_snippets-0.531/torch_snippets/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/registry.py` & `torch_snippets-0.531/torch_snippets/registry.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/scp.py` & `torch_snippets-0.531/torch_snippets/scp.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/sklegos.py` & `torch_snippets-0.531/torch_snippets/sklegos.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/text_utils.py` & `torch_snippets-0.531/torch_snippets/text_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/thinc_parser/parser.py` & `torch_snippets-0.531/torch_snippets/thinc_parser/parser.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/torch_loader.py` & `torch_snippets-0.531/torch_snippets/torch_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/trainer/capsule.py` & `torch_snippets-0.531/torch_snippets/trainer/capsule.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/trainer/config.py` & `torch_snippets-0.531/torch_snippets/trainer/config.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/trainer/hooks.py` & `torch_snippets-0.531/torch_snippets/trainer/hooks.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets/video.py` & `torch_snippets-0.531/torch_snippets/video.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.530/torch_snippets.egg-info/PKG-INFO` & `torch_snippets-0.531/torch_snippets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-snippets
-Version: 0.530
+Version: 0.531
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
 Platform: UNKNOWN
```

### Comparing `torch_snippets-0.530/torch_snippets.egg-info/SOURCES.txt` & `torch_snippets-0.531/torch_snippets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

