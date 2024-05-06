# Comparing `tmp/skyrim-0.0.0.tar.gz` & `tmp/skyrim-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyrim-0.0.0.tar", last modified: Mon May  6 19:07:35 2024, max compression
+gzip compressed data, was "skyrim-0.0.1.tar", last modified: Mon May  6 21:30:02 2024, max compression
```

## Comparing `skyrim-0.0.0.tar` & `skyrim-0.0.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.917900 skyrim-0.0.0/
--rw-r--r--   0 efes       (501) staff       (20)      172 2024-04-29 13:57:55.000000 skyrim-0.0.0/.env.example
--rw-r--r--   0 efes       (501) staff       (20)     3403 2024-04-29 14:01:02.000000 skyrim-0.0.0/.gitignore
--rw-r--r--   0 efes       (501) staff       (20)      507 2024-05-06 16:29:30.000000 skyrim-0.0.0/.pre-commit-config.yaml
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.866253 skyrim-0.0.0/.vscode/
--rw-r--r--   0 efes       (501) staff       (20)      176 2024-05-06 12:08:10.000000 skyrim-0.0.0/.vscode/settings.json
--rw-r--r--   0 efes       (501) staff       (20)     1294 2024-05-06 16:47:29.000000 skyrim-0.0.0/CONTRIBUTING.md
--rw-r--r--   0 efes       (501) staff       (20)      267 2024-04-29 14:01:02.000000 skyrim-0.0.0/Dockerfile
--rw-r--r--   0 efes       (501) staff       (20)    11309 2024-04-29 17:53:50.000000 skyrim-0.0.0/LICENSE
--rw-r--r--   0 efes       (501) staff       (20)      422 2024-05-06 19:07:20.000000 skyrim-0.0.0/Makefile
--rw-r--r--   0 efes       (501) staff       (20)    22321 2024-05-06 19:07:35.917660 skyrim-0.0.0/PKG-INFO
--rw-r--r--   0 efes       (501) staff       (20)     8212 2024-05-06 17:10:33.000000 skyrim-0.0.0/README.md
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.916712 skyrim-0.0.0/Skyrim.egg-info/
--rw-r--r--   0 efes       (501) staff       (20)    22321 2024-05-06 19:07:35.000000 skyrim-0.0.0/Skyrim.egg-info/PKG-INFO
--rw-r--r--   0 efes       (501) staff       (20)     1321 2024-05-06 19:07:35.000000 skyrim-0.0.0/Skyrim.egg-info/SOURCES.txt
--rw-r--r--   0 efes       (501) staff       (20)        1 2024-05-06 19:07:35.000000 skyrim-0.0.0/Skyrim.egg-info/dependency_links.txt
--rw-r--r--   0 efes       (501) staff       (20)       50 2024-05-06 19:07:35.000000 skyrim-0.0.0/Skyrim.egg-info/entry_points.txt
--rw-r--r--   0 efes       (501) staff       (20)      154 2024-05-06 19:07:35.000000 skyrim-0.0.0/Skyrim.egg-info/requires.txt
--rw-r--r--   0 efes       (501) staff       (20)       14 2024-05-06 19:07:35.000000 skyrim-0.0.0/Skyrim.egg-info/top_level.txt
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.901274 skyrim-0.0.0/assets/
--rw-r--r--   0 efes       (501) staff       (20)  1688209 2024-04-21 15:21:21.000000 skyrim-0.0.0/assets/output_animation.gif
--rw-r--r--   0 efes       (501) staff       (20)  2447871 2024-04-21 15:21:21.000000 skyrim-0.0.0/assets/output_animation_ortho.gif
--rw-r--r--   0 efes       (501) staff       (20)   752038 2024-04-29 16:50:47.000000 skyrim-0.0.0/assets/skyrim_banner_1.png
--rw-r--r--   0 efes       (501) staff       (20)     1000 2024-05-06 12:08:10.000000 skyrim-0.0.0/build.sh
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.910741 skyrim-0.0.0/notebooks/
--rw-r--r--   0 efes       (501) staff       (20)    67195 2024-04-29 17:37:38.000000 skyrim-0.0.0/notebooks/01_quickstart.ipynb
--rw-r--r--   0 efes       (501) staff       (20)     2313 2024-05-06 19:03:39.000000 skyrim-0.0.0/pyproject.toml
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.912120 skyrim-0.0.0/remote/
--rw-r--r--   0 efes       (501) staff       (20)     4614 2024-05-06 19:02:54.000000 skyrim-0.0.0/remote/forecast.py
--rw-r--r--   0 efes       (501) staff       (20)     4689 2024-05-06 16:19:48.000000 skyrim-0.0.0/remote/forecast_dev.py
--rw-r--r--   0 efes       (501) staff       (20)      241 2024-05-06 12:08:10.000000 skyrim-0.0.0/requirements.txt
--rw-r--r--   0 efes       (501) staff       (20)       38 2024-05-06 19:07:35.917951 skyrim-0.0.0/setup.cfg
--rw-r--r--   0 efes       (501) staff       (20)       37 2024-04-29 14:01:02.000000 skyrim-0.0.0/setup.py
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.912530 skyrim-0.0.0/skyrim/
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.912664 skyrim-0.0.0/skyrim/client/
--rw-r--r--   0 efes       (501) staff       (20)      266 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/client/__init__.py
--rw-r--r--   0 efes       (501) staff       (20)     5215 2024-05-06 18:45:32.000000 skyrim-0.0.0/skyrim/common.py
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.913442 skyrim-0.0.0/skyrim/core/
--rw-r--r--   0 efes       (501) staff       (20)      101 2024-05-06 13:13:39.000000 skyrim-0.0.0/skyrim/core/__init__.py
--rw-r--r--   0 efes       (501) staff       (20)      899 2024-05-06 18:45:26.000000 skyrim-0.0.0/skyrim/core/consts.py
--rw-r--r--   0 efes       (501) staff       (20)     6635 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/core/fetch.py
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.914962 skyrim-0.0.0/skyrim/core/models/
--rw-r--r--   0 efes       (501) staff       (20)      699 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/core/models/__init__.py
--rw-r--r--   0 efes       (501) staff       (20)     7890 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/core/models/base.py
--rw-r--r--   0 efes       (501) staff       (20)     1274 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/core/models/dlwp.py
--rw-r--r--   0 efes       (501) staff       (20)     4991 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/core/models/ensemble.py
--rw-r--r--   0 efes       (501) staff       (20)     1696 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/core/models/fourcastnet.py
--rw-r--r--   0 efes       (501) staff       (20)     2122 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/core/models/fourcastnet_v2.py
--rw-r--r--   0 efes       (501) staff       (20)     1620 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/core/models/fuxi.py
--rw-r--r--   0 efes       (501) staff       (20)     4298 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/core/models/graphcast.py
--rw-r--r--   0 efes       (501) staff       (20)     2501 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/core/models/pangu.py
--rw-r--r--   0 efes       (501) staff       (20)     2984 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/core/models/utils.py
--rw-r--r--   0 efes       (501) staff       (20)     2835 2024-05-06 12:35:57.000000 skyrim-0.0.0/skyrim/core/skyrim.py
--rw-r--r--   0 efes       (501) staff       (20)      838 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/core/utils.py
--rw-r--r--   0 efes       (501) staff       (20)     3616 2024-05-06 19:05:41.000000 skyrim-0.0.0/skyrim/forecast.py
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.915083 skyrim-0.0.0/skyrim/libs/
--rw-r--r--   0 efes       (501) staff       (20)        0 2024-04-21 15:21:21.000000 skyrim-0.0.0/skyrim/libs/__init__.py
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.915186 skyrim-0.0.0/skyrim/libs/finetune/
--rw-r--r--   0 efes       (501) staff       (20)      275 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/libs/finetune/__init__.py
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.915439 skyrim-0.0.0/skyrim/libs/ic/
--rw-r--r--   0 efes       (501) staff       (20)      540 2024-04-29 14:01:02.000000 skyrim-0.0.0/skyrim/libs/ic/__init__.py
--rw-r--r--   0 efes       (501) staff       (20)     4484 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/libs/ic/ifs.py
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.915917 skyrim-0.0.0/skyrim/libs/plotting/
--rw-r--r--   0 efes       (501) staff       (20)      119 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/libs/plotting/__init__.py
--rw-r--r--   0 efes       (501) staff       (20)     5812 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/libs/plotting/generate_rollout_gif.py
--rw-r--r--   0 efes       (501) staff       (20)     2413 2024-05-06 12:08:10.000000 skyrim-0.0.0/skyrim/libs/plotting/plot_wind_speed.py
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.916286 skyrim-0.0.0/tests/
--rw-r--r--   0 efes       (501) staff       (20)        0 2024-04-24 14:55:20.000000 skyrim-0.0.0/tests/__init__.py
--rw-r--r--   0 efes       (501) staff       (20)      126 2024-05-06 12:08:10.000000 skyrim-0.0.0/tests/conftest.py
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 19:07:35.916532 skyrim-0.0.0/tests/core/
--rw-r--r--   0 efes       (501) staff       (20)      702 2024-05-06 12:08:10.000000 skyrim-0.0.0/tests/core/test_base.py
--rw-r--r--   0 efes       (501) staff       (20)      239 2024-05-06 12:08:10.000000 skyrim-0.0.0/tests/core/test_skyrim.py
--rw-r--r--   0 efes       (501) staff       (20)     2693 2024-05-06 12:08:10.000000 skyrim-0.0.0/tests/test_common.py
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.972526 skyrim-0.0.1/
+-rw-r--r--   0 efes       (501) staff       (20)      172 2024-04-29 13:57:55.000000 skyrim-0.0.1/.env.example
+-rw-r--r--   0 efes       (501) staff       (20)     3403 2024-04-29 14:01:02.000000 skyrim-0.0.1/.gitignore
+-rw-r--r--   0 efes       (501) staff       (20)      522 2024-05-06 21:01:04.000000 skyrim-0.0.1/.pre-commit-config.yaml
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.945000 skyrim-0.0.1/.vscode/
+-rw-r--r--   0 efes       (501) staff       (20)      176 2024-05-06 12:08:10.000000 skyrim-0.0.1/.vscode/settings.json
+-rw-r--r--   0 efes       (501) staff       (20)     1294 2024-05-06 16:47:29.000000 skyrim-0.0.1/CONTRIBUTING.md
+-rw-r--r--   0 efes       (501) staff       (20)      267 2024-04-29 14:01:02.000000 skyrim-0.0.1/Dockerfile
+-rw-r--r--   0 efes       (501) staff       (20)    11309 2024-04-29 17:53:50.000000 skyrim-0.0.1/LICENSE
+-rw-r--r--   0 efes       (501) staff       (20)      549 2024-05-06 21:26:05.000000 skyrim-0.0.1/Makefile
+-rw-r--r--   0 efes       (501) staff       (20)    22380 2024-05-06 21:30:02.972278 skyrim-0.0.1/PKG-INFO
+-rw-r--r--   0 efes       (501) staff       (20)     8217 2024-05-06 21:28:37.000000 skyrim-0.0.1/README.md
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.971337 skyrim-0.0.1/Skyrim.egg-info/
+-rw-r--r--   0 efes       (501) staff       (20)    22380 2024-05-06 21:30:02.000000 skyrim-0.0.1/Skyrim.egg-info/PKG-INFO
+-rw-r--r--   0 efes       (501) staff       (20)     1321 2024-05-06 21:30:02.000000 skyrim-0.0.1/Skyrim.egg-info/SOURCES.txt
+-rw-r--r--   0 efes       (501) staff       (20)        1 2024-05-06 21:30:02.000000 skyrim-0.0.1/Skyrim.egg-info/dependency_links.txt
+-rw-r--r--   0 efes       (501) staff       (20)       50 2024-05-06 21:30:02.000000 skyrim-0.0.1/Skyrim.egg-info/entry_points.txt
+-rw-r--r--   0 efes       (501) staff       (20)      154 2024-05-06 21:30:02.000000 skyrim-0.0.1/Skyrim.egg-info/requires.txt
+-rw-r--r--   0 efes       (501) staff       (20)       14 2024-05-06 21:30:02.000000 skyrim-0.0.1/Skyrim.egg-info/top_level.txt
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.959659 skyrim-0.0.1/assets/
+-rw-r--r--   0 efes       (501) staff       (20)  1688209 2024-04-21 15:21:21.000000 skyrim-0.0.1/assets/output_animation.gif
+-rw-r--r--   0 efes       (501) staff       (20)  2447871 2024-04-21 15:21:21.000000 skyrim-0.0.1/assets/output_animation_ortho.gif
+-rw-r--r--   0 efes       (501) staff       (20)   752038 2024-04-29 16:50:47.000000 skyrim-0.0.1/assets/skyrim_banner_1.png
+-rw-r--r--   0 efes       (501) staff       (20)     1000 2024-05-06 12:08:10.000000 skyrim-0.0.1/build.sh
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.962984 skyrim-0.0.1/notebooks/
+-rw-r--r--   0 efes       (501) staff       (20)    67195 2024-04-29 17:37:38.000000 skyrim-0.0.1/notebooks/01_quickstart.ipynb
+-rw-r--r--   0 efes       (501) staff       (20)     2615 2024-05-06 21:29:02.000000 skyrim-0.0.1/pyproject.toml
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.964105 skyrim-0.0.1/remote/
+-rw-r--r--   0 efes       (501) staff       (20)     4614 2024-05-06 19:02:54.000000 skyrim-0.0.1/remote/forecast.py
+-rw-r--r--   0 efes       (501) staff       (20)     4689 2024-05-06 16:19:48.000000 skyrim-0.0.1/remote/forecast_dev.py
+-rw-r--r--   0 efes       (501) staff       (20)      241 2024-05-06 12:08:10.000000 skyrim-0.0.1/requirements.txt
+-rw-r--r--   0 efes       (501) staff       (20)       38 2024-05-06 21:30:02.972569 skyrim-0.0.1/setup.cfg
+-rw-r--r--   0 efes       (501) staff       (20)       37 2024-04-29 14:01:02.000000 skyrim-0.0.1/setup.py
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.964377 skyrim-0.0.1/skyrim/
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.964500 skyrim-0.0.1/skyrim/client/
+-rw-r--r--   0 efes       (501) staff       (20)      266 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/client/__init__.py
+-rw-r--r--   0 efes       (501) staff       (20)     5215 2024-05-06 18:45:32.000000 skyrim-0.0.1/skyrim/common.py
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.966389 skyrim-0.0.1/skyrim/core/
+-rw-r--r--   0 efes       (501) staff       (20)      101 2024-05-06 13:13:39.000000 skyrim-0.0.1/skyrim/core/__init__.py
+-rw-r--r--   0 efes       (501) staff       (20)      899 2024-05-06 18:45:26.000000 skyrim-0.0.1/skyrim/core/consts.py
+-rw-r--r--   0 efes       (501) staff       (20)     6635 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/core/fetch.py
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.968618 skyrim-0.0.1/skyrim/core/models/
+-rw-r--r--   0 efes       (501) staff       (20)      699 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/core/models/__init__.py
+-rw-r--r--   0 efes       (501) staff       (20)     7890 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/core/models/base.py
+-rw-r--r--   0 efes       (501) staff       (20)     1274 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/core/models/dlwp.py
+-rw-r--r--   0 efes       (501) staff       (20)     4991 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/core/models/ensemble.py
+-rw-r--r--   0 efes       (501) staff       (20)     1696 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/core/models/fourcastnet.py
+-rw-r--r--   0 efes       (501) staff       (20)     2122 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/core/models/fourcastnet_v2.py
+-rw-r--r--   0 efes       (501) staff       (20)     1620 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/core/models/fuxi.py
+-rw-r--r--   0 efes       (501) staff       (20)     4298 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/core/models/graphcast.py
+-rw-r--r--   0 efes       (501) staff       (20)     2501 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/core/models/pangu.py
+-rw-r--r--   0 efes       (501) staff       (20)     2984 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/core/models/utils.py
+-rw-r--r--   0 efes       (501) staff       (20)     2835 2024-05-06 12:35:57.000000 skyrim-0.0.1/skyrim/core/skyrim.py
+-rw-r--r--   0 efes       (501) staff       (20)      838 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/core/utils.py
+-rw-r--r--   0 efes       (501) staff       (20)     3558 2024-05-06 21:03:56.000000 skyrim-0.0.1/skyrim/forecast.py
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.968844 skyrim-0.0.1/skyrim/libs/
+-rw-r--r--   0 efes       (501) staff       (20)        0 2024-04-21 15:21:21.000000 skyrim-0.0.1/skyrim/libs/__init__.py
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.968936 skyrim-0.0.1/skyrim/libs/finetune/
+-rw-r--r--   0 efes       (501) staff       (20)      275 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/libs/finetune/__init__.py
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.969389 skyrim-0.0.1/skyrim/libs/ic/
+-rw-r--r--   0 efes       (501) staff       (20)      540 2024-04-29 14:01:02.000000 skyrim-0.0.1/skyrim/libs/ic/__init__.py
+-rw-r--r--   0 efes       (501) staff       (20)     4484 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/libs/ic/ifs.py
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.970025 skyrim-0.0.1/skyrim/libs/plotting/
+-rw-r--r--   0 efes       (501) staff       (20)      119 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/libs/plotting/__init__.py
+-rw-r--r--   0 efes       (501) staff       (20)     5812 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/libs/plotting/generate_rollout_gif.py
+-rw-r--r--   0 efes       (501) staff       (20)     2413 2024-05-06 12:08:10.000000 skyrim-0.0.1/skyrim/libs/plotting/plot_wind_speed.py
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.970547 skyrim-0.0.1/tests/
+-rw-r--r--   0 efes       (501) staff       (20)        0 2024-04-24 14:55:20.000000 skyrim-0.0.1/tests/__init__.py
+-rw-r--r--   0 efes       (501) staff       (20)      126 2024-05-06 12:08:10.000000 skyrim-0.0.1/tests/conftest.py
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2024-05-06 21:30:02.971138 skyrim-0.0.1/tests/core/
+-rw-r--r--   0 efes       (501) staff       (20)      702 2024-05-06 12:08:10.000000 skyrim-0.0.1/tests/core/test_base.py
+-rw-r--r--   0 efes       (501) staff       (20)      239 2024-05-06 12:08:10.000000 skyrim-0.0.1/tests/core/test_skyrim.py
+-rw-r--r--   0 efes       (501) staff       (20)     2693 2024-05-06 12:08:10.000000 skyrim-0.0.1/tests/test_common.py
```

### Comparing `skyrim-0.0.0/.gitignore` & `skyrim-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/CONTRIBUTING.md` & `skyrim-0.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/LICENSE` & `skyrim-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/PKG-INFO` & `skyrim-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Skyrim
-Version: 0.0.0
+Version: 0.0.1
 Summary: AI weather models united.
 Maintainer-email: SecondLaw Research <efe@2lw.ai>, SecondLaw Research <murat@2lw.ai>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,15 +202,16 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/secondlaw-ai/skyrim
-Project-URL: Bug Tracker, https://github.com/secondlaw-ai/skyrim/issues
+Project-URL: Tracker, https://github.com/secondlaw-ai/skyrim/issues
+Project-URL: Docs, https://github.com/secondlaw-ai/skyrim
 Keywords: pytorch,weather,forecasting,ai,ml,xarray,dl
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -275,21 +276,21 @@
 You will need a [modal](https://modal.com/) key to run your forecast as we are loading large weather models (it requires NVIDIA GPU with at least 24GB memory). Modal comes with $30 free credits and a single forecast costs about 2 cents. Alternatively, see the [bare metal](#bare-metal) or [vast.ai](#vastai-setup) setup to run on your own GPUs.
 
 ### Forecasting using Modal:
 
 If you are running on modal then run:
 
 ```bash
-modal run modal/forecast.py
+modal run remote/forecast.py
 ```
 
 This by default uses `pangu` model to forecast for the next 6 hours, starting from yesterday. It gets initial conditions from NOAA GFS and writes the forecast to a modal volume. You can explore the forecast by running a notebook (without GPU) in modal:
 
 ```bash
-modal run modal/forecast.py:run_analysis
+modal run remote/forecast.py:run_analysis
 ```
 
 The forecast will be at `/skyrim/outputs/` volume that you can access from the jupyter notebook.
 
 ```
 import xarray as xr
 forecast = xr.open_dataset('/skyrim/outputs/[forecast_id]/[filename], engine='scipy')
@@ -300,15 +301,15 @@
 ```bash
 modal volume rm forecasts /[model_name] -r
 ```
 
 If you don't want to use modal volume, and want to aggregate results in cloud, we currently support s3 buckets. You just have to run:
 
 ```bash
-modal run modal/forecast.py --output_dir s3://skyrim-dev
+modal run remote/forecast.py --output_dir s3://skyrim-dev
 ```
 
 where `skyrim-dev` is the bucket that you want to aggregate the forecasts. By default, `zarr` format is used to store in AWS/GCP so you can read and move only the parts of the forecasts that you need.
 
 Say interested in wind at 37.0344° N, 27.4305 E to see if we can kite. If we are interested in wind speed, we need to pull wind vectors at about surface level, these are u10m and v10m [components](http://colaweb.gmu.edu/dev/clim301/lectures/wind/wind-uv) of wind. Here is how you do it:
 
 ```python
@@ -350,26 +351,26 @@
 
 For each run, you will first pull the initial conditions of your interest (most recent one by default), then the model will run for the desired time step. Initial conditions are pulled from GFS, ECMWF IFS (Operational) or CDS (ERA5 Reanalysis Dataset).
 
 If you are using CDS initial conditions, then you will need a [CDS](https://cds.climate.copernicus.eu/user/login?destination=%2Fcdsapp%23!%2Fdataset%2Freanalysis-era5-single-levels) API key in your `.env` –`cp .env.example` and paste.
 
 ### Examples
 
-All examples are from local setup, but you can run them as it is if you just change `forecast` to `modal run modal/forecast.py` and also make snake case kebab-case -i.e. `model_name` to `model-name`.
+All examples are from local setup, but you can run them as it is if you just change `forecast` to `modal run remote/forecast.py` and also make snake case kebab-case -i.e. `model_name` to `model-name`.
 
 Example 1: Forecast using `graphcast` model, with ERA5 initial conditions, starting from 2024-04-30T00:00:00 and with a lead time of a week (forecast for the next week, i.e. 168 hours):
 
 ```bash
 forecast --model_name graphcast --initial_conditions cds --date 20240403 -output_dir s3://skyrim-dev --lead_time 168
 ```
 
 or in modal:
 
 ```bash
-modal run modal/forecast.py --model-name graphcast --initial-conditions cds --date 20240403 -output-dir s3://skyrim-dev --lead-time 168
+modal run remote/forecast.py --model-name graphcast --initial-conditions cds --date 20240403 -output-dir s3://skyrim-dev --lead-time 168
 ```
 
 ## Supported initial conditions and caveats
 
 1. GFS
 2. ECMWF IFS
 3. ERA5 Re-analysis Dataset
```

### Comparing `skyrim-0.0.0/README.md` & `skyrim-0.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 You will need a [modal](https://modal.com/) key to run your forecast as we are loading large weather models (it requires NVIDIA GPU with at least 24GB memory). Modal comes with $30 free credits and a single forecast costs about 2 cents. Alternatively, see the [bare metal](#bare-metal) or [vast.ai](#vastai-setup) setup to run on your own GPUs.
 
 ### Forecasting using Modal:
 
 If you are running on modal then run:
 
 ```bash
-modal run modal/forecast.py
+modal run remote/forecast.py
 ```
 
 This by default uses `pangu` model to forecast for the next 6 hours, starting from yesterday. It gets initial conditions from NOAA GFS and writes the forecast to a modal volume. You can explore the forecast by running a notebook (without GPU) in modal:
 
 ```bash
-modal run modal/forecast.py:run_analysis
+modal run remote/forecast.py:run_analysis
 ```
 
 The forecast will be at `/skyrim/outputs/` volume that you can access from the jupyter notebook.
 
 ```
 import xarray as xr
 forecast = xr.open_dataset('/skyrim/outputs/[forecast_id]/[filename], engine='scipy')
@@ -62,15 +62,15 @@
 ```bash
 modal volume rm forecasts /[model_name] -r
 ```
 
 If you don't want to use modal volume, and want to aggregate results in cloud, we currently support s3 buckets. You just have to run:
 
 ```bash
-modal run modal/forecast.py --output_dir s3://skyrim-dev
+modal run remote/forecast.py --output_dir s3://skyrim-dev
 ```
 
 where `skyrim-dev` is the bucket that you want to aggregate the forecasts. By default, `zarr` format is used to store in AWS/GCP so you can read and move only the parts of the forecasts that you need.
 
 Say interested in wind at 37.0344° N, 27.4305 E to see if we can kite. If we are interested in wind speed, we need to pull wind vectors at about surface level, these are u10m and v10m [components](http://colaweb.gmu.edu/dev/clim301/lectures/wind/wind-uv) of wind. Here is how you do it:
 
 ```python
@@ -112,26 +112,26 @@
 
 For each run, you will first pull the initial conditions of your interest (most recent one by default), then the model will run for the desired time step. Initial conditions are pulled from GFS, ECMWF IFS (Operational) or CDS (ERA5 Reanalysis Dataset).
 
 If you are using CDS initial conditions, then you will need a [CDS](https://cds.climate.copernicus.eu/user/login?destination=%2Fcdsapp%23!%2Fdataset%2Freanalysis-era5-single-levels) API key in your `.env` –`cp .env.example` and paste.
 
 ### Examples
 
-All examples are from local setup, but you can run them as it is if you just change `forecast` to `modal run modal/forecast.py` and also make snake case kebab-case -i.e. `model_name` to `model-name`.
+All examples are from local setup, but you can run them as it is if you just change `forecast` to `modal run remote/forecast.py` and also make snake case kebab-case -i.e. `model_name` to `model-name`.
 
 Example 1: Forecast using `graphcast` model, with ERA5 initial conditions, starting from 2024-04-30T00:00:00 and with a lead time of a week (forecast for the next week, i.e. 168 hours):
 
 ```bash
 forecast --model_name graphcast --initial_conditions cds --date 20240403 -output_dir s3://skyrim-dev --lead_time 168
 ```
 
 or in modal:
 
 ```bash
-modal run modal/forecast.py --model-name graphcast --initial-conditions cds --date 20240403 -output-dir s3://skyrim-dev --lead-time 168
+modal run remote/forecast.py --model-name graphcast --initial-conditions cds --date 20240403 -output-dir s3://skyrim-dev --lead-time 168
 ```
 
 ## Supported initial conditions and caveats
 
 1. GFS
 2. ECMWF IFS
 3. ERA5 Re-analysis Dataset
```

#### html2text {}

```diff
@@ -12,26 +12,26 @@
 the repo, set an env (either conda or venv) and then run `pip install .`. This
 will install bare-minimum to run your first forecast. ## Run your first
 forecast You will need a [modal](https://modal.com/) key to run your forecast
 as we are loading large weather models (it requires NVIDIA GPU with at least
 24GB memory). Modal comes with $30 free credits and a single forecast costs
 about 2 cents. Alternatively, see the [bare metal](#bare-metal) or [vast.ai]
 (#vastai-setup) setup to run on your own GPUs. ### Forecasting using Modal: If
-you are running on modal then run: ```bash modal run modal/forecast.py ``` This
-by default uses `pangu` model to forecast for the next 6 hours, starting from
-yesterday. It gets initial conditions from NOAA GFS and writes the forecast to
-a modal volume. You can explore the forecast by running a notebook (without
-GPU) in modal: ```bash modal run modal/forecast.py:run_analysis ``` The
-forecast will be at `/skyrim/outputs/` volume that you can access from the
+you are running on modal then run: ```bash modal run remote/forecast.py ```
+This by default uses `pangu` model to forecast for the next 6 hours, starting
+from yesterday. It gets initial conditions from NOAA GFS and writes the
+forecast to a modal volume. You can explore the forecast by running a notebook
+(without GPU) in modal: ```bash modal run remote/forecast.py:run_analysis ```
+The forecast will be at `/skyrim/outputs/` volume that you can access from the
 jupyter notebook. ``` import xarray as xr forecast = xr.open_dataset('/skyrim/
 outputs/[forecast_id]/[filename], engine='scipy') ``` Once you are done, best
 is to delete the volume as a daily forecast is about 2GB: ```bash modal volume
 rm forecasts /[model_name] -r ``` If you don't want to use modal volume, and
 want to aggregate results in cloud, we currently support s3 buckets. You just
-have to run: ```bash modal run modal/forecast.py --output_dir s3://skyrim-dev
+have to run: ```bash modal run remote/forecast.py --output_dir s3://skyrim-dev
 ``` where `skyrim-dev` is the bucket that you want to aggregate the forecasts.
 By default, `zarr` format is used to store in AWS/GCP so you can read and move
 only the parts of the forecasts that you need. Say interested in wind at
 37.0344Â° N, 27.4305 E to see if we can kite. If we are interested in wind
 speed, we need to pull wind vectors at about surface level, these are u10m and
 v10m [components](http://colaweb.gmu.edu/dev/clim301/lectures/wind/wind-uv) of
 wind. Here is how you do it: ```python import xarray as xr import pandas as pd
@@ -58,21 +58,21 @@
 default), then the model will run for the desired time step. Initial conditions
 are pulled from GFS, ECMWF IFS (Operational) or CDS (ERA5 Reanalysis Dataset).
 If you are using CDS initial conditions, then you will need a [CDS](https://
 cds.climate.copernicus.eu/user/
 login?destination=%2Fcdsapp%23!%2Fdataset%2Freanalysis-era5-single-levels) API
 key in your `.env` â`cp .env.example` and paste. ### Examples All examples
 are from local setup, but you can run them as it is if you just change
-`forecast` to `modal run modal/forecast.py` and also make snake case kebab-case
--i.e. `model_name` to `model-name`. Example 1: Forecast using `graphcast`
+`forecast` to `modal run remote/forecast.py` and also make snake case kebab-
+case -i.e. `model_name` to `model-name`. Example 1: Forecast using `graphcast`
 model, with ERA5 initial conditions, starting from 2024-04-30T00:00:00 and with
 a lead time of a week (forecast for the next week, i.e. 168 hours): ```bash
 forecast --model_name graphcast --initial_conditions cds --date 20240403 -
 output_dir s3://skyrim-dev --lead_time 168 ``` or in modal: ```bash modal run
-modal/forecast.py --model-name graphcast --initial-conditions cds --date
+remote/forecast.py --model-name graphcast --initial-conditions cds --date
 20240403 -output-dir s3://skyrim-dev --lead-time 168 ``` ## Supported initial
 conditions and caveats 1. GFS 2. ECMWF IFS 3. ERA5 Re-analysis Dataset ## Large
 weather models supported Currently supported models are: - [x] [Graphcast]
 (https://arxiv.org/abs/2212.12794) - [x] [Pangu](https://arxiv.org/abs/
 2211.02556) - [x] [Fourcastnet](https://arxiv.org/abs/2202.11214) (v1 & v2) -
 [x] [DLWP](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2020MS002109) -
 [ ] [Fuxi](https://www.nature.com/articles/s41612-023-00512-1) - [ ] [MetNet-3]
```

### Comparing `skyrim-0.0.0/Skyrim.egg-info/PKG-INFO` & `skyrim-0.0.1/Skyrim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Skyrim
-Version: 0.0.0
+Version: 0.0.1
 Summary: AI weather models united.
 Maintainer-email: SecondLaw Research <efe@2lw.ai>, SecondLaw Research <murat@2lw.ai>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,15 +202,16 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/secondlaw-ai/skyrim
-Project-URL: Bug Tracker, https://github.com/secondlaw-ai/skyrim/issues
+Project-URL: Tracker, https://github.com/secondlaw-ai/skyrim/issues
+Project-URL: Docs, https://github.com/secondlaw-ai/skyrim
 Keywords: pytorch,weather,forecasting,ai,ml,xarray,dl
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -275,21 +276,21 @@
 You will need a [modal](https://modal.com/) key to run your forecast as we are loading large weather models (it requires NVIDIA GPU with at least 24GB memory). Modal comes with $30 free credits and a single forecast costs about 2 cents. Alternatively, see the [bare metal](#bare-metal) or [vast.ai](#vastai-setup) setup to run on your own GPUs.
 
 ### Forecasting using Modal:
 
 If you are running on modal then run:
 
 ```bash
-modal run modal/forecast.py
+modal run remote/forecast.py
 ```
 
 This by default uses `pangu` model to forecast for the next 6 hours, starting from yesterday. It gets initial conditions from NOAA GFS and writes the forecast to a modal volume. You can explore the forecast by running a notebook (without GPU) in modal:
 
 ```bash
-modal run modal/forecast.py:run_analysis
+modal run remote/forecast.py:run_analysis
 ```
 
 The forecast will be at `/skyrim/outputs/` volume that you can access from the jupyter notebook.
 
 ```
 import xarray as xr
 forecast = xr.open_dataset('/skyrim/outputs/[forecast_id]/[filename], engine='scipy')
@@ -300,15 +301,15 @@
 ```bash
 modal volume rm forecasts /[model_name] -r
 ```
 
 If you don't want to use modal volume, and want to aggregate results in cloud, we currently support s3 buckets. You just have to run:
 
 ```bash
-modal run modal/forecast.py --output_dir s3://skyrim-dev
+modal run remote/forecast.py --output_dir s3://skyrim-dev
 ```
 
 where `skyrim-dev` is the bucket that you want to aggregate the forecasts. By default, `zarr` format is used to store in AWS/GCP so you can read and move only the parts of the forecasts that you need.
 
 Say interested in wind at 37.0344° N, 27.4305 E to see if we can kite. If we are interested in wind speed, we need to pull wind vectors at about surface level, these are u10m and v10m [components](http://colaweb.gmu.edu/dev/clim301/lectures/wind/wind-uv) of wind. Here is how you do it:
 
 ```python
@@ -350,26 +351,26 @@
 
 For each run, you will first pull the initial conditions of your interest (most recent one by default), then the model will run for the desired time step. Initial conditions are pulled from GFS, ECMWF IFS (Operational) or CDS (ERA5 Reanalysis Dataset).
 
 If you are using CDS initial conditions, then you will need a [CDS](https://cds.climate.copernicus.eu/user/login?destination=%2Fcdsapp%23!%2Fdataset%2Freanalysis-era5-single-levels) API key in your `.env` –`cp .env.example` and paste.
 
 ### Examples
 
-All examples are from local setup, but you can run them as it is if you just change `forecast` to `modal run modal/forecast.py` and also make snake case kebab-case -i.e. `model_name` to `model-name`.
+All examples are from local setup, but you can run them as it is if you just change `forecast` to `modal run remote/forecast.py` and also make snake case kebab-case -i.e. `model_name` to `model-name`.
 
 Example 1: Forecast using `graphcast` model, with ERA5 initial conditions, starting from 2024-04-30T00:00:00 and with a lead time of a week (forecast for the next week, i.e. 168 hours):
 
 ```bash
 forecast --model_name graphcast --initial_conditions cds --date 20240403 -output_dir s3://skyrim-dev --lead_time 168
 ```
 
 or in modal:
 
 ```bash
-modal run modal/forecast.py --model-name graphcast --initial-conditions cds --date 20240403 -output-dir s3://skyrim-dev --lead-time 168
+modal run remote/forecast.py --model-name graphcast --initial-conditions cds --date 20240403 -output-dir s3://skyrim-dev --lead-time 168
 ```
 
 ## Supported initial conditions and caveats
 
 1. GFS
 2. ECMWF IFS
 3. ERA5 Re-analysis Dataset
```

### Comparing `skyrim-0.0.0/Skyrim.egg-info/SOURCES.txt` & `skyrim-0.0.1/Skyrim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/assets/output_animation.gif` & `skyrim-0.0.1/assets/output_animation.gif`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/assets/output_animation_ortho.gif` & `skyrim-0.0.1/assets/output_animation_ortho.gif`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/assets/skyrim_banner_1.png` & `skyrim-0.0.1/assets/skyrim_banner_1.png`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/build.sh` & `skyrim-0.0.1/build.sh`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/notebooks/01_quickstart.ipynb` & `skyrim-0.0.1/notebooks/01_quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/pyproject.toml` & `skyrim-0.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Skyrim"
-version = "0.0.0"
+version = "0.0.1"
 description = "AI weather models united."
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
 maintainers = [
   { name = "SecondLaw Research", email = "efe@2lw.ai" },
   { name = "SecondLaw Research", email = "murat@2lw.ai" },
@@ -50,15 +50,16 @@
   'coverage',
   "twine",
   "build",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/secondlaw-ai/skyrim"
-"Bug Tracker" = "https://github.com/secondlaw-ai/skyrim/issues"
+"Tracker" = "https://github.com/secondlaw-ai/skyrim/issues"
+"Docs" = "https://github.com/secondlaw-ai/skyrim"
 
 [tool.black]
 line-length = 88
 target-version = ["py310"]
 skip-string-normalization = false
 skip-magic-trailing-comma = false
 include = '\.pyi?$'
@@ -93,7 +94,18 @@
 output = "skyrim.coverage.xml"
 
 [tool.coverage.report]
 exclude_lines = ["pragma: no cover"]
 omit = ["tests/*"]
 show_missing = true
 fail_under = 20
+
+[tool.bumpver]
+current_version = "0.0.1"
+version_pattern = "MAJOR.MINOR.PATCH"
+commit_message = "Bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = false
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = ['version = "{version}"']
```

### Comparing `skyrim-0.0.0/remote/forecast.py` & `skyrim-0.0.1/remote/forecast.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/remote/forecast_dev.py` & `skyrim-0.0.1/remote/forecast_dev.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/common.py` & `skyrim-0.0.1/skyrim/common.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/consts.py` & `skyrim-0.0.1/skyrim/core/consts.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/fetch.py` & `skyrim-0.0.1/skyrim/core/fetch.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/models/__init__.py` & `skyrim-0.0.1/skyrim/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/models/base.py` & `skyrim-0.0.1/skyrim/core/models/base.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/models/dlwp.py` & `skyrim-0.0.1/skyrim/core/models/dlwp.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/models/ensemble.py` & `skyrim-0.0.1/skyrim/core/models/ensemble.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/models/fourcastnet.py` & `skyrim-0.0.1/skyrim/core/models/fourcastnet.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/models/fourcastnet_v2.py` & `skyrim-0.0.1/skyrim/core/models/fourcastnet_v2.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/models/fuxi.py` & `skyrim-0.0.1/skyrim/core/models/fuxi.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/models/graphcast.py` & `skyrim-0.0.1/skyrim/core/models/graphcast.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/models/pangu.py` & `skyrim-0.0.1/skyrim/core/models/pangu.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/models/utils.py` & `skyrim-0.0.1/skyrim/core/models/utils.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/skyrim.py` & `skyrim-0.0.1/skyrim/core/skyrim.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/core/utils.py` & `skyrim-0.0.1/skyrim/core/utils.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/forecast.py` & `skyrim-0.0.1/skyrim/forecast.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,32 +85,32 @@
     "--filter_vars",
     "-f",
     type=str,
     default="",
     help="Filter variables such as t2m (temperature) before saving forecasts.",
 )
 @click.option(
-    "--backend",
-    "-b",
-    type=click.Choice(["local", "modal"], case_sensitive=False),
-    default="local",
-    help="Where to run the forecasts.",
+    "--modal",
+    "-mo",
+    type=bool,
+    default=False,
+    help="If set true, then will run on modal.",
 )
 def main(
     model_name: str,
     date: str,
     time: str,
     lead_time: int,
     list_models: bool,
     initial_conditions: str,
     output_dir: str,
     filter_vars: str,
-    backend: str,
+    modal: bool,
 ):
-    if backend == "modal":
+    if modal:
         return subprocess.run(
             [
                 "modal",
                 "run",
                 "remote/forecast.py",
                 "--model-name",
                 model_name,
```

### Comparing `skyrim-0.0.0/skyrim/libs/ic/__init__.py` & `skyrim-0.0.1/skyrim/libs/ic/__init__.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/libs/ic/ifs.py` & `skyrim-0.0.1/skyrim/libs/ic/ifs.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/libs/plotting/generate_rollout_gif.py` & `skyrim-0.0.1/skyrim/libs/plotting/generate_rollout_gif.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/skyrim/libs/plotting/plot_wind_speed.py` & `skyrim-0.0.1/skyrim/libs/plotting/plot_wind_speed.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/tests/core/test_base.py` & `skyrim-0.0.1/tests/core/test_base.py`

 * *Files identical despite different names*

### Comparing `skyrim-0.0.0/tests/test_common.py` & `skyrim-0.0.1/tests/test_common.py`

 * *Files identical despite different names*

