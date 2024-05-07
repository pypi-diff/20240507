# Comparing `tmp/green_tsetlin-0.1.9.tar.gz` & `tmp/green_tsetlin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "green_tsetlin-0.1.9.tar", last modified: Mon Sep  4 09:50:39 2023, max compression
+gzip compressed data, was "green_tsetlin-1.0.0.tar", last modified: Tue May  7 11:49:12 2024, max compression
```

## Comparing `green_tsetlin-0.1.9.tar` & `green_tsetlin-1.0.0.tar`

### file list

```diff
@@ -1,117 +1,199 @@
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-09-04 09:50:39.678101 green_tsetlin-0.1.9/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1066 2023-07-17 21:10:12.000000 green_tsetlin-0.1.9/LICENSE
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      169 2023-07-17 21:28:58.000000 green_tsetlin-0.1.9/MANIFEST.in
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1967 2023-09-04 09:50:39.678101 green_tsetlin-0.1.9/PKG-INFO
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      742 2023-07-17 23:21:05.000000 green_tsetlin-0.1.9/README.md
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-09-04 09:50:39.662101 green_tsetlin-0.1.9/docs/
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-09-04 09:50:39.662101 green_tsetlin-0.1.9/docs/_build/
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-09-04 09:50:39.662101 green_tsetlin-0.1.9/docs/_build/doctrees/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    11277 2023-07-15 15:16:12.000000 green_tsetlin-0.1.9/docs/_build/doctrees/environment.pickle
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4963 2023-07-15 15:16:12.000000 green_tsetlin-0.1.9/docs/_build/doctrees/index.doctree
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-09-04 09:50:39.666101 green_tsetlin-0.1.9/docs/_build/html/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      230 2023-07-15 15:16:13.000000 green_tsetlin-0.1.9/docs/_build/html/.buildinfo
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-09-04 09:50:39.666101 green_tsetlin-0.1.9/docs/_build/html/_sources/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      455 2023-07-08 11:11:41.000000 green_tsetlin-0.1.9/docs/_build/html/_sources/index.rst.txt
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-09-04 09:50:39.666101 green_tsetlin-0.1.9/docs/_build/html/_static/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4418 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    11185 2023-07-15 15:16:13.000000 green_tsetlin-0.1.9/docs/_build/html/_static/alabaster.css
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    15228 2023-07-15 15:16:12.000000 green_tsetlin-0.1.9/docs/_build/html/_static/basic.css
--rw-rw-r--   0 ooki      (1000) ooki      (1000)       42 2021-01-29 11:59:09.000000 green_tsetlin-0.1.9/docs/_build/html/_static/custom.css
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     8171 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/html/_static/doctools.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      421 2023-07-15 15:16:12.000000 green_tsetlin-0.1.9/docs/_build/html/_static/documentation_options.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      286 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/html/_static/file.png
--rw-rw-r--   0 ooki      (1000) ooki      (1000)   288580 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/html/_static/jquery-3.6.0.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    89501 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/html/_static/jquery.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4758 2023-07-15 15:16:12.000000 green_tsetlin-0.1.9/docs/_build/html/_static/language_data.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)       90 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/html/_static/minus.png
--rw-rw-r--   0 ooki      (1000) ooki      (1000)       90 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/html/_static/plus.png
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     5249 2023-07-15 15:16:12.000000 green_tsetlin-0.1.9/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    17088 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/html/_static/searchtools.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    68420 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/html/_static/underscore-1.13.1.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    19530 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/html/_static/underscore.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2482 2023-07-15 15:16:12.000000 green_tsetlin-0.1.9/docs/_build/html/genindex.html
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3431 2023-07-15 15:16:12.000000 green_tsetlin-0.1.9/docs/_build/html/index.html
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      268 2023-07-15 15:16:13.000000 green_tsetlin-0.1.9/docs/_build/html/objects.inv
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2759 2023-07-15 15:16:12.000000 green_tsetlin-0.1.9/docs/_build/html/search.html
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      633 2023-07-15 15:16:13.000000 green_tsetlin-0.1.9/docs/_build/html/searchindex.js
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-09-04 09:50:39.670102 green_tsetlin-0.1.9/docs/_build/latex/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4366 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/LICRcyr2utf8.xdy
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    10188 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/LICRlatin2utf8.xdy
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    18693 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/LatinRules.xdy
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2465 2023-07-15 15:17:48.000000 green_tsetlin-0.1.9/docs/_build/latex/green_tsetlin.tex
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      473 2023-07-15 15:17:48.000000 green_tsetlin-0.1.9/docs/_build/latex/make.bat
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      392 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/python.ist
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    12780 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinx.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     9474 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinx.xdy
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     6679 2023-07-15 15:17:48.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxhighlight.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3256 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxhowto.cls
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     6238 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxlatexadmonitions.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      901 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxlatexcontainers.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4840 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxlatexgraphics.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2066 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxlatexindbibtoc.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     5139 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxlatexlists.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    35719 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxlatexliterals.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4532 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxlatexnumfig.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     9066 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxlatexobjects.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3885 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxlatexshadowbox.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3253 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxlatexstyleheadings.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3064 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxlatexstylepage.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     6177 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxlatexstyletext.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    21848 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxlatextables.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4241 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxmanual.cls
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      745 2023-07-15 15:17:48.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxmessages.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2061 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxoptionsgeometry.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1094 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxoptionshyperref.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2590 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxpackagecyrillic.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    15217 2022-07-14 07:38:19.000000 green_tsetlin-0.1.9/docs/_build/latex/sphinxpackagefootnote.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1950 2023-07-08 11:11:41.000000 green_tsetlin-0.1.9/docs/conf.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      455 2023-07-08 11:11:41.000000 green_tsetlin-0.1.9/docs/index.rst
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      800 2023-07-08 11:11:41.000000 green_tsetlin-0.1.9/docs/make.bat
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-09-04 09:50:39.674101 green_tsetlin-0.1.9/green_tsetlin/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      399 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/green_tsetlin/__init__.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     6439 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/green_tsetlin/dataset_generator.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      484 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/green_tsetlin/pandas_connector.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      403 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/green_tsetlin/predictor.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     8381 2023-09-04 09:50:29.000000 green_tsetlin-0.1.9/green_tsetlin/rules.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    11797 2023-09-01 09:53:11.000000 green_tsetlin-0.1.9/green_tsetlin/trainer.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    10372 2023-08-21 09:51:03.000000 green_tsetlin-0.1.9/green_tsetlin/tsetlin_machine.py
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-09-04 09:50:39.674101 green_tsetlin-0.1.9/green_tsetlin.egg-info/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1967 2023-09-04 09:50:39.000000 green_tsetlin-0.1.9/green_tsetlin.egg-info/PKG-INFO
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3258 2023-09-04 09:50:39.000000 green_tsetlin-0.1.9/green_tsetlin.egg-info/SOURCES.txt
--rw-rw-r--   0 ooki      (1000) ooki      (1000)        1 2023-09-04 09:50:39.000000 green_tsetlin-0.1.9/green_tsetlin.egg-info/dependency_links.txt
--rw-rw-r--   0 ooki      (1000) ooki      (1000)        1 2023-07-16 16:16:33.000000 green_tsetlin-0.1.9/green_tsetlin.egg-info/not-zip-safe
--rw-rw-r--   0 ooki      (1000) ooki      (1000)       70 2023-09-04 09:50:39.000000 green_tsetlin-0.1.9/green_tsetlin.egg-info/requires.txt
--rw-rw-r--   0 ooki      (1000) ooki      (1000)       33 2023-09-04 09:50:39.000000 green_tsetlin-0.1.9/green_tsetlin.egg-info/top_level.txt
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      429 2023-07-17 22:54:56.000000 green_tsetlin-0.1.9/pyproject.toml
--rw-rw-r--   0 ooki      (1000) ooki      (1000)       38 2023-09-04 09:50:39.678101 green_tsetlin-0.1.9/setup.cfg
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3346 2023-09-04 09:50:29.000000 green_tsetlin-0.1.9/setup.py
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-09-04 09:50:39.674101 green_tsetlin-0.1.9/src/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    33063 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/src/BS_thread_pool.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2164 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/src/circular_buffer.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    20989 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/src/clause_block.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     9096 2023-08-21 09:51:03.000000 green_tsetlin-0.1.9/src/executor.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    10465 2023-08-29 12:24:13.000000 green_tsetlin-0.1.9/src/feedback_block.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    38013 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/src/func_avx2.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    41681 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/src/func_neon.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    19063 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/src/func_nv.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4662 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/src/func_sparse.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     5568 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/src/functors_interface.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      214 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/src/gt_common.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1049 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/src/gt_utils.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    10088 2023-09-04 09:50:29.000000 green_tsetlin-0.1.9/src/inference.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    13436 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/src/input_block.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    19641 2023-09-04 09:50:29.000000 green_tsetlin-0.1.9/src/main.cpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     9885 2023-07-15 10:37:24.000000 green_tsetlin-0.1.9/src/random_generator.hpp
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-09-04 09:50:39.678101 green_tsetlin-0.1.9/tests/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    19029 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/tests/test_clause_block_avx2_impl.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    15805 2023-07-15 10:37:24.000000 green_tsetlin-0.1.9/tests/test_clause_block_neon_impl.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    14813 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/tests/test_clause_block_nv_impl.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1223 2023-07-15 10:37:24.000000 green_tsetlin-0.1.9/tests/test_dataset_reader.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2527 2023-09-04 09:18:11.000000 green_tsetlin-0.1.9/tests/test_dense_multi_label.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4303 2023-09-04 09:50:29.000000 green_tsetlin-0.1.9/tests/test_inference_impl.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2248 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/tests/test_input_block.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     7708 2023-09-04 09:18:11.000000 green_tsetlin-0.1.9/tests/test_rules.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      548 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/tests/test_sparse_block.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4474 2023-07-31 09:28:00.000000 green_tsetlin-0.1.9/tests/test_trainer.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     5677 2023-07-31 09:28:00.000000 green_tsetlin-0.1.9/tests/test_tsetlin_machine.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3523 2023-07-08 09:51:47.000000 green_tsetlin-0.1.9/tests/tests_dataset_generator.py
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.081299 green_tsetlin-1.0.0/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1066 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/LICENSE
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      169 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/MANIFEST.in
+-rw-r--r--   0 ooki      (1000) ooki      (1000)     1762 2024-05-07 11:49:12.081299 green_tsetlin-1.0.0/PKG-INFO
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      157 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/README.md
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.053299 green_tsetlin-1.0.0/docs/
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.049299 green_tsetlin-1.0.0/docs/_build/
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.053299 green_tsetlin-1.0.0/docs/_build/doctrees/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   487697 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/environment.pickle
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.053299 green_tsetlin-1.0.0/docs/_build/doctrees/examples/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5981 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/examples/california_housing_example.doctree
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    17526 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/examples/imdb_example.doctree
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2802 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/examples.doctree
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   221876 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/green_tsetlin.doctree
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    11183 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/green_tsetlin.py_gtc.doctree
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     6915 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/green_tsetlin.writers.doctree
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3563 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/green_tsetlin_core.doctree
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4240 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/index.doctree
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2986 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/installation.doctree
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2796 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/modules.doctree
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.049299 green_tsetlin-1.0.0/docs/_build/doctrees/nbsphinx/
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.053299 green_tsetlin-1.0.0/docs/_build/doctrees/nbsphinx/examples/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1938 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/nbsphinx/examples/california_housing_example.ipynb
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5625 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/nbsphinx/examples/imdb_example.ipynb
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.053299 green_tsetlin-1.0.0/docs/_build/doctrees/nbsphinx/notebooks/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1938 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/nbsphinx/notebooks/california_housing_example.ipynb
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5625 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/nbsphinx/notebooks/imdb_example.ipynb
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.057299 green_tsetlin-1.0.0/docs/_build/doctrees/notebooks/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5982 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/notebooks/california_housing_example.doctree
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    17527 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/notebooks/imdb_example.doctree
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2433 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/doctrees/setup.doctree
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.057299 green_tsetlin-1.0.0/docs/_build/html/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      230 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/.buildinfo
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.057299 green_tsetlin-1.0.0/docs/_build/html/_modules/
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.057299 green_tsetlin-1.0.0/docs/_build/html/_modules/green_tsetlin/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    25709 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_modules/green_tsetlin/dataset_generator.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    38215 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_modules/green_tsetlin/hpsearch.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    35842 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_modules/green_tsetlin/predictor.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    21564 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_modules/green_tsetlin/ruleset.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    43234 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_modules/green_tsetlin/sparse_tsetlin_machine.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    71136 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_modules/green_tsetlin/trainer.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    59934 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_modules/green_tsetlin/tsetlin_machine.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4637 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_modules/index.html
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.057299 green_tsetlin-1.0.0/docs/_build/html/_sources/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      153 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_sources/examples.rst.txt
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1082 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_sources/green_tsetlin.rst.txt
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      455 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_sources/index.rst.txt
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      175 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_sources/installation.rst.txt
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.057299 green_tsetlin-1.0.0/docs/_build/html/_sources/notebooks/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1938 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_sources/notebooks/california_housing_example.ipynb.txt
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5625 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_sources/notebooks/imdb_example.ipynb.txt
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.061299 green_tsetlin-1.0.0/docs/_build/html/_static/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4289 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    15094 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/basic.css
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.061299 green_tsetlin-1.0.0/docs/_build/html/_static/css/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3229 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/badge_only.css
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.069299 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    87624 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    67312 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    86288 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    66444 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   165742 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   444379 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   165548 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    98024 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    77160 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   323344 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   193308 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   309728 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   184912 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   328412 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   195704 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   309192 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   182708 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   135314 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/css/theme.css
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4885 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5435 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/custom.scss
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4472 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/doctools.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      328 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/documentation_options.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5477 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/favicon.png
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      286 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/file.png
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.049299 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.073299 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    41929 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Bold.eot
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    64400 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Bold.otf
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   143212 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Bold.svg
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    34008 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Bold.ttf
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    27428 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Bold.woff
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    32025 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Medium.eot
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    67588 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Medium.otf
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   184627 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Medium.svg
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    97400 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Medium.ttf
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    39796 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Medium.woff
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    33521 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Regular.eot
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    68328 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Regular.otf
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   218393 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Regular.svg
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   104412 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Regular.ttf
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    42368 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts/calcutta/Calcutta-Regular.woff
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1823 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/fonts.css
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    89501 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/jquery.js
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.073299 green_tsetlin-1.0.0/docs/_build/html/_static/js/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      934 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/js/badge_only.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4370 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2734 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/js/html5shiv.min.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5023 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/js/theme.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4758 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/language_data.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)       90 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4467 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     6861 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/nbsphinx-code-cells.css
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      584 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/nbsphinx-gallery.css
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2871 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)       90 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4902 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    18732 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/searchtools.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5123 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/_static/sphinx_highlight.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5381 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/examples.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    18049 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/genindex.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   101043 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/green_tsetlin.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     6553 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/index.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5347 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/installation.html
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.073299 green_tsetlin-1.0.0/docs/_build/html/notebooks/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    10657 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/notebooks/california_housing_example.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    18701 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/notebooks/imdb_example.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1717 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/objects.inv
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     6130 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/py-modindex.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4364 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/search.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    18458 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/_build/html/searchindex.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1150 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/conf.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      153 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/examples.rst
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1082 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/green_tsetlin.rst
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.073299 green_tsetlin-1.0.0/docs/image/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    40216 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/image/Green Tsetlin transparent brown.png
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    40238 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/image/Green Tsetlin transparent gray.png
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    35323 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/image/Green Tsetlin transparent.png
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    88553 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/image/Green Tsetlin transparent.svg
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    81801 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/image/Green Tsetlin.png
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   308598 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/image/Green Tsetlin.psd
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   117304 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/image/Green Tsetlin.svg
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      455 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/index.rst
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      175 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/installation.rst
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      800 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/make.bat
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.073299 green_tsetlin-1.0.0/docs/notebooks/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1938 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/notebooks/california_housing_example.ipynb
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5625 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/docs/notebooks/imdb_example.ipynb
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.077299 green_tsetlin-1.0.0/green_tsetlin/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      568 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/green_tsetlin/__init__.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3317 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/green_tsetlin/backend.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4149 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/green_tsetlin/dataset_generator.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     8318 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/green_tsetlin/hpsearch.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     7033 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/green_tsetlin/predictor.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3435 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/green_tsetlin/ruleset.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     9021 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/green_tsetlin/sparse_tsetlin_machine.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    16668 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/green_tsetlin/trainer.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    14924 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/green_tsetlin/tsetlin_machine.py
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.081299 green_tsetlin-1.0.0/green_tsetlin.egg-info/
+-rw-r--r--   0 ooki      (1000) ooki      (1000)     1762 2024-05-07 11:49:12.000000 green_tsetlin-1.0.0/green_tsetlin.egg-info/PKG-INFO
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     6894 2024-05-07 11:49:12.000000 green_tsetlin-1.0.0/green_tsetlin.egg-info/SOURCES.txt
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)        1 2024-05-07 11:49:12.000000 green_tsetlin-1.0.0/green_tsetlin.egg-info/dependency_links.txt
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)        1 2024-05-07 11:49:10.000000 green_tsetlin-1.0.0/green_tsetlin.egg-info/not-zip-safe
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)       77 2024-05-07 11:49:12.000000 green_tsetlin-1.0.0/green_tsetlin.egg-info/requires.txt
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)       33 2024-05-07 11:49:12.000000 green_tsetlin-1.0.0/green_tsetlin.egg-info/top_level.txt
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      429 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/pyproject.toml
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)       38 2024-05-07 11:49:12.081299 green_tsetlin-1.0.0/setup.cfg
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3553 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/setup.py
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.077299 green_tsetlin-1.0.0/src/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    33063 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/BS_thread_pool.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4963 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/aligned_tsetlin_state.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    18354 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/clause_block.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     9809 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/executor.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    13076 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/feedback_block.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    30118 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/func_avx2.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    16650 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/func_conv_avx2.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     9283 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/func_conv_tm.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    30455 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/func_neon.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    36823 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/func_sparse.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    15233 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/func_tm.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      861 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/gt_common.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     7779 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/inference.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    15600 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/input_block.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    24152 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/main.cpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5725 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/random_generator.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3438 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/src/sparse_tsetlin_state.hpp
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2024-05-07 11:49:12.081299 green_tsetlin-1.0.0/tests/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      861 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_gtc_avx2_clause_block.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1123 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_gtc_avx2_conv_clause_block.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      266 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_gtc_clause_block_base.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      856 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_gtc_executors.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1450 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_gtc_feedback_block.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2914 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_gtc_inference.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2287 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_gtc_input_block.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     7837 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_gtc_sparse_clause_block.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3638 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_gtc_tm_clause_block.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2764 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_gtc_tm_conv_clause_block.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     7135 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_hpsearch.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5113 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_predictor.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2698 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_ruleset.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4037 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_sparse_tsetlin_machine.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    19426 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_trainer.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3069 2024-05-07 11:46:05.000000 green_tsetlin-1.0.0/tests/test_tsetlin_machine.py
```

### Comparing `green_tsetlin-0.1.9/LICENSE` & `green_tsetlin-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.9/docs/_build/doctrees/index.doctree` & `green_tsetlin-1.0.0/docs/_build/doctrees/index.doctree`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-00000000: 8005 9558 1300 0000 0000 008c 0f73 7068  ...X.........sph
+00000000: 8005 9585 1000 0000 0000 008c 0f73 7068  .............sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 288c 0e64  .children.].(..d
 00000050: 6f63 7574 696c 732e 6e6f 6465 7394 8c07  ocutils.nodes...
 00000060: 636f 6d6d 656e 7494 9394 2981 947d 9428  comment...)..}.(
 00000070: 6805 8cd2 6772 6565 6e5f 7473 6574 6c69  h...green_tsetli
 00000080: 6e20 646f 6375 6d65 6e74 6174 696f 6e20  n documentation 
 00000090: 6d61 7374 6572 2066 696c 652c 2063 7265  master file, cre
 000000a0: 6174 6564 2062 790a 7370 6869 6e78 2d71  ated by.sphinx-q
-000000b0: 7569 636b 7374 6172 7420 6f6e 2053 6174  uickstart on Sat
-000000c0: 204a 756c 2020 3820 3133 3a31 313a 3431   Jul  8 13:11:41
-000000d0: 2032 3032 332e 0a59 6f75 2063 616e 2061   2023..You can a
+000000b0: 7569 636b 7374 6172 7420 6f6e 204d 6f6e  uickstart on Mon
+000000c0: 2041 7072 2020 3820 3130 3a32 393a 3432   Apr  8 10:29:42
+000000d0: 2032 3032 342e 0a59 6f75 2063 616e 2061   2024..You can a
 000000e0: 6461 7074 2074 6869 7320 6669 6c65 2063  dapt this file c
 000000f0: 6f6d 706c 6574 656c 7920 746f 2079 6f75  ompletely to you
 00000100: 7220 6c69 6b69 6e67 2c20 6275 7420 6974  r liking, but it
 00000110: 2073 686f 756c 6420 6174 206c 6561 7374   should at least
 00000120: 0a63 6f6e 7461 696e 2074 6865 2072 6f6f  .contain the roo
 00000130: 7420 6074 6f63 7472 6565 6020 6469 7265  t `toctree` dire
 00000140: 6374 6976 652e 9468 075d 9468 098c 0454  ctive..h.].h...T
 00000150: 6578 7494 9394 8cd2 6772 6565 6e5f 7473  ext.....green_ts
 00000160: 6574 6c69 6e20 646f 6375 6d65 6e74 6174  etlin documentat
 00000170: 696f 6e20 6d61 7374 6572 2066 696c 652c  ion master file,
 00000180: 2063 7265 6174 6564 2062 790a 7370 6869   created by.sphi
 00000190: 6e78 2d71 7569 636b 7374 6172 7420 6f6e  nx-quickstart on
-000001a0: 2053 6174 204a 756c 2020 3820 3133 3a31   Sat Jul  8 13:1
-000001b0: 313a 3431 2032 3032 332e 0a59 6f75 2063  1:41 2023..You c
+000001a0: 204d 6f6e 2041 7072 2020 3820 3130 3a32   Mon Apr  8 10:2
+000001b0: 393a 3432 2032 3032 342e 0a59 6f75 2063  9:42 2024..You c
 000001c0: 616e 2061 6461 7074 2074 6869 7320 6669  an adapt this fi
 000001d0: 6c65 2063 6f6d 706c 6574 656c 7920 746f  le completely to
 000001e0: 2079 6f75 7220 6c69 6b69 6e67 2c20 6275   your liking, bu
 000001f0: 7420 6974 2073 686f 756c 6420 6174 206c  t it should at l
 00000200: 6561 7374 0a63 6f6e 7461 696e 2074 6865  east.contain the
 00000210: 2072 6f6f 7420 6074 6f63 7472 6565 6020   root `toctree` 
 00000220: 6469 7265 6374 6976 652e 9485 9481 947d  directive......}
@@ -38,274 +38,228 @@
 00000250: 0369 6473 945d 948c 0763 6c61 7373 6573  .ids.]...classes
 00000260: 945d 948c 056e 616d 6573 945d 948c 0864  .]...names.]...d
 00000270: 7570 6e61 6d65 7394 5d94 8c08 6261 636b  upnames.]...back
 00000280: 7265 6673 945d 948c 0978 6d6c 3a73 7061  refs.]...xml:spa
 00000290: 6365 948c 0870 7265 7365 7276 6594 758c  ce...preserve.u.
 000002a0: 0774 6167 6e61 6d65 9468 0a68 1668 038c  .tagname.h.h.h..
 000002b0: 095f 646f 6375 6d65 6e74 9468 038c 0673  ._document.h...s
-000002c0: 6f75 7263 6594 8c30 2f68 6f6d 652f 6f6f  ource..0/home/oo
-000002d0: 6b69 2f70 726f 6a65 6374 732f 6772 6565  ki/projects/gree
-000002e0: 6e5f 7473 6574 6c69 6e2f 646f 6373 2f69  n_tsetlin/docs/i
-000002f0: 6e64 6578 2e72 7374 948c 046c 696e 6594  ndex.rst...line.
-00000300: 4b05 7562 6809 8c07 7365 6374 696f 6e94  K.ubh...section.
-00000310: 9394 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
-00000320: 2868 098c 0574 6974 6c65 9493 9429 8194  (h...title...)..
-00000330: 7d94 2868 058c 2957 656c 636f 6d65 2074  }.(h..)Welcome t
-00000340: 6f20 6772 6565 6e5f 7473 6574 6c69 6e27  o green_tsetlin'
-00000350: 7320 646f 6375 6d65 6e74 6174 696f 6e21  s documentation!
-00000360: 9468 075d 9468 118c 2b57 656c 636f 6d65  .h.].h..+Welcome
-00000370: 2074 6f20 6772 6565 6e5f 7473 6574 6c69   to green_tsetli
-00000380: 6ee2 8099 7320 646f 6375 6d65 6e74 6174  n...s documentat
-00000390: 696f 6e21 9485 9481 947d 9428 6816 6831  ion!.....}.(h.h1
-000003a0: 6826 6803 6827 4e68 294e 7562 6168 177d  h&h.h'Nh)Nubah.}
-000003b0: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-000003c0: 5d94 6821 5d94 7568 2568 2f68 1668 2c68  ].h!].uh%h/h.h,h
-000003d0: 2668 0368 2768 2868 294b 0775 6268 098c  &h.h'h(h)K.ubh..
-000003e0: 0863 6f6d 706f 756e 6494 9394 2981 947d  .compound...)..}
-000003f0: 9428 6805 6806 6807 5d94 6800 8c07 746f  .(h.h.h.].h...to
-00000400: 6374 7265 6594 9394 2981 947d 9428 6805  ctree...)..}.(h.
-00000410: 6806 6807 5d94 6817 7d94 2868 195d 9468  h.h.].h.}.(h.].h
-00000420: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9468  .].h.].h.].h!].h
-00000430: 168c 0569 6e64 6578 948c 0765 6e74 7269  ...index...entri
-00000440: 6573 945d 948c 0c69 6e63 6c75 6465 6669  es.]...includefi
-00000450: 6c65 7394 5d94 8c08 6d61 7864 6570 7468  les.]...maxdepth
-00000460: 944b 028c 0763 6170 7469 6f6e 948c 0943  .K...caption...C
-00000470: 6f6e 7465 6e74 733a 948c 0467 6c6f 6294  ontents:...glob.
-00000480: 898c 0668 6964 6465 6e94 898c 0d69 6e63  ...hidden....inc
-00000490: 6c75 6465 6869 6464 656e 9489 8c08 6e75  ludehidden....nu
-000004a0: 6d62 6572 6564 944b 008c 0a74 6974 6c65  mbered.K...title
-000004b0: 736f 6e6c 7994 898c 0a72 6177 656e 7472  sonly....rawentr
-000004c0: 6965 7394 5d94 8c0a 7261 7763 6170 7469  ies.]...rawcapti
-000004d0: 6f6e 9468 5675 6825 6844 6827 6828 6829  on.hVuh%hDh'h(h)
-000004e0: 4b09 6816 6841 7562 6168 177d 9428 6819  K.h.hAubah.}.(h.
-000004f0: 5d94 681b 5d94 8c0f 746f 6374 7265 652d  ].h.]...toctree-
-00000500: 7772 6170 7065 7294 6168 1d5d 9468 1f5d  wrapper.ah.].h.]
-00000510: 9468 215d 9475 6825 683f 6816 682c 6826  .h!].uh%h?h.h,h&
-00000520: 6803 6827 6828 6829 4e75 6265 6817 7d94  h.h'h(h)Nubeh.}.
-00000530: 2868 195d 948c 2877 656c 636f 6d65 2d74  (h.]..(welcome-t
-00000540: 6f2d 6772 6565 6e2d 7473 6574 6c69 6e2d  o-green-tsetlin-
-00000550: 732d 646f 6375 6d65 6e74 6174 696f 6e94  s-documentation.
-00000560: 6168 1b5d 9468 1d5d 948c 2977 656c 636f  ah.].h.]..)welco
-00000570: 6d65 2074 6f20 6772 6565 6e5f 7473 6574  me to green_tset
-00000580: 6c69 6e27 7320 646f 6375 6d65 6e74 6174  lin's documentat
-00000590: 696f 6e21 9461 681f 5d94 6821 5d94 7568  ion!.ah.].h!].uh
-000005a0: 2568 2a68 1668 0368 2668 0368 2768 2868  %h*h.h.h&h.h'h(h
-000005b0: 294b 0775 6268 2b29 8194 7d94 2868 0568  )K.ubh+)..}.(h.h
-000005c0: 0668 075d 9428 6830 2981 947d 9428 6805  .h.].(h0)..}.(h.
-000005d0: 8c12 496e 6469 6365 7320 616e 6420 7461  ..Indices and ta
-000005e0: 626c 6573 9468 075d 9468 118c 1249 6e64  bles.h.].h...Ind
-000005f0: 6963 6573 2061 6e64 2074 6162 6c65 7394  ices and tables.
-00000600: 8594 8194 7d94 2868 1668 7168 2668 0368  ....}.(h.hqh&h.h
-00000610: 274e 6829 4e75 6261 6817 7d94 2868 195d  'Nh)Nubah.}.(h.]
-00000620: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
-00000630: 9475 6825 682f 6816 686e 6826 6803 6827  .uh%h/h.hnh&h.h'
-00000640: 6828 6829 4b10 7562 6809 8c0b 6275 6c6c  h(h)K.ubh...bull
-00000650: 6574 5f6c 6973 7494 9394 2981 947d 9428  et_list...)..}.(
-00000660: 6805 6806 6807 5d94 2868 098c 096c 6973  h.h.h.].(h...lis
-00000670: 745f 6974 656d 9493 9429 8194 7d94 2868  t_item...)..}.(h
-00000680: 058c 0f3a 7265 663a 6067 656e 696e 6465  ...:ref:`geninde
-00000690: 7860 9468 075d 9468 098c 0970 6172 6167  x`.h.].h...parag
-000006a0: 7261 7068 9493 9429 8194 7d94 2868 0568  raph...)..}.(h.h
-000006b0: 8868 075d 9468 008c 0c70 656e 6469 6e67  .h.].h...pending
-000006c0: 5f78 7265 6694 9394 2981 947d 9428 6805  _xref...)..}.(h.
-000006d0: 6888 6807 5d94 6809 8c06 696e 6c69 6e65  h.h.].h...inline
-000006e0: 9493 9429 8194 7d94 2868 0568 8868 075d  ...)..}.(h.h.h.]
-000006f0: 9468 118c 0867 656e 696e 6465 7894 8594  .h...genindex...
-00000700: 8194 7d94 2868 1668 9668 2668 0368 274e  ..}.(h.h.h&h.h'N
-00000710: 6829 4e75 6261 6817 7d94 2868 195d 9468  h)Nubah.}.(h.].h
-00000720: 1b5d 9428 8c04 7872 6566 948c 0373 7464  .].(..xref...std
-00000730: 948c 0773 7464 2d72 6566 9465 681d 5d94  ...std-ref.eh.].
-00000740: 681f 5d94 6821 5d94 7568 2568 9468 1668  h.].h!].uh%h.h.h
-00000750: 9175 6261 6817 7d94 2868 195d 9468 1b5d  .ubah.}.(h.].h.]
-00000760: 9468 1d5d 9468 1f5d 9468 215d 948c 0672  .h.].h.].h!]...r
-00000770: 6566 646f 6394 684f 8c09 7265 6664 6f6d  efdoc.hO..refdom
-00000780: 6169 6e94 68a1 8c07 7265 6674 7970 6594  ain.h...reftype.
-00000790: 8c03 7265 6694 8c0b 7265 6665 7870 6c69  ..ref...refexpli
-000007a0: 6369 7494 898c 0772 6566 7761 726e 9488  cit....refwarn..
-000007b0: 8c09 7265 6674 6172 6765 7494 8c08 6765  ..reftarget...ge
-000007c0: 6e69 6e64 6578 9475 6825 688f 6827 6828  nindex.uh%h.h'h(
-000007d0: 6829 4b12 6816 688c 7562 6168 177d 9428  h)K.h.h.ubah.}.(
-000007e0: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
-000007f0: 6821 5d94 7568 2568 8a68 2768 2868 294b  h!].uh%h.h'h(h)K
-00000800: 1268 1668 8675 6261 6817 7d94 2868 195d  .h.h.ubah.}.(h.]
-00000810: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
-00000820: 9475 6825 6884 6816 6881 6826 6803 6827  .uh%h.h.h.h&h.h'
-00000830: 6828 6829 4e75 6268 8529 8194 7d94 2868  h(h)Nubh.)..}.(h
-00000840: 058c 0f3a 7265 663a 606d 6f64 696e 6465  ...:ref:`modinde
-00000850: 7860 9468 075d 9468 8b29 8194 7d94 2868  x`.h.].h.)..}.(h
-00000860: 0568 c268 075d 9468 9029 8194 7d94 2868  .h.h.].h.)..}.(h
-00000870: 0568 c268 075d 9468 9529 8194 7d94 2868  .h.h.].h.)..}.(h
-00000880: 0568 c268 075d 9468 118c 086d 6f64 696e  .h.h.].h...modin
-00000890: 6465 7894 8594 8194 7d94 2868 1668 ca68  dex.....}.(h.h.h
-000008a0: 2668 0368 274e 6829 4e75 6261 6817 7d94  &h.h'Nh)Nubah.}.
-000008b0: 2868 195d 9468 1b5d 9428 68a0 8c03 7374  (h.].h.].(h...st
-000008c0: 6494 8c07 7374 642d 7265 6694 6568 1d5d  d...std-ref.eh.]
-000008d0: 9468 1f5d 9468 215d 9475 6825 6894 6816  .h.].h!].uh%h.h.
-000008e0: 68c7 7562 6168 177d 9428 6819 5d94 681b  h.ubah.}.(h.].h.
-000008f0: 5d94 681d 5d94 681f 5d94 6821 5d94 8c06  ].h.].h.].h!]...
-00000900: 7265 6664 6f63 9468 4f8c 0972 6566 646f  refdoc.hO..refdo
-00000910: 6d61 696e 9468 d48c 0772 6566 7479 7065  main.h...reftype
-00000920: 948c 0372 6566 948c 0b72 6566 6578 706c  ...ref...refexpl
-00000930: 6963 6974 9489 8c07 7265 6677 6172 6e94  icit....refwarn.
-00000940: 8868 b28c 086d 6f64 696e 6465 7894 7568  .h...modindex.uh
-00000950: 2568 8f68 2768 2868 294b 1368 1668 c475  %h.h'h(h)K.h.h.u
-00000960: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
-00000970: 1d5d 9468 1f5d 9468 215d 9475 6825 688a  .].h.].h!].uh%h.
-00000980: 6827 6828 6829 4b13 6816 68c0 7562 6168  h'h(h)K.h.h.ubah
-00000990: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
-000009a0: 681f 5d94 6821 5d94 7568 2568 8468 1668  h.].h!].uh%h.h.h
-000009b0: 8168 2668 0368 2768 2868 294e 7562 6885  .h&h.h'h(h)Nubh.
-000009c0: 2981 947d 9428 6805 8c0d 3a72 6566 3a60  )..}.(h...:ref:`
-000009d0: 7365 6172 6368 6094 6807 5d94 688b 2981  search`.h.].h.).
-000009e0: 947d 9428 6805 68f4 6807 5d94 6890 2981  .}.(h.h.h.].h.).
-000009f0: 947d 9428 6805 68f4 6807 5d94 6895 2981  .}.(h.h.h.].h.).
-00000a00: 947d 9428 6805 68f4 6807 5d94 6811 8c06  .}.(h.h.h.].h...
-00000a10: 7365 6172 6368 9485 9481 947d 9428 6816  search.....}.(h.
-00000a20: 68fc 6826 6803 6827 4e68 294e 7562 6168  h.h&h.h'Nh)Nubah
-00000a30: 177d 9428 6819 5d94 681b 5d94 2868 a08c  .}.(h.].h.].(h..
-00000a40: 0373 7464 948c 0773 7464 2d72 6566 9465  .std...std-ref.e
-00000a50: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
-00000a60: 9468 1668 f975 6261 6817 7d94 2868 195d  .h.h.ubah.}.(h.]
-00000a70: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
-00000a80: 948c 0672 6566 646f 6394 684f 8c09 7265  ...refdoc.hO..re
-00000a90: 6664 6f6d 6169 6e94 6a06 0100 008c 0772  fdomain.j......r
-00000aa0: 6566 7479 7065 948c 0372 6566 948c 0b72  eftype...ref...r
-00000ab0: 6566 6578 706c 6963 6974 9489 8c07 7265  efexplicit....re
-00000ac0: 6677 6172 6e94 8868 b28c 0673 6561 7263  fwarn..h...searc
-00000ad0: 6894 7568 2568 8f68 2768 2868 294b 1468  h.uh%h.h'h(h)K.h
-00000ae0: 1668 f675 6261 6817 7d94 2868 195d 9468  .h.ubah.}.(h.].h
-00000af0: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
-00000b00: 6825 688a 6827 6828 6829 4b14 6816 68f2  h%h.h'h(h)K.h.h.
-00000b10: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
-00000b20: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
-00000b30: 8468 1668 8168 2668 0368 2768 2868 294e  .h.h.h&h.h'h(h)N
-00000b40: 7562 6568 177d 9428 6819 5d94 681b 5d94  ubeh.}.(h.].h.].
-00000b50: 681d 5d94 681f 5d94 6821 5d94 8c06 6275  h.].h.].h!]...bu
-00000b60: 6c6c 6574 948c 012a 9475 6825 687f 6827  llet...*.uh%h.h'
-00000b70: 6828 6829 4b12 6816 686e 6826 6803 7562  h(h)K.h.hnh&h.ub
-00000b80: 6568 177d 9428 6819 5d94 8c12 696e 6469  eh.}.(h.]...indi
-00000b90: 6365 732d 616e 642d 7461 626c 6573 9461  ces-and-tables.a
-00000ba0: 681b 5d94 681d 5d94 8c12 696e 6469 6365  h.].h.]...indice
-00000bb0: 7320 616e 6420 7461 626c 6573 9461 681f  s and tables.ah.
-00000bc0: 5d94 6821 5d94 7568 2568 2a68 1668 0368  ].h!].uh%h*h.h.h
-00000bd0: 2668 0368 2768 2868 294b 1075 6265 6817  &h.h'h(h)K.ubeh.
-00000be0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00000bf0: 1f5d 9468 215d 948c 0673 6f75 7263 6594  .].h!]...source.
-00000c00: 6828 7568 2568 018c 0e63 7572 7265 6e74  h(uh%h...current
-00000c10: 5f73 6f75 7263 6594 4e8c 0c63 7572 7265  _source.N..curre
-00000c20: 6e74 5f6c 696e 6594 4e8c 0873 6574 7469  nt_line.N..setti
-00000c30: 6e67 7394 8c11 646f 6375 7469 6c73 2e66  ngs...docutils.f
-00000c40: 726f 6e74 656e 6494 8c06 5661 6c75 6573  rontend...Values
-00000c50: 9493 9429 8194 7d94 2868 2f4e 8c09 6765  ...)..}.(h/N..ge
-00000c60: 6e65 7261 746f 7294 4e8c 0964 6174 6573  nerator.N..dates
-00000c70: 7461 6d70 944e 8c0b 736f 7572 6365 5f6c  tamp.N..source_l
-00000c80: 696e 6b94 4e8c 0a73 6f75 7263 655f 7572  ink.N..source_ur
-00000c90: 6c94 4e8c 0d74 6f63 5f62 6163 6b6c 696e  l.N..toc_backlin
-00000ca0: 6b73 948c 0565 6e74 7279 948c 1266 6f6f  ks...entry...foo
-00000cb0: 746e 6f74 655f 6261 636b 6c69 6e6b 7394  tnote_backlinks.
-00000cc0: 4b01 8c0d 7365 6374 6e75 6d5f 7866 6f72  K...sectnum_xfor
-00000cd0: 6d94 4b01 8c0e 7374 7269 705f 636f 6d6d  m.K...strip_comm
-00000ce0: 656e 7473 944e 8c1b 7374 7269 705f 656c  ents.N..strip_el
-00000cf0: 656d 656e 7473 5f77 6974 685f 636c 6173  ements_with_clas
-00000d00: 7365 7394 4e8c 0d73 7472 6970 5f63 6c61  ses.N..strip_cla
-00000d10: 7373 6573 944e 8c0c 7265 706f 7274 5f6c  sses.N..report_l
-00000d20: 6576 656c 944b 028c 0a68 616c 745f 6c65  evel.K...halt_le
-00000d30: 7665 6c94 4b05 8c11 6578 6974 5f73 7461  vel.K...exit_sta
-00000d40: 7475 735f 6c65 7665 6c94 4b05 8c05 6465  tus_level.K...de
-00000d50: 6275 6794 4e8c 0e77 6172 6e69 6e67 5f73  bug.N..warning_s
-00000d60: 7472 6561 6d94 4e8c 0974 7261 6365 6261  tream.N..traceba
-00000d70: 636b 9488 8c0e 696e 7075 745f 656e 636f  ck....input_enco
-00000d80: 6469 6e67 948c 0975 7466 2d38 2d73 6967  ding...utf-8-sig
-00000d90: 948c 1c69 6e70 7574 5f65 6e63 6f64 696e  ...input_encodin
-00000da0: 675f 6572 726f 725f 6861 6e64 6c65 7294  g_error_handler.
-00000db0: 8c06 7374 7269 6374 948c 0f6f 7574 7075  ..strict...outpu
-00000dc0: 745f 656e 636f 6469 6e67 948c 0575 7466  t_encoding...utf
-00000dd0: 2d38 948c 1d6f 7574 7075 745f 656e 636f  -8...output_enco
-00000de0: 6469 6e67 5f65 7272 6f72 5f68 616e 646c  ding_error_handl
-00000df0: 6572 946a 5701 0000 8c0e 6572 726f 725f  er.jW.....error_
-00000e00: 656e 636f 6469 6e67 948c 0575 7466 2d38  encoding...utf-8
-00000e10: 948c 1c65 7272 6f72 5f65 6e63 6f64 696e  ...error_encodin
-00000e20: 675f 6572 726f 725f 6861 6e64 6c65 7294  g_error_handler.
-00000e30: 8c10 6261 636b 736c 6173 6872 6570 6c61  ..backslashrepla
-00000e40: 6365 948c 0d6c 616e 6775 6167 655f 636f  ce...language_co
-00000e50: 6465 948c 0265 6e94 8c13 7265 636f 7264  de...en...record
-00000e60: 5f64 6570 656e 6465 6e63 6965 7394 4e8c  _dependencies.N.
-00000e70: 0663 6f6e 6669 6794 4e8c 0969 645f 7072  .config.N..id_pr
-00000e80: 6566 6978 9468 068c 0e61 7574 6f5f 6964  efix.h...auto_id
-00000e90: 5f70 7265 6669 7894 8c02 6964 948c 0d64  _prefix...id...d
-00000ea0: 756d 705f 7365 7474 696e 6773 944e 8c0e  ump_settings.N..
-00000eb0: 6475 6d70 5f69 6e74 6572 6e61 6c73 944e  dump_internals.N
-00000ec0: 8c0f 6475 6d70 5f74 7261 6e73 666f 726d  ..dump_transform
-00000ed0: 7394 4e8c 0f64 756d 705f 7073 6575 646f  s.N..dump_pseudo
-00000ee0: 5f78 6d6c 944e 8c10 6578 706f 7365 5f69  _xml.N..expose_i
-00000ef0: 6e74 6572 6e61 6c73 944e 8c0e 7374 7269  nternals.N..stri
-00000f00: 6374 5f76 6973 6974 6f72 944e 8c0f 5f64  ct_visitor.N.._d
-00000f10: 6973 6162 6c65 5f63 6f6e 6669 6794 4e8c  isable_config.N.
-00000f20: 075f 736f 7572 6365 9468 288c 0c5f 6465  ._source.h(.._de
-00000f30: 7374 696e 6174 696f 6e94 4e8c 0d5f 636f  stination.N.._co
-00000f40: 6e66 6967 5f66 696c 6573 945d 948c 1666  nfig_files.]...f
-00000f50: 696c 655f 696e 7365 7274 696f 6e5f 656e  ile_insertion_en
-00000f60: 6162 6c65 6494 888c 0b72 6177 5f65 6e61  abled....raw_ena
-00000f70: 626c 6564 944b 018c 116c 696e 655f 6c65  bled.K...line_le
-00000f80: 6e67 7468 5f6c 696d 6974 944d 1027 8c0e  ngth_limit.M.'..
-00000f90: 7065 705f 7265 6665 7265 6e63 6573 944e  pep_references.N
-00000fa0: 8c0c 7065 705f 6261 7365 5f75 726c 948c  ..pep_base_url..
-00000fb0: 1868 7474 7073 3a2f 2f70 6570 732e 7079  .https://peps.py
-00000fc0: 7468 6f6e 2e6f 7267 2f94 8c15 7065 705f  thon.org/...pep_
-00000fd0: 6669 6c65 5f75 726c 5f74 656d 706c 6174  file_url_templat
-00000fe0: 6594 8c08 7065 702d 2530 3464 948c 0e72  e...pep-%04d...r
-00000ff0: 6663 5f72 6566 6572 656e 6365 7394 4e8c  fc_references.N.
-00001000: 0c72 6663 5f62 6173 655f 7572 6c94 8c26  .rfc_base_url..&
-00001010: 6874 7470 733a 2f2f 6461 7461 7472 6163  https://datatrac
-00001020: 6b65 722e 6965 7466 2e6f 7267 2f64 6f63  ker.ietf.org/doc
-00001030: 2f68 746d 6c2f 948c 0974 6162 5f77 6964  /html/...tab_wid
-00001040: 7468 944b 088c 1d74 7269 6d5f 666f 6f74  th.K...trim_foot
-00001050: 6e6f 7465 5f72 6566 6572 656e 6365 5f73  note_reference_s
-00001060: 7061 6365 9489 8c10 7379 6e74 6178 5f68  pace....syntax_h
-00001070: 6967 686c 6967 6874 948c 046c 6f6e 6794  ighlight...long.
-00001080: 8c0c 736d 6172 745f 7175 6f74 6573 9488  ..smart_quotes..
-00001090: 8c13 736d 6172 7471 756f 7465 735f 6c6f  ..smartquotes_lo
-000010a0: 6361 6c65 7394 5d94 8c1d 6368 6172 6163  cales.]...charac
-000010b0: 7465 725f 6c65 7665 6c5f 696e 6c69 6e65  ter_level_inline
-000010c0: 5f6d 6172 6b75 7094 898c 0e64 6f63 7469  _markup....docti
-000010d0: 746c 655f 7866 6f72 6d94 898c 0d64 6f63  tle_xform....doc
-000010e0: 696e 666f 5f78 666f 726d 944b 018c 1273  info_xform.K...s
-000010f0: 6563 7473 7562 7469 746c 655f 7866 6f72  ectsubtitle_xfor
-00001100: 6d94 898c 0d69 6d61 6765 5f6c 6f61 6469  m....image_loadi
-00001110: 6e67 948c 046c 696e 6b94 8c10 656d 6265  ng...link...embe
-00001120: 645f 7374 796c 6573 6865 6574 9489 8c15  d_stylesheet....
-00001130: 636c 6f61 6b5f 656d 6169 6c5f 6164 6472  cloak_email_addr
-00001140: 6573 7365 7394 888c 1173 6563 7469 6f6e  esses....section
-00001150: 5f73 656c 665f 6c69 6e6b 9489 8c03 656e  _self_link....en
-00001160: 7694 4e75 628c 0872 6570 6f72 7465 7294  v.Nub..reporter.
-00001170: 4e8c 1069 6e64 6972 6563 745f 7461 7267  N..indirect_targ
-00001180: 6574 7394 5d94 8c11 7375 6273 7469 7475  ets.]...substitu
-00001190: 7469 6f6e 5f64 6566 7394 7d94 8c12 7375  tion_defs.}...su
-000011a0: 6273 7469 7475 7469 6f6e 5f6e 616d 6573  bstitution_names
-000011b0: 947d 948c 0872 6566 6e61 6d65 7394 7d94  .}...refnames.}.
-000011c0: 8c06 7265 6669 6473 947d 948c 076e 616d  ..refids.}...nam
-000011d0: 6569 6473 947d 9428 686b 6868 6a31 0100  eids.}.(hkhhj1..
-000011e0: 006a 2e01 0000 758c 096e 616d 6574 7970  .j....u..nametyp
-000011f0: 6573 947d 9428 686b 896a 3101 0000 8975  es.}.(hk.j1....u
-00001200: 6819 7d94 2868 6868 2c6a 2e01 0000 686e  h.}.(hhh,j....hn
-00001210: 758c 0d66 6f6f 746e 6f74 655f 7265 6673  u..footnote_refs
-00001220: 947d 948c 0d63 6974 6174 696f 6e5f 7265  .}...citation_re
-00001230: 6673 947d 948c 0d61 7574 6f66 6f6f 746e  fs.}...autofootn
-00001240: 6f74 6573 945d 948c 1161 7574 6f66 6f6f  otes.]...autofoo
-00001250: 746e 6f74 655f 7265 6673 945d 948c 1073  tnote_refs.]...s
-00001260: 796d 626f 6c5f 666f 6f74 6e6f 7465 7394  ymbol_footnotes.
-00001270: 5d94 8c14 7379 6d62 6f6c 5f66 6f6f 746e  ]...symbol_footn
-00001280: 6f74 655f 7265 6673 945d 948c 0966 6f6f  ote_refs.]...foo
-00001290: 746e 6f74 6573 945d 948c 0963 6974 6174  tnotes.]...citat
-000012a0: 696f 6e73 945d 948c 1261 7574 6f66 6f6f  ions.]...autofoo
-000012b0: 746e 6f74 655f 7374 6172 7494 4b01 8c15  tnote_start.K...
-000012c0: 7379 6d62 6f6c 5f66 6f6f 746e 6f74 655f  symbol_footnote_
-000012d0: 7374 6172 7494 4b00 8c0a 6964 5f63 6f75  start.K...id_cou
-000012e0: 6e74 6572 948c 0b63 6f6c 6c65 6374 696f  nter...collectio
-000012f0: 6e73 948c 0743 6f75 6e74 6572 9493 947d  ns...Counter...}
-00001300: 9485 9452 948c 0e70 6172 7365 5f6d 6573  ...R...parse_mes
-00001310: 7361 6765 7394 5d94 8c12 7472 616e 7366  sages.]...transf
-00001320: 6f72 6d5f 6d65 7373 6167 6573 945d 948c  orm_messages.]..
-00001330: 0b74 7261 6e73 666f 726d 6572 944e 8c0b  .transformer.N..
-00001340: 696e 636c 7564 655f 6c6f 6794 5d94 8c0a  include_log.]...
-00001350: 6465 636f 7261 7469 6f6e 944e 6826 6803  decoration.Nh&h.
-00001360: 7562 2e                                  ub.
+000002c0: 6f75 7263 6594 8c34 2f68 6f6d 652f 6b6f  ource..4/home/ko
+000002d0: 6c6c 612f 636c 6f6e 6564 5f6c 6962 732f  lla/cloned_libs/
+000002e0: 6772 6565 6e5f 7473 6574 6c69 6e2f 646f  green_tsetlin/do
+000002f0: 6373 2f69 6e64 6578 2e72 7374 948c 046c  cs/index.rst...l
+00000300: 696e 6594 4b05 7562 6809 8c07 7365 6374  ine.K.ubh...sect
+00000310: 696f 6e94 9394 2981 947d 9428 6805 6806  ion...)..}.(h.h.
+00000320: 6807 5d94 2868 098c 0574 6974 6c65 9493  h.].(h...title..
+00000330: 9429 8194 7d94 2868 058c 1b47 7265 656e  .)..}.(h...Green
+00000340: 2054 7365 746c 696e 2064 6f63 756d 656e   Tsetlin documen
+00000350: 7461 7469 6f6e 9468 075d 9468 118c 1b47  tation.h.].h...G
+00000360: 7265 656e 2054 7365 746c 696e 2064 6f63  reen Tsetlin doc
+00000370: 756d 656e 7461 7469 6f6e 9485 9481 947d  umentation.....}
+00000380: 9428 6816 6831 6826 6803 6827 4e68 294e  .(h.h1h&h.h'Nh)N
+00000390: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
+000003a0: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
+000003b0: 2f68 1668 2c68 2668 0368 2768 2868 294b  /h.h,h&h.h'h(h)K
+000003c0: 0775 6268 098c 0863 6f6d 706f 756e 6494  .ubh...compound.
+000003d0: 9394 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+000003e0: 6800 8c07 746f 6374 7265 6594 9394 2981  h...toctree...).
+000003f0: 947d 9428 6805 6806 6807 5d94 6817 7d94  .}.(h.h.h.].h.}.
+00000400: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
+00000410: 9468 215d 9468 168c 0569 6e64 6578 948c  .h!].h...index..
+00000420: 0765 6e74 7269 6573 945d 9428 4e8c 0c69  .entries.].(N..i
+00000430: 6e73 7461 6c6c 6174 696f 6e94 8694 4e8c  nstallation...N.
+00000440: 0865 7861 6d70 6c65 7394 8694 4e8c 0d67  .examples...N..g
+00000450: 7265 656e 5f74 7365 746c 696e 9486 9465  reen_tsetlin...e
+00000460: 8c0c 696e 636c 7564 6566 696c 6573 945d  ..includefiles.]
+00000470: 9428 6852 6854 6856 658c 086d 6178 6465  .(hRhThVe..maxde
+00000480: 7074 6894 4b02 8c07 6361 7074 696f 6e94  pth.K...caption.
+00000490: 8c09 436f 6e74 656e 7473 3a94 8c04 676c  ..Contents:...gl
+000004a0: 6f62 9489 8c06 6869 6464 656e 9489 8c0d  ob....hidden....
+000004b0: 696e 636c 7564 6568 6964 6465 6e94 898c  includehidden...
+000004c0: 086e 756d 6265 7265 6494 4b00 8c0a 7469  .numbered.K...ti
+000004d0: 746c 6573 6f6e 6c79 9489 8c0a 7261 7765  tlesonly....rawe
+000004e0: 6e74 7269 6573 945d 948c 0a72 6177 6361  ntries.]...rawca
+000004f0: 7074 696f 6e94 685c 7568 2568 4468 2768  ption.h\uh%hDh'h
+00000500: 2868 294b 0968 1668 4175 6261 6817 7d94  (h)K.h.hAubah.}.
+00000510: 2868 195d 9468 1b5d 948c 0f74 6f63 7472  (h.].h.]...toctr
+00000520: 6565 2d77 7261 7070 6572 9461 681d 5d94  ee-wrapper.ah.].
+00000530: 681f 5d94 6821 5d94 7568 2568 3f68 1668  h.].h!].uh%h?h.h
+00000540: 2c68 2668 0368 2768 2868 294e 7562 6568  ,h&h.h'h(h)Nubeh
+00000550: 177d 9428 6819 5d94 8c1b 6772 6565 6e2d  .}.(h.]...green-
+00000560: 7473 6574 6c69 6e2d 646f 6375 6d65 6e74  tsetlin-document
+00000570: 6174 696f 6e94 6168 1b5d 9468 1d5d 948c  ation.ah.].h.]..
+00000580: 1b67 7265 656e 2074 7365 746c 696e 2064  .green tsetlin d
+00000590: 6f63 756d 656e 7461 7469 6f6e 9461 681f  ocumentation.ah.
+000005a0: 5d94 6821 5d94 7568 2568 2a68 1668 0368  ].h!].uh%h*h.h.h
+000005b0: 2668 0368 2768 2868 294b 0775 6268 2b29  &h.h'h(h)K.ubh+)
+000005c0: 8194 7d94 2868 0568 0668 075d 9428 6830  ..}.(h.h.h.].(h0
+000005d0: 2981 947d 9428 6805 8c12 496e 6469 6365  )..}.(h...Indice
+000005e0: 7320 616e 6420 7461 626c 6573 9468 075d  s and tables.h.]
+000005f0: 9468 118c 1249 6e64 6963 6573 2061 6e64  .h...Indices and
+00000600: 2074 6162 6c65 7394 8594 8194 7d94 2868   tables.....}.(h
+00000610: 1668 7768 2668 0368 274e 6829 4e75 6261  .hwh&h.h'Nh)Nuba
+00000620: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+00000630: 9468 1f5d 9468 215d 9475 6825 682f 6816  .h.].h!].uh%h/h.
+00000640: 6874 6826 6803 6827 6828 6829 4b13 7562  hth&h.h'h(h)K.ub
+00000650: 6809 8c0b 6275 6c6c 6574 5f6c 6973 7494  h...bullet_list.
+00000660: 9394 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+00000670: 6809 8c09 6c69 7374 5f69 7465 6d94 9394  h...list_item...
+00000680: 2981 947d 9428 6805 8c0f 3a72 6566 3a60  )..}.(h...:ref:`
+00000690: 6765 6e69 6e64 6578 6094 6807 5d94 6809  genindex`.h.].h.
+000006a0: 8c09 7061 7261 6772 6170 6894 9394 2981  ..paragraph...).
+000006b0: 947d 9428 6805 688e 6807 5d94 6800 8c0c  .}.(h.h.h.].h...
+000006c0: 7065 6e64 696e 675f 7872 6566 9493 9429  pending_xref...)
+000006d0: 8194 7d94 2868 0568 8e68 075d 9468 098c  ..}.(h.h.h.].h..
+000006e0: 0669 6e6c 696e 6594 9394 2981 947d 9428  .inline...)..}.(
+000006f0: 6805 688e 6807 5d94 6811 8c08 6765 6e69  h.h.h.].h...geni
+00000700: 6e64 6578 9485 9481 947d 9428 6816 689c  ndex.....}.(h.h.
+00000710: 6826 6803 6827 4e68 294e 7562 6168 177d  h&h.h'Nh)Nubah.}
+00000720: 9428 6819 5d94 681b 5d94 288c 0478 7265  .(h.].h.].(..xre
+00000730: 6694 8c03 7374 6494 8c07 7374 642d 7265  f...std...std-re
+00000740: 6694 6568 1d5d 9468 1f5d 9468 215d 9475  f.eh.].h.].h!].u
+00000750: 6825 689a 6816 6897 7562 6168 177d 9428  h%h.h.h.ubah.}.(
+00000760: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+00000770: 6821 5d94 8c06 7265 6664 6f63 9468 4f8c  h!]...refdoc.hO.
+00000780: 0972 6566 646f 6d61 696e 9468 a78c 0772  .refdomain.h...r
+00000790: 6566 7479 7065 948c 0372 6566 948c 0b72  eftype...ref...r
+000007a0: 6566 6578 706c 6963 6974 9489 8c07 7265  efexplicit....re
+000007b0: 6677 6172 6e94 888c 0972 6566 7461 7267  fwarn....reftarg
+000007c0: 6574 948c 0867 656e 696e 6465 7894 7568  et...genindex.uh
+000007d0: 2568 9568 2768 2868 294b 1568 1668 9275  %h.h'h(h)K.h.h.u
+000007e0: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+000007f0: 1d5d 9468 1f5d 9468 215d 9475 6825 6890  .].h.].h!].uh%h.
+00000800: 6827 6828 6829 4b15 6816 688c 7562 6168  h'h(h)K.h.h.ubah
+00000810: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00000820: 681f 5d94 6821 5d94 7568 2568 8a68 1668  h.].h!].uh%h.h.h
+00000830: 8768 2668 0368 2768 2868 294e 7562 6168  .h&h.h'h(h)Nubah
+00000840: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00000850: 681f 5d94 6821 5d94 8c06 6275 6c6c 6574  h.].h!]...bullet
+00000860: 948c 012a 9475 6825 6885 6827 6828 6829  ...*.uh%h.h'h(h)
+00000870: 4b15 6816 6874 6826 6803 7562 6568 177d  K.h.hth&h.ubeh.}
+00000880: 9428 6819 5d94 8c12 696e 6469 6365 732d  .(h.]...indices-
+00000890: 616e 642d 7461 626c 6573 9461 681b 5d94  and-tables.ah.].
+000008a0: 681d 5d94 8c12 696e 6469 6365 7320 616e  h.]...indices an
+000008b0: 6420 7461 626c 6573 9461 681f 5d94 6821  d tables.ah.].h!
+000008c0: 5d94 7568 2568 2a68 1668 0368 2668 0368  ].uh%h*h.h.h&h.h
+000008d0: 2768 2868 294b 1375 6265 6817 7d94 2868  'h(h)K.ubeh.}.(h
+000008e0: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
+000008f0: 215d 948c 0673 6f75 7263 6594 6828 8c14  !]...source.h(..
+00000900: 7472 616e 736c 6174 696f 6e5f 7072 6f67  translation_prog
+00000910: 7265 7373 947d 9428 8c05 746f 7461 6c94  ress.}.(..total.
+00000920: 4b00 8c0a 7472 616e 736c 6174 6564 944b  K...translated.K
+00000930: 0075 7568 2568 018c 0e63 7572 7265 6e74  .uuh%h...current
+00000940: 5f73 6f75 7263 6594 4e8c 0c63 7572 7265  _source.N..curre
+00000950: 6e74 5f6c 696e 6594 4e8c 0873 6574 7469  nt_line.N..setti
+00000960: 6e67 7394 8c11 646f 6375 7469 6c73 2e66  ngs...docutils.f
+00000970: 726f 6e74 656e 6494 8c06 5661 6c75 6573  rontend...Values
+00000980: 9493 9429 8194 7d94 288c 066f 7574 7075  ...)..}.(..outpu
+00000990: 7494 4e68 2f4e 8c09 6765 6e65 7261 746f  t.Nh/N..generato
+000009a0: 7294 4e8c 0964 6174 6573 7461 6d70 944e  r.N..datestamp.N
+000009b0: 8c0b 736f 7572 6365 5f6c 696e 6b94 4e8c  ..source_link.N.
+000009c0: 0a73 6f75 7263 655f 7572 6c94 4e8c 0d74  .source_url.N..t
+000009d0: 6f63 5f62 6163 6b6c 696e 6b73 948c 0565  oc_backlinks...e
+000009e0: 6e74 7279 948c 1266 6f6f 746e 6f74 655f  ntry...footnote_
+000009f0: 6261 636b 6c69 6e6b 7394 4b01 8c0d 7365  backlinks.K...se
+00000a00: 6374 6e75 6d5f 7866 6f72 6d94 4b01 8c0e  ctnum_xform.K...
+00000a10: 7374 7269 705f 636f 6d6d 656e 7473 944e  strip_comments.N
+00000a20: 8c1b 7374 7269 705f 656c 656d 656e 7473  ..strip_elements
+00000a30: 5f77 6974 685f 636c 6173 7365 7394 4e8c  _with_classes.N.
+00000a40: 0d73 7472 6970 5f63 6c61 7373 6573 944e  .strip_classes.N
+00000a50: 8c0c 7265 706f 7274 5f6c 6576 656c 944b  ..report_level.K
+00000a60: 028c 0a68 616c 745f 6c65 7665 6c94 4b05  ...halt_level.K.
+00000a70: 8c11 6578 6974 5f73 7461 7475 735f 6c65  ..exit_status_le
+00000a80: 7665 6c94 4b05 8c05 6465 6275 6794 4e8c  vel.K...debug.N.
+00000a90: 0e77 6172 6e69 6e67 5f73 7472 6561 6d94  .warning_stream.
+00000aa0: 4e8c 0974 7261 6365 6261 636b 9488 8c0e  N..traceback....
+00000ab0: 696e 7075 745f 656e 636f 6469 6e67 948c  input_encoding..
+00000ac0: 0975 7466 2d38 2d73 6967 948c 1c69 6e70  .utf-8-sig...inp
+00000ad0: 7574 5f65 6e63 6f64 696e 675f 6572 726f  ut_encoding_erro
+00000ae0: 725f 6861 6e64 6c65 7294 8c06 7374 7269  r_handler...stri
+00000af0: 6374 948c 0f6f 7574 7075 745f 656e 636f  ct...output_enco
+00000b00: 6469 6e67 948c 0575 7466 2d38 948c 1d6f  ding...utf-8...o
+00000b10: 7574 7075 745f 656e 636f 6469 6e67 5f65  utput_encoding_e
+00000b20: 7272 6f72 5f68 616e 646c 6572 9468 fe8c  rror_handler.h..
+00000b30: 0e65 7272 6f72 5f65 6e63 6f64 696e 6794  .error_encoding.
+00000b40: 8c05 7574 662d 3894 8c1c 6572 726f 725f  ..utf-8...error_
+00000b50: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
+00000b60: 616e 646c 6572 948c 1062 6163 6b73 6c61  andler...backsla
+00000b70: 7368 7265 706c 6163 6594 8c0d 6c61 6e67  shreplace...lang
+00000b80: 7561 6765 5f63 6f64 6594 8c02 656e 948c  uage_code...en..
+00000b90: 1372 6563 6f72 645f 6465 7065 6e64 656e  .record_dependen
+00000ba0: 6369 6573 944e 8c06 636f 6e66 6967 944e  cies.N..config.N
+00000bb0: 8c09 6964 5f70 7265 6669 7894 6806 8c0e  ..id_prefix.h...
+00000bc0: 6175 746f 5f69 645f 7072 6566 6978 948c  auto_id_prefix..
+00000bd0: 0269 6494 8c0d 6475 6d70 5f73 6574 7469  .id...dump_setti
+00000be0: 6e67 7394 4e8c 0e64 756d 705f 696e 7465  ngs.N..dump_inte
+00000bf0: 726e 616c 7394 4e8c 0f64 756d 705f 7472  rnals.N..dump_tr
+00000c00: 616e 7366 6f72 6d73 944e 8c0f 6475 6d70  ansforms.N..dump
+00000c10: 5f70 7365 7564 6f5f 786d 6c94 4e8c 1065  _pseudo_xml.N..e
+00000c20: 7870 6f73 655f 696e 7465 726e 616c 7394  xpose_internals.
+00000c30: 4e8c 0e73 7472 6963 745f 7669 7369 746f  N..strict_visito
+00000c40: 7294 4e8c 0f5f 6469 7361 626c 655f 636f  r.N.._disable_co
+00000c50: 6e66 6967 944e 8c07 5f73 6f75 7263 6594  nfig.N.._source.
+00000c60: 6828 8c0c 5f64 6573 7469 6e61 7469 6f6e  h(.._destination
+00000c70: 944e 8c0d 5f63 6f6e 6669 675f 6669 6c65  .N.._config_file
+00000c80: 7394 5d94 8c16 6669 6c65 5f69 6e73 6572  s.]...file_inser
+00000c90: 7469 6f6e 5f65 6e61 626c 6564 9488 8c0b  tion_enabled....
+00000ca0: 7261 775f 656e 6162 6c65 6494 4b01 8c11  raw_enabled.K...
+00000cb0: 6c69 6e65 5f6c 656e 6774 685f 6c69 6d69  line_length_limi
+00000cc0: 7494 4a00 e1f5 058c 0e70 6570 5f72 6566  t.J......pep_ref
+00000cd0: 6572 656e 6365 7394 4e8c 0c70 6570 5f62  erences.N..pep_b
+00000ce0: 6173 655f 7572 6c94 8c18 6874 7470 733a  ase_url...https:
+00000cf0: 2f2f 7065 7073 2e70 7974 686f 6e2e 6f72  //peps.python.or
+00000d00: 672f 948c 1570 6570 5f66 696c 655f 7572  g/...pep_file_ur
+00000d10: 6c5f 7465 6d70 6c61 7465 948c 0870 6570  l_template...pep
+00000d20: 2d25 3034 6494 8c0e 7266 635f 7265 6665  -%04d...rfc_refe
+00000d30: 7265 6e63 6573 944e 8c0c 7266 635f 6261  rences.N..rfc_ba
+00000d40: 7365 5f75 726c 948c 2668 7474 7073 3a2f  se_url..&https:/
+00000d50: 2f64 6174 6174 7261 636b 6572 2e69 6574  /datatracker.iet
+00000d60: 662e 6f72 672f 646f 632f 6874 6d6c 2f94  f.org/doc/html/.
+00000d70: 8c09 7461 625f 7769 6474 6894 4b08 8c1d  ..tab_width.K...
+00000d80: 7472 696d 5f66 6f6f 746e 6f74 655f 7265  trim_footnote_re
+00000d90: 6665 7265 6e63 655f 7370 6163 6594 898c  ference_space...
+00000da0: 1073 796e 7461 785f 6869 6768 6c69 6768  .syntax_highligh
+00000db0: 7494 8c04 6c6f 6e67 948c 0c73 6d61 7274  t...long...smart
+00000dc0: 5f71 756f 7465 7394 888c 1373 6d61 7274  _quotes....smart
+00000dd0: 7175 6f74 6573 5f6c 6f63 616c 6573 945d  quotes_locales.]
+00000de0: 948c 1d63 6861 7261 6374 6572 5f6c 6576  ...character_lev
+00000df0: 656c 5f69 6e6c 696e 655f 6d61 726b 7570  el_inline_markup
+00000e00: 9489 8c0e 646f 6374 6974 6c65 5f78 666f  ....doctitle_xfo
+00000e10: 726d 9489 8c0d 646f 6369 6e66 6f5f 7866  rm....docinfo_xf
+00000e20: 6f72 6d94 4b01 8c12 7365 6374 7375 6274  orm.K...sectsubt
+00000e30: 6974 6c65 5f78 666f 726d 9489 8c0d 696d  itle_xform....im
+00000e40: 6167 655f 6c6f 6164 696e 6794 8c04 6c69  age_loading...li
+00000e50: 6e6b 948c 1065 6d62 6564 5f73 7479 6c65  nk...embed_style
+00000e60: 7368 6565 7494 898c 1563 6c6f 616b 5f65  sheet....cloak_e
+00000e70: 6d61 696c 5f61 6464 7265 7373 6573 9488  mail_addresses..
+00000e80: 8c11 7365 6374 696f 6e5f 7365 6c66 5f6c  ..section_self_l
+00000e90: 696e 6b94 898c 0365 6e76 944e 7562 8c08  ink....env.Nub..
+00000ea0: 7265 706f 7274 6572 944e 8c10 696e 6469  reporter.N..indi
+00000eb0: 7265 6374 5f74 6172 6765 7473 945d 948c  rect_targets.]..
+00000ec0: 1173 7562 7374 6974 7574 696f 6e5f 6465  .substitution_de
+00000ed0: 6673 947d 948c 1273 7562 7374 6974 7574  fs.}...substitut
+00000ee0: 696f 6e5f 6e61 6d65 7394 7d94 8c08 7265  ion_names.}...re
+00000ef0: 666e 616d 6573 947d 948c 0672 6566 6964  fnames.}...refid
+00000f00: 7394 7d94 8c07 6e61 6d65 6964 7394 7d94  s.}...nameids.}.
+00000f10: 2868 7168 6e68 d368 d075 8c09 6e61 6d65  (hqhnh.h.u..name
+00000f20: 7479 7065 7394 7d94 2868 7189 68d3 8975  types.}.(hq.h..u
+00000f30: 6819 7d94 2868 6e68 2c68 d068 7475 8c0d  h.}.(hnh,h.htu..
+00000f40: 666f 6f74 6e6f 7465 5f72 6566 7394 7d94  footnote_refs.}.
+00000f50: 8c0d 6369 7461 7469 6f6e 5f72 6566 7394  ..citation_refs.
+00000f60: 7d94 8c0d 6175 746f 666f 6f74 6e6f 7465  }...autofootnote
+00000f70: 7394 5d94 8c11 6175 746f 666f 6f74 6e6f  s.]...autofootno
+00000f80: 7465 5f72 6566 7394 5d94 8c10 7379 6d62  te_refs.]...symb
+00000f90: 6f6c 5f66 6f6f 746e 6f74 6573 945d 948c  ol_footnotes.]..
+00000fa0: 1473 796d 626f 6c5f 666f 6f74 6e6f 7465  .symbol_footnote
+00000fb0: 5f72 6566 7394 5d94 8c09 666f 6f74 6e6f  _refs.]...footno
+00000fc0: 7465 7394 5d94 8c09 6369 7461 7469 6f6e  tes.]...citation
+00000fd0: 7394 5d94 8c12 6175 746f 666f 6f74 6e6f  s.]...autofootno
+00000fe0: 7465 5f73 7461 7274 944b 018c 1573 796d  te_start.K...sym
+00000ff0: 626f 6c5f 666f 6f74 6e6f 7465 5f73 7461  bol_footnote_sta
+00001000: 7274 944b 008c 0a69 645f 636f 756e 7465  rt.K...id_counte
+00001010: 7294 8c0b 636f 6c6c 6563 7469 6f6e 7394  r...collections.
+00001020: 8c07 436f 756e 7465 7294 9394 7d94 8594  ..Counter...}...
+00001030: 5294 8c0e 7061 7273 655f 6d65 7373 6167  R...parse_messag
+00001040: 6573 945d 948c 1274 7261 6e73 666f 726d  es.]...transform
+00001050: 5f6d 6573 7361 6765 7394 5d94 8c0b 7472  _messages.]...tr
+00001060: 616e 7366 6f72 6d65 7294 4e8c 0b69 6e63  ansformer.N..inc
+00001070: 6c75 6465 5f6c 6f67 945d 948c 0a64 6563  lude_log.]...dec
+00001080: 6f72 6174 696f 6e94 4e68 2668 0375 622e  oration.Nh&h.ub.
```

### Comparing `green_tsetlin-0.1.9/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `green_tsetlin-1.0.0/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,12 @@
-/*
- * _sphinx_javascript_frameworks_compat.js
- * ~~~~~~~~~~
+/* Compatability shim for jQuery and underscores.js.
  *
- * Compatability shim for jQuery and underscores.js.
- *
- * WILL BE REMOVED IN Sphinx 6.0
- * xref RemovedInSphinx60Warning
- *
- */
-
-/**
- * select a different prefix for underscore
+ * Copyright Sphinx contributors
+ * Released under the two clause BSD licence
  */
-$u = _.noConflict();
-
 
 /**
  * small helper function to urldecode strings
  *
  * See https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/decodeURIComponent#Decoding_query_parameters_from_a_URL
  */
 jQuery.urldecode = function(x) {
```

### Comparing `green_tsetlin-0.1.9/docs/_build/html/_static/basic.css` & `green_tsetlin-1.0.0/docs/_build/html/_static/basic.css`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * basic.css
  * ~~~~~~~~~
  *
  * Sphinx stylesheet -- basic theme.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 /* -- main layout ----------------------------------------------------------- */
 
 div.clearer {
@@ -233,14 +233,18 @@
     hyphens: auto;
 }
 
 a.headerlink {
     visibility: hidden;
 }
 
+a:visited {
+    color: #551A8B;
+}
+
 h1:hover > a.headerlink,
 h2:hover > a.headerlink,
 h3:hover > a.headerlink,
 h4:hover > a.headerlink,
 h5:hover > a.headerlink,
 h6:hover > a.headerlink,
 dt:hover > a.headerlink,
@@ -320,25 +324,25 @@
     clear: right;
     overflow-x: auto;
 }
 
 p.sidebar-title {
     font-weight: bold;
 }
+
 nav.contents,
 aside.topic,
-
 div.admonition, div.topic, blockquote {
     clear: left;
 }
 
 /* -- topics ---------------------------------------------------------------- */
+
 nav.contents,
 aside.topic,
-
 div.topic {
     border: 1px solid #ccc;
     padding: 7px;
     margin: 10px 0 10px 0;
 }
 
 p.topic-title {
@@ -371,25 +375,23 @@
 
 /* -- content of sidebars/topics/admonitions -------------------------------- */
 
 div.sidebar > :last-child,
 aside.sidebar > :last-child,
 nav.contents > :last-child,
 aside.topic > :last-child,
-
 div.topic > :last-child,
 div.admonition > :last-child {
     margin-bottom: 0;
 }
 
 div.sidebar::after,
 aside.sidebar::after,
 nav.contents::after,
 aside.topic::after,
-
 div.topic::after,
 div.admonition::after,
 blockquote::after {
     display: block;
     content: '';
     clear: both;
 }
@@ -607,33 +609,14 @@
 }
 
 ol.simple p,
 ul.simple p {
     margin-bottom: 0;
 }
 
-/* Docutils 0.17 and older (footnotes & citations) */
-dl.footnote > dt,
-dl.citation > dt {
-    float: left;
-    margin-right: 0.5em;
-}
-
-dl.footnote > dd,
-dl.citation > dd {
-    margin-bottom: 0em;
-}
-
-dl.footnote > dd:after,
-dl.citation > dd:after {
-    content: "";
-    clear: both;
-}
-
-/* Docutils 0.18+ (footnotes & citations) */
 aside.footnote > span,
 div.citation > span {
     float: left;
 }
 aside.footnote > span:last-of-type,
 div.citation > span:last-of-type {
   padding-right: 0.5em;
@@ -650,32 +633,26 @@
 }
 aside.footnote > p:last-of-type:after,
 div.citation > p:last-of-type:after {
     content: "";
     clear: both;
 }
 
-/* Footnotes & citations ends */
-
 dl.field-list {
     display: grid;
     grid-template-columns: fit-content(30%) auto;
 }
 
 dl.field-list > dt {
     font-weight: bold;
     word-break: break-word;
     padding-left: 0.5em;
     padding-right: 5px;
 }
 
-dl.field-list > dt:after {
-    content: ":";
-}
-
 dl.field-list > dd {
     padding-left: 0.5em;
     margin-top: 0em;
     margin-left: 0em;
     margin-bottom: 0em;
 }
 
@@ -693,14 +670,24 @@
 
 dd {
     margin-top: 3px;
     margin-bottom: 10px;
     margin-left: 30px;
 }
 
+.sig dd {
+    margin-top: 0px;
+    margin-bottom: 0px;
+}
+
+.sig dl {
+    margin-top: 0px;
+    margin-bottom: 0px;
+}
+
 dl > dd:last-child,
 dl > dd:last-child > :last-child {
     margin-bottom: 0;
 }
 
 dt:target, span.highlighted {
     background-color: #fbe54e;
@@ -761,14 +748,22 @@
 }
 
 abbr, acronym {
     border-bottom: dotted 1px;
     cursor: help;
 }
 
+.translated {
+    background-color: rgba(207, 255, 207, 0.2)
+}
+
+.untranslated {
+    background-color: rgba(255, 207, 207, 0.2)
+}
+
 /* -- code displays --------------------------------------------------------- */
 
 pre {
     overflow: auto;
     overflow-y: hidden;  /* fixes display issues on Chrome browsers */
 }
```

### Comparing `green_tsetlin-0.1.9/docs/_build/html/_static/jquery.js` & `green_tsetlin-1.0.0/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.9/docs/_build/html/_static/language_data.js` & `green_tsetlin-1.0.0/docs/_build/html/_static/language_data.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 /*
  * language_data.js
  * ~~~~~~~~~~~~~~~~
  *
  * This script contains the language-specific data used by searchtools.js,
  * namely the list of stopwords, stemmer, scorer and splitter.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 var stopwords = ["a", "and", "are", "as", "at", "be", "but", "by", "for", "if", "in", "into", "is", "it", "near", "no", "not", "of", "on", "or", "such", "that", "the", "their", "then", "there", "these", "they", "this", "to", "was", "will", "with"];
```

### Comparing `green_tsetlin-0.1.9/docs/_build/html/_static/pygments.css` & `green_tsetlin-1.0.0/docs/_build/html/_static/pygments.css`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,75 @@
 pre { line-height: 125%; }
 td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 .highlight .hll { background-color: #ffffcc }
 .highlight { background: #f8f8f8; }
-.highlight .c { color: #8f5902; font-style: italic } /* Comment */
-.highlight .err { color: #a40000; border: 1px solid #ef2929 } /* Error */
-.highlight .g { color: #000000 } /* Generic */
-.highlight .k { color: #004461; font-weight: bold } /* Keyword */
-.highlight .l { color: #000000 } /* Literal */
-.highlight .n { color: #000000 } /* Name */
-.highlight .o { color: #582800 } /* Operator */
-.highlight .x { color: #000000 } /* Other */
-.highlight .p { color: #000000; font-weight: bold } /* Punctuation */
-.highlight .ch { color: #8f5902; font-style: italic } /* Comment.Hashbang */
-.highlight .cm { color: #8f5902; font-style: italic } /* Comment.Multiline */
-.highlight .cp { color: #8f5902 } /* Comment.Preproc */
-.highlight .cpf { color: #8f5902; font-style: italic } /* Comment.PreprocFile */
-.highlight .c1 { color: #8f5902; font-style: italic } /* Comment.Single */
-.highlight .cs { color: #8f5902; font-style: italic } /* Comment.Special */
-.highlight .gd { color: #a40000 } /* Generic.Deleted */
-.highlight .ge { color: #000000; font-style: italic } /* Generic.Emph */
-.highlight .gr { color: #ef2929 } /* Generic.Error */
+.highlight .c { color: #3D7B7B; font-style: italic } /* Comment */
+.highlight .err { border: 1px solid #FF0000 } /* Error */
+.highlight .k { color: #008000; font-weight: bold } /* Keyword */
+.highlight .o { color: #666666 } /* Operator */
+.highlight .ch { color: #3D7B7B; font-style: italic } /* Comment.Hashbang */
+.highlight .cm { color: #3D7B7B; font-style: italic } /* Comment.Multiline */
+.highlight .cp { color: #9C6500 } /* Comment.Preproc */
+.highlight .cpf { color: #3D7B7B; font-style: italic } /* Comment.PreprocFile */
+.highlight .c1 { color: #3D7B7B; font-style: italic } /* Comment.Single */
+.highlight .cs { color: #3D7B7B; font-style: italic } /* Comment.Special */
+.highlight .gd { color: #A00000 } /* Generic.Deleted */
+.highlight .ge { font-style: italic } /* Generic.Emph */
+.highlight .ges { font-weight: bold; font-style: italic } /* Generic.EmphStrong */
+.highlight .gr { color: #E40000 } /* Generic.Error */
 .highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
-.highlight .gi { color: #00A000 } /* Generic.Inserted */
-.highlight .go { color: #888888 } /* Generic.Output */
-.highlight .gp { color: #745334 } /* Generic.Prompt */
-.highlight .gs { color: #000000; font-weight: bold } /* Generic.Strong */
+.highlight .gi { color: #008400 } /* Generic.Inserted */
+.highlight .go { color: #717171 } /* Generic.Output */
+.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
+.highlight .gs { font-weight: bold } /* Generic.Strong */
 .highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
-.highlight .gt { color: #a40000; font-weight: bold } /* Generic.Traceback */
-.highlight .kc { color: #004461; font-weight: bold } /* Keyword.Constant */
-.highlight .kd { color: #004461; font-weight: bold } /* Keyword.Declaration */
-.highlight .kn { color: #004461; font-weight: bold } /* Keyword.Namespace */
-.highlight .kp { color: #004461; font-weight: bold } /* Keyword.Pseudo */
-.highlight .kr { color: #004461; font-weight: bold } /* Keyword.Reserved */
-.highlight .kt { color: #004461; font-weight: bold } /* Keyword.Type */
-.highlight .ld { color: #000000 } /* Literal.Date */
-.highlight .m { color: #990000 } /* Literal.Number */
-.highlight .s { color: #4e9a06 } /* Literal.String */
-.highlight .na { color: #c4a000 } /* Name.Attribute */
-.highlight .nb { color: #004461 } /* Name.Builtin */
-.highlight .nc { color: #000000 } /* Name.Class */
-.highlight .no { color: #000000 } /* Name.Constant */
-.highlight .nd { color: #888888 } /* Name.Decorator */
-.highlight .ni { color: #ce5c00 } /* Name.Entity */
-.highlight .ne { color: #cc0000; font-weight: bold } /* Name.Exception */
-.highlight .nf { color: #000000 } /* Name.Function */
-.highlight .nl { color: #f57900 } /* Name.Label */
-.highlight .nn { color: #000000 } /* Name.Namespace */
-.highlight .nx { color: #000000 } /* Name.Other */
-.highlight .py { color: #000000 } /* Name.Property */
-.highlight .nt { color: #004461; font-weight: bold } /* Name.Tag */
-.highlight .nv { color: #000000 } /* Name.Variable */
-.highlight .ow { color: #004461; font-weight: bold } /* Operator.Word */
-.highlight .w { color: #f8f8f8; text-decoration: underline } /* Text.Whitespace */
-.highlight .mb { color: #990000 } /* Literal.Number.Bin */
-.highlight .mf { color: #990000 } /* Literal.Number.Float */
-.highlight .mh { color: #990000 } /* Literal.Number.Hex */
-.highlight .mi { color: #990000 } /* Literal.Number.Integer */
-.highlight .mo { color: #990000 } /* Literal.Number.Oct */
-.highlight .sa { color: #4e9a06 } /* Literal.String.Affix */
-.highlight .sb { color: #4e9a06 } /* Literal.String.Backtick */
-.highlight .sc { color: #4e9a06 } /* Literal.String.Char */
-.highlight .dl { color: #4e9a06 } /* Literal.String.Delimiter */
-.highlight .sd { color: #8f5902; font-style: italic } /* Literal.String.Doc */
-.highlight .s2 { color: #4e9a06 } /* Literal.String.Double */
-.highlight .se { color: #4e9a06 } /* Literal.String.Escape */
-.highlight .sh { color: #4e9a06 } /* Literal.String.Heredoc */
-.highlight .si { color: #4e9a06 } /* Literal.String.Interpol */
-.highlight .sx { color: #4e9a06 } /* Literal.String.Other */
-.highlight .sr { color: #4e9a06 } /* Literal.String.Regex */
-.highlight .s1 { color: #4e9a06 } /* Literal.String.Single */
-.highlight .ss { color: #4e9a06 } /* Literal.String.Symbol */
-.highlight .bp { color: #3465a4 } /* Name.Builtin.Pseudo */
-.highlight .fm { color: #000000 } /* Name.Function.Magic */
-.highlight .vc { color: #000000 } /* Name.Variable.Class */
-.highlight .vg { color: #000000 } /* Name.Variable.Global */
-.highlight .vi { color: #000000 } /* Name.Variable.Instance */
-.highlight .vm { color: #000000 } /* Name.Variable.Magic */
-.highlight .il { color: #990000 } /* Literal.Number.Integer.Long */
+.highlight .gt { color: #0044DD } /* Generic.Traceback */
+.highlight .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
+.highlight .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
+.highlight .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
+.highlight .kp { color: #008000 } /* Keyword.Pseudo */
+.highlight .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
+.highlight .kt { color: #B00040 } /* Keyword.Type */
+.highlight .m { color: #666666 } /* Literal.Number */
+.highlight .s { color: #BA2121 } /* Literal.String */
+.highlight .na { color: #687822 } /* Name.Attribute */
+.highlight .nb { color: #008000 } /* Name.Builtin */
+.highlight .nc { color: #0000FF; font-weight: bold } /* Name.Class */
+.highlight .no { color: #880000 } /* Name.Constant */
+.highlight .nd { color: #AA22FF } /* Name.Decorator */
+.highlight .ni { color: #717171; font-weight: bold } /* Name.Entity */
+.highlight .ne { color: #CB3F38; font-weight: bold } /* Name.Exception */
+.highlight .nf { color: #0000FF } /* Name.Function */
+.highlight .nl { color: #767600 } /* Name.Label */
+.highlight .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
+.highlight .nt { color: #008000; font-weight: bold } /* Name.Tag */
+.highlight .nv { color: #19177C } /* Name.Variable */
+.highlight .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
+.highlight .w { color: #bbbbbb } /* Text.Whitespace */
+.highlight .mb { color: #666666 } /* Literal.Number.Bin */
+.highlight .mf { color: #666666 } /* Literal.Number.Float */
+.highlight .mh { color: #666666 } /* Literal.Number.Hex */
+.highlight .mi { color: #666666 } /* Literal.Number.Integer */
+.highlight .mo { color: #666666 } /* Literal.Number.Oct */
+.highlight .sa { color: #BA2121 } /* Literal.String.Affix */
+.highlight .sb { color: #BA2121 } /* Literal.String.Backtick */
+.highlight .sc { color: #BA2121 } /* Literal.String.Char */
+.highlight .dl { color: #BA2121 } /* Literal.String.Delimiter */
+.highlight .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
+.highlight .s2 { color: #BA2121 } /* Literal.String.Double */
+.highlight .se { color: #AA5D1F; font-weight: bold } /* Literal.String.Escape */
+.highlight .sh { color: #BA2121 } /* Literal.String.Heredoc */
+.highlight .si { color: #A45A77; font-weight: bold } /* Literal.String.Interpol */
+.highlight .sx { color: #008000 } /* Literal.String.Other */
+.highlight .sr { color: #A45A77 } /* Literal.String.Regex */
+.highlight .s1 { color: #BA2121 } /* Literal.String.Single */
+.highlight .ss { color: #19177C } /* Literal.String.Symbol */
+.highlight .bp { color: #008000 } /* Name.Builtin.Pseudo */
+.highlight .fm { color: #0000FF } /* Name.Function.Magic */
+.highlight .vc { color: #19177C } /* Name.Variable.Class */
+.highlight .vg { color: #19177C } /* Name.Variable.Global */
+.highlight .vi { color: #19177C } /* Name.Variable.Instance */
+.highlight .vm { color: #19177C } /* Name.Variable.Magic */
+.highlight .il { color: #666666 } /* Literal.Number.Integer.Long */
```

### Comparing `green_tsetlin-0.1.9/docs/_build/html/_static/searchtools.js` & `green_tsetlin-1.0.0/docs/_build/html/_static/searchtools.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*
  * searchtools.js
  * ~~~~~~~~~~~~~~~~
  *
  * Sphinx JavaScript utilities for the full-text search.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 "use strict";
 
 /**
  * Simple result scoring code.
@@ -53,55 +53,60 @@
 
 /**
  * See https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions#escaping
  */
 const _escapeRegExp = (string) =>
     string.replace(/[.*+\-?^${}()|[\]\\]/g, "\\$&"); // $& means the whole matched string
 
-const _displayItem = (item, highlightTerms, searchTerms) => {
+const _displayItem = (item, searchTerms, highlightTerms) => {
     const docBuilder = DOCUMENTATION_OPTIONS.BUILDER;
-    const docUrlRoot = DOCUMENTATION_OPTIONS.URL_ROOT;
     const docFileSuffix = DOCUMENTATION_OPTIONS.FILE_SUFFIX;
     const docLinkSuffix = DOCUMENTATION_OPTIONS.LINK_SUFFIX;
     const showSearchSummary = DOCUMENTATION_OPTIONS.SHOW_SEARCH_SUMMARY;
+    const contentRoot = document.documentElement.dataset.content_root;
 
-    const [docName, title, anchor, descr] = item;
+    const [docName, title, anchor, descr, score, _filename] = item;
 
     let listItem = document.createElement("li");
     let requestUrl;
     let linkUrl;
     if (docBuilder === "dirhtml") {
         // dirhtml builder
         let dirname = docName + "/";
         if (dirname.match(/\/index\/$/))
             dirname = dirname.substring(0, dirname.length - 6);
         else if (dirname === "index/") dirname = "";
-        requestUrl = docUrlRoot + dirname;
+        requestUrl = contentRoot + dirname;
         linkUrl = requestUrl;
     } else {
         // normal html builders
-        requestUrl = docUrlRoot + docName + docFileSuffix;
+        requestUrl = contentRoot + docName + docFileSuffix;
         linkUrl = docName + docLinkSuffix;
     }
-    const params = new URLSearchParams();
-    params.set("highlight", [...highlightTerms].join(" "));
     let linkEl = listItem.appendChild(document.createElement("a"));
-    linkEl.href = linkUrl + "?" + params.toString() + anchor;
+    linkEl.href = linkUrl + anchor;
+    linkEl.dataset.score = score;
     linkEl.innerHTML = title;
-    if (descr)
-        listItem.appendChild(document.createElement("span")).innerText =
-        " (" + descr + ")";
-    else if (showSearchSummary)
+    if (descr) {
+        listItem.appendChild(document.createElement("span")).innerHTML =
+            " (" + descr + ")";
+        // highlight search terms in the description
+        if (SPHINX_HIGHLIGHT_ENABLED) // set in sphinx_highlight.js
+            highlightTerms.forEach((term) => _highlightText(listItem, term, "highlighted"));
+    } else if (showSearchSummary)
         fetch(requestUrl)
         .then((responseData) => responseData.text())
         .then((data) => {
             if (data)
                 listItem.appendChild(
-                    Search.makeSearchSummary(data, searchTerms, highlightTerms)
+                    Search.makeSearchSummary(data, searchTerms)
                 );
+            // highlight search terms in the summary
+            if (SPHINX_HIGHLIGHT_ENABLED) // set in sphinx_highlight.js
+                highlightTerms.forEach((term) => _highlightText(listItem, term, "highlighted"));
         });
     Search.output.appendChild(listItem);
 };
 const _finishSearch = (resultCount) => {
     Search.stopPulse();
     Search.title.innerText = _("Search Results");
     if (!resultCount)
@@ -112,23 +117,23 @@
         Search.status.innerText = _(
             `Search finished, found ${resultCount} page(s) matching the search query.`
         );
 };
 const _displayNextItem = (
     results,
     resultCount,
+    searchTerms,
     highlightTerms,
-    searchTerms
 ) => {
     // results left, load the summary and display it
     // this is intended to be dynamic (don't sub resultsCount)
     if (results.length) {
-        _displayItem(results.pop(), highlightTerms, searchTerms);
+        _displayItem(results.pop(), searchTerms, highlightTerms);
         setTimeout(
-            () => _displayNextItem(results, resultCount, highlightTerms, searchTerms),
+            () => _displayNextItem(results, resultCount, searchTerms, highlightTerms),
             5
         );
     }
     // search finished, update title and status message
     else _finishSearch(resultCount);
 };
 
@@ -151,18 +156,18 @@
  */
 const Search = {
     _index: null,
     _queued_query: null,
     _pulse_status: -1,
 
     htmlToText: (htmlString) => {
-        const htmlElement = document
-            .createRange()
-            .createContextualFragment(htmlString);
-        _removeChildren(htmlElement.querySelectorAll(".headerlink"));
+        const htmlElement = new DOMParser().parseFromString(htmlString, 'text/html');
+        htmlElement.querySelectorAll(".headerlink").forEach((el) => {
+            el.remove()
+        });
         const docContent = htmlElement.querySelector('[role="main"]');
         if (docContent !== undefined) return docContent.textContent;
         console.warn(
             "Content block not found. Sphinx search tries to obtain it via '[role=main]'. Could you check your theme or template."
         );
         return "";
     },
@@ -235,14 +240,20 @@
         else Search.deferQuery(query);
     },
 
     /**
      * execute search (requires search index to be loaded)
      */
     query: (query) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+        const allTitles = Search._index.alltitles;
+        const indexEntries = Search._index.indexentries;
+
         // stem the search terms and add them to the correct list
         const stemmer = new Stemmer();
         const searchTerms = new Set();
         const excludedTerms = new Set();
         const highlightTerms = new Set();
         const objectTerms = new Set(splitQuery(query.toLowerCase().trim()));
         splitQuery(query.trim()).forEach((queryTerm) => {
@@ -262,22 +273,60 @@
             if (word[0] === "-") excludedTerms.add(word.substr(1));
             else {
                 searchTerms.add(word);
                 highlightTerms.add(queryTermLower);
             }
         });
 
+        if (SPHINX_HIGHLIGHT_ENABLED) { // set in sphinx_highlight.js
+            localStorage.setItem("sphinx_highlight_terms", [...highlightTerms].join(" "))
+        }
+
         // console.debug("SEARCH: searching for:");
         // console.info("required: ", [...searchTerms]);
         // console.info("excluded: ", [...excludedTerms]);
 
         // array of [docname, title, anchor, descr, score, filename]
         let results = [];
         _removeChildren(document.getElementById("search-progress"));
 
+        const queryLower = query.toLowerCase();
+        for (const [title, foundTitles] of Object.entries(allTitles)) {
+            if (title.toLowerCase().includes(queryLower) && (queryLower.length >= title.length / 2)) {
+                for (const [file, id] of foundTitles) {
+                    let score = Math.round(100 * queryLower.length / title.length)
+                    results.push([
+                        docNames[file],
+                        titles[file] !== title ? `${titles[file]} > ${title}` : title,
+                        id !== null ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
+
+        // search for explicit entries in index directives
+        for (const [entry, foundEntries] of Object.entries(indexEntries)) {
+            if (entry.includes(queryLower) && (queryLower.length >= entry.length / 2)) {
+                for (const [file, id] of foundEntries) {
+                    let score = Math.round(100 * queryLower.length / entry.length)
+                    results.push([
+                        docNames[file],
+                        titles[file],
+                        id ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
+
         // lookup as object
         objectTerms.forEach((term) =>
             results.push(...Search.performObjectSearch(term, objectTerms))
         );
 
         // lookup as search terms in fulltext
         results.push(...Search.performTermsSearch(searchTerms, excludedTerms));
@@ -316,15 +365,15 @@
         results = results.reverse();
 
         // for debugging
         //Search.lastresults = results.slice();  // a copy
         // console.info("search results:", Search.lastresults);
 
         // print the results
-        _displayNextItem(results, results.length, highlightTerms, searchTerms);
+        _displayNextItem(results, results.length, searchTerms, highlightTerms);
     },
 
     /**
      * search for object names
      */
     performObjectSearch: (object, objectTerms) => {
         const filenames = Search._index.filenames;
@@ -397,16 +446,16 @@
     /**
      * search for full-text terms in the index
      */
     performTermsSearch: (searchTerms, excludedTerms) => {
         // prepare search
         const terms = Search._index.terms;
         const titleTerms = Search._index.titleterms;
-        const docNames = Search._index.docnames;
         const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
         const titles = Search._index.titles;
 
         const scoreMap = new Map();
         const fileMap = new Map();
 
         // perform the search on the required terms
         searchTerms.forEach((word) => {
@@ -504,37 +553,32 @@
         }
         return results;
     },
 
     /**
      * helper function to return a node containing the
      * search summary for a given text. keywords is a list
-     * of stemmed words, highlightWords is the list of normal, unstemmed
-     * words. the first one is used to find the occurrence, the
-     * latter for highlighting it.
+     * of stemmed words.
      */
-    makeSearchSummary: (htmlText, keywords, highlightWords) => {
-        const text = Search.htmlToText(htmlText).toLowerCase();
+    makeSearchSummary: (htmlText, keywords) => {
+        const text = Search.htmlToText(htmlText);
         if (text === "") return null;
 
+        const textLower = text.toLowerCase();
         const actualStartPosition = [...keywords]
-            .map((k) => text.indexOf(k.toLowerCase()))
+            .map((k) => textLower.indexOf(k.toLowerCase()))
             .filter((i) => i > -1)
             .slice(-1)[0];
         const startWithContext = Math.max(actualStartPosition - 120, 0);
 
         const top = startWithContext === 0 ? "" : "...";
         const tail = startWithContext + 240 < text.length ? "..." : "";
 
-        let summary = document.createElement("div");
+        let summary = document.createElement("p");
         summary.classList.add("context");
-        summary.innerText = top + text.substr(startWithContext, 240).trim() + tail;
-
-        highlightWords.forEach((highlightWord) =>
-            _highlightText(summary, highlightWord, "highlighted")
-        );
+        summary.textContent = top + text.substr(startWithContext, 240).trim() + tail;
 
         return summary;
     },
 };
 
 _ready(Search.init);
```

### Comparing `green_tsetlin-0.1.9/docs/make.bat` & `green_tsetlin-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.9/setup.py` & `green_tsetlin-1.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from cpuinfo import get_cpu_info
 from setuptools import setup
 
 import distutils
 distutils.log.set_verbosity(1)
 
 
-__version__ = "0.1.9"
+__version__ = "1.0.0"
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 cpu_info = get_cpu_info()
 has_avx2 = "avx2" in cpu_info.get("flags", "")
 
@@ -25,29 +25,29 @@
 
 
 
 compile_args = []
 define_macros = [('VERSION_INFO', __version__)]
 
 if sys.platform.startswith('darwin') and has_neon:
-    print("TODO: replace -mcpu=native with a proper build flag! ALSO: check if NEON is in flags somehow...")
+    # print("TODO: replace -mcpu=native with a proper build flag! ALSO: check if NEON is in flags somehow...")
     # compile_args = ["-target arm64-apple-macos11", "-arch=arm64", "-O3", "-mmacosx-version-min=10.15", "-mfloat-abi=hard"]  # -mfloat-abi=hard needs to be used with neon
     compile_args = ["-mcpu=native", "-arch=arm64", "-O3", "-mmacosx-version-min=10.15", "-mfloat-abi=hard"]  # -mfloat-abi=hard needs to be used with neon
 
     # also took out: "-arch=arm64", "-mfloat-abi=hard", 
     define_macros.append(("USE_NEON", 1))
 
 
 elif sys.platform.startswith('linux') or (sys.platform.startswith('darwin') and has_neon is False):    
     compile_args =["-mavx2", "-mfma", "-O3", "-pthread"]
 
     if has_avx2:
         define_macros.append(("USE_AVX2", 1))
      
-print("using defines:", define_macros)
+# print("using defines:", define_macros)
 
 ext_modules = [
     Pybind11Extension("green_tsetlin_core",
         ["src/main.cpp"],
         define_macros = define_macros,
         cxx_std=17,
         include_dirs=["src/"],       
@@ -64,40 +64,43 @@
     project_urls= {
         "Bug Tracker": "https://github.com/ooki/green_tsetlin/issues",
         "Documentation": "https://github.com/ooki/green_tsetlin",
         "Source Code": "https://github.com/ooki/green_tsetlin",
     },
     description="A fast Tsetlin Machine impl, based on c++",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: C",
+        "Programming Language :: C++",
         "Programming Language :: Python",
         "Topic :: Software Development",
         "Topic :: Scientific/Engineering",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Operating System :: MacOS",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",        
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12"
     ],
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     ext_modules=ext_modules,
     extras_require={"test": "pytest"},
     zip_safe=False,
     python_requires=">=3.8",
     packages=['green_tsetlin'],
     install_requires=[
           'numpy >= 1.24',
           'scipy >= 1.10.1',
           'scikit-learn >= 1.2',
-          'tqdm >= 4.65'
-          
+          'tqdm >= 4.65',
+          'optuna'
       ],
-    
 )
```

### Comparing `green_tsetlin-0.1.9/src/BS_thread_pool.hpp` & `green_tsetlin-1.0.0/src/BS_thread_pool.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.9/src/executor.hpp` & `green_tsetlin-1.0.0/src/executor.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,15 @@
 #ifndef __EXECUTOR_HPP_
 #define __EXECUTOR_HPP_
 
 
-#include <iostream>
-#include <vector>
-#include <stdexcept>
-#include <cstring>
-#include <thread>
-#include <mutex>
-#include <random>
-#include <vector>
 
 #include <BS_thread_pool.hpp>
 
 
-// #include <input_block.hpp>
-// #include <clause_block.hpp>
-// #include <feedback_block.hpp>
-
-
 namespace green_tsetlin
 {
     class InputBlock;
     class ClauseBlock;
     class FeedbackBlock;
 
     class DummyThreadPool
@@ -32,56 +19,45 @@
             DummyThreadPool(int i) {}
 
             void push_task(...) {}
             void wait_for_tasks() {}
 
 
     };
-    
+
+
     template <bool enable_multithread, typename _ThreadPool>
     class Executor    
     {
         public:
-            Executor(std::vector<InputBlock*> input_blocks, std::vector<ClauseBlock*> clause_blocks, FeedbackBlock* feedback_block, int seed)
-                : Executor(input_blocks, clause_blocks, feedback_block, 0, seed) {}
-
-            Executor(std::vector<InputBlock*> input_blocks, std::vector<ClauseBlock*> clause_blocks, FeedbackBlock* feedback_block, int num_threads, int seed)
+            Executor(InputBlock* input_block, std::vector<ClauseBlock*> clause_blocks, FeedbackBlock* feedback_block, int num_threads, int seed)
                 : m_pool(num_threads)
             {
-                if(input_blocks.size() < 1)
-                    throw std::runtime_error("Cannot create executor with 0 input blocks.");
+                if(!enable_multithread)
+                {
+                    if(num_threads != 1)
+                        throw std::runtime_error("Can only create a Single Thread Executor with num_threads set to 1.");                        
+                }
+
+                if(input_block == nullptr)
+                    throw std::runtime_error("Cannot create executor with nullptr input block.");
 
                 if(clause_blocks.size() < 1)
                     throw std::runtime_error("Cannot create executor with 0 clause blocks.");
 
                 if(feedback_block == nullptr)
                     throw std::runtime_error("Cannot create executor with a null feedback block.");
 
-                m_inputs = input_blocks;
+                m_input_block = input_block;
                 m_clause_blocks = clause_blocks;
                 m_feedback_block = feedback_block;
-                m_label_input = nullptr;
                 m_num_threads = num_threads;
 
-                for(auto ib : input_blocks)
-                {
-                    if(ib->is_label_block())
-                    {
-                        if(m_label_input != nullptr)                   
-                            throw std::runtime_error("Cannot have more than one LabelBlock in an Executor()");
-
-                        m_label_input = ib;                                            
-                    }
-                }
-
-                if(m_label_input == nullptr)                   
-                    throw std::runtime_error("No InputBlock is marked as a LabelBlock in an Executor()");
-
-                int n_labels_per_example = m_label_input->get_num_labels_per_example();
-                if(m_label_input->is_multi_label())
+                int n_labels_per_example = m_input_block->get_num_labels_per_example();
+                if(m_input_block->is_multi_label())
                 {
                     // std::cout << "exec:" << "n_labels_per_example: " << n_labels_per_example << " " << "#classes:" << feedback_block->get_number_of_classes() << std::endl;
                     if(n_labels_per_example != feedback_block->get_number_of_classes())
                         throw std::runtime_error("InputBlock is multilabel but Input labels does match feedback labels() in Executor()");
                     
                     for(auto cb : clause_blocks)
                     {
@@ -92,144 +68,180 @@
                 }
 
 
                 for( auto cb : clause_blocks )
                 {
                     if(!cb->is_init())                   
                         throw std::runtime_error("All ClauseBlocks must be init() before constructing an Executor()");
+
+                    if(cb->get_input_block() == nullptr)
+                        throw std::runtime_error("All ClauseBlocks must be have a InputBlock before constructing an Executor()");
+
+                    if(cb->get_feedback() == nullptr)
+                        throw std::runtime_error("All ClauseBlocks must be have a FeedbackBlock before constructing an Executor()");
+
+                    if(cb->is_trainable())
+                        m_trainable_clause_blocks.push_back(cb);
                 }
 
                 m_rng.seed(seed);                        
             }            
 
             double train_epoch()
-            {                
-                m_feedback_block->reset_train_predict_counter();                
+            {            
+                m_feedback_block->reset_train_predict_counter();             
+
                 int n_examples = get_number_of_examples_ready();
                 train_slice(0, n_examples);
 
                 return m_feedback_block->get_train_accuracy();
             }
 
             void train_slice(int start_index, int end_index)
-            {                                
+            {                            
                 int n_examples = get_number_of_examples_ready();
-                //bool m_label_input->is_multi_label();
                 
                 if(start_index == 0)
                 {                                       
                     //std::cout << "n_examples:" << n_examples << std::endl;
                     m_index_set.resize(n_examples);
                     std::iota (std::begin(m_index_set), std::end(m_index_set), 0); // fill 0 -> n_examples
                     std::shuffle(std::begin(m_index_set), std::end(m_index_set), m_rng);
                 }
-
                 
                 for(int i = start_index; i < end_index; ++i)
                 {
-                    
                     m_feedback_block->reset();
-
                     int example_index = m_index_set[i];
-                    for(auto ib : m_inputs)
-                    {                
-                        ib->prepare_example(example_index);
-                    }
+
+                    m_input_block->prepare_example(example_index);
 
                     for(auto cb : m_clause_blocks)
                     {             
                         if(enable_multithread)
                         {
                             m_pool.push_task(&ClauseBlock::train_example, cb);
                         }
                         else
                         {
                             cb->train_example();
-                        }
-                                       
+                        }                                       
                     }
 
                     if(enable_multithread)
                         m_pool.wait_for_tasks();
 
-
-                    m_feedback_block->process(m_label_input->pull_current_label());
+                    m_feedback_block->process(m_input_block->pull_current_label());
 
                     uint32_t positive_class = m_feedback_block->get_positive_class();
                     uint32_t negative_class = m_feedback_block->get_negative_class();
                     double pup = m_feedback_block->get_positive_update_probability();                    
                     double nup = m_feedback_block->get_negative_update_probability();
-                                                                                
-                    for(auto cb : m_clause_blocks)
-                    {      
+                    
+                    for(auto cb : m_trainable_clause_blocks)
+                    {   
+                        if(!cb->is_trainable())
+                            continue;
+
                         if(enable_multithread)
                             m_pool.push_task(&ClauseBlock::train_update, cb, positive_class, pup, negative_class, nup);
                         else                        
                             cb->train_update(positive_class, pup, negative_class, nup);
                     }
 
                     if(enable_multithread)
                         m_pool.wait_for_tasks();
                 }
             }
 
 
-           std::vector<int> eval_predict()
+           bool eval_predict(pybind11::array_t<uint32_t> out_array)
            {
+                pybind11::buffer_info buffer_info = out_array.request();
+                std::vector<ssize_t> shape2 = buffer_info.shape;
+
                 int n_examples = get_number_of_examples_ready();
+                if(shape2[0] != n_examples)
+                    return false;
+
+                uint32_t* output = static_cast<uint32_t*>(buffer_info.ptr);
                 
-                std::vector<int> output;
-                output.resize(n_examples);
+                //std::vector<int> output;
+                //output.resize(n_examples);
 
                 for(int i = 0; i < n_examples; ++i)
                 {
-                    m_feedback_block->reset();
-                    for(auto ib : m_inputs)   
-                        ib->prepare_example(i);
+                    m_feedback_block->reset();  
+                    m_input_block->prepare_example(i);
 
-                    for(auto cb : m_clause_blocks)                    
-                        cb->eval_example();                    
+                    for(auto cb : m_clause_blocks)
+                    {   
+                        if(enable_multithread)
+                        {
+                            m_pool.push_task(&ClauseBlock::eval_example, cb);
+                        }
+                        else
+                        {
+                            cb->eval_example();
+                        }                     
+                    }
+
+                    if(enable_multithread)
+                        m_pool.wait_for_tasks();
 
                     output[i] = m_feedback_block->predict();
-                }
-                
-                return output;
+                }         
+
+                return true;   
             }
 
-            std::vector<std::vector<int>> eval_predict_multi()
+            
+            bool eval_predict_multi(pybind11::array_t<uint32_t> out_array)
             {
-                int n_examples = get_number_of_examples_ready();                
+                std::cout << "eval_predict_multi IS BROKEN!!!!!!!!!!" << std::endl;
+                exit(1);
+
+                pybind11::buffer_info buffer_info = out_array.request();      
+                std::vector<ssize_t> shape2 = buffer_info.shape;                      
                 
-                std::vector<std::vector<int>> output;
-                output.resize(n_examples);
+
+                int n_examples = get_number_of_examples_ready();                                      
+                if(shape2[0] != n_examples)
+                    return false;        
+
+                int n_classes = m_feedback_block->get_number_of_classes();
+                if(shape2[1] != n_classes)
+                    return false;
+
+                uint32_t* output = static_cast<uint32_t*>(buffer_info.ptr);        
 
                 for(int i = 0; i < n_examples; ++i)
                 {
                     m_feedback_block->reset();
-                    for(auto ib : m_inputs)   
-                        ib->prepare_example(i);
+                    m_input_block->prepare_example(i);
 
                     for(auto cb : m_clause_blocks)
                         cb->eval_example();
                     
-                    //output[i] = m_feedback_block->predict();
-                    output[i] = m_feedback_block->predict_multi();
+                    uint32_t* example_ptr = &output[n_examples]; // fix this index to be multi label
+                    m_feedback_block->predict_multi(example_ptr);                    
                 }
-                return output;
+
+                return true;
             }
 
             int get_number_of_examples_ready() const
             {
-                return m_label_input->get_number_of_examples();
+                return m_input_block->get_number_of_examples();
             }
 
         private:        
-            std::vector<InputBlock*>   m_inputs;
-            InputBlock*                m_label_input;
+            InputBlock*                m_input_block;
             std::vector<ClauseBlock*>  m_clause_blocks;
+            std::vector<ClauseBlock*>  m_trainable_clause_blocks;
             FeedbackBlock* m_feedback_block;
             std::vector<int> m_index_set;
 
             // TODO: fix random
             std::default_random_engine m_rng;
 
             int m_num_threads;
@@ -239,12 +251,14 @@
 
     };
 
     int get_recommended_number_of_threads()
     {
         return std::thread::hardware_concurrency() - 1;
     }
-
+    
 }; // namespace green_tsetlin
 
 
-#endif // #ifndef __EXECUTOR_HPP_
+
+#endif // #ifndef __EXECUTOR_HPP_
+
```

### Comparing `green_tsetlin-0.1.9/src/feedback_block.hpp` & `green_tsetlin-1.0.0/src/feedback_block.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 #ifndef __FEEDBACK_BLOCK_HPP_
 #define __FEEDBACK_BLOCK_HPP_
 
 
-#include <iostream>
+#include <stdint.h>
 #include <vector>
-#include <stdexcept>
-#include <cstring>
+#include <random>
 #include <thread>
 #include <mutex>
-#include <random>
-#include <vector>
-#include <array>
+#include <algorithm>
 
-#include <random_generator.hpp>
+#include <pybind11/pybind11.h>
+#include <pybind11/numpy.h>
 
 #include <gt_common.hpp>
 
 namespace green_tsetlin
 {
-
-
     class FeedbackBlock
     {
         public:
             FeedbackBlock(int num_classes, double threshold, int seed)
             {
                 m_num_classes = num_classes;
                 m_threshold = threshold;
@@ -32,18 +28,14 @@
                 m_votes.resize(m_num_classes, 0);
                 
                 if(seed == 0)
                     seed = std::random_device()();                
                 m_rng.seed(seed);
             }
 
-            FeedbackBlock(int num_classes, double threshold)
-                : FeedbackBlock(num_classes, threshold, 0)
-            {}
-
             virtual ~FeedbackBlock() {}
 
 
             uint32_t get_positive_class() const
             {
                 return m_positive_class;
             }
@@ -78,15 +70,14 @@
             }
 
             virtual void process(const uint32_t* labels)
             {
                 
                 std::scoped_lock lock(m_votes_lock);
 
-                // TODO: support multi label 
                 uint32_t positive_class = labels[0];                
                 m_positive_class = positive_class;
                 
                 WeightInt most_votes = m_votes[0];
                 uint32_t predicted_class = 0;
 
                 // calcuate update probabilies and find the negative target using negative focused sampling.
@@ -96,15 +87,15 @@
                     if(votes > most_votes)
                     {
                         most_votes = votes;
                         predicted_class = class_k;
                     }
 
                     double v_clamped = std::clamp(static_cast<double>(votes), -m_threshold, m_threshold);
-                    m_update_probability[class_k] = ( (m_threshold + v_clamped) / (2*m_threshold) ) + 1e-30; // 1e-30 is used as epsilon                 
+                    m_update_probability[class_k] = ( (m_threshold + v_clamped) / (2*m_threshold) ) + 1e-16; // 1e-16 is used as epsilon                 
                     
                     //if(class_k != m_positive_class)
                     //    std::cout << "\t update prob of class " << class_k << " is: " << m_update_probability[class_k] << " from:" << m_votes[class_k] << std::endl;
                 }
 
                 m_total_train_predict += 1.0;
                 if(predicted_class == positive_class)                
@@ -117,15 +108,15 @@
                 std::discrete_distribution<int> weighted_sampler(m_update_probability.begin(), m_update_probability.end());
                 m_negative_class = weighted_sampler(m_rng);
                 m_update_prob_negative = m_update_probability[m_negative_class];
                 
 
                 // get the positive update prob
                 double v_clamped_pos = std::clamp(static_cast<double>(m_votes[m_positive_class]), -m_threshold, m_threshold);
-                m_update_prob_positive =  (m_threshold - v_clamped_pos) / (2*m_threshold);
+                m_update_prob_positive = (m_threshold - v_clamped_pos) / (2*m_threshold);
 
                 
                 //std::cout << "\t update prob of class " << m_positive_class << " is: " << m_update_probability[m_positive_class] << " from:" << m_votes[m_positive_class] << std::endl;
 
                 //std::cout << "neg class is:" << m_negative_class << std::endl;
                 //std::cout << "pos class is " << m_positive_class << std::endl;
 
@@ -145,64 +136,80 @@
                         best_v = m_votes[i];
                     }
                 }
 
                 return best_k;
             }            
 
-            virtual std::vector<int> predict_multi() const
+            virtual bool predict_multi(uint32_t* out) const
             {
+                // TODO: fix - this is wrong!!
+
                 int best_k = 0;
                 int best_v = m_votes[0];
                 
-                std::vector<int> o;
-                o.resize(m_num_classes, 0);
+                // std::vector<int> o;
+                // o.resize(m_num_classes, 0);
 
                 for(int i = 1; i < m_num_classes; ++i)
                 {
                     if(m_votes[i] > best_v)
                     {
                         best_k = i;
                         best_v = m_votes[i];
                     }
                 }
                 
-                o[best_k] = 1;
-                return o;
+                out[best_k] = 1;
+                return false;
             }
 
             std::vector<double> get_update_probabilities() const
             {
                 //std::fill(m_votes.begin(), m_votes.end(), 1.0);
                 std::scoped_lock lock(m_votes_lock);
-                return m_update_probability;
+                return m_update_probability; // TODO: remove this alloc
+            }
+
+            void register_votes_npy(pybind11::array_t<WeightInt> in_array)
+            {
+                pybind11::buffer_info buffer_info = in_array.request();                            
+                WeightInt* votes = static_cast<WeightInt*>(buffer_info.ptr);
+                
+                register_votes(votes);
             }
 
             void register_votes(WeightInt* votes)
             {
                 std::scoped_lock lock(m_votes_lock);
                 
                 //std::cout << "register vote" << std::endl;
                 for(int i = 0; i < m_num_classes; ++i)
                 {
                     //std::cout << "register vote: " << i << " adding:" <<  votes[i] << std::endl;
                     m_votes[i] += votes[i];
                 }
             }
 
+            pybind11::array_t<WeightInt> get_votes_npy() const
+            {
+                std::scoped_lock lock(m_votes_lock);
+                return pybind11::array_t<WeightInt>(m_votes.size(), m_votes.data());
+            }
+
             void reset()
             {
                 std::scoped_lock lock(m_votes_lock);
                 std::fill(m_votes.begin(), m_votes.end(), 0);
             }
 
             int get_number_of_classes() const
             {
                 return m_num_classes;
-            }
+            }            
 
         protected:
             int m_num_classes = -42;       
             double m_threshold = -1337.0;
 
             // random numbers : TODO fix so it is handled fast and in a more centralized way            
             std::default_random_engine m_rng;
@@ -218,17 +225,16 @@
             double m_update_prob_negative = 0.0;
 
 
             double m_correct_train_predict = 0.0;
             double m_total_train_predict = 0.0;
 
             mutable std::mutex m_votes_lock;
-    };
+    };  
 
-    
     class FeedbackBlockMultiLabel : public FeedbackBlock
     {
         public:
             FeedbackBlockMultiLabel(int num_classes, double threshold, int seed)                
                 : FeedbackBlock(num_classes, threshold, seed)
             {                
 
@@ -280,24 +286,81 @@
                         if(m_votes[class_k] < m_votes[class_k + m_num_classes])
                             m_correct_train_predict += 1.0;
                     }
                 }
 
             }
 
-            virtual std::vector<int> predict_multi() const
+            virtual bool predict_multi(uint32_t* out) const
             {               
                 std::vector<int> preds(m_num_classes, 0);
                 for(int i = 0; i < m_num_classes; ++i)
                 {                    
                     if(m_votes[i] >= m_votes[i+m_num_classes])
                         preds[i] = 1;                          
                 }
 
-                return preds;
+                // return preds;
+                return false;
             }      
     };
 
 
+    class FeedbackBlockUniform : public FeedbackBlock
+    {
+        public:
+            FeedbackBlockUniform(int num_classes, double threshold, int seed)                
+                : FeedbackBlock(num_classes, threshold, seed) {}
+
+
+            virtual void process(const uint32_t* labels)
+            {
+                std::scoped_lock lock(m_votes_lock);
+
+                uint32_t positive_class = labels[0];                
+                m_positive_class = positive_class;
+
+                std::uniform_int_distribution<> distrib(0, m_num_classes - 1);
+
+                m_negative_class = distrib(m_rng);
+                while(m_negative_class == m_positive_class)
+                    m_negative_class = distrib(m_rng);
+
+                double v_clamped = std::clamp(static_cast<double>(m_votes[m_negative_class]), -m_threshold, m_threshold);
+                m_update_prob_negative = ( (m_threshold + v_clamped) / (2*m_threshold) ) + 1e-16; // 1e-16 is used as epsilon 
+
+                v_clamped = std::clamp(static_cast<double>(m_votes[m_positive_class]), -m_threshold, m_threshold);
+                m_update_prob_positive = (m_threshold - v_clamped) / (2*m_threshold);                
+
+                WeightInt most_votes = m_votes[0];
+                uint32_t predicted_class = 0;
+
+                for(int class_k = 1; class_k < m_num_classes; ++class_k)
+                {   
+                    WeightInt votes = m_votes[class_k];
+                    if(votes > most_votes)
+                    {
+                        most_votes = votes;
+                        predicted_class = class_k;
+                    }
+
+                    
+                    //if(class_k != m_positive_class)
+                    //    std::cout << "\t update prob of class " << class_k << " is: " << m_update_probability[class_k] << " from:" << m_votes[class_k] << std::endl;
+                }
+
+                m_total_train_predict += 1.0;
+                if(predicted_class == positive_class)                
+                {
+                    m_correct_train_predict += 1.0;
+                }
+            }
+    };
+    
 }; // namespace green_tsetlin
 
-#endif // #ifndef __FEEDBACK_BLOCK_HPP_
+
+
+
+
+#endif // #define __FEEDBACK_BLOCK_HPP_
+
```

### Comparing `green_tsetlin-0.1.9/src/func_avx2.hpp` & `green_tsetlin-1.0.0/src/func_avx2.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,205 +1,36 @@
-#ifndef _FUNC_AVX2_HPP_
-#define _FUNC_AVX2_HPP_
-
-#include <stdlib.h>
-#include <cmath>
-#include <algorithm>
+#ifndef _FUNC_AVX2_H_
+#define _FUNC_AVX2_H_
 
 #include <immintrin.h> // intrics
 
-#include <random_generator.hpp>
-#include <gt_common.hpp>
-
-
 namespace green_tsetlin
 {
-    void int8_print(const int8_t* c, int n)
-    {
-        for(int i = 0; i < n; ++i)
-            printf(" %d ", c[i]);
-        printf("\n");
-    }
-
-
-    void _mm256_print_epi8(__m256i vec)
-    {
-        int8_t temp[32];
-        _mm256_storeu_si256((__m256i*)&temp[0], vec);
-        int8_print(temp, 32);
-    }
 
     // to be used for counting active ta's
     inline int _avx2_mask_count(const __m256i in)
     {
         __m256i _zeros = _mm256_set1_epi8(0);
         __m256i _on = _mm256_cmpgt_epi8(in, _zeros);
         int bits = _mm256_movemask_epi8(_on);
         return __builtin_popcount(bits); // TODO: wrap into save version (or force std::popcount() c++20)
     }
 
-    class CoaleasedTsetlinStateAligned32
-    {
-        public:
-            constexpr const static int literals_per_vector = 32;
-            constexpr const static int outputs_per_vector = 256 / sizeof(WeightInt);
-
-            double s = -42.0;
-            int num_clauses = 0;
-            int num_classes = 0;
-            int num_class_weights_mem = 0;
-
-            int num_literals = 0;
-            int num_literals_mem = 0;
-            int num_reminder = 0;
-
-            int8_t* clauses = nullptr;
-            ClauseOutputUint* clause_outputs = nullptr;
-            WeightInt* class_votes = nullptr;
-            WeightInt* clause_weights = nullptr;
-
-            uint32_t* literal_counts = nullptr;
-            uint32_t literal_budget = 0xFFFF;
-
-
-            int8_t* reminder_mask = nullptr;
-            int8_t gtcmp_for_s = 0;
-
-            std::default_random_engine rng;
-            XorShift128plus4G rng_avx2;
-            Wyhash64 rng_nv;
-
-
-            inline void set_s(double s_param)
-            {
-                s = s_param;
-                double p = 1 / s;
-                int32_t tmp = ((int32_t)(p * 255)) - 127;                
-                tmp += 1; // size we use < to compare and not <=
-
-                gtcmp_for_s = (int8_t)std::clamp(tmp, -127, 126);
-            }
-
-            inline double get_s() const { return s; }
-
-            inline int8_t get_ta_state(int clause_k, int ta_i, bool ta_polarity)
-            {
-                if(ta_polarity)
-                    return clauses[(clause_k * num_literals_mem * 2) + ta_i];
-                else
-                    return clauses[(clause_k * num_literals_mem * 2) + num_literals_mem + ta_i];
-            }
-
-            inline void set_ta_state(int clause_k, int ta_i, bool ta_polarity, int8_t new_state)
-            {
-                if(ta_polarity)
-                    clauses[(clause_k * num_literals_mem * 2) + ta_i] = new_state;
-                else
-                {
-                    std::cout << "setting TA state: " << ta_i << " index:" << (clause_k * num_literals_mem * 2) + num_literals_mem + ta_i << " to: " << (int)new_state << std::endl;
-                    clauses[(clause_k * num_literals_mem * 2) + num_literals_mem + ta_i] = new_state;                    
-                }
-            }
-
-            inline WeightInt get_clause_weight(int clause_index, int target_class)
-            {
-                return clause_weights[(clause_index * num_class_weights_mem) + target_class];
-            }
-
-            inline void set_clause_weight(int clause_index, int target_class, WeightInt new_weight)
-            {
-                clause_weights[(clause_index * num_class_weights_mem) + target_class] = new_weight;
-            }
-
-            inline WeightInt* get_class_votes() const
-            {
-                return class_votes;
-            }
-
-            inline std::vector<int8_t> get_copy_clauses() const
-            {                
-                std::size_t n_total_literals = num_clauses * (num_literals_mem*2);                
-                std::vector<int8_t>  states(clauses, clauses + n_total_literals);
-                return states;
-            }
-
-            inline std::vector<uint32_t> get_copy_literal_counts() const 
-            {          
-                std::vector<uint32_t>  counts(literal_counts, literal_counts + num_clauses);
-                return counts;
-            }
-
-            inline void get_clause_state(int8_t* dst, int clause_offset)
-            {
-                for(int i = 0; i < num_clauses; i++)
-                {
-                    const int src_o = i * num_literals_mem * 2;
-                    const int dst_o = (i+clause_offset) * num_literals * 2;
-
-                    memcpy(&dst[dst_o],
-                           &clauses[src_o], num_literals);
-
-                    memcpy(&dst[dst_o + num_literals],
-                           &clauses[src_o + num_literals_mem], num_literals);
-                }
-            }
-
-            inline void set_clause_state(int8_t* src, int clause_offset)
-            {
-
-                for(int i = 0; i < num_clauses; i++)
-                {                    
-                    const int src_o = (i+clause_offset) * (num_literals * 2);
-                    const int dst_o = i * (num_literals_mem * 2);
-
-                    memcpy(&clauses[dst_o],
-                           &src[src_o], num_literals);
-
-                    memcpy(&clauses[dst_o + num_literals_mem],
-                           &src[src_o + num_literals], num_literals);
-                }
-            }
-
-            inline void set_clause_weights(WeightInt* src, int clause_offset)
-            {
-                //const size_t weight_mem = num_clauses * num_classes * sizeof(WeightInt);
-                //memcpy(clause_weights, src, weight_mem);
-
-                for(int i = 0; i < num_clauses; i++)
-                {                    
-                    const int src_o = (i+clause_offset) * num_classes;
-                    const int dst_o = i * num_class_weights_mem;
-
-                    memcpy(&clause_weights[dst_o],
-                           &src[src_o], num_classes * sizeof(WeightInt));
-                }
-            }
-
-            inline void get_clause_weights(WeightInt* dst, int clause_offset)
-            {
-                for(int i = 0; i < num_clauses; i++)
-                {
-                    const int src_o = i * num_class_weights_mem;
-                    const int dst_o = (i+clause_offset) * num_classes;
-
-                    memcpy(&dst[dst_o],
-                           &clause_weights[src_o], num_classes * sizeof(WeightInt));
-                }
-            }
-
-    };
 
     template <typename _State, bool pad_class_weights,  bool do_literal_budget>
-    class InitializeAligned32
+    class InitializeAVX2
     {
         public:                        
             bool operator()(_State& state, unsigned int seed)
             {            
-                state.rng_avx2.seed(seed);
-                state.rng_nv.seed(seed);
+                if(seed == 0)
+                    return false;
+
+                state.avx2_rng.seed(seed);
+                state.fast_rng.seed(seed);
                 state.rng.seed(seed);
 
                 state.reminder_mask = reinterpret_cast<int8_t*>(aligned_alloc(32, state.literals_per_vector));
                 for(int i = 0; i < state.literals_per_vector; ++i)
                         state.reminder_mask[i] = 0xFF;
                         
                 if( (state.num_literals % state.literals_per_vector) == 0)
@@ -217,15 +48,15 @@
                 }
                 
                 #ifdef PRINT_DEBUG
                     std::cout << "[DEBUG]" << "allocated " << state.num_literals_mem << " <- from " << state.num_literals <<" literals. #vec:" << state.literals_per_vector << std::endl;
                 #endif 
 
                 int clause_mem = state.num_clauses * state.num_literals_mem * 2;
-                state.clauses = reinterpret_cast<int8_t*>(aligned_alloc(32, clause_mem));
+                state.clauses = reinterpret_cast<int8_t*>(safe_aligned_alloc(32, clause_mem));
 
                 if(do_literal_budget)
                     state.literal_counts = new uint32_t[state.num_clauses];
 
                 
                 // align so that we can loop over with vectors of 32ints
                 
@@ -268,16 +99,23 @@
 
                 for(int clause_k = 0; clause_k < state.num_clauses; ++clause_k)
                 {
                     int8_t* clause_row = &state.clauses[clause_k * (state.num_literals_mem * 2)];
                                         
                     for(int literal_k = 0; literal_k < state.num_literals; ++literal_k)
                     {
-                        clause_row[literal_k] = dist(state.rng); // pos
-                        clause_row[literal_k + state.num_literals_mem] = dist(state.rng); // neg
+                        if(state.fast_rng.next_u() > 0.5)
+                            clause_row[literal_k] = 0; // pos
+                        else
+                            clause_row[literal_k] = -1; 
+
+                        if(state.fast_rng.next_u() > 0.5) // negated
+                            clause_row[literal_k + state.num_literals_mem] = 0;
+                        else
+                            clause_row[literal_k + state.num_literals_mem] = -1;
                     }
 
                     // set filler states to -109 and -111 (pos and neg)
                     for(int filler_lit_k = state.num_literals; filler_lit_k < state.num_literals_mem; ++filler_lit_k)
                     {
                         clause_row[filler_lit_k] = -109;
                         clause_row[filler_lit_k + state.num_literals_mem] = -111;
@@ -288,35 +126,26 @@
             void init_clause_weights(_State& state)
             {
                 std::bernoulli_distribution dist(0.5);
                 for(int clause_k = 0; clause_k < state.num_clauses; clause_k++)
                 {
                     for(int class_i = 0; class_i < state.num_classes; class_i++)
                     {
-                        if(dist(state.rng))
+                        if(state.fast_rng.next_u() > 0.5)
                             state.clause_weights[(clause_k * state.num_class_weights_mem) + class_i] = 1;
                         else
                             state.clause_weights[(clause_k * state.num_class_weights_mem) + class_i] = -1;
                     }
                 }
-                /*
-                const int num_weights_total = state.num_clauses * state.num_classes;
-                for(int k = 0; k < num_weights_total; ++k)
-                {
-                    if(dist(state.rng))
-                        state.clause_weights[k] = 1;
-                    else
-                        state.clause_weights[k] = -1;
-                }
-                */
             }        
     };
 
+
     template <typename _State, bool do_literal_budget>
-    class CleanupAligned32
+    class CleanupAVX2
     {
         public:                        
             void operator()(_State& state)
             {
                 free(state.clauses);
                 state.clauses = nullptr;     
 
@@ -334,17 +163,14 @@
                     delete[] state.literal_counts;
                     state.literal_counts = nullptr;
                 }
             }
     };
 
 
-
-
-
     template <typename _State, bool do_literal_budget>
     class SetClauseOutputAVX2
     {
         public:
             void operator()(_State& state, uint8_t* literals)
             {
                 int8_t* clauses = (int8_t*)__builtin_assume_aligned(state.clauses, 32);
@@ -352,27 +178,28 @@
                 __m256i _reminder_mask = _mm256_load_si256((__m256i const*)state.reminder_mask);
                 __m256i _zeros = _mm256_set1_epi8(0);
 
                 const int n_chunks = (state.num_literals_mem / state.literals_per_vector) - 1;
 
                 for(int clause_k = 0; clause_k < state.num_clauses; ++clause_k)
                 {
-                    state.literal_counts[clause_k] = 0;
+                    uint32_t literal_count = 0;
+
                     state.clause_outputs[clause_k] = 1;
 
                     const int8_t* clause_row =  &clauses[clause_k * (state.num_literals_mem * 2)];
 
                     for(int chunk_i = 0; chunk_i < n_chunks; ++chunk_i)
                     {
                         __m256i _literals = _mm256_load_si256((__m256i const*)&literals[chunk_i * 32]);                        
                         __m256i _clauses = _mm256_load_si256((__m256i const*)&clause_row[chunk_i * 32]);
                         __m256i _not_active = _mm256_cmpgt_epi8(_zeros, _clauses);
                         
                         if(do_literal_budget)
-                            state.literal_counts[clause_k] += __builtin_popcount(_mm256_movemask_epi8(~_not_active));
+                            literal_count += __builtin_popcount(_mm256_movemask_epi8(~_not_active));
 
                         __m256i clause_imply_literal = _mm256_or_si256(_not_active, _literals);                        
                         __m256i _is_false = _mm256_cmpeq_epi8(clause_imply_literal, _zeros);
                         if(_mm256_testz_si256(_is_false, _is_false) == 0)
                         {
                             state.clause_outputs[clause_k] = 0;
                             goto endclause;
@@ -380,15 +207,15 @@
 
                         __m256i _neg_literals = _mm256_cmpeq_epi8(_zeros, _literals);                        
                         _clauses = _mm256_load_si256((__m256i const*)&clause_row[state.num_literals_mem + (chunk_i * 32)]);
 
                         _not_active = _mm256_cmpgt_epi8(_zeros, _clauses);
                         
                         if(do_literal_budget)
-                            state.literal_counts[clause_k] += __builtin_popcount(_mm256_movemask_epi8(~_not_active));
+                            literal_count += __builtin_popcount(_mm256_movemask_epi8(~_not_active));
 
                         clause_imply_literal = _mm256_or_si256(_not_active, _neg_literals);
                         
                         _is_false = _mm256_cmpeq_epi8(clause_imply_literal, _zeros);
                         if(_mm256_testz_si256(_is_false, _is_false) == 0)
                         {
                             state.clause_outputs[clause_k] = 0;
@@ -401,15 +228,15 @@
                     {
                         __m256i _literals = _mm256_load_si256((__m256i const*)&literals[n_chunks * 32]);                        
                         __m256i _clauses = _mm256_load_si256((__m256i const*)&clause_row[n_chunks * 32]);
                         __m256i _not_active = _mm256_cmpgt_epi8(_zeros, _clauses);
 
                         __m256i _active_masked =  _mm256_and_si256(~_not_active, _reminder_mask);
                         if(do_literal_budget)
-                            state.literal_counts[clause_k] += __builtin_popcount(_mm256_movemask_epi8(_active_masked));
+                            literal_count += __builtin_popcount(_mm256_movemask_epi8(_active_masked));
                             
                         __m256i _clause_imply_literal = _mm256_or_si256(~_active_masked, _literals);                                                                                                                                    
                         __m256i _is_false = _mm256_cmpeq_epi8(_clause_imply_literal, _zeros);
                         //_is_false = _mm256_and_si256(_is_false, _reminder_mask);
                         if(_mm256_testz_si256(_is_false, _is_false) == 0)
                         {
                             state.clause_outputs[clause_k] = 0;
@@ -418,33 +245,36 @@
 
                         __m256i _neg_literals = _mm256_cmpeq_epi8(_zeros, _literals);                        
                         _clauses = _mm256_load_si256((__m256i const*)&clause_row[state.num_literals_mem + (n_chunks * 32)]);
 
                         _not_active = _mm256_cmpgt_epi8(_zeros, _clauses);
                         _active_masked =  _mm256_and_si256(~_not_active, _reminder_mask);
                         if(do_literal_budget)
-                            state.literal_counts[clause_k] += __builtin_popcount(_mm256_movemask_epi8(_active_masked));
+                            literal_count += __builtin_popcount(_mm256_movemask_epi8(_active_masked));
 
                         //_clause_imply_literal = _mm256_or_si256(_not_active, _neg_literals);
                         _clause_imply_literal = _mm256_or_si256(~_active_masked, _neg_literals);                                                                                                                                    
 
                         
                         _is_false = _mm256_cmpeq_epi8(_clause_imply_literal, _zeros);
                         //_is_false = _mm256_and_si256(_is_false, _reminder_mask);
                         if(_mm256_testz_si256(_is_false, _is_false) == 0)
                         {
                             state.clause_outputs[clause_k] = 0;                            
                         }
                     }
                     
-                    endclause:;
+                    endclause:
+                        if(do_literal_budget)
+                            state.literal_counts[clause_k] = literal_count;
                 }
             }
     };
 
+
     template <typename _State>
     class EvalClauseOutputAVX2
     {
         public:
             void operator()(_State& state, uint8_t* literals)
             {
                 int8_t* clauses = (int8_t*)__builtin_assume_aligned(state.clauses, 32);
@@ -531,22 +361,14 @@
 
                     endclause:;                
                     
                 }
             }
     };
 
-
-    template <typename _State>
-    class EmptyCountVotesAVX2
-    {
-        public:
-            void operator()(_State& state) {}
-    };
-
     template <typename _State>
     class CountVotesAVX2
     {
         public:
             // TODO: rewrite to avx2
             void operator()(_State& state)
             {                
@@ -564,53 +386,14 @@
                             state.class_votes[class_k] += to_add;
                         }
                     }
                 }
             }
     };
 
-    #include <unistd.h>
-
-    template <typename _State>
-    class CountVotesVectorAVX2
-    {
-        public:
-            void operator()(_State& state)
-            {   
-                std::cout << " --------------- Not Impl CountVotesVectorAVX2 --------" << std::endl;
-
-                const int num_chunks = state.num_class_weights_mem / state.outputs_per_vector;                
-
-                int32_t* votes = (int32_t*)__builtin_assume_aligned(state.class_votes, 32);
-                __m256i _zero = _mm256_set1_epi32(0);                
-                for(int chunk_i = 0; chunk_i < num_chunks; chunk_i++)
-                    _mm256_store_si256((__m256i*)&votes[chunk_i * state.outputs_per_vector], _zero);
-                
-
-                const int32_t* cw = (int32_t*)__builtin_assume_aligned(state.clause_weights, 32);
-                for(int clause_k = 0; clause_k < state.num_clauses; ++clause_k)
-                {
-                    if(state.clause_outputs[clause_k] == 1)
-                    {
-                        const int clause_weight_i = clause_k * state.num_class_weights_mem;
-                        for(int chunk_i = 0; chunk_i < num_chunks; chunk_i++)
-                        {
-                            __m256i _votes = _mm256_load_si256((__m256i const*)&votes[chunk_i * state.outputs_per_vector]);
-                            __m256i _weights = _mm256_load_si256((__m256i const*)&cw[clause_weight_i + (chunk_i * state.outputs_per_vector)]);
-
-                            _votes = _mm256_add_epi32(_votes, _weights);
-                            _mm256_store_si256((__m256i*)&votes[chunk_i * state.outputs_per_vector], _votes);
-                        }
-                    }
-                }   
-
-                //usleep(200 * 1000);
-            }
-    };
-
     template <typename _State, typename _ClauseUpdate, bool do_literal_budget>
     class TrainUpdateAVX2
     {
         public:
             void operator()(_State& state, uint8_t* literals, int positive_class, double prob_positive, int negative_class, double prob_negative)
             {
 
@@ -623,72 +406,70 @@
 
                     if(do_literal_budget)
                     {
                         if(state.literal_counts[clause_k] > state.literal_budget)
                             state.clause_outputs[clause_k] = 0;
                     }
 
-                    if( state.rng_nv.next_u() < prob_positive)
+                    if( state.fast_rng.next_u() < prob_positive)
                     {
                         _ClauseUpdate clause_update;
                         clause_update(state, clause_row, clause_weights + positive_class, 1, literals, state.clause_outputs[clause_k]);                    
                     }
       
-                    if( state.rng_nv.next_u() < prob_negative)
+                    if( state.fast_rng.next_u() < prob_negative)
                     {
                         _ClauseUpdate update_clause;
                         update_clause(state, clause_row, clause_weights + negative_class, -1, literals, state.clause_outputs[clause_k]);
                     }
                 }
             }
-
     };
 
-
     template <typename _State, typename _T1aFeedback, typename _T1bFeedback, typename _T2Feedback>
     class ClauseUpdateAVX2
     {
         public:
             void operator()(_State& state, int8_t* clause_row, WeightInt* clause_weight, int target, uint8_t* literals, ClauseOutputUint clause_output)
             {
+                
                 WeightInt sign = (*clause_weight) >= 0 ? +1 : -1;                
                 
                 if( (target * sign) > 0)
                 {
                     if(clause_output == 1)
                     {
                         (*clause_weight) += sign;
 
                         _T1aFeedback t1a;
                         t1a(state, clause_row, literals);                    
                     }
                     else
                     {
                         _T1bFeedback t1b;
-                        t1b(state, clause_row, literals);      
+                        t1b(state, clause_row);
                     }
                 }
 
                 else if((target * sign) < 0 && clause_output == 1)
                 {
                     (*clause_weight) -= sign;
 
                     _T2Feedback t2;
                     t2(state, clause_row, literals);
                 }
             }
     };
 
-    template <typename _State>
+    template <typename _State, bool use_boost_true_positive>
     class Type1aFeedbackAVX2
     {
         public:
             void operator()(_State& state, int8_t* clause_row, const uint8_t* literals_in)
             {
-                constexpr bool use_boost_true_positive = false;
 
                  int8_t* clause = (int8_t*)__builtin_assume_aligned(clause_row, 32);
                  const uint8_t* literals = (uint8_t*)__builtin_assume_aligned(literals_in, 32);
 
                 __m256i _minus_one = _mm256_set1_epi8(-1);                
                 __m256i _cmp_s = _mm256_set1_epi8(state.gtcmp_for_s);
 
@@ -698,15 +479,15 @@
 
                 for(int chunk_i = 0; chunk_i < n_chunks; ++chunk_i)
                 {                                                
                     __m256i _literals = _mm256_load_si256((__m256i const*)&literals[chunk_i * state.literals_per_vector]);
                     __m256i _clause = _mm256_load_si256((__m256i const*)&clause[chunk_i * state.literals_per_vector]);                    
                     __m256i _literal_on = _mm256_cmpeq_epi8(_literals, _ones);
 
-                    __m256i _rand = state.rng_avx2.next();
+                    __m256i _rand = state.avx2_rng.next();
                     __m256i _update = _mm256_cmpgt_epi8(_cmp_s, _rand);
 
                     __m256i _subtract = _mm256_and_si256(~_literal_on, _update);
                     _subtract = _mm256_and_si256(_minus_one, _subtract);
                     
                     __m256i _add;
                     if(use_boost_true_positive)
@@ -721,15 +502,15 @@
                     
                     
                     _clause = _mm256_adds_epi8(_clause, _mm256_or_si256(_subtract, _add));
                     _mm256_store_si256((__m256i*)&clause_row[chunk_i * state.literals_per_vector], _clause);
 
                     // --- negated ----
                     _clause = _mm256_load_si256((__m256i const*)&clause[state.num_literals_mem + (chunk_i * state.literals_per_vector)]);
-                    _rand = state.rng_avx2.next();
+                    _rand = state.avx2_rng.next();
                     _update = _mm256_cmpgt_epi8(_cmp_s, _rand);
 
                     _subtract = _mm256_and_si256(_literal_on, _update);
                     _subtract = _mm256_and_si256(_minus_one, _subtract);
 
                     // boost
                     _add = _mm256_and_si256(~_literal_on, ~_update);
@@ -738,42 +519,46 @@
                                             
                     _clause = _mm256_adds_epi8(_clause, _mm256_or_si256(_subtract, _add));
                     _mm256_store_si256((__m256i*)&clause_row[state.num_literals_mem + (chunk_i * state.literals_per_vector)], _clause);
                 }
             }
     };
 
-
     template <typename _State>
     class Type1bFeedbackAVX2
     {
         public:
-            void operator()(_State& state, int8_t* clause_row, const uint8_t* literals_in)
+            void operator()(_State& state, int8_t* clause_row)
             {
-                 int8_t* clause = (int8_t*)__builtin_assume_aligned(clause_row, 32);
+
+                int8_t* clause = (int8_t*)__builtin_assume_aligned(clause_row, 32);
+
+  
 
                 __m256i _minus_one = _mm256_set1_epi8(-1);                
                 __m256i _cmp_s = _mm256_set1_epi8(state.gtcmp_for_s);
 
                 const int n_chunks = (state.num_literals_mem / state.literals_per_vector);
-                                
+
+                                         
                 for(int chunk_i = 0; chunk_i < n_chunks; ++chunk_i)
                 {
+                    //__m256i _clause = _mm256_load_si256((__m256i const*)&clause[chunk_i * state.literals_per_vector]);
                     __m256i _clause = _mm256_load_si256((__m256i const*)&clause[chunk_i * state.literals_per_vector]);
-                    __m256i _rand = state.rng_avx2.next();
+                    __m256i _rand = state.avx2_rng.next();
 
                     __m256i _update = _mm256_cmpgt_epi8(_cmp_s, _rand);
                     _update = _mm256_and_si256(_minus_one, _update);
 
                     _clause = _mm256_adds_epi8(_clause, _update);
                     _mm256_store_si256((__m256i*)&clause_row[chunk_i * state.literals_per_vector], _clause);
 
                     // -- negated
                     _clause = _mm256_load_si256((__m256i const*)&clause[state.num_literals_mem + (chunk_i * state.literals_per_vector)]);
-                    _rand = state.rng_avx2.next(); // TODO:  check if doing both and store is faster ( rand0 = next(); rand1 = next() )
+                    _rand = state.avx2_rng.next(); // TODO:  check if doing both and store is faster ( rand0 = next(); rand1 = next() )
 
                     _update = _mm256_cmpgt_epi8(_cmp_s, _rand);
                     _update = _mm256_and_si256(_minus_one, _update);
                     _clause = _mm256_adds_epi8(_clause, _update);
 
                     _mm256_store_si256((__m256i*)&clause_row[state.num_literals_mem + (chunk_i * state.literals_per_vector)], _clause);
                 }
@@ -840,16 +625,23 @@
                     _not_active = _mm256_cmpgt_epi8(_zeros, _clause);
 
                     _add_mask = _mm256_and_si256(~_lit_mask, _not_active);
                     _inc = _mm256_and_si256(_add_mask, _ones);
                     _clause = _mm256_adds_epi8(_clause, _inc);
                     _mm256_store_si256((__m256i*)&clause_row[state.num_literals_mem + (n_chunks * 32)], _clause);
                 }
-                */
-                
+                */                
             }
     };
 
-
 }; // namespace green_tsetlin
 
-#endif // #ifndef _FUNC_AVX2_HPP_
+
+
+
+
+
+
+
+
+
+#endif // #ifndef _FUNC_AVX2_H_
```

### Comparing `green_tsetlin-0.1.9/src/func_neon.hpp` & `green_tsetlin-1.0.0/src/func_neon.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -33,369 +33,48 @@
     // TODO: check for faster ways of doing this - a horizontal add seems slow
     inline uint32_t count_on_masks_neon(const uint8x16_t& v)
     {
         uint8x16_t msb_shifted = vshrq_n_u8(v, 7);
         return static_cast<uint32_t>(vaddvq_u8(msb_shifted));
     }
 
-    void test_neon()
-    {
-        std::cout << "start neon test" << std::endl;
-        int8x16_t  v;
-
-        int8_t clauses[16];
-        for(int i = 0; i < 16; i++)
-            clauses[i] = 42;
-
-        
-            //clauses[i] = (i < 8) ? -1 - i : 0 + i;
-        clauses[8] = 0;
-
-        int8_t literals[16];
-        for(int i = 0; i < 16; i++)
-            literals[i] = ((i % 2) == 0) ? 1 : 0;
-        
-
-        // int8_t numbers[16];
-        // for(int i = 0; i < 16; i++)
-        //     numbers[i] = -8 + i;
-        // // v = vld1q_s8(clauses);
-        // neon_print("v", v);
-        
-        // int8x16_t _zeros = vmovq_n_s8(0);
-        // int8x16_t _is_false = vcgeq_s8(v, _zeros);
-
-        // int8_t buffer[16];
-        // vst1q_s8(buffer, _is_false);
-        // int8_print(buffer, 16);
-
-        // if( vmaxvq_s8(_is_false) == 0)
-        //     std::cout << "vmaxvq_s8() == 0" << std::endl;
-        // else
-        //     std::cout << "vmaxvq_s8() == 1" << std::endl;
-
-        //int8x16_t _minus_ones = vmovq_n_s8(-1);
-        int8x16_t _zeros = vmovq_n_s8(0);
-        int8x16_t _literals = vld1q_s8(literals);                        
-        int8x16_t _clauses = vld1q_s8(clauses);
-        // int8x16_t _numbers = vld1q_s8(numbers);
-        //neon_print("_minus_ones", _minus_ones);
-        neon_print("_zeros", _zeros);
-        neon_print("literals", _literals);
-        neon_print("clauses", _clauses);
-
-
-        //int8x16_t neg_literals2 = vceqq_s8(_zeros, _literals);                        
-        //neon_print("neg_literals2", neg_literals2);
-        //_literals = neg_literals2;
-        // //neon_print("_numbers", _numbers);
-        // int8x16_t _gt_zeros = vcgeq_s8(_numbers, _zeros);
-        // //neon_print("_gt_zeros", _gt_zeros);
-
-
-        // int8x16_t _gt_zeros_flip = vcgeq_s8(_zeros, _numbers);
-        // //neon_print("_gt_zeros_flip", _gt_zeros_flip);
-
-        int8x16_t _not_active = vcgtq_s8(_zeros, _clauses);
-        neon_print("_not_active", _not_active);
-
-
-        uint8_t count = count_on_masks_neon(~_not_active);
-        std::cout << "Count: " << (int)count << std::endl;
-
-
-                // int8x16_t _minus_one = vdupq_n_s8(-1);                
-                // int8x16_t _cmp_s = vdupq_n_s8(state.gtcmp_for_s);
-
-                                
-
-                // const int n_chunks = (state.num_literals_mem / state.literals_per_vector);                                            
-                // int8x16_t _ones = vdupq_n_s8(1);
-
-
-
-                    //         int8x16_t _literals = vld1q_s8(&literals[chunk_i * state.literals_per_vector]);
-                    // int8x16_t _clause = vld1q_s8(&clause[chunk_i * state.literals_per_vector]);
-                    // int8x16_t _literal_on = vceqq_s8(_literals, _ones);
-
-                    
-                    // int8x16_t _rand = state.rng_neon.next();
-                    // int8x16_t _update = vcgtq_s8(_cmp_s, _rand);
-
-                    // int8x16_t _subtract = vandq_s8(~_literal_on, _update);
-                    // _subtract = vandq_s8(_minus_one, _subtract);
-
-                    // int8x16_t _add;
-                    // if(use_boost_true_positive)
-                    // {
-                    //     _add = vandq_s8(_literal_on, _ones);
-                    // }
-                    // else
-                    // {
-                    //     _add = vandq_s8(_literal_on, ~_update);
-                    //     _add = vandq_s8(_ones, _add); // -> boost
-                    // }
-
-                    // _clause = vqaddq_s8(_clause, vorrq_s8(_subtract, _add));
-                    // vst1q_s8(&clause_row[chunk_i * state.literals_per_vector], _clause);
-
-
-        // int8x16_t _clause_imply_literal = vorrq_s8(_not_active, _literals);                        
-        // neon_print("clause_imply_literal", _clause_imply_literal);
-
-
-        // std::cout << " max s8: " << (int)vmaxvq_s8(_clause_imply_literal) << std::endl;
-        // if(vmaxvq_s8(_clause_imply_literal) == 1)
-        // {
-        //     std::cout << "clause output == 0"<< std::endl;
-        // }
-        // else
-        // {
-        //     std::cout << "clause is true" << std::endl;
-        // }
-
-        // int8x16_t _neg_literals = vnegq_s8(_literals);
-        // neon_print("neg literals", _neg_literals);
-
-
-        // int8x16_t _signed_or = vqaddq_s8(_neg_literals, _not_active);
-        // std::cout << " max s8 (neg): " << (int)vmaxvq_s8(_signed_or) << std::endl;
-        // if(vmaxvq_s8(_signed_or) == 1)
-        // {
-        //     std::cout << "neg clause output == 0"<< std::endl;
-        // }
-        // else
-        // {
-        //     std::cout << "neg clause is true" << std::endl;
-        // }
-
-        // int8x16_t _is_false = vcgeq_s8(clause_imply_literal, _zeros);
-
-        // int8x16_t out = vaddq_s8(v, a);
-        
-        // int8_t results[16];
-        // vst1q_s8(results, out);
-
-        // int8_print(results, 16);
-
-        // std::cout << "- neon  generate random !! "<< std::endl;
-
-        // XorShift128Plus2G   rng(16);
-
-        // int8x16_t o = rng.next();
-        // vst1q_s8(results, o);
-
-        // int8_print(results, 16);
-
-        // std::cout << "- neon  generate random !! DONE "<< std::endl;
-    }
-
     inline uint64_t neon_movemask(uint8x16_t mask)
     {
         const uint16x8_t equal_mask = vreinterpretq_u16_u8(mask);
         const uint8x8_t res = vshrn_n_u16(equal_mask, 4);
         const uint64_t matches = vget_lane_u64(vreinterpret_u64_u8(res), 0);
         return matches;
     }
 
-    
-    
-
-    void* neon_alloc(int align_to, int mem)
-    {
-        int new_mem = mem;
-        int r = mem % align_to;
-
-        if(mem < align_to)
-            new_mem = align_to;
-            
-        else if(r > 0)
-            new_mem += (align_to - r);
-
-        void* p = std::aligned_alloc(align_to, new_mem);
-        if(p == nullptr)
-        {
-            std::string msg = "NEON failed to allocate mem: " + std::to_string(new_mem) + " aligned to: " + std::to_string(align_to) + " req:" + std::to_string(mem);
-            throw std::runtime_error(msg);
-        }
-        return p;
-    }
-
 
     //
     // TODO: to increase efficency we should unroll the 16 into 2x16 that are interleaved
     // 
     // load 16 first -> a
     // load 16 next  -> b
     //  cmp a mask
     //  cmp b mask
     // Since each vector operation has some cycles delay (we dont want to stall the pipeline)
     //
 
-    class CoaleasedTsetlinStateAlignedNeon32
-    {
-        public:
-            constexpr static const int literals_per_vector = 16;
-            constexpr static const int outputs_per_vector = 8;
-            constexpr static const int align_to = 32;
-
-
-            double s = -42.0;
-            int num_clauses = 0;
-            int num_classes = 0;
-            int num_literals = 0;
-            int num_literals_mem = 0;
-            int num_reminder = 0;
-            int num_class_weights_mem = 0;
-
-            std::default_random_engine rng;
-            int8_t* clauses = nullptr;
-            ClauseOutputUint* clause_outputs = nullptr;
-            WeightInt* class_votes = nullptr;
-            WeightInt* clause_weights = nullptr;
-
-            uint32_t* literal_counts = nullptr;
-            uint32_t literal_budget = 0xFFFF;
-
-            int8_t* reminder_mask = nullptr;
-            int8_t gtcmp_for_s = 0;
-
-            //XorShift128Plus2G rng_neon;
-            Xoshiro128Plus rng_neon;
-            Wyhash64 rng_nv;
-
-            inline void set_s(double s_param)
-            {
-                s = s_param;
-                double p = 1 / s;
-                int32_t tmp = ((int32_t)(p * 255)) - 127;                
-                tmp += 1; // size we use < to compare and not <=
-
-                gtcmp_for_s = (int8_t)std::clamp(tmp, -127, 126);
-            }
-
-            inline double get_s() const { return s; }
-
-            inline int8_t get_ta_state(int clause_k, int ta_i, bool ta_polarity)
-            {
-                if(ta_polarity)
-                    return clauses[(clause_k * num_literals_mem * 2) + ta_i];
-                else
-                    return clauses[(clause_k * num_literals_mem * 2) + num_literals_mem + ta_i];
-            }
-
-            inline void set_ta_state(int clause_k, int ta_i, bool ta_polarity, int8_t new_state)
-            {
-                if(ta_polarity)
-                    clauses[(clause_k * num_literals_mem * 2) + ta_i] = new_state;
-                else
-                    clauses[(clause_k * num_literals_mem * 2) + num_literals_mem + ta_i] = new_state;
-            }
-
-            inline WeightInt get_clause_weight(int clause_index, int target_class)
-            {
-                return clause_weights[(clause_index * num_classes) + target_class];
-            }
-
-            inline void set_clause_weight(int clause_index, int target_class, WeightInt new_weight)
-            {
-                clause_weights[(clause_index * num_classes) + target_class] = new_weight;
-            }
-
-            inline WeightInt* get_class_votes() const
-            {
-                return class_votes;
-            }
-
-            inline std::vector<int8_t> get_copy_clauses() const
-            {                
-                std::size_t n_total_literals = num_clauses * (num_literals_mem*2);                
-                std::vector<int8_t>  states(clauses, clauses + n_total_literals);
-               return states;
-            }
-
-            inline std::vector<uint32_t> get_copy_literal_counts() const 
-            {          
-                std::vector<uint32_t>  counts(literal_counts, literal_counts + num_clauses);
-                return counts;
-            }
-
-            inline void get_clause_state(int8_t* dst, int clause_offset)
-            {
-                for(int i = 0; i < num_clauses; i++)
-                {
-                    const int src_o = i * num_literals_mem * 2;
-                    const int dst_o = (i+clause_offset) * num_literals * 2;
-
-                    memcpy(&dst[dst_o],
-                           &clauses[src_o], num_literals);
-
-                    memcpy(&dst[dst_o + num_literals],
-                           &clauses[src_o + num_literals_mem], num_literals);
-                }
-            }
-
-            inline void set_clause_state(int8_t* src, int clause_offset)
-            {
-
-                for(int i = 0; i < num_clauses; i++)
-                {                    
-                    const int src_o = (i+clause_offset) * (num_literals * 2);
-                    const int dst_o = i * (num_literals_mem * 2);
-
-                    memcpy(&clauses[dst_o],
-                           &src[src_o], num_literals);
-
-                    memcpy(&clauses[dst_o + num_literals_mem],
-                           &src[src_o + num_literals], num_literals);
-                }
-            }
-
-            inline void set_clause_weights(WeightInt* src, int clause_offset)
-            {
-                //const size_t weight_mem = num_clauses * num_classes * sizeof(WeightInt);
-                //memcpy(clause_weights, src, weight_mem);
-
-                for(int i = 0; i < num_clauses; i++)
-                {                    
-                    const int src_o = (i+clause_offset) * num_classes;
-                    const int dst_o = i * num_class_weights_mem;
-
-                    memcpy(&clause_weights[dst_o],
-                           &src[src_o], num_classes * sizeof(WeightInt));
-                }
-            }
-
-            inline void get_clause_weights(WeightInt* dst, int clause_offset)
-            {
-                for(int i = 0; i < num_clauses; i++)
-                {
-                    const int src_o = i * num_class_weights_mem;
-                    const int dst_o = (i+clause_offset) * num_classes;
-
-                    memcpy(&dst[dst_o],
-                           &clause_weights[src_o], num_classes * sizeof(WeightInt));
-                }
-            }
-
-    };
-
-
-
     // TODO: impl padded class weights (for neon support on vote counts)
     template <typename _State,  bool do_literal_budget>
-    class InitializeAlignedNeon32
+    class InitializeAlignedNeon
     {
         public:                        
             bool operator()(_State& state, unsigned int seed)
-            {            
+            {
+                if(seed == 0)
+                    return false;
+
                 state.rng_neon.seed(seed);
-                state.rng_nv.seed(seed);
+                state.fast_rng.seed(seed);
+                state.rng.seed(seed);
                 
-                state.reminder_mask = reinterpret_cast<int8_t*>(neon_alloc(state.align_to, state.literals_per_vector));
+                state.reminder_mask = reinterpret_cast<int8_t*>(safe_aligned_alloc(32, state.literals_per_vector));
                 for(int i = 0; i < state.literals_per_vector; ++i)
                         state.reminder_mask[i] = 0xFF;
 
                 if( (state.num_literals % state.literals_per_vector) == 0)
                 {
                     state.num_literals_mem = state.num_literals;
                     state.num_reminder = 0;                    
@@ -407,34 +86,33 @@
                     
                     for(int i = state.num_reminder; i < state.literals_per_vector; ++i)
                         state.reminder_mask[i] = 0x00;
                 }
 
                 int clause_mem = state.num_clauses * state.num_literals_mem * 2;
 
-                state.clauses = reinterpret_cast<int8_t*>(neon_alloc(state.align_to, clause_mem));
+                state.clauses = reinterpret_cast<int8_t*>(safe_aligned_alloc(32, clause_mem));
                 if(do_literal_budget)
                     state.literal_counts = new uint32_t[state.num_clauses];
                 
                 // align so that we can loop over with vectors of 32ints
                 int num_aligned_clause_output =  ((state.num_clauses / state.outputs_per_vector) + 1) * state.outputs_per_vector;
-                state.clause_outputs = reinterpret_cast<ClauseOutputUint*>(neon_alloc(32, num_aligned_clause_output * sizeof(ClauseOutputUint)));
+                state.clause_outputs = reinterpret_cast<ClauseOutputUint*>(safe_aligned_alloc(32, num_aligned_clause_output * sizeof(ClauseOutputUint)));
                 memset(state.clause_outputs, 0, sizeof(ClauseOutputUint) * num_aligned_clause_output);
 
                 //state.clause_weights = new int32_t[state.num_clauses * state.num_classes];
                 int weights_mem = state.num_clauses * state.num_classes * sizeof(WeightInt);
                 state.num_class_weights_mem = state.num_classes;
 
-                state.clause_weights = reinterpret_cast<WeightInt*>(neon_alloc(32, weights_mem));
+                state.clause_weights = reinterpret_cast<WeightInt*>(safe_aligned_alloc(32, weights_mem));
 
                 //state.class_votes = new int32_t[state.num_classes];
-                state.class_votes =  reinterpret_cast<WeightInt*>(neon_alloc(16, state.num_classes * sizeof(WeightInt)));
+                state.class_votes =  reinterpret_cast<WeightInt*>(safe_aligned_alloc(32, state.num_classes * sizeof(WeightInt)));
 
                 memset(state.class_votes, 0, sizeof(WeightInt) * state.num_classes);
-                state.rng.seed(seed);
 
                 init_clauses(state);
                 init_clause_weights(state);
 
                 return true;
             }
 
@@ -475,15 +153,15 @@
                         state.clause_weights[k] = -1;
 
                 }
             }        
     };
 
     template <typename _State,  bool do_literal_budget>
-    class CleanupAlignedNeon32
+    class CleanupAlignedNeon
     {
         public:                        
             void operator()(_State& state)
             {
                 free(state.clauses);
                 state.clauses = nullptr;     
 
@@ -806,21 +484,21 @@
 
                     if(do_literal_budget)
                     {
                         if(state.literal_counts[clause_k] > state.literal_budget)
                             state.clause_outputs[clause_k] = 0;
                     }
 
-                    if( state.rng_nv.next_u() < prob_positive)
+                    if( state.fast_rng.next_u() < prob_positive)
                     {
                         _ClauseUpdate clause_update;
                         clause_update(state, clause_row, clause_weights + positive_class, 1, literals, state.clause_outputs[clause_k]);                    
                     }
       
-                    if( state.rng_nv.next_u() < prob_negative)
+                    if( state.fast_rng.next_u() < prob_negative)
                     {
                         _ClauseUpdate update_clause;
                         update_clause(state, clause_row, clause_weights + negative_class, -1, literals, state.clause_outputs[clause_k]);
                     }
                 }
             }
     };
@@ -856,27 +534,26 @@
 
                     _T2Feedback t2;
                     t2(state, clause_row, literals);
                 }
             }
     };
 
-    template <typename _State>
+    template <typename _State, bool use_boost_true_positive>
     class Type1aFeedbackNeon
     {
         public:
             void operator()(_State& state, int8_t* clause_row, const uint8_t* literals_in)
             {
                 //std::cout << "==== NEON T1a - start ========" << std::endl;
-                constexpr bool use_boost_true_positive = false;
 
                 int8_t* clause = (int8_t*)__builtin_assume_aligned(clause_row, 32);
                 const int8_t* literals = (int8_t*)__builtin_assume_aligned(literals_in, 32);
 
-                int8x16_t _minus_one = vdupq_n_s8(-1);                
+                // int8x16_t _minus_one = vdupq_n_s8(-1);                
                 int8x16_t _cmp_s = vdupq_n_s8(state.gtcmp_for_s);
 
                                 
 
                 const int n_chunks = (state.num_literals_mem / state.literals_per_vector);                                            
                 int8x16_t _ones = vdupq_n_s8(1);
```

### Comparing `green_tsetlin-0.1.9/src/func_nv.hpp` & `green_tsetlin-1.0.0/src/func_tm.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,143 +1,47 @@
-#ifndef _FUNC_UPDATE_HPP_
-#define _FUNC_UPDATE_HPP_
-
-
+#ifndef _FUNC_TM_HPP_
+#define _FUNC_TM_HPP_
 
 #include <random>
 #include <vector>
 
 #include <gt_common.hpp>
 
 
 namespace green_tsetlin
 {
-    class CoaleasedTsetlinStateNV
-    {
-        public:
-            double s = -42.0;
-            int num_clauses = 0;
-            int num_classes = 0;
-            int num_literals = 0;
-            int num_literals_mem = 0; 
-
-            std::default_random_engine rng;
-            int8_t* clauses = nullptr;
-            ClauseOutputUint* clause_outputs = nullptr;
-            WeightInt* class_votes = nullptr;
-            WeightInt* clause_weights = nullptr;
-
-            uint32_t* literal_counts = nullptr;
-            uint32_t literal_budget = 0xFFFF;
-
-            inline void set_s(double s_param) { s = s_param; }
-            inline double get_s() const { return s; }
-
-            inline int8_t get_ta_state(int clause_k, int ta_i, bool ta_polarity)
-            {
-                if(ta_polarity)
-                    return clauses[(clause_k * num_literals * 2) + ta_i];
-                else
-                    return clauses[(clause_k * num_literals * 2) + num_literals + ta_i];
-            }
-
-            inline void set_ta_state(int clause_k, int ta_i, bool ta_polarity, int8_t new_state)
-            {
-                if(ta_polarity)
-                    clauses[(clause_k * num_literals * 2) + ta_i] = new_state;
-                else
-                    clauses[(clause_k * num_literals * 2) + num_literals + ta_i] = new_state;
-            }
-
-            inline WeightInt get_clause_weight(int clause_index, int target_class)
-            {
-                //std::cout << "get_clause_weight(NV):" << clause_index << ", " << target_class << std::endl;
-                //int index = (clause_index * num_classes) + target_class;
-                //std::cout << "@:" << index << std::endl;
-                //clause_index << ", " << target_class << " num_classes:" << num_classes << std::endl;
-                return clause_weights[(clause_index * num_classes) + target_class];
-            }
-
-            inline void set_clause_weight(int clause_index, int target_class, int32_t new_weight)
-            {
-                clause_weights[(clause_index * num_classes) + target_class] = new_weight;
-            }
-
-            inline WeightInt* get_class_votes() const
-            {
-                return class_votes;
-            }
-
-            inline std::vector<int8_t> get_copy_clauses() const
-            {                
-                std::size_t n_total_literals = num_clauses * (num_literals*2);                
-                std::vector<int8_t>  states(clauses, clauses + n_total_literals);
-               return states;
-            }
-
-            inline std::vector<uint32_t> get_copy_literal_counts() const 
-            {          
-                std::vector<uint32_t>  counts(literal_counts, literal_counts + num_clauses);
-                return counts;
-            }
-
-            inline void get_clause_state(int8_t* dst, int clause_offset)
-            {
-                const size_t state_size = num_clauses * (num_literals * 2);
-                const size_t dst_offset = clause_offset * (num_literals * 2);
-
-                memcpy(&dst[dst_offset], clauses, state_size);
-            }
-
-            inline void set_clause_state(int8_t* src, int clause_offset)
-            {
-                const size_t state_size = num_clauses * num_literals * 2;
-                const size_t src_offset = clause_offset * (num_literals * 2);
-                memcpy(clauses, &src[src_offset], state_size);
-            }
-
-            inline void get_clause_weights(WeightInt* dst, int clause_offset) 
-            {
-                const size_t weight_mem = num_clauses * num_classes * sizeof(WeightInt);
-                const size_t dst_offset = (clause_offset * num_classes);
-                memcpy(&dst[dst_offset], clause_weights, weight_mem);
-            }
-
-            inline void set_clause_weights(WeightInt* src, int clause_offset)
-            {
-                const size_t weight_mem = num_clauses * num_classes * sizeof(WeightInt);
-                const size_t src_offset = (clause_offset * num_classes);
-
-                memcpy(clause_weights, &src[src_offset], weight_mem);
-            }
-    };
 
     template <typename _State, bool do_literal_budget>
-    class InitializeNV
+    class InitializeTM
     {
         public:                        
             bool operator()(_State& state, unsigned int seed)
             {
+                if(seed == 0)
+                    return false;
+                    
                 int clause_mem = state.num_clauses * state.num_literals * 2;
                 state.clauses = new int8_t[clause_mem];
 
                 state.num_literals_mem = state.num_literals;
 
                 state.clause_outputs = new ClauseOutputUint[state.num_clauses];                
                 memset(state.clause_outputs, 0, sizeof(ClauseOutputUint) * state.num_clauses);
                 
                 state.clause_weights = new WeightInt[state.num_clauses * state.num_classes];
+                state.num_class_weights_mem = state.num_classes;
 
                 state.class_votes = new WeightInt[state.num_classes];
                 memset(state.class_votes, 0, sizeof(WeightInt) * state.num_classes);
 
                 if(do_literal_budget)
                     state.literal_counts = new uint32_t[state.num_clauses];
 
                 state.rng.seed(seed);
+                state.fast_rng.seed(seed);
 
                 init_clauses(state);
                 init_clause_weights(state);
 
                 return true;
             }
 
@@ -156,25 +60,25 @@
 
             void init_clause_weights(_State& state)
             {
                 std::bernoulli_distribution dist(0.5);
                 const int num_weights_total = state.num_clauses * state.num_classes;
                 for(int k = 0; k < num_weights_total; ++k)
                 {
-                    if(dist(state.rng))
+                    if(state.fast_rng.next_u() > 0.5)
                         state.clause_weights[k] = 1;
                     else
                         state.clause_weights[k] = -1;
 
                 }
             }        
-    };
+    }; 
 
     template <typename _State, bool do_literal_budget>
-    class CleanupNV
+    class CleanupTM
     {
         public:                        
             void operator()(_State& state)
             {
                 delete[] state.clauses;
                 state.clauses = nullptr;     
 
@@ -189,27 +93,26 @@
                     delete[] state.literal_counts;
                     state.literal_counts = nullptr;
                 }
             }
     };
 
 
-    
-
     template <typename _State, bool do_literal_budget>
-    class SetClauseOutputNV
+    class SetClauseOutputTM
     {
         public: 
             void operator()(_State& state, uint8_t* literals)
             {
                 for(int clause_k = 0; clause_k < state.num_clauses; ++clause_k)
                 {
+                    uint32_t pos_literal_count = 0;
+                    uint32_t neg_literal_count = 0;
+
                     state.clause_outputs[clause_k] = 1;
-                    if(do_literal_budget)
-                        state.literal_counts[clause_k] = 0;
                         
                     int8_t* pl_pos = &state.clauses[clause_k * (state.num_literals*2)];
                     int8_t* pl_neg = &state.clauses[(clause_k * (state.num_literals*2)) + state.num_literals];
 
                     for(int literal_k = 0; literal_k < state.num_literals; ++literal_k)
                     {                        
 
@@ -218,37 +121,42 @@
                             if(literals[literal_k] == 0)
                             {
                                 state.clause_outputs[clause_k] = 0;
                                 break;
                             }
 
                             if(do_literal_budget)
-                                state.literal_counts[clause_k]++;
+                               pos_literal_count++;
                         }
                         pl_pos++;
 
                         if(*pl_neg >= 0) 
                         {                            
                             if(literals[literal_k] == 1)
                             {
                                 state.clause_outputs[clause_k] = 0;
                                 break;
                             }
 
                             if(do_literal_budget)
-                                state.literal_counts[clause_k]++;
+                                neg_literal_count++;
                         }
                         pl_neg++;                                                                     
                     }
+                        
+                    if(do_literal_budget)
+                        state.literal_counts[clause_k] = pos_literal_count + neg_literal_count;
+                    
                 }
             }
     };
 
+
     template <typename _State>
-    class EvalClauseOutputNV
+    class EvalClauseOutputTM
     {
         public:
             void operator()(_State& state, uint8_t* literals)
             {
                 for(int clause_k = 0; clause_k < state.num_clauses; ++clause_k)
                 {                    
                     state.clause_outputs[clause_k] = 1;
@@ -285,22 +193,22 @@
                     if(is_empty_clause)
                         state.clause_outputs[clause_k] = 0;
                 }
             }
     };
 
     template <typename _State>
-    class EmptyCountVotesNV
+    class EmptyCountVotesTM
     {
         public:
             void operator()(_State& state) {}
     };
 
     template <typename _State>
-    class CountVotesNV
+    class CountVotesTM
     {
         public:
             void operator()(_State& state)
             {
                 memset(state.class_votes, 0, sizeof(WeightInt) * state.num_classes);                
                 for(int clause_k = 0; clause_k < state.num_clauses; ++clause_k)
                 {
@@ -313,51 +221,48 @@
                         }
                     }
                 }   
             }
     };
 
     template <typename _State, typename _ClauseUpdate, bool do_literal_budget>
-    class TrainUpdateNV
+    class TrainUpdateTM
     {
         public:
             void operator()(_State& state, uint8_t* literals, int positive_class, double prob_positive, int negative_class, double prob_negative)
             {
-                std::uniform_real_distribution<double> u(0.0,1.0);
-
                 const int n_features = state.num_literals * 2;
                 for(int clause_k = 0; clause_k < state.num_clauses; ++clause_k)
                 {
                     int8_t* clause_row = &state.clauses[clause_k * n_features];
                     WeightInt* clause_weights = &state.clause_weights[clause_k * state.num_classes];
 
                     if(do_literal_budget)
                     {
                         if(state.literal_counts[clause_k] > state.literal_budget)
                             state.clause_outputs[clause_k] = 0;
                     }
 
-                    if( u(state.rng) < prob_positive)
+                    if(state.fast_rng.next_u() < prob_positive)
                     {
                         _ClauseUpdate clause_update;
                         clause_update(state, clause_row, clause_weights + positive_class, 1, literals, state.clause_outputs[clause_k]);                    
                     }
       
-                    if( u(state.rng) < prob_negative)
+                    if(state.fast_rng.next_u() < prob_negative)
                     {
                         _ClauseUpdate update_clause;
                         update_clause(state, clause_row, clause_weights + negative_class, -1, literals, state.clause_outputs[clause_k]);
                     }
                 }
             }
-
     };
 
     template <typename _State, typename _T1aFeedback, typename _T1bFeedback, typename _T2Feedback>
-    class ClauseUpdateNV
+    class ClauseUpdateTM
     {
         public:
             void operator()(_State& state, int8_t* clause_row, WeightInt* clause_weight, int target, uint8_t* literals, ClauseOutputUint clause_output)
             {
                 int32_t sign = (*clause_weight) >= 0 ? +1 : -1;                
                 
                 if( (target * sign) > 0)
@@ -368,130 +273,128 @@
 
                         _T1aFeedback    t1a;
                         t1a(state, clause_row, literals);
                     }
                     else
                     {
                         _T1bFeedback    t1b;
-                        t1b(state, clause_row, literals);
+                        t1b(state, clause_row);
                     }
                 }
                 else if((target * sign) < 0 && clause_output == 1)
                 {
                     (*clause_weight) -= sign;
 
                     _T2Feedback t2;
                     t2(state, clause_row, literals);
                 }
             }
     };
 
-    template <typename _State>
-    class Type1aFeedbackNV
+    template <typename _State, bool boost_true_positive>
+    class Type1aFeedbackTM
     {
         public:
             void operator()(_State& state, int8_t* clause_row, uint8_t* literals)
             {
-                constexpr bool use_boost_true_positive = false;
-
                 std::uniform_real_distribution<double> u(0.0,1.0);
                 
-                const double s_inv = (1.0 / state.s);
-                const double s_min1_inv = (state.s - 1.0) / state.s;
+                // const double s_inv = (1.0 / state.s);
+                // const double s_min1_inv = (state.s - 1.0) / state.s;
 
                 const int8_t lower_state = -127;
                 const int8_t upper_state =  127;
                 
                 int8_t* neg_clause_row = &clause_row[state.num_literals]; 
                                
                 for(int literal_k = 0; literal_k < state.num_literals; ++literal_k)
                 {
                     if(literals[literal_k] == 1)
                     {
                         
                         // POS 2
-                        if(use_boost_true_positive)
+                        if(boost_true_positive)
                         {
                             if(clause_row[literal_k] < upper_state)
                                 clause_row[literal_k] += 1;
                         }
                         else
                         {
-                            if( u(state.rng) <= s_min1_inv)
+                            if( u(state.rng) <= state.s_min1_inv)
                             {
                                 if(clause_row[literal_k] < upper_state)
                                     clause_row[literal_k] += 1;
                             }
                         }
                         
 
                         // NEG 3
-                        if( u(state.rng) <= s_inv )
+                        if( u(state.rng) <= state.s_inv )
                         {
                             if(neg_clause_row[literal_k] > lower_state)
                                 neg_clause_row[literal_k] -= 1;
                         }
                     }
                     else
                     {
                         // POS 3
-                        if( u(state.rng) <= s_inv )
+                        if( u(state.rng) <= state.s_inv )
                         {
                             if(clause_row[literal_k] > lower_state)
                                 clause_row[literal_k] -= 1;
                         }
 
                         // NEG 2
-                        if( u(state.rng) <= s_min1_inv)
+                        if( u(state.rng) <= state.s_min1_inv)
                         {
                             if(neg_clause_row[literal_k] < upper_state)
                                 neg_clause_row[literal_k] += 1;
                         }
                     }
                 }
             }
     };
 
-     template <typename _State>
-    class Type1bFeedbackNV
+    template <typename _State>
+    class Type1bFeedbackTM
     {
         public:
-            void operator()(_State& state, int8_t* clause_row, uint8_t* literals)
+            void operator()(_State& state, int8_t* clause_row)
             {
                 std::uniform_real_distribution<double> u(0.0,1.0);
                 
-                const double s_inv = (1.0 / state.s);
+                // const double s_inv = (1.0 / state.s);
                 const int8_t lower_state = -127;
                 
                 int8_t* neg_clause_row = &clause_row[state.num_literals]; 
                 for(int literal_k = 0; literal_k < state.num_literals; ++literal_k)
                 {
                     // POS 1
-                    if(u(state.rng) <= s_inv)
+                    if(u(state.rng) <= state.s_inv)
                     {
                         if(clause_row[literal_k] > lower_state)
                             clause_row[literal_k] -= 1;
                         
                     }
 
                     // NEG 1
-                    if(u(state.rng) <= s_inv)
+                    if(u(state.rng) <= state.s_inv)
                     {
                         if(neg_clause_row[literal_k] > lower_state)
                             neg_clause_row[literal_k] -= 1;
                         
                     }
                 }
                 
             }
     };
 
 
     template <typename _State>
-    class Type2FeedbackNV
+    class Type2FeedbackTM
     {
         public:
             // Assume that clause_output == 1
             void operator()(_State& state, int8_t* clause_row, uint8_t* literals)
             {
                 int8_t* neg_clause_row = &clause_row[state.num_literals];                
                 for(int literal_k = 0; literal_k < state.num_literals; ++literal_k)
@@ -507,15 +410,15 @@
                         if(neg_clause_row[literal_k] < 0)                        
                             neg_clause_row[literal_k] += 1;                        
                     }
                 }
             }
     };
 
-    
-}; // namespace name
+
+}; // namespace green_tsetlin
 
 
 
 
 
-#endif // #ifndef _FUNC_UPDATE_HPP_
+#endif // #ifndef _FUNC_TM_HPP_
```

### Comparing `green_tsetlin-0.1.9/src/func_sparse.hpp` & `green_tsetlin-1.0.0/src/aligned_tsetlin_state.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,183 +1,147 @@
-#ifndef _FUNC_SPARSE_HPP_
-#define _FUNC_SPARSE_HPP_
+#ifndef _ALIGNED_TSETLIN_STATE_HPP_
+#define _ALIGNED_TSETLIN_STATE_HPP_
+
+#include <stdlib.h>
+#include <cmath>
+#include <algorithm>
+#include <vector>
 
-#include <circular_buffer.hpp>
 #include <gt_common.hpp>
+#include <random_generator.hpp>
 
 namespace green_tsetlin
 {
-    // TODO: set these types correctly 
-    // either": unordered_set / unordered_map / vector / set / map    
-    typedef typename std::unordered_set<uint32_t> SparseLiterals;  // used in SparseInput
-
-    typedef typename std::unordered_map<uint32_t, int8_t> SparseClause;
-
-    
 
-    // a clause index is type: uint32_t
-
-    class CoaleasedTsetlinStateSparseNV
+    template<int _literals_per_vector, int _outputs_per_vector>
+    class AlignedTsetlinState
     {
         public:
+            constexpr const static int literals_per_vector = _literals_per_vector;
+            constexpr const static int outputs_per_vector = _outputs_per_vector;
+
             double s = -42.0;
+            double s_inv = 1.0 / s;
+            double s_min1_inv = (s - 1.0) / s;
             int num_clauses = 0;
             int num_classes = 0;
-            int num_literals = 0;
-
-            int literal_buffer_size = 0;
-            int literal_budget = 0;
+            int num_class_weights_mem = 0;
             
-            //std::vector<SparseClause> sparse_clauses;
-            CircularBuffer<uint32_t>  active_literals;
+            int num_literals = 0;
+            int num_literals_mem = 0;
+            int num_reminder = 0;
 
-            std::default_random_engine rng;
             int8_t* clauses = nullptr;
-            int8_t* clause_outputs = nullptr;
+            ClauseOutputUint* clause_outputs = nullptr;
             WeightInt* class_votes = nullptr;
             WeightInt* clause_weights = nullptr;
 
-            inline void set_s(double s_param) { s = s_param; }
-            inline double get_s() const { return s; }
+            // literal budget
+            uint32_t* literal_counts = nullptr;
+            uint32_t literal_budget = 0xFFFF;
+
+            // conv states
+            int       num_patches_per_example= -1;
+            uint32_t* active_patches = nullptr;
+            uint32_t* literal_counts_per_patch = nullptr;
+            std::vector<uint32_t> active_patches_storage;
 
+            int8_t* reminder_mask = nullptr;
+            int8_t gtcmp_for_s = 0;
 
-            inline int8_t get_ta_state(int clause_k, int ta_i, bool ta_polarity)
-            {
-                return 0;
-            }
+            std::default_random_engine rng;
+            Wyhash64                   fast_rng;
 
-            inline void set_ta_state(int clause_k, int ta_i, bool ta_polarity, int8_t new_state)
+            #ifdef USE_AVX2
+            XorShift128plus4G           avx2_rng;
+            #endif 
+
+            #ifdef USE_NEON
+            Xoshiro128Plus  rng_neon;
+            #endif 
+            
+            inline void set_s(double s_param)
             {
-            }
+                s = s_param;
+                s_inv = 1.0 / s;
+                s_min1_inv = (s - 1.0) / s;
 
-            inline WeightInt get_clause_weight(int clause_index, int target_class)
-            {
-                return 0;
-            }
+                double p = 1 / s;
+                int32_t tmp = ((int32_t)(p * 255)) - 127;                
+                tmp += 1; // size we use < to compare and not <=
 
-            inline void set_clause_weight(int clause_index, int target_class, int32_t new_weight)
-            {
+                gtcmp_for_s = (int8_t)std::clamp(tmp, -127, 126);
             }
+            inline double get_s() const { return s; }
+
+            inline int get_number_of_patches_per_example() const { return num_patches_per_example; }
+            inline void set_number_of_patches_per_example(int a_num_patches_per_example) { num_patches_per_example = a_num_patches_per_example; }
 
             inline WeightInt* get_class_votes() const
             {
-                // just return the class votes
                 return class_votes;
             }
 
-            // ---
             inline void get_clause_state(int8_t* dst, int clause_offset)
             {
+                for(int i = 0; i < num_clauses; i++)
+                {
+                    const int src_o = i * num_literals_mem * 2;
+                    const int dst_o = (i+clause_offset) * num_literals * 2;
+
+                    memcpy(&dst[dst_o],
+                           &clauses[src_o], num_literals);
+
+                    memcpy(&dst[dst_o + num_literals],
+                           &clauses[src_o + num_literals_mem], num_literals);
+                }
             }
 
             inline void set_clause_state(int8_t* src, int clause_offset)
             {
-            }
-
-            inline void set_clause_weights(WeightInt* src, int clause_offset)
-            {
-            }
-
-            inline void get_clause_weights(WeightInt* dst, int clause_offset)
-            {
-            }
-
-    };
-
-    template <typename _State>
-    class InitializeSparseNV
-    {
-        public:                        
-            bool operator()(_State& state, unsigned int seed)
-            {
-                state.rng.seed(seed);
-
-                init_clauses(state);
-                init_clause_weights(state);
-
-                return true;
-            }
-
-        
-        private:
-            void init_clauses(_State& state)
-            {
-            }
 
-            void init_clause_weights(_State& state)
-            {
-            }        
-    };
-
-    template <typename _State>
-    class CleanupSparseNV
-    {
-        public:                        
-            void operator()(_State& state)
-            {
+                for(int i = 0; i < num_clauses; i++)
+                {                    
+                    const int src_o = (i+clause_offset) * (num_literals * 2);
+                    const int dst_o = i * (num_literals_mem * 2);
+
+                    memcpy(&clauses[dst_o],
+                           &src[src_o], num_literals);
+
+                    memcpy(&clauses[dst_o + num_literals_mem],
+                           &src[src_o + num_literals], num_literals);
+                }
             }
-    };
 
-
-
-    template <typename _State>
-    class SetClauseOutputSparseNV
-    {
-        public: 
-            void operator()(_State& state, const SparseLiterals* literals)
-            {
-            }
-    };
-    
-    template <typename _State>
-    class EvalClauseOutputSparseNV
-    {
-        public:
-            void operator()(_State& state, const SparseLiterals* literals)
+            inline void set_clause_weights(WeightInt* src, int clause_offset)
             {
-            }
-    };
+                //const size_t weight_mem = num_clauses * num_classes * sizeof(WeightInt);
+                //memcpy(clause_weights, src, weight_mem);
 
-    template <typename _State, typename _SparseClauseUpdate>
-    class TrainUpdateSparseNV
-    {
-        public:
-            void operator()(_State& state, const SparseLiterals* literals, int positive_class, double prob_positive, int negative_class, double prob_negative)
-            {      
+                for(int i = 0; i < num_clauses; i++)
+                {                    
+                    const int src_o = (i+clause_offset) * num_classes;
+                    const int dst_o = i * num_class_weights_mem;
+
+                    memcpy(&clause_weights[dst_o],
+                           &src[src_o], num_classes * sizeof(WeightInt));
+                }
             }
-    };
-
-    template <typename _State, typename _T1Feedback, typename _T2Feedback>
-    class ClauseUpdateSparseNV
-    {
-        public:
-            void operator()(_State& state, int clause_k, int32_t* clause_weight, int target, const SparseLiterals* literals, int8_t clause_output)
-            {
-            }
-    };
-
 
-    template <typename _State>
-    class Type1FeedbackSparseNV
-    {
-        public:
-            void operator()(_State& state, int clause_k, int8_t clause_output, const SparseLiterals* literals)
+            inline void get_clause_weights(WeightInt* dst, int clause_offset)
             {
+                for(int i = 0; i < num_clauses; i++)
+                {
+                    const int src_o = i * num_class_weights_mem;
+                    const int dst_o = (i+clause_offset) * num_classes;
+
+                    memcpy(&dst[dst_o],
+                           &clause_weights[src_o], num_classes * sizeof(WeightInt));
+                }
             }
-    };
-
-
-    template <typename _State>
-    class Type2FeedbackSparseNV
-    {
-        public:
-            // Assume that clause_output == 1
-            void operator()(_State& state, int clause_k, const SparseLiterals* literals)
-            {               
-            }
-    };
+    };  
 }; // namespace green_tsetlin
 
 
 
 
-#endif // #ifndef _FUNC_SPARSE_HPP_
+#endif // #define _ALIGNED_TSETLIN_STATE_HPP_
```

### Comparing `green_tsetlin-0.1.9/src/inference.hpp` & `green_tsetlin-1.0.0/src/inference.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,156 +1,147 @@
-#ifndef __INFERENCE__HPP_
-#define __INFERENCE__HPP_
-
+#ifndef _INFERENCE_HPP_
+#define _INFERENCE_HPP_
 
 #include <iostream>
 #include <vector>
 #include <vector>
 #include <cstdlib>
 #include <unordered_set>
 
 #include <pybind11/pybind11.h>
 #include <pybind11/numpy.h>
 
+
 namespace green_tsetlin
 {
-    typedef std::vector<uint32_t> InfRule;
-    typedef std::vector<InfRule>  RuleVector;
-
-    typedef std::vector<WeightInt> RuleWeights;
-
+    typedef std::vector<uint32_t> InferenceRule;    
+    typedef std::vector<int32_t> RuleWeights;
 
-    template <typename _ExampleType, bool calculate_literal_importance>
+    template <typename _ExampleType, bool calculate_feature_importance, bool calculate_literal_importance, bool exclude_negative_clauses>
     class Inference
     {
         public:
             typedef _ExampleType example_type;
 
-            // note that for multi-label the num_classes will be 2x the actual classes, with ON classes first, and OFF afterwards.
-            Inference(int num_literals, int num_clauses, int num_classes, int num_features)
+            Inference(int num_literals, int num_classes, int num_explanations)
             {
                 m_num_literals = num_literals;
-                m_num_clauses = num_clauses;
                 m_num_classes = num_classes;
-                m_num_features = num_features;
+                m_num_explanations = num_explanations;
 
                 m_votes.resize(m_num_classes, 0);
-                m_feature_importance.resize(m_num_features, 0.0);
-
-                if(calculate_literal_importance)                 
-                    m_literal_importance.resize(m_num_literals*2, 0.0);
-                
 
+                if(calculate_literal_importance)
+                    m_importance_literals.resize(m_num_literals*2, 0.0);                
 
+                if(calculate_feature_importance)                                 
+                    m_importance_features.resize(num_explanations, 0.0);                                   
+                
                 // change to aligned malloc?
                 m_example = new example_type[m_num_literals*2];
                 //m_clause_features = new uint32_t[]                
             }
 
+            virtual ~Inference()
+            {
+                if(m_example != nullptr)
+                {
+                    delete[] m_example;
+                    m_example = nullptr;
+                }
+            }
+
             void set_empty_class_output(uint32_t empty_class)
             {
                 m_empty_class = empty_class;
             }
 
             uint32_t get_empty_class_output()
             {
                 return m_empty_class;
             }
 
-            virtual ~Inference()
+
+            void set_rules(std::vector<InferenceRule>& l, std::vector<RuleWeights>& w)
             {
-                if(m_example != nullptr)
-                {
-                    delete[] m_example;
-                    m_example = nullptr;
-                }
+                m_rules = l;                
+                m_weights = w;
             }
 
-
-            void set_rules_and_features(RuleVector& l, std::vector<RuleWeights>& w, RuleVector& f)
+            void set_features(std::vector<InferenceRule>& f)
             {
-                m_rules = l;
-                m_weights = w;  
-                m_features = f;
-            }
+                if(calculate_feature_importance)
+                {
+                    if(f.size() != m_num_explanations)
+                        throw std::runtime_error("Number of features much match number of explanations set.");   
 
+                    m_features = f;
+                }
+                else
+                {
+                    throw std::runtime_error("Cannot set features while note requesting feature importance.");   
+                }
+            }
 
             uint32_t predict_npy(pybind11::array_t<example_type> examples)
             {
                 pybind11::buffer_info buffer_info = examples.request();
                 std::vector<ssize_t> shape = buffer_info.shape;
 
                 example_type* example_ptr = static_cast<example_type*>(buffer_info.ptr);
                 
-                uint32_t y_hat = predict(example_ptr);            
+                uint32_t y_hat = predict(example_ptr);
                 return y_hat;
             }
 
-            pybind11::array_t<uint32_t> predict_multi_npy(pybind11::array_t<example_type> examples)
+            void calculate_explanations(uint32_t target_class)
             {
-                pybind11::buffer_info buffer_info = examples.request();
-                std::vector<ssize_t> shape = buffer_info.shape;
-
-                example_type* example_ptr = static_cast<example_type*>(buffer_info.ptr);
-                return pybind11::cast(predict_multi(example_ptr));
+                calculate_importance(target_class); 
             }
 
+
             pybind11::array_t<int32_t> get_votes_npy() 
             {
                 return pybind11::cast(m_votes);
             }
 
-            pybind11::array_t<double> calc_local_importance_npy(uint32_t target_class, bool normalize)
-            {   
-                calculate_importance_score(target_class, normalize);             
-                return pybind11::cast(m_feature_importance);
-            }
-
-            pybind11::array_t<double> get_cached_literal_importance_npy()
-            {
-                return pybind11::cast(m_literal_importance);
-            }
-
             pybind11::array_t<int> get_active_clauses_npy()
             {
                 return pybind11::cast(m_active_clauses);
             }
 
-            pybind11::array_t<uint32_t> get_rule_by_literals_npy(int k)
-            {
-                return pybind11::cast(m_rules[k]);
+            pybind11::array_t<int32_t> get_literal_importance_npy()
+            {                               
+                return pybind11::cast(m_importance_literals);
             }
 
-
-            pybind11::array_t<double>  calculate_global_importance(int y, bool normalize)
-            {
-                m_active_clauses.resize(m_num_clauses);
-                std::iota(m_active_clauses.begin(), m_active_clauses.end(), 0); // set all clauses to active => [ fill with 0 -> m_num_clauses-1 ]
-                calculate_importance_score(y, normalize);
-
-                return pybind11::cast(m_feature_importance);
+            pybind11::array_t<int32_t> get_feature_importance_npy()
+            {   
+                return pybind11::cast(m_importance_features);
             }
 
-
             uint32_t predict(example_type* example)
             {                
                 std::fill(m_votes.begin(), m_votes.end(), 0);
                 m_active_clauses.clear();
                 // copy -> rewrite to use vectors
 
                 memcpy(m_example, example, m_num_literals * sizeof(example_type));
                 for(int i = 0; i < m_num_literals; i++)
                     m_example[m_num_literals+i] = !m_example[i];
 
                 for(uint32_t clause_k = 0; clause_k < m_rules.size(); clause_k++)
                 {                    
                     for(uint32_t lit_index : m_rules[clause_k])
                     {
-                        if(m_example[lit_index] == 0)                        
+                        if(m_example[lit_index] == 0)       
+                        {
+                            //std::cout << "predict - exit: clause: " << clause_k << " l_i: " << lit_index << " x[.] == 0 (" << m_example[lit_index] << ")" << std::endl;
                             goto end_of_clause;                        
+                        }
                     }
 
                     m_active_clauses.push_back(clause_k);
 
                     for(int i = 0; i < m_num_classes; i++)
                         m_votes[i] += m_weights[clause_k][i];
 
@@ -168,134 +159,78 @@
                     {
                         best_k = i;
                         best_v = m_votes[i];
                     }
                 }
 
                 return best_k;
-
             }
 
-            std::vector<uint32_t> predict_multi(example_type* example)
+            void calculate_importance(uint32_t y)
             {
-                std::fill(m_votes.begin(), m_votes.end(), 0);
-                m_active_clauses.clear();
-                // copy -> rewrite to use vectors
-
-                memcpy(m_example, example, m_num_literals * sizeof(example_type));
-                for(int i = 0; i < m_num_literals; i++)
-                    m_example[m_num_literals+i] = !m_example[i];
-
-                for(uint32_t clause_k = 0; clause_k < m_rules.size(); clause_k++)
-                {                    
-                    for(uint32_t lit_index : m_rules[clause_k])
-                    {
-                        if(m_example[lit_index] == 0)                        
-                            goto end_of_clause;                        
-                    }
-
-                    m_active_clauses.push_back(clause_k);
-
-                    for(int i = 0; i < m_num_classes; i++)
-                        m_votes[i] += m_weights[clause_k][i];
-
-                    end_of_clause:;
-                }                
-
-                
-                int num_output_classes = m_num_classes / 2;
-                std::vector<uint32_t> multi_predict(num_output_classes, 0);
-                for(int i = 0; i < num_output_classes; ++i)
-                { 
-                    if(m_votes[i] >= m_votes[i + num_output_classes])                    
-                        multi_predict[i] = 1;                    
-                }
-
-                return multi_predict;
-            }
-
-        protected:
+                if(calculate_literal_importance)
+                    std::fill(m_importance_literals.begin(), m_importance_literals.end(), 0);
 
-            void calculate_importance_score(uint32_t y, bool normalize)
-            {
-                std::fill(m_feature_importance.begin(), m_feature_importance.end(), 0);
+                if(calculate_feature_importance)
+                    std::fill(m_importance_features.begin(), m_importance_features.end(), 0);
 
-                if(calculate_literal_importance)
-                    std::fill(m_literal_importance.begin(), m_literal_importance.end(), 0);
 
-                double z_f = 0.0;
-                double z_l = 0.0;
                 for(auto it = m_active_clauses.begin(); it != m_active_clauses.end(); it++)
                 {                                         
                     const int clause_k = *it;
-                    int16_t w_i = m_weights[clause_k][y];
+                    int32_t w_i = m_weights[clause_k][y];
                     
-                    if(w_i < 1) // only count positive clauses (that count towards the class)
-                        continue;
-
-                    double w = (double)w_i;                        
-                    for(uint32_t feature_index : m_features[clause_k])
+                    if(exclude_negative_clauses)
                     {
-                        m_feature_importance[feature_index] += w;
-                        z_f += w;
+                        if(w_i < 1) // only count positive clauses (that count towards the class)
+                            continue;
                     }
-                    
-                    if(calculate_literal_importance)
+
+                    if(calculate_feature_importance)
                     {
-                        for(uint32_t literal_k : m_rules[clause_k])
-                        {  
-                            m_literal_importance[literal_k] += w;     
-                            z_l += w;
+                        for(uint32_t feature_index : m_features[clause_k])
+                        {
+                            m_importance_features[feature_index] += w_i;
                         }
-                    }
-                }
 
-                if(normalize)
-                {
-                    z_f = std::max(z_f, 1.0);
-
-                    for(int feature_k = 0; feature_k < m_num_features; feature_k++)
-                        m_feature_importance[feature_k] /= z_f;
+                    }
 
                     if(calculate_literal_importance)
                     {
-                        z_l = std::max(z_l, 1.0);
-                        for(int literal_k = 0; literal_k < m_num_literals; literal_k++)
-                            m_literal_importance[literal_k] /=  z_l;                    
+                        for(uint32_t literal_k : m_rules[clause_k])
+                        {  
+                            m_importance_literals[literal_k] += w_i;
+                        }
                     }
                 }
             }
 
 
+
+        protected:
             int m_num_literals = 0;
             int m_num_clauses = 0;
             int m_num_classes = 0;
-            int m_num_features = 0;
+            size_t m_num_explanations = 0;
             uint32_t m_empty_class = 0;
 
-            RuleVector  m_rules;
-            RuleVector  m_features;
+            size_t explanation_cache_counter = 0;
+
+            std::vector<InferenceRule>  m_rules;
+            std::vector<InferenceRule>  m_features;
 
             std::vector<RuleWeights> m_weights;
             std::vector<int>         m_active_clauses;
-
-            std::vector<double>     m_feature_importance;
-            std::vector<double>     m_literal_importance;
-            
-            std::vector<int32_t> m_votes;
+            std::vector<int32_t>     m_importance_literals;
+            std::vector<int32_t>     m_importance_features;
+            std::vector<int32_t>     m_votes;
             example_type* m_example;
-    };
-
-}; // namespace green_tsetlin
-
 
 
+    };
 
 
-
-#endif // #ifndef __INFERENCE__HPP_
-
-
-
+}; // namespace green_tsetlin
 
 
 
+#endif // #ifndef _INFERENCE_HPP_
```

### Comparing `green_tsetlin-0.1.9/src/input_block.hpp` & `green_tsetlin-1.0.0/src/input_block.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 #ifndef __INPUT_BLOCK_HPP_
 #define __INPUT_BLOCK_HPP_
 
-
 #include <iostream>
-#include <vector>
-#include <stdexcept>
-#include <cstring>
-#include <thread>
-#include <mutex>
-#include <random>
-#include <vector>
-
-#include <cstdlib>
-
 #include <pybind11/pybind11.h>
 #include <pybind11/numpy.h>
+#include <stdint.h>
 
-
-//#include <clause_block.hpp>
+#include <gt_common.hpp>
 
 namespace green_tsetlin
 {
 
+
     class InputBlock
     {
         public:
             virtual ~InputBlock() {}
 
             virtual void prepare_example(int index) {}
             virtual const uint32_t* pull_current_label() const
@@ -33,31 +23,26 @@
                 return nullptr;
             }
             virtual int get_number_of_examples() const 
             {
                 return -42;
             }
 
-            virtual bool is_label_block() const
-            {
-                return false;
-            }
-
             virtual bool is_multi_label() const 
             {
                 return get_num_labels_per_example() > 1;
             }
 
             virtual int get_num_labels_per_example() const 
             {
                 return 0;
             }
     };
 
-    
+
     template <typename _ExampleType>
     class DenseInputBlock : public InputBlock
     {
         public:
             typedef _ExampleType example_type;
 
             DenseInputBlock(int num_literals)
@@ -71,19 +56,18 @@
                 m_num_examples = 0;
                 int one_example_mem = (((num_literals * sizeof(_ExampleType)) / align_to) + 1) * align_to;
 
                 m_labels = nullptr;
                 m_data = nullptr;
 
                 // allocate aligned mem for 1 data point
-                m_current_example = reinterpret_cast<_ExampleType*>(std::aligned_alloc(32, one_example_mem));
+                m_current_example = reinterpret_cast<_ExampleType*>(std::aligned_alloc(align_to, one_example_mem));
 
                 for(int i = 0; i  < one_example_mem; ++i)
                     m_current_example[i] = 0;
-
             }
 
             virtual ~DenseInputBlock()
             {
                 if(m_current_example != nullptr)
                 {
                     free(m_current_example);
@@ -94,18 +78,16 @@
             virtual int get_number_of_examples() const 
             {
                 return m_num_examples;
             }
 
             virtual void prepare_example(int index)
             {
-                if(m_labels != nullptr)
-                {                                            
-                    m_current_label = &m_labels[index*m_num_labels_per_example];
-                }
+                if(m_labels != nullptr)                                      
+                    m_current_label = &m_labels[index*m_num_labels_per_example];                
                     
                 memcpy(m_current_example, &m_data[index * m_num_literals], m_num_literals);
             }
 
             uint8_t* pull_current_example() const
             {
                 return m_current_example;
@@ -151,90 +133,145 @@
                     else                    
                         m_num_labels_per_example = shape2[1];
                     
                     m_labels = static_cast<uint32_t*>(buffer_info2.ptr);
                 }
             }
 
-            virtual bool is_label_block() const
-            {
-                return m_labels != nullptr;
-            }
-
         protected:
             int m_num_literals;
             int m_num_examples;
             int m_align_example_to;            
             int m_num_labels_per_example;
 
             example_type*               m_data;            
             uint32_t*                   m_labels;
 
             example_type*               m_current_example = nullptr;
             uint32_t*                   m_current_label;
+    };
+
+    
+    template <typename _ExampleType>
+    class SparseInputDenseOutputBlock : public DenseInputBlock<_ExampleType>
+    {
+        public:
+            SparseInputDenseOutputBlock(int num_literals) : DenseInputBlock<_ExampleType>(num_literals) {}        
+            virtual ~SparseInputDenseOutputBlock() {}
 
             
-    };
+            virtual void prepare_example(int index)
+            {
+                if(this->m_labels != nullptr)
+                    this->m_current_label = &this->m_labels[index*this->m_num_labels_per_example];
+
+                memset(this->m_current_example, 0, this->m_num_literals);
 
+                const int32_t row_end = m_indptr[index+1];
+                for(int32_t row_iter = m_indptr[index]; row_iter < row_end; row_iter++)                                    
+                {
+                    this->m_current_example[m_indices[row_iter]] = 1;
+                }   
+            }
+            
+            void set_data_sparse(pybind11::array indices, pybind11::array indptr, pybind11::array labels)
+            {
+                // 
+                pybind11::buffer_info indices_info = indices.request();                            
+                m_indices = static_cast<int32_t*>(indices_info.ptr);
+
+                pybind11::buffer_info indptr_info = indptr.request();                            
+                std::vector<ssize_t> shape_indptr = indptr_info.shape;
+
+                this->m_num_examples = shape_indptr[0] - 1;
+                m_indptr = static_cast<int32_t*>(indptr_info.ptr);
+
+                // labels
+                pybind11::buffer_info buffer_info2 = labels.request();                            
+                std::vector<ssize_t> shape2 = buffer_info2.shape;      
+                
+                if(shape2[0] != this->m_num_examples)
+                    throw std::runtime_error("Number of examples in labeles does not match number of examples provided in set_data().");
+                
+                //std::cout << "shape2.size(): " << shape2.size() << "  [0] = " << shape2[0] << std::endl;
+                if(shape2.size() == 1)                    
+                    this->m_num_labels_per_example = 1;                    
+                else                    
+                    this->m_num_labels_per_example = shape2[1];
+                
+                this->m_labels = static_cast<uint32_t*>(buffer_info2.ptr);            
+            }
+            void set_data(pybind11::array_t<uint8_t> examples, pybind11::array_t<uint32_t> labels)
+            {
+                throw std::runtime_error("Cannot use dense input for SparseInputDenseOutputBlock.");
+            }
+            
+            
+        protected:
+            int32_t*                    m_indices;
+            int32_t*                    m_indptr;
+        };
     
+
+
     template <typename _ExampleType>
     class SparseInputBlock : public InputBlock
     {
         public:
             typedef _ExampleType example_type;
 
             SparseInputBlock(int num_literals)
             {   
                 const int align_to = 32;
 
                 m_num_literals = num_literals;
                 m_align_example_to = align_to;                
                                              
                 m_num_examples = 0;
+                m_num_labels_per_example = 0;
                 m_labels = nullptr;
                 m_indices = nullptr;
                 m_indptr = nullptr;
                 
-                const int load_factor = num_literals; // TODO: check if we should have a sparsity constraint here
-                m_current_example.reserve(load_factor);
+                m_current_example.reserve(num_literals); // TODO: do we need to have memory alloc for a full example here if it is sparse?
             }
 
             virtual ~SparseInputBlock()
             {            
             }
 
             virtual int get_number_of_examples() const 
             {
                 return m_num_examples;
             }
 
             virtual void prepare_example(int index)
             {
                 if(m_labels != nullptr)
-                    m_current_label = m_labels[index];
+                    m_current_label = &m_labels[index*m_num_labels_per_example];
 
                 m_current_example.clear();
 
                 const int32_t row_end = m_indptr[index+1];
                 for(int32_t row_iter = m_indptr[index]; row_iter < row_end; row_iter++)
-                    m_current_example.insert(m_indices[row_iter]);                
-            }
-
-            std::vector<int>  get_copy_current_example()
-            {
-                std::vector<int>    out(m_current_example.begin(), m_current_example.end());
-                return out;
+                {
+                    // change here if you change SparseLiteral def (top of sparse_tsetlin_state.hpp)
+                    
+                    m_current_example.push_back(m_indices[row_iter]); // vector 
+                    // m_current_example.insert(m_indices[row_iter]); // unordered_map
+                }
+                    
             }
 
             _ExampleType* pull_current_example()
             {
                 return &m_current_example;
             }
 
-            virtual uint32_t pull_current_positive_class() const
+            virtual const uint32_t* pull_current_label() const
             {
                 return m_current_label;
             }
 
             void set_data(pybind11::array indices, pybind11::array indptr, pybind11::array labels)
             {
                 // 
@@ -243,117 +280,112 @@
 
                 pybind11::buffer_info indptr_info = indptr.request();                            
                 std::vector<ssize_t> shape_indptr = indptr_info.shape;
 
                 m_num_examples = shape_indptr[0] - 1;
                 m_indptr = static_cast<int32_t*>(indptr_info.ptr);
 
-                 // labels
-                pybind11::buffer_info label_info = labels.request();                                            
-                std::vector<ssize_t> shape2 = label_info.shape;                 
-                if(shape2.size() == 0 || shape2[0] == 0)
-                {
-                    m_labels = nullptr;
-                }           
-                else
-                {
-                    if(shape2[0] != m_num_examples)
-                        throw std::runtime_error("Number of examples in labeles does not match number of examples provided in set_csr_data().");
-
-                    m_labels = static_cast<uint32_t*>(label_info.ptr);
-                }
+                // labels
+                pybind11::buffer_info buffer_info2 = labels.request();                            
+                std::vector<ssize_t> shape2 = buffer_info2.shape;      
+                
+                if(shape2[0] != m_num_examples)
+                    throw std::runtime_error("Number of examples in labeles does not match number of examples provided in set_data().");
+                
+                //std::cout << "shape2.size(): " << shape2.size() << "  [0] = " << shape2[0] << std::endl;
+                if(shape2.size() == 1)                    
+                    m_num_labels_per_example = 1;                    
+                else                    
+                    m_num_labels_per_example = shape2[1];
+                
+                m_labels = static_cast<uint32_t*>(buffer_info2.ptr);
+            
             }
             
         protected:
             int m_num_literals;
             int m_num_examples;
             int m_align_example_to;            
+            int m_num_labels_per_example;
 
             int32_t*                    m_indices;
             int32_t*                    m_indptr;
             uint32_t*                   m_labels;
 
             example_type               m_current_example;
-            uint32_t                   m_current_label;
+            uint32_t*                  m_current_label;
     };
 
-    
-    /*
 
     inline uint8_t* cumlative_encode(uint8_t* out, uint32_t number, uint32_t size)
     {
         std::memset(out, 0, size);
         for(uint32_t i = 0; i < number; ++i)      
-        {
-            //std::cout << "adding ce-pos-emb:" << i << " of " << size << std::endl;
             out[i] = 1;        
-        }
-
+        
         return out + size;
     }
 
-
-    //std::vector<int> tsetlin_im2col(int patch_width, int patch_height, pybind11::array numpy_examples)
-    pybind11::array_t<uint8_t> tsetlin_im2col(int patch_width, int patch_height, pybind11::array_t<uint8_t> numpy_examples)
+    pybind11::array_t<uint8_t> tsetlin_im2col(pybind11::array_t<uint8_t> numpy_examples, int patch_width, int patch_height)
     {
+        /**
+         * A function for converting input image patches to a column matrix for the (Convolutional) Tsetlin Machine.
+         *
+         * @param numpy_examples input examples in a NumPy array
+         * @param patch_width width of the image patch
+         * @param patch_height height of the image patch         
+         *
+         * @return a NumPy array representing the column matrix
+         *
+         * @throws None
+         */
+        
         //data 
         pybind11::buffer_info buffer_info = numpy_examples.request();                            
         std::vector<ssize_t> shape = buffer_info.shape;
         
         const int n_examples = shape[0];
         const int width = shape[1];
         const int height = shape[2];
         const int channels = shape[3];
         uint8_t* src = static_cast<uint8_t*>(buffer_info.ptr);
 
-
         // no padding : stride is 1
         const int n_patches_y = (height - patch_height + 1);
         const int n_patches_x = (width - patch_width + 1);
         const int n_patches = n_patches_x * n_patches_y;
-        //std::cout << "n_patches_y:" << n_patches_y << std::endl;
-        //std::cout << "n_patches_x:" << n_patches_x << std::endl;
-        //std::cout << "n_patches:" << n_patches << std::endl;
 
         const int literals_features_per_patch = (patch_width * patch_height) * channels;
         const int position_emb_x_size = (width - patch_width);
         const int position_emb_y_size = (height - patch_height);
-        //std::cout << "position_emb_x_size:" << position_emb_x_size << std::endl;
-        //std::cout << "position_emb_y_size:" << position_emb_y_size << std::endl;
-        //std::cout << "literals_features_per_patch:" << literals_features_per_patch << std::endl;
 
         const int literals_per_patch = literals_features_per_patch + position_emb_x_size + position_emb_y_size;
-        //std::cout << "literals_per_patch:" << literals_per_patch << std::endl;
-
         int total_mem = n_examples * n_patches * literals_per_patch * sizeof(uint8_t);
-        //std::cout << "total mem:" << total_mem << std::endl;
-
-        uint8_t* dst_root = (uint8_t*)aligned_alloc(32, total_mem);
-        //for(int i = 0; i < total_mem; ++i)        
-        //    dst_root[i] = 133;
+        //uint8_t* dst_root = (uint8_t*)aligned_alloc(32, total_mem);
+        //uint8_t* dst_root = (uint8_t*)malloc(total_mem);
+        uint8_t* dst_root = reinterpret_cast<uint8_t*>(safe_aligned_alloc(32, total_mem));
         
         for(int example_index = 0; example_index < n_examples; ++ example_index)
         {
             uint8_t* example = &src[ example_index * (width * height * channels)];
             uint8_t* dst = &dst_root[ example_index * (n_patches * literals_per_patch) ];
 
             int patch_index = 0;
             for(int py = 0; py < n_patches_y; ++py)
             {
                 for(int px = 0; px < n_patches_x; ++px)
-                {                                        
+                {                                     
                     uint8_t* patch_dst = dst + (patch_index * literals_per_patch);
 
                     cumlative_encode(patch_dst, py, position_emb_y_size);
                     patch_dst += position_emb_y_size;
                     
                     cumlative_encode(patch_dst, px, position_emb_x_size);                
                     patch_dst += position_emb_x_size;
 
-                    
                     for(int y = 0; y < patch_height; ++y)
                     {
                         uint8_t* patch_row_start = example + ((py+y)*width*channels) + (px * channels);
                         std::memcpy(patch_dst, patch_row_start, patch_width * channels);
                         patch_dst += patch_width * channels;
                     }
                     patch_index += 1;
@@ -367,23 +399,13 @@
             free(array_mem);
         });
 
         return pybind11::array_t<uint8_t>(
             {n_examples, n_patches, literals_per_patch}, // shape
             dst_root, // the data pointer
             free_when_done);
-
-        
-
-        // std::vector<int> out;
-        // for(int i = 0; i < total_mem; ++i)
-        //     out.push_back(dst_root[i]);
-
-        // free(dst_root);
-        // return out;
-        //return dst_root;
     }
-    */
+
 
 }; // namespace green_tsetin
 
-#endif // #ifndef __INPUT_BLOCK_HPP_
+#endif // #define __INPUT_BLOCK_HPP_
```

