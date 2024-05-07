# Comparing `tmp/cinemol-0.0.1.tar.gz` & `tmp/cinemol-0.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cinemol-0.0.1.tar", last modified: Tue May  7 00:12:53 2024, max compression
+gzip compressed data, was "cinemol-0.0.1.dev0.tar", last modified: Tue May  7 00:07:35 2024, max compression
```

## Comparing `cinemol-0.0.1.tar` & `cinemol-0.0.1.dev0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:12:53.559738 cinemol-0.0.1/
--rw-r--r--   0 davidmeijer   (501) staff       (20)     1068 2024-04-29 14:26:26.000000 cinemol-0.0.1/LICENSE
--rw-r--r--   0 davidmeijer   (501) staff       (20)      669 2024-05-06 12:27:07.000000 cinemol-0.0.1/MANIFEST.in
--rw-r--r--   0 davidmeijer   (501) staff       (20)     8124 2024-05-07 00:12:53.560013 cinemol-0.0.1/PKG-INFO
--rw-r--r--   0 davidmeijer   (501) staff       (20)     6753 2024-05-07 00:02:08.000000 cinemol-0.0.1/README.md
-drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:12:53.526361 cinemol-0.0.1/docs/
-drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:12:53.529986 cinemol-0.0.1/docs/source/
-drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:12:53.532255 cinemol-0.0.1/docs/source/cinemol/
--rw-r--r--   0 davidmeijer   (501) staff       (20)       68 2024-05-01 22:13:52.000000 cinemol-0.0.1/docs/source/cinemol/api.rst
--rw-r--r--   0 davidmeijer   (501) staff       (20)       76 2024-05-01 22:16:22.000000 cinemol-0.0.1/docs/source/cinemol/fitting.rst
--rw-r--r--   0 davidmeijer   (501) staff       (20)       79 2024-05-01 22:16:28.000000 cinemol-0.0.1/docs/source/cinemol/geometry.rst
--rw-r--r--   0 davidmeijer   (501) staff       (20)      121 2024-05-01 22:13:52.000000 cinemol-0.0.1/docs/source/cinemol/index.rst
--rw-r--r--   0 davidmeijer   (501) staff       (20)       70 2024-05-01 22:16:32.000000 cinemol-0.0.1/docs/source/cinemol/model.rst
--rw-r--r--   0 davidmeijer   (501) staff       (20)       76 2024-05-01 22:16:36.000000 cinemol-0.0.1/docs/source/cinemol/parsers.rst
--rw-r--r--   0 davidmeijer   (501) staff       (20)       70 2024-05-01 22:16:41.000000 cinemol-0.0.1/docs/source/cinemol/style.rst
--rw-r--r--   0 davidmeijer   (501) staff       (20)       64 2024-05-01 22:16:45.000000 cinemol-0.0.1/docs/source/cinemol/svg.rst
--rw-r--r--   0 davidmeijer   (501) staff       (20)      216 2024-05-01 09:31:54.000000 cinemol-0.0.1/docs/source/cli.rst
--rw-r--r--   0 davidmeijer   (501) staff       (20)     7229 2024-05-07 00:09:21.000000 cinemol-0.0.1/docs/source/conf.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     1822 2024-05-01 22:16:05.000000 cinemol-0.0.1/docs/source/index.rst
--rw-r--r--   0 davidmeijer   (501) staff       (20)      498 2024-05-01 21:35:57.000000 cinemol-0.0.1/docs/source/installation.rst
--rw-r--r--   0 davidmeijer   (501) staff       (20)     2332 2024-05-01 22:16:16.000000 cinemol-0.0.1/docs/source/usage.rst
-drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:12:53.533220 cinemol-0.0.1/examples/
-drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:12:53.534124 cinemol-0.0.1/examples/create_figures/
--rw-r--r--   0 davidmeijer   (501) staff       (20)     4577 2024-05-07 00:06:38.000000 cinemol-0.0.1/examples/create_figures/measure_performance.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)    14910 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/create_figures/visual_explanation_algorithm.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     8991 2024-05-06 23:32:11.000000 cinemol-0.0.1/examples/create_figures/visual_summary_performance.py
-drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:12:53.535725 cinemol-0.0.1/examples/data/
--rw-r--r--   0 davidmeijer   (501) staff       (20)   140940 2024-04-30 23:17:46.000000 cinemol-0.0.1/examples/data/9lyz.pdb
--rw-r--r--   0 davidmeijer   (501) staff       (20)      261 2024-05-06 22:08:11.000000 cinemol-0.0.1/examples/data/README.md
--rw-r--r--   0 davidmeijer   (501) staff       (20)     6473 2024-04-30 23:17:46.000000 cinemol-0.0.1/examples/data/penicillin_G.sdf
--rw-r--r--   0 davidmeijer   (501) staff       (20)  1952977 2024-05-06 22:47:37.000000 cinemol-0.0.1/examples/data/performance_on_platinum_dataset.tsv
--rw-r--r--   0 davidmeijer   (501) staff       (20)     2141 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/draw_all_depictions_for_molecule.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     3120 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/draw_protein_with_ligands.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     4828 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/draw_substructure_highlights.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     4454 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/draw_superimposed_conformers.py
-drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:12:53.550210 cinemol-0.0.1/examples/svgs/
--rw-r--r--   0 davidmeijer   (501) staff       (20)   175931 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/svgs/cartoon_ballandstick.svg
--rw-r--r--   0 davidmeijer   (501) staff       (20)    64549 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/svgs/cartoon_spacefilling.svg
--rw-r--r--   0 davidmeijer   (501) staff       (20)    74985 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/svgs/cartoon_tube.svg
--rw-r--r--   0 davidmeijer   (501) staff       (20)   205876 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/svgs/glossy_ballandstick.svg
--rw-r--r--   0 davidmeijer   (501) staff       (20)    74496 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/svgs/glossy_spacefilling.svg
--rw-r--r--   0 davidmeijer   (501) staff       (20)    93236 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/svgs/glossy_tube.svg
--rw-r--r--   0 davidmeijer   (501) staff       (20)   134498 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/svgs/protein_with_ligands.svg
--rw-r--r--   0 davidmeijer   (501) staff       (20)   122771 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/svgs/substructure_highlights.svg
--rw-r--r--   0 davidmeijer   (501) staff       (20)   211027 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/svgs/superimposed_conformers.svg
--rw-r--r--   0 davidmeijer   (501) staff       (20)    13918 2024-05-07 00:02:08.000000 cinemol-0.0.1/examples/svgs/wireframe.svg
--rw-r--r--   0 davidmeijer   (501) staff       (20)    40699 2022-09-15 22:13:54.000000 cinemol-0.0.1/logo.png
--rw-r--r--   0 davidmeijer   (501) staff       (20)      361 2024-04-30 23:17:46.000000 cinemol-0.0.1/pyproject.toml
--rw-r--r--   0 davidmeijer   (501) staff       (20)     2451 2024-05-07 00:12:53.560624 cinemol-0.0.1/setup.cfg
-drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:12:53.527070 cinemol-0.0.1/src/
-drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:12:53.553399 cinemol-0.0.1/src/cinemol/
--rw-r--r--   0 davidmeijer   (501) staff       (20)      227 2024-05-01 09:36:28.000000 cinemol-0.0.1/src/cinemol/__init__.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)      324 2024-04-30 23:59:47.000000 cinemol-0.0.1/src/cinemol/__main__.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)    17404 2024-05-07 00:02:08.000000 cinemol-0.0.1/src/cinemol/api.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     3822 2024-05-07 00:02:08.000000 cinemol-0.0.1/src/cinemol/cli.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     3833 2024-05-02 13:19:27.000000 cinemol-0.0.1/src/cinemol/fitting.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)    24515 2024-05-07 00:02:08.000000 cinemol-0.0.1/src/cinemol/geometry.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)    24415 2024-05-07 00:02:08.000000 cinemol-0.0.1/src/cinemol/model.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     1786 2024-05-06 11:54:47.000000 cinemol-0.0.1/src/cinemol/parsers.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)        0 2024-04-30 23:17:46.000000 cinemol-0.0.1/src/cinemol/py.typed
--rw-r--r--   0 davidmeijer   (501) staff       (20)    15608 2024-04-30 23:17:46.000000 cinemol-0.0.1/src/cinemol/style.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     7748 2024-05-06 11:31:12.000000 cinemol-0.0.1/src/cinemol/svg.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     1022 2024-05-07 00:09:21.000000 cinemol-0.0.1/src/cinemol/version.py
-drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:12:53.554709 cinemol-0.0.1/src/cinemol.egg-info/
--rw-r--r--   0 davidmeijer   (501) staff       (20)     8124 2024-05-07 00:12:53.000000 cinemol-0.0.1/src/cinemol.egg-info/PKG-INFO
--rw-r--r--   0 davidmeijer   (501) staff       (20)     2079 2024-05-07 00:12:53.000000 cinemol-0.0.1/src/cinemol.egg-info/SOURCES.txt
--rw-r--r--   0 davidmeijer   (501) staff       (20)        1 2024-05-07 00:12:53.000000 cinemol-0.0.1/src/cinemol.egg-info/dependency_links.txt
--rw-r--r--   0 davidmeijer   (501) staff       (20)       45 2024-05-07 00:12:53.000000 cinemol-0.0.1/src/cinemol.egg-info/entry_points.txt
--rw-r--r--   0 davidmeijer   (501) staff       (20)        1 2024-05-01 00:03:43.000000 cinemol-0.0.1/src/cinemol.egg-info/not-zip-safe
--rw-r--r--   0 davidmeijer   (501) staff       (20)      149 2024-05-07 00:12:53.000000 cinemol-0.0.1/src/cinemol.egg-info/requires.txt
--rw-r--r--   0 davidmeijer   (501) staff       (20)        8 2024-05-07 00:12:53.000000 cinemol-0.0.1/src/cinemol.egg-info/top_level.txt
-drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:12:53.557783 cinemol-0.0.1/tests/
--rw-r--r--   0 davidmeijer   (501) staff       (20)       57 2024-04-30 23:17:46.000000 cinemol-0.0.1/tests/__init__.py
-drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:12:53.559349 cinemol-0.0.1/tests/fixtures/
--rw-r--r--   0 davidmeijer   (501) staff       (20)     6473 2024-02-07 23:58:23.000000 cinemol-0.0.1/tests/fixtures/test_input_001.sdf
--rw-r--r--   0 davidmeijer   (501) staff       (20)     3892 2024-02-07 23:58:26.000000 cinemol-0.0.1/tests/fixtures/test_input_002.sdf
--rw-r--r--   0 davidmeijer   (501) staff       (20)    10481 2024-02-08 00:01:20.000000 cinemol-0.0.1/tests/fixtures/test_input_003.sdf
--rw-r--r--   0 davidmeijer   (501) staff       (20)    16954 2024-02-07 23:57:36.000000 cinemol-0.0.1/tests/fixtures/test_input_004.sdf
--rw-r--r--   0 davidmeijer   (501) staff       (20)    13945 2024-05-06 12:27:07.000000 cinemol-0.0.1/tests/test_api.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     1739 2024-05-06 21:28:32.000000 cinemol-0.0.1/tests/test_cli.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     5487 2024-05-05 22:18:02.000000 cinemol-0.0.1/tests/test_fitting.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)    26223 2024-05-06 21:11:51.000000 cinemol-0.0.1/tests/test_geometry.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     2268 2024-05-06 12:27:07.000000 cinemol-0.0.1/tests/test_model.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)     2187 2024-05-06 11:55:00.000000 cinemol-0.0.1/tests/test_parsers.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)       81 2024-05-05 22:18:02.000000 cinemol-0.0.1/tests/test_style.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)       79 2024-05-05 22:18:02.000000 cinemol-0.0.1/tests/test_svg.py
--rw-r--r--   0 davidmeijer   (501) staff       (20)      741 2024-05-05 22:18:02.000000 cinemol-0.0.1/tests/test_version.py
+drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:07:35.009807 cinemol-0.0.1.dev0/
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     1068 2024-04-29 14:26:26.000000 cinemol-0.0.1.dev0/LICENSE
+-rw-r--r--   0 davidmeijer   (501) staff       (20)      669 2024-05-06 12:27:07.000000 cinemol-0.0.1.dev0/MANIFEST.in
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     8129 2024-05-07 00:07:35.009920 cinemol-0.0.1.dev0/PKG-INFO
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     6753 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/README.md
+drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:07:34.977422 cinemol-0.0.1.dev0/docs/
+drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:07:34.981475 cinemol-0.0.1.dev0/docs/source/
+drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:07:34.984005 cinemol-0.0.1.dev0/docs/source/cinemol/
+-rw-r--r--   0 davidmeijer   (501) staff       (20)       68 2024-05-01 22:13:52.000000 cinemol-0.0.1.dev0/docs/source/cinemol/api.rst
+-rw-r--r--   0 davidmeijer   (501) staff       (20)       76 2024-05-01 22:16:22.000000 cinemol-0.0.1.dev0/docs/source/cinemol/fitting.rst
+-rw-r--r--   0 davidmeijer   (501) staff       (20)       79 2024-05-01 22:16:28.000000 cinemol-0.0.1.dev0/docs/source/cinemol/geometry.rst
+-rw-r--r--   0 davidmeijer   (501) staff       (20)      121 2024-05-01 22:13:52.000000 cinemol-0.0.1.dev0/docs/source/cinemol/index.rst
+-rw-r--r--   0 davidmeijer   (501) staff       (20)       70 2024-05-01 22:16:32.000000 cinemol-0.0.1.dev0/docs/source/cinemol/model.rst
+-rw-r--r--   0 davidmeijer   (501) staff       (20)       76 2024-05-01 22:16:36.000000 cinemol-0.0.1.dev0/docs/source/cinemol/parsers.rst
+-rw-r--r--   0 davidmeijer   (501) staff       (20)       70 2024-05-01 22:16:41.000000 cinemol-0.0.1.dev0/docs/source/cinemol/style.rst
+-rw-r--r--   0 davidmeijer   (501) staff       (20)       64 2024-05-01 22:16:45.000000 cinemol-0.0.1.dev0/docs/source/cinemol/svg.rst
+-rw-r--r--   0 davidmeijer   (501) staff       (20)      216 2024-05-01 09:31:54.000000 cinemol-0.0.1.dev0/docs/source/cli.rst
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     7233 2024-05-06 12:41:11.000000 cinemol-0.0.1.dev0/docs/source/conf.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     1822 2024-05-01 22:16:05.000000 cinemol-0.0.1.dev0/docs/source/index.rst
+-rw-r--r--   0 davidmeijer   (501) staff       (20)      498 2024-05-01 21:35:57.000000 cinemol-0.0.1.dev0/docs/source/installation.rst
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     2332 2024-05-01 22:16:16.000000 cinemol-0.0.1.dev0/docs/source/usage.rst
+drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:07:34.985431 cinemol-0.0.1.dev0/examples/
+drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:07:34.986230 cinemol-0.0.1.dev0/examples/create_figures/
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     4577 2024-05-07 00:06:38.000000 cinemol-0.0.1.dev0/examples/create_figures/measure_performance.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    14910 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/create_figures/visual_explanation_algorithm.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     8991 2024-05-06 23:32:11.000000 cinemol-0.0.1.dev0/examples/create_figures/visual_summary_performance.py
+drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:07:34.987990 cinemol-0.0.1.dev0/examples/data/
+-rw-r--r--   0 davidmeijer   (501) staff       (20)   140940 2024-04-30 23:17:46.000000 cinemol-0.0.1.dev0/examples/data/9lyz.pdb
+-rw-r--r--   0 davidmeijer   (501) staff       (20)      261 2024-05-06 22:08:11.000000 cinemol-0.0.1.dev0/examples/data/README.md
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     6473 2024-04-30 23:17:46.000000 cinemol-0.0.1.dev0/examples/data/penicillin_G.sdf
+-rw-r--r--   0 davidmeijer   (501) staff       (20)  1952977 2024-05-06 22:47:37.000000 cinemol-0.0.1.dev0/examples/data/performance_on_platinum_dataset.tsv
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     2141 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/draw_all_depictions_for_molecule.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     3120 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/draw_protein_with_ligands.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     4828 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/draw_substructure_highlights.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     4454 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/draw_superimposed_conformers.py
+drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:07:35.000991 cinemol-0.0.1.dev0/examples/svgs/
+-rw-r--r--   0 davidmeijer   (501) staff       (20)   175931 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/svgs/cartoon_ballandstick.svg
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    64549 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/svgs/cartoon_spacefilling.svg
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    74985 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/svgs/cartoon_tube.svg
+-rw-r--r--   0 davidmeijer   (501) staff       (20)   205876 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/svgs/glossy_ballandstick.svg
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    74496 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/svgs/glossy_spacefilling.svg
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    93236 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/svgs/glossy_tube.svg
+-rw-r--r--   0 davidmeijer   (501) staff       (20)   134498 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/svgs/protein_with_ligands.svg
+-rw-r--r--   0 davidmeijer   (501) staff       (20)   122771 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/svgs/substructure_highlights.svg
+-rw-r--r--   0 davidmeijer   (501) staff       (20)   211027 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/svgs/superimposed_conformers.svg
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    13918 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/examples/svgs/wireframe.svg
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    40699 2022-09-15 22:13:54.000000 cinemol-0.0.1.dev0/logo.png
+-rw-r--r--   0 davidmeijer   (501) staff       (20)      361 2024-04-30 23:17:46.000000 cinemol-0.0.1.dev0/pyproject.toml
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     2455 2024-05-07 00:07:35.010978 cinemol-0.0.1.dev0/setup.cfg
+drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:07:34.977961 cinemol-0.0.1.dev0/src/
+drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:07:35.004328 cinemol-0.0.1.dev0/src/cinemol/
+-rw-r--r--   0 davidmeijer   (501) staff       (20)      227 2024-05-01 09:36:28.000000 cinemol-0.0.1.dev0/src/cinemol/__init__.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)      324 2024-04-30 23:59:47.000000 cinemol-0.0.1.dev0/src/cinemol/__main__.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    17404 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/src/cinemol/api.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     3822 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/src/cinemol/cli.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     3833 2024-05-02 13:19:27.000000 cinemol-0.0.1.dev0/src/cinemol/fitting.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    24515 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/src/cinemol/geometry.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    24415 2024-05-07 00:02:08.000000 cinemol-0.0.1.dev0/src/cinemol/model.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     1786 2024-05-06 11:54:47.000000 cinemol-0.0.1.dev0/src/cinemol/parsers.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)        0 2024-04-30 23:17:46.000000 cinemol-0.0.1.dev0/src/cinemol/py.typed
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    15608 2024-04-30 23:17:46.000000 cinemol-0.0.1.dev0/src/cinemol/style.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     7748 2024-05-06 11:31:12.000000 cinemol-0.0.1.dev0/src/cinemol/svg.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     1026 2024-05-06 12:41:11.000000 cinemol-0.0.1.dev0/src/cinemol/version.py
+drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:07:35.005593 cinemol-0.0.1.dev0/src/cinemol.egg-info/
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     8129 2024-05-07 00:07:34.000000 cinemol-0.0.1.dev0/src/cinemol.egg-info/PKG-INFO
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     2079 2024-05-07 00:07:34.000000 cinemol-0.0.1.dev0/src/cinemol.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmeijer   (501) staff       (20)        1 2024-05-07 00:07:34.000000 cinemol-0.0.1.dev0/src/cinemol.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmeijer   (501) staff       (20)       45 2024-05-07 00:07:34.000000 cinemol-0.0.1.dev0/src/cinemol.egg-info/entry_points.txt
+-rw-r--r--   0 davidmeijer   (501) staff       (20)        1 2024-05-01 00:03:43.000000 cinemol-0.0.1.dev0/src/cinemol.egg-info/not-zip-safe
+-rw-r--r--   0 davidmeijer   (501) staff       (20)      149 2024-05-07 00:07:34.000000 cinemol-0.0.1.dev0/src/cinemol.egg-info/requires.txt
+-rw-r--r--   0 davidmeijer   (501) staff       (20)        8 2024-05-07 00:07:34.000000 cinemol-0.0.1.dev0/src/cinemol.egg-info/top_level.txt
+drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:07:35.008267 cinemol-0.0.1.dev0/tests/
+-rw-r--r--   0 davidmeijer   (501) staff       (20)       57 2024-04-30 23:17:46.000000 cinemol-0.0.1.dev0/tests/__init__.py
+drwxr-xr-x   0 davidmeijer   (501) staff       (20)        0 2024-05-07 00:07:35.009479 cinemol-0.0.1.dev0/tests/fixtures/
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     6473 2024-02-07 23:58:23.000000 cinemol-0.0.1.dev0/tests/fixtures/test_input_001.sdf
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     3892 2024-02-07 23:58:26.000000 cinemol-0.0.1.dev0/tests/fixtures/test_input_002.sdf
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    10481 2024-02-08 00:01:20.000000 cinemol-0.0.1.dev0/tests/fixtures/test_input_003.sdf
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    16954 2024-02-07 23:57:36.000000 cinemol-0.0.1.dev0/tests/fixtures/test_input_004.sdf
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    13945 2024-05-06 12:27:07.000000 cinemol-0.0.1.dev0/tests/test_api.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     1739 2024-05-06 21:28:32.000000 cinemol-0.0.1.dev0/tests/test_cli.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     5487 2024-05-05 22:18:02.000000 cinemol-0.0.1.dev0/tests/test_fitting.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)    26223 2024-05-06 21:11:51.000000 cinemol-0.0.1.dev0/tests/test_geometry.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     2268 2024-05-06 12:27:07.000000 cinemol-0.0.1.dev0/tests/test_model.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)     2187 2024-05-06 11:55:00.000000 cinemol-0.0.1.dev0/tests/test_parsers.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)       81 2024-05-05 22:18:02.000000 cinemol-0.0.1.dev0/tests/test_style.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)       79 2024-05-05 22:18:02.000000 cinemol-0.0.1.dev0/tests/test_svg.py
+-rw-r--r--   0 davidmeijer   (501) staff       (20)      741 2024-05-05 22:18:02.000000 cinemol-0.0.1.dev0/tests/test_version.py
```

### Comparing `cinemol-0.0.1/LICENSE` & `cinemol-0.0.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/MANIFEST.in` & `cinemol-0.0.1.dev0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/PKG-INFO` & `cinemol-0.0.1.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cinemol
-Version: 0.0.1
+Version: 0.0.1.dev0
 Summary: CineMol is a tool for drawing small molecule configurations directly to SVG.
 Home-page: https://github.com/moltools/CineMol
 Download-URL: https://github.com/moltools/CineMol/releases
 Author: David Meijer
 Author-email: david.meijer@wur.nl
 Maintainer: David Meijer
 Maintainer-email: david.meijer@wur.nl
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: cinemol Version: 0.0.1 Summary: CineMol is a tool
-for drawing small molecule configurations directly to SVG. Home-page: https://
-github.com/moltools/CineMol Download-URL: https://github.com/moltools/CineMol/
-releases Author: David Meijer Author-email: david.meijer@wur.nl Maintainer:
-David Meijer Maintainer-email: david.meijer@wur.nl License: MIT Project-URL:
-Tracker, https://github.com/moltools/CineMol/issues Project-URL: Source, https:
-//github.com/moltools/CineMol Project-URL: Documentation, https://
-cinemol.readthedocs.io Keywords: snekpack,cookiecutter,scalable vector
+Metadata-Version: 2.1 Name: cinemol Version: 0.0.1.dev0 Summary: CineMol is a
+tool for drawing small molecule configurations directly to SVG. Home-page:
+https://github.com/moltools/CineMol Download-URL: https://github.com/moltools/
+CineMol/releases Author: David Meijer Author-email: david.meijer@wur.nl
+Maintainer: David Meijer Maintainer-email: david.meijer@wur.nl License: MIT
+Project-URL: Tracker, https://github.com/moltools/CineMol/issues Project-URL:
+Source, https://github.com/moltools/CineMol Project-URL: Documentation, https:/
+/cinemol.readthedocs.io Keywords: snekpack,cookiecutter,scalable vector
 graphics,three-dimensional structure,molecular drawing,visualization
 Classifier: Development Status :: 1 - Planning Classifier: Environment ::
 Console Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest Classifier: Framework :: tox Classifier:
 Framework :: Sphinx Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `cinemol-0.0.1/README.md` & `cinemol-0.0.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/docs/source/conf.py` & `cinemol-0.0.1.dev0/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "cinemol"
 copyright = f"{date.today().year}, David Meijer"
 author = "David Meijer"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.0.1"
+release = "0.0.1-dev"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `cinemol-0.0.1/docs/source/index.rst` & `cinemol-0.0.1.dev0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/docs/source/usage.rst` & `cinemol-0.0.1.dev0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/create_figures/measure_performance.py` & `cinemol-0.0.1.dev0/examples/create_figures/measure_performance.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/create_figures/visual_explanation_algorithm.py` & `cinemol-0.0.1.dev0/examples/create_figures/visual_explanation_algorithm.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/create_figures/visual_summary_performance.py` & `cinemol-0.0.1.dev0/examples/create_figures/visual_summary_performance.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/data/9lyz.pdb` & `cinemol-0.0.1.dev0/examples/data/9lyz.pdb`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/data/penicillin_G.sdf` & `cinemol-0.0.1.dev0/examples/data/penicillin_G.sdf`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/data/performance_on_platinum_dataset.tsv` & `cinemol-0.0.1.dev0/examples/data/performance_on_platinum_dataset.tsv`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/draw_all_depictions_for_molecule.py` & `cinemol-0.0.1.dev0/examples/draw_all_depictions_for_molecule.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/draw_protein_with_ligands.py` & `cinemol-0.0.1.dev0/examples/draw_protein_with_ligands.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/draw_substructure_highlights.py` & `cinemol-0.0.1.dev0/examples/draw_substructure_highlights.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/draw_superimposed_conformers.py` & `cinemol-0.0.1.dev0/examples/draw_superimposed_conformers.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/svgs/cartoon_ballandstick.svg` & `cinemol-0.0.1.dev0/examples/svgs/cartoon_ballandstick.svg`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/svgs/cartoon_spacefilling.svg` & `cinemol-0.0.1.dev0/examples/svgs/cartoon_spacefilling.svg`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/svgs/cartoon_tube.svg` & `cinemol-0.0.1.dev0/examples/svgs/cartoon_tube.svg`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/svgs/glossy_ballandstick.svg` & `cinemol-0.0.1.dev0/examples/svgs/glossy_ballandstick.svg`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/svgs/glossy_spacefilling.svg` & `cinemol-0.0.1.dev0/examples/svgs/glossy_spacefilling.svg`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/svgs/glossy_tube.svg` & `cinemol-0.0.1.dev0/examples/svgs/glossy_tube.svg`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/svgs/protein_with_ligands.svg` & `cinemol-0.0.1.dev0/examples/svgs/protein_with_ligands.svg`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/svgs/substructure_highlights.svg` & `cinemol-0.0.1.dev0/examples/svgs/substructure_highlights.svg`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/svgs/superimposed_conformers.svg` & `cinemol-0.0.1.dev0/examples/svgs/superimposed_conformers.svg`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/examples/svgs/wireframe.svg` & `cinemol-0.0.1.dev0/examples/svgs/wireframe.svg`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/logo.png` & `cinemol-0.0.1.dev0/logo.png`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/setup.cfg` & `cinemol-0.0.1.dev0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cinemol
-version = 0.0.1
+version = 0.0.1-dev
 description = CineMol is a tool for drawing small molecule configurations directly to SVG.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/moltools/CineMol
 download_url = https://github.com/moltools/CineMol/releases
 project_urls = 
 	Tracker = https://github.com/moltools/CineMol/issues
```

### Comparing `cinemol-0.0.1/src/cinemol/api.py` & `cinemol-0.0.1.dev0/src/cinemol/api.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/src/cinemol/cli.py` & `cinemol-0.0.1.dev0/src/cinemol/cli.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/src/cinemol/fitting.py` & `cinemol-0.0.1.dev0/src/cinemol/fitting.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/src/cinemol/geometry.py` & `cinemol-0.0.1.dev0/src/cinemol/geometry.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/src/cinemol/model.py` & `cinemol-0.0.1.dev0/src/cinemol/model.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/src/cinemol/parsers.py` & `cinemol-0.0.1.dev0/src/cinemol/parsers.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/src/cinemol/style.py` & `cinemol-0.0.1.dev0/src/cinemol/style.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/src/cinemol/svg.py` & `cinemol-0.0.1.dev0/src/cinemol/svg.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/src/cinemol/version.py` & `cinemol-0.0.1.dev0/src/cinemol/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.0.1"
+VERSION = "0.0.1-dev"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`cinemol` git hash."""
     with open(os.devnull, "w", encoding="utf-8") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `cinemol-0.0.1/src/cinemol.egg-info/PKG-INFO` & `cinemol-0.0.1.dev0/src/cinemol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cinemol
-Version: 0.0.1
+Version: 0.0.1.dev0
 Summary: CineMol is a tool for drawing small molecule configurations directly to SVG.
 Home-page: https://github.com/moltools/CineMol
 Download-URL: https://github.com/moltools/CineMol/releases
 Author: David Meijer
 Author-email: david.meijer@wur.nl
 Maintainer: David Meijer
 Maintainer-email: david.meijer@wur.nl
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: cinemol Version: 0.0.1 Summary: CineMol is a tool
-for drawing small molecule configurations directly to SVG. Home-page: https://
-github.com/moltools/CineMol Download-URL: https://github.com/moltools/CineMol/
-releases Author: David Meijer Author-email: david.meijer@wur.nl Maintainer:
-David Meijer Maintainer-email: david.meijer@wur.nl License: MIT Project-URL:
-Tracker, https://github.com/moltools/CineMol/issues Project-URL: Source, https:
-//github.com/moltools/CineMol Project-URL: Documentation, https://
-cinemol.readthedocs.io Keywords: snekpack,cookiecutter,scalable vector
+Metadata-Version: 2.1 Name: cinemol Version: 0.0.1.dev0 Summary: CineMol is a
+tool for drawing small molecule configurations directly to SVG. Home-page:
+https://github.com/moltools/CineMol Download-URL: https://github.com/moltools/
+CineMol/releases Author: David Meijer Author-email: david.meijer@wur.nl
+Maintainer: David Meijer Maintainer-email: david.meijer@wur.nl License: MIT
+Project-URL: Tracker, https://github.com/moltools/CineMol/issues Project-URL:
+Source, https://github.com/moltools/CineMol Project-URL: Documentation, https:/
+/cinemol.readthedocs.io Keywords: snekpack,cookiecutter,scalable vector
 graphics,three-dimensional structure,molecular drawing,visualization
 Classifier: Development Status :: 1 - Planning Classifier: Environment ::
 Console Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest Classifier: Framework :: tox Classifier:
 Framework :: Sphinx Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `cinemol-0.0.1/src/cinemol.egg-info/SOURCES.txt` & `cinemol-0.0.1.dev0/src/cinemol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/tests/fixtures/test_input_001.sdf` & `cinemol-0.0.1.dev0/tests/fixtures/test_input_001.sdf`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/tests/fixtures/test_input_002.sdf` & `cinemol-0.0.1.dev0/tests/fixtures/test_input_002.sdf`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/tests/fixtures/test_input_003.sdf` & `cinemol-0.0.1.dev0/tests/fixtures/test_input_003.sdf`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/tests/fixtures/test_input_004.sdf` & `cinemol-0.0.1.dev0/tests/fixtures/test_input_004.sdf`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/tests/test_api.py` & `cinemol-0.0.1.dev0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/tests/test_cli.py` & `cinemol-0.0.1.dev0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/tests/test_fitting.py` & `cinemol-0.0.1.dev0/tests/test_fitting.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/tests/test_geometry.py` & `cinemol-0.0.1.dev0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/tests/test_model.py` & `cinemol-0.0.1.dev0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/tests/test_parsers.py` & `cinemol-0.0.1.dev0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `cinemol-0.0.1/tests/test_version.py` & `cinemol-0.0.1.dev0/tests/test_version.py`

 * *Files identical despite different names*

