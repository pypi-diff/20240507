# Comparing `tmp/textdescriptives-2.8.0.tar.gz` & `tmp/textdescriptives-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textdescriptives-2.8.0.tar", last modified: Tue Apr  9 13:29:22 2024, max compression
+gzip compressed data, was "textdescriptives-2.8.1.tar", last modified: Tue May  7 13:29:32 2024, max compression
```

## Comparing `textdescriptives-2.8.0.tar` & `textdescriptives-2.8.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.628338 textdescriptives-2.8.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.608338 textdescriptives-2.8.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.608338 textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      582 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.612338 textdescriptives-2.8.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1247 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      669 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/workflows/draft-pdf.yml
--rw-r--r--   0 root         (0) root         (0)     2592 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      867 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/workflows/stale.yml
--rw-r--r--   0 root         (0) root         (0)     2254 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)     2140 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1395 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      907 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)   185655 2024-04-09 13:29:19.000000 textdescriptives-2.8.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1361 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/CITATION.cff
--rw-r--r--   0 root         (0) root         (0)     5242 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4473 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    24980 2024-04-09 13:29:22.628338 textdescriptives-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9398 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.612338 textdescriptives-2.8.0/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.616338 textdescriptives-2.8.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)   642030 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   139565 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/_static/icon_dark_old.png
--rw-r--r--   0 root         (0) root         (0)   125611 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/_static/icon_old.png
--rw-r--r--   0 root         (0) root         (0)     3540 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/coherence.rst
--rw-r--r--   0 root         (0) root         (0)     3547 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     3189 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/dependencydistance.rst
--rw-r--r--   0 root         (0) root         (0)     3198 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/descriptivestats.rst
--rw-r--r--   0 root         (0) root         (0)      477 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/extractors.rst
--rw-r--r--   0 root         (0) root         (0)     1909 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2752 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     2374 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/information_theory.rst
--rw-r--r--   0 root         (0) root         (0)      859 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      795 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      987 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)     2790 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/posstats.rst
--rw-r--r--   0 root         (0) root         (0)     8242 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/quality.rst
--rw-r--r--   0 root         (0) root         (0)     7051 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/readability.rst
--rw-r--r--   0 root         (0) root         (0)      388 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/tutorial.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.616338 textdescriptives-2.8.0/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    86776 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/tutorials/filter_corpus_using_quality.ipynb
--rw-r--r--   0 root         (0) root         (0)   115780 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/tutorials/introductory_tutorial.ipynb
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/tutorials/requirements.txt
--rw-r--r--   0 root         (0) root         (0)    13090 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/tutorials/sklearn_integration.ipynb
--rw-r--r--   0 root         (0) root         (0)     7465 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/usingthepackage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.616338 textdescriptives-2.8.0/paper/
--rw-r--r--   0 root         (0) root         (0)    23688 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9237 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)    42220 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/paper/paper_quarto.pdf
--rw-r--r--   0 root         (0) root         (0)     9724 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/paper/paper_quarto.qmd
--rw-r--r--   0 root         (0) root         (0)      473 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/paper/readme.md
--rw-r--r--   0 root         (0) root         (0)     2989 2024-04-09 13:29:19.000000 textdescriptives-2.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 13:29:22.628338 textdescriptives-2.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.604339 textdescriptives-2.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.620338 textdescriptives-2.8.0/src/textdescriptives/
--rw-r--r--   0 root         (0) root         (0)      328 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/__init__.py
--rw-r--r--   0 root         (0) root         (0)      492 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.624338 textdescriptives-2.8.0/src/textdescriptives/components/
--rw-r--r--   0 root         (0) root         (0)      396 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5353 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/coherence.py
--rw-r--r--   0 root         (0) root         (0)     5706 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     8335 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     6231 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/information_theory.py
--rw-r--r--   0 root         (0) root         (0)     4374 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)    22261 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/quality.py
--rw-r--r--   0 root         (0) root         (0)    10429 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/quality_data_classes.py
--rw-r--r--   0 root         (0) root         (0)     8209 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/readability.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.624338 textdescriptives-2.8.0/src/textdescriptives/data/
--rw-r--r--   0 root         (0) root         (0)   503663 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/data/spam.csv
--rw-r--r--   0 root         (0) root         (0)     6127 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/extractors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.624338 textdescriptives-2.8.0/src/textdescriptives/integrations/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/integrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4355 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/integrations/sklearn_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     1331 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/load_components.py
--rw-r--r--   0 root         (0) root         (0)     6212 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.628338 textdescriptives-2.8.0/src/textdescriptives.egg-info/
--rw-r--r--   0 root         (0) root         (0)    24980 2024-04-09 13:29:22.000000 textdescriptives-2.8.0/src/textdescriptives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2508 2024-04-09 13:29:22.000000 textdescriptives-2.8.0/src/textdescriptives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 13:29:22.000000 textdescriptives-2.8.0/src/textdescriptives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      500 2024-04-09 13:29:22.000000 textdescriptives-2.8.0/src/textdescriptives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-09 13:29:22.000000 textdescriptives-2.8.0/src/textdescriptives.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.628338 textdescriptives-2.8.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28399 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/books.py
--rw-r--r--   0 root         (0) root         (0)      382 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2821 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_coherence.py
--rw-r--r--   0 root         (0) root         (0)     2930 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     3505 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     5331 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_extractors.py
--rw-r--r--   0 root         (0) root         (0)     1384 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_information.py
--rw-r--r--   0 root         (0) root         (0)      705 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_load_components.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)     9308 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_quality.py
--rw-r--r--   0 root         (0) root         (0)     5308 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_readability.py
--rw-r--r--   0 root         (0) root         (0)      572 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.404860 textdescriptives-2.8.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.380860 textdescriptives-2.8.1/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.384860 textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.384860 textdescriptives-2.8.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      669 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     2592 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)      867 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/workflows/stale.yml
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)     2140 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1395 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      907 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)   187345 2024-05-07 13:29:28.000000 textdescriptives-2.8.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1361 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/CITATION.cff
+-rw-r--r--   0 root         (0) root         (0)     5242 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4473 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    24980 2024-05-07 13:29:32.404860 textdescriptives-2.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9398 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.388860 textdescriptives-2.8.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.388860 textdescriptives-2.8.1/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)   642030 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   139565 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/_static/icon_dark_old.png
+-rw-r--r--   0 root         (0) root         (0)   125611 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/_static/icon_old.png
+-rw-r--r--   0 root         (0) root         (0)     3540 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/coherence.rst
+-rw-r--r--   0 root         (0) root         (0)     3547 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/dependencydistance.rst
+-rw-r--r--   0 root         (0) root         (0)     3198 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/descriptivestats.rst
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/extractors.rst
+-rw-r--r--   0 root         (0) root         (0)     1909 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2752 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/information_theory.rst
+-rw-r--r--   0 root         (0) root         (0)      859 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      795 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      987 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/posstats.rst
+-rw-r--r--   0 root         (0) root         (0)     8242 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/quality.rst
+-rw-r--r--   0 root         (0) root         (0)     7051 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/readability.rst
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/tutorial.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.388860 textdescriptives-2.8.1/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    86776 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/tutorials/filter_corpus_using_quality.ipynb
+-rw-r--r--   0 root         (0) root         (0)   115780 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/tutorials/introductory_tutorial.ipynb
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/tutorials/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)    13090 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/tutorials/sklearn_integration.ipynb
+-rw-r--r--   0 root         (0) root         (0)     7465 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/usingthepackage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.392860 textdescriptives-2.8.1/paper/
+-rw-r--r--   0 root         (0) root         (0)    23688 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9237 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)    42220 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/paper/paper_quarto.pdf
+-rw-r--r--   0 root         (0) root         (0)     9724 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/paper/paper_quarto.qmd
+-rw-r--r--   0 root         (0) root         (0)      473 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/paper/readme.md
+-rw-r--r--   0 root         (0) root         (0)     2989 2024-05-07 13:29:28.000000 textdescriptives-2.8.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 13:29:32.404860 textdescriptives-2.8.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.380860 textdescriptives-2.8.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.392860 textdescriptives-2.8.1/src/textdescriptives/
+-rw-r--r--   0 root         (0) root         (0)      328 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      492 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.396860 textdescriptives-2.8.1/src/textdescriptives/components/
+-rw-r--r--   0 root         (0) root         (0)      396 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/coherence.py
+-rw-r--r--   0 root         (0) root         (0)     5748 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     8377 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     6261 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/information_theory.py
+-rw-r--r--   0 root         (0) root         (0)     4416 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)    21832 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/quality.py
+-rw-r--r--   0 root         (0) root         (0)    10429 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/quality_data_classes.py
+-rw-r--r--   0 root         (0) root         (0)     8209 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/readability.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.396860 textdescriptives-2.8.1/src/textdescriptives/data/
+-rw-r--r--   0 root         (0) root         (0)   503663 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/data/spam.csv
+-rw-r--r--   0 root         (0) root         (0)     6127 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/extractors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.396860 textdescriptives-2.8.1/src/textdescriptives/integrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/integrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/integrations/sklearn_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/load_components.py
+-rw-r--r--   0 root         (0) root         (0)     6212 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.400859 textdescriptives-2.8.1/src/textdescriptives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    24980 2024-05-07 13:29:32.000000 textdescriptives-2.8.1/src/textdescriptives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2508 2024-05-07 13:29:32.000000 textdescriptives-2.8.1/src/textdescriptives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 13:29:32.000000 textdescriptives-2.8.1/src/textdescriptives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      500 2024-05-07 13:29:32.000000 textdescriptives-2.8.1/src/textdescriptives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 13:29:32.000000 textdescriptives-2.8.1/src/textdescriptives.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.400859 textdescriptives-2.8.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28399 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/books.py
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2821 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_coherence.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_extractors.py
+-rw-r--r--   0 root         (0) root         (0)     1384 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_information.py
+-rw-r--r--   0 root         (0) root         (0)      705 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_load_components.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)     9278 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_quality.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_readability.py
+-rw-r--r--   0 root         (0) root         (0)      572 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_utils.py
```

### Comparing `textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/01_bugs.md` & `textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/config.yml` & `textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/.github/dependabot.yml` & `textdescriptives-2.8.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/.github/workflows/dependabot_automerge.yml` & `textdescriptives-2.8.1/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/.github/workflows/documentation.yml` & `textdescriptives-2.8.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/.github/workflows/draft-pdf.yml` & `textdescriptives-2.8.1/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/.github/workflows/release.yml` & `textdescriptives-2.8.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/.github/workflows/stale.yml` & `textdescriptives-2.8.1/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/.github/workflows/tests.yml` & `textdescriptives-2.8.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/.gitignore` & `textdescriptives-2.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/.pre-commit-config.yaml` & `textdescriptives-2.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/.zenodo.json` & `textdescriptives-2.8.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/CHANGELOG.md` & `textdescriptives-2.8.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,46 @@
 # CHANGELOG
 
 
 
+## v2.8.1 (2024-05-07)
+
+### Documentation
+
+* docs: fix link to document in readme ([`096a6b8`](https://github.com/HLasse/TextDescriptives/commit/096a6b8f92b4b2ccf03ec70e5caf320830ce113b))
+
+### Fix
+
+* fix: correctly set `symbols` and `contains` in `Quality` with custom values ([`a4dab94`](https://github.com/HLasse/TextDescriptives/commit/a4dab94c371fed1ca4c9cdb3ad9cd2dc7a0b8e8b))
+
+### Style
+
+* style: lint ([`76fa958`](https://github.com/HLasse/TextDescriptives/commit/76fa9583211af16b7ef1c60abff4b13ed3e61461))
+
+### Unknown
+
+* Merge pull request #353 from HLasse/fix-quality-threshold-not-set
+
+fix: `contains` and `symbols` not updated in `Quality` ([`cfe9b87`](https://github.com/HLasse/TextDescriptives/commit/cfe9b876885e052d8b3e62a24d7c559e0e064718))
+
+* tests: update test ([`7915eeb`](https://github.com/HLasse/TextDescriptives/commit/7915eeba0768c699dedb99f0ea6c3419e2f9104d))
+
+* Merge pull request #344 from HLasse/HLasse-patch-1
+
+docs: fix link to document in readme ([`e470db7`](https://github.com/HLasse/TextDescriptives/commit/e470db7cc759309e318aa1eaba675f755fae7ae9))
+
+* Merge pull request #342 from HLasse/update-docs
+
+Update docs ([`93b1d59`](https://github.com/HLasse/TextDescriptives/commit/93b1d59278dc86cd4e8df80247e8a1a5afda2f59))
+
+* Merge pull request #340 from sondalex/update_documentation
+
+Fix docstrings example module import error &amp; Add doctrings missing imports ([`7064c3b`](https://github.com/HLasse/TextDescriptives/commit/7064c3b5a748df7e4fdf09d4199a5cdaa7307444))
+
+
 ## v2.8.0 (2024-04-09)
 
 ### Build
 
 * build: update autodoc_pydantic to support pydantic 2 ([`e236d0d`](https://github.com/HLasse/TextDescriptives/commit/e236d0da869a71d331ac3ce19bf5c4e0045520a5))
 
 * build: require pydantic &lt;2.0.0 ([`e18a6aa`](https://github.com/HLasse/TextDescriptives/commit/e18a6aa613fed976bb86ad7010312eccd9c90fb3))
@@ -34,14 +69,16 @@
 
 * tests: update spacy model version for tests to 3.6 ([`4e2029f`](https://github.com/HLasse/TextDescriptives/commit/4e2029f9d0e0cf12ec36d8c8f0ce67bd5f01f24b))
 
 * CI: update sem ver version ([`7b24af8`](https://github.com/HLasse/TextDescriptives/commit/7b24af8fe2bbf549643bedd431f59e340a3e970c))
 
 * deps: update min spacy version to 3.6 ([`d7d5a30`](https://github.com/HLasse/TextDescriptives/commit/d7d5a30ea19a399e3800e94e220264bbd2bb45c8))
 
+* Fix docstrings example module import error &amp; Add doctring missing import ([`f33a28d`](https://github.com/HLasse/TextDescriptives/commit/f33a28d70404c69c0ef745cd7adef8f32b657858))
+
 * Merge pull request #320 from HLasse/pre-commit-ci-update-config
 
 [pre-commit.ci] pre-commit autoupdate ([`5c7015a`](https://github.com/HLasse/TextDescriptives/commit/5c7015a541c717bd1001637585b65d25ac8ee70d))
 
 * [pre-commit.ci] pre-commit autoupdate
 
 updates:
```

### Comparing `textdescriptives-2.8.0/CITATION.cff` & `textdescriptives-2.8.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/CODE_OF_CONDUCT.md` & `textdescriptives-2.8.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/CONTRIBUTING.md` & `textdescriptives-2.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/LICENSE` & `textdescriptives-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/PKG-INFO` & `textdescriptives-2.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.8.0
+Version: 2.8.1
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -274,15 +274,15 @@
 
 # 🔧 Installation
 `pip install textdescriptives`
 
 # 📰 News
 
 * We now have a TextDescriptives-powered web-app so you can extract and downloads metrics without a single line of code! Check it out [here](https://huggingface.co/spaces/HLasse/textdescriptives)
-* Version 2.0 out with a new API, a new component, updated documentation, and tutorials! Components are now called by "`textdescriptives/{metric_name}`. New `coherence` component for calculating the semantic coherence between sentences. See the [documentation](https://github.com/HLasse/TextDescriptives) for tutorials and more information!  
+* Version 2.0 out with a new API, a new component, updated documentation, and tutorials! Components are now called by "`textdescriptives/{metric_name}`. New `coherence` component for calculating the semantic coherence between sentences. See the [documentation](https://hlasse.github.io/TextDescriptives/) for tutorials and more information!  
 
 
 
 # ⚡ Quick Start
 
 Use `extract_metrics` to quickly extract your desired metrics. To see available methods you can simply run:
 ```python
```

### Comparing `textdescriptives-2.8.0/README.md` & `textdescriptives-2.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # 🔧 Installation
 `pip install textdescriptives`
 
 # 📰 News
 
 * We now have a TextDescriptives-powered web-app so you can extract and downloads metrics without a single line of code! Check it out [here](https://huggingface.co/spaces/HLasse/textdescriptives)
-* Version 2.0 out with a new API, a new component, updated documentation, and tutorials! Components are now called by "`textdescriptives/{metric_name}`. New `coherence` component for calculating the semantic coherence between sentences. See the [documentation](https://github.com/HLasse/TextDescriptives) for tutorials and more information!  
+* Version 2.0 out with a new API, a new component, updated documentation, and tutorials! Components are now called by "`textdescriptives/{metric_name}`. New `coherence` component for calculating the semantic coherence between sentences. See the [documentation](https://hlasse.github.io/TextDescriptives/) for tutorials and more information!  
 
 
 
 # ⚡ Quick Start
 
 Use `extract_metrics` to quickly extract your desired metrics. To see available methods you can simply run:
 ```python
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 extensions. # ð§ Installation `pip install textdescriptives` # ð° News * We
 now have a TextDescriptives-powered web-app so you can extract and downloads
 metrics without a single line of code! Check it out [here](https://
 huggingface.co/spaces/HLasse/textdescriptives) * Version 2.0 out with a new
 API, a new component, updated documentation, and tutorials! Components are now
 called by "`textdescriptives/{metric_name}`. New `coherence` component for
 calculating the semantic coherence between sentences. See the [documentation]
-(https://github.com/HLasse/TextDescriptives) for tutorials and more
+(https://hlasse.github.io/TextDescriptives/) for tutorials and more
 information! # â¡ Quick Start Use `extract_metrics` to quickly extract your
 desired metrics. To see available methods you can simply run: ```python import
 textdescriptives as td td.get_valid_metrics() # {'quality', 'readability',
 'all', 'descriptive_stats', 'dependency_distance', 'pos_proportions',
 'information_theory', 'coherence'} ``` Set the `spacy_model` parameter to
 specify which spaCy model to use, otherwise, TextDescriptives will auto-
 download an appropriate one based on `lang`. If `lang` is set, `spacy_model` is
```

### Comparing `textdescriptives-2.8.0/docs/Makefile` & `textdescriptives-2.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/_static/icon.png` & `textdescriptives-2.8.1/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/_static/icon_dark_old.png` & `textdescriptives-2.8.1/docs/_static/icon_dark_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/_static/icon_old.png` & `textdescriptives-2.8.1/docs/_static/icon_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/coherence.rst` & `textdescriptives-2.8.1/docs/coherence.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/conf.py` & `textdescriptives-2.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/dependencydistance.rst` & `textdescriptives-2.8.1/docs/dependencydistance.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/descriptivestats.rst` & `textdescriptives-2.8.1/docs/descriptivestats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/faq.rst` & `textdescriptives-2.8.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/index.rst` & `textdescriptives-2.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/information_theory.rst` & `textdescriptives-2.8.1/docs/information_theory.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/installation.rst` & `textdescriptives-2.8.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/make.bat` & `textdescriptives-2.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/news.rst` & `textdescriptives-2.8.1/docs/news.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/posstats.rst` & `textdescriptives-2.8.1/docs/posstats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/quality.rst` & `textdescriptives-2.8.1/docs/quality.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/readability.rst` & `textdescriptives-2.8.1/docs/readability.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/tutorials/filter_corpus_using_quality.ipynb` & `textdescriptives-2.8.1/docs/tutorials/filter_corpus_using_quality.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/tutorials/introductory_tutorial.ipynb` & `textdescriptives-2.8.1/docs/tutorials/introductory_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/tutorials/sklearn_integration.ipynb` & `textdescriptives-2.8.1/docs/tutorials/sklearn_integration.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/docs/usingthepackage.rst` & `textdescriptives-2.8.1/docs/usingthepackage.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/paper/paper.bib` & `textdescriptives-2.8.1/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/paper/paper.md` & `textdescriptives-2.8.1/paper/paper.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/paper/paper_quarto.pdf` & `textdescriptives-2.8.1/paper/paper_quarto.pdf`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/paper/paper_quarto.qmd` & `textdescriptives-2.8.1/paper/paper_quarto.qmd`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/pyproject.toml` & `textdescriptives-2.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "textdescriptives"
-version = "2.8.0"
+version = "2.8.1"
 description = "A library for calculating a variety of features from text using spaCy"
 authors = [
     { name = "Lasse Hansen", email = "lasseh0310@gmail.com" },
     { name = "Kenneth Enevoldsen" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `textdescriptives-2.8.0/src/textdescriptives/components/coherence.py` & `textdescriptives-2.8.1/src/textdescriptives/components/coherence.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,14 +134,15 @@
             nlp.add_pipe call, using the name argument.
 
     Returns:
         Callable[[Doc], Doc]: The Coherence component to be added to the pipe.
 
     Examples:
         >>> import spacy
+        >>> import textdescriptives as td
         >>> nlp = spacy.load("en_core_web_md")
         >>> nlp.add_pipe("textdescriptives/coherence")
         >>> # apply the pipeline to a text
         >>> doc = nlp("This is a sentence. This is another sentence.")
         >>> # get coherence values
         >>> doc._.coherence
     """
```

### Comparing `textdescriptives-2.8.0/src/textdescriptives/components/dependency_distance.py` & `textdescriptives-2.8.1/src/textdescriptives/components/dependency_distance.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,15 @@
             nlp.add_pipe call, using the name argument.
 
     Returns:
         Callable[[Doc], Doc]: The DependencyDistance component
 
     Example:
         >>> import spacy
+        >>> import textdescriptives as td
         >>> nlp = spacy.load("en_core_web_sm")
         >>> nlp.add_pipe("textdescriptives/dependency_distance")
         >>> # apply the pipeline to a text
         >>> doc = nlp("This is a sentence.")
         >>> # access the dependency distance attributes
         >>> doc._.dependency_distance
     """
```

### Comparing `textdescriptives-2.8.0/src/textdescriptives/components/descriptive_stats.py` & `textdescriptives-2.8.1/src/textdescriptives/components/descriptive_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,15 @@
             nlp.add_pipe call, using the name argument.
 
     Returns:
         Callable[[Doc], Doc]: DescriptiveStatistics component
 
     Example:
         >>> import spacy
+        >>> import textdescriptives as td
         >>> nlp = spacy.blank("en")
         >>> # add sentencizer
         >>> nlp.add_pipe("sentencizer")
         >>> # add descriptive stats
         >>> nlp.add_pipe("textdescriptives/descriptive_stats")
         >>> # apply to a document
         >>> doc = nlp("This is a sentence. This is another sentence.")
```

### Comparing `textdescriptives-2.8.0/src/textdescriptives/components/information_theory.py` & `textdescriptives-2.8.1/src/textdescriptives/components/information_theory.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,15 @@
 
     Args:
         - nlp: The spaCy Language object.
         - name: The name of the component.
 
     Example:
         >>> import spacy
-        >>> nlp = spacy.blank('en_core_web_lg')
+        >>> import textdescriptives as td
+        >>> nlp = spacy.blank('en')
         >>> nlp.add_pipe('textdescriptives/information_theory')
         >>> doc = nlp('This is a sentence.')
         >>> doc._.information_theory
         {'entropy': ...
     """
     return InformationTheory(nlp, name, force=False)
```

### Comparing `textdescriptives-2.8.0/src/textdescriptives/components/pos_proportions.py` & `textdescriptives-2.8.1/src/textdescriptives/components/pos_proportions.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
             detailed token.tag attribute.
 
     Returns:
         Callable[[Doc], Doc]: The POSProportions component to be added to the pipe.
 
     Example:
         >>> import spacy
+        >>> import textdescriptives as td
         >>> nlp = spacy.load("en_core_web_sm")
         >>> nlp.add_pipe("textdescriptives/pos_proportions")
         >>> # apply the component to a document
         >>> doc = nlp("This is a test sentence.")
         >>> doc._.pos_proportions
     """
```

### Comparing `textdescriptives-2.8.0/src/textdescriptives/components/quality.py` & `textdescriptives-2.8.1/src/textdescriptives/components/quality.py`

 * *Files 3% similar despite different names*

```diff
@@ -363,34 +363,32 @@
     attribute.
     """
 
     def __init__(  # pylint: disable=dangerous-default-value
         self,
         nlp: Language,
         name: str,
-        symbols: List[str],
-        contains: List[str],
         top_ngram_range: Tuple[int, int],
         top_ngram_min_count: int,
         duplicate_n_gram_fraction_range: Tuple[int, int],
         vocab: Optional[Mapping],
         quality_thresholds: Optional[QualityThresholds] = None,
         force: bool = False,
     ):  # noqa: D107
         """Initialise components."""
         self.name = name
         self.force = force
-        self.symbols = symbols
-        self.contains = contains
         self.top_ngram_range = top_ngram_range
         self.top_ngram_min_count = top_ngram_min_count
         self.duplicate_n_gram_fraction_range = duplicate_n_gram_fraction_range
+
         if quality_thresholds is None:
             quality_thresholds = QualityThresholds()
-        self.quality_thresholds = quality_thresholds
+        self.set_quality_thresholds(quality_thresholds)
+
         self.vocab = vocab
 
         self.set_extensions()
 
     def quality_setter(
         self,
         span: Union[Span, Doc],
@@ -556,14 +554,16 @@
     def set_quality_thresholds(self, thresholds: QualityThresholds) -> None:
         """Sets the quality thresholds.
 
         Args:
             thresholds (QualityThresholds): The desired quality thresholds.
         """
         self.quality_thresholds = thresholds
+        self.contains = list(self.quality_thresholds.contains.keys())
+        self.symbols = list(self.quality_thresholds.symbol_to_word_ratio.keys())
 
     def __call__(self, doc: Doc):
         """Run the pipeline component."""
         self.set_quality(doc)
         return doc
 
 
@@ -572,28 +572,24 @@
     assigns=[
         "doc._.quality",
         "doc._.passed_quality_check",
         "span._.quality",
         "span._.passed_quality_check",
     ],
     default_config={
-        "symbols": ["#"],
-        "contains": ["lorem ipsum"],
         "top_ngram_range": [2, 4],
         "top_ngram_min_count": 3,
         "duplicate_n_gram_fraction_range": [5, 10],
         "vocab": None,
         "force": True,
     },
 )
 def create_quality_component(
     nlp: Language,
     name: str,
-    symbols: List[str],
-    contains: List[str],
     top_ngram_range: Tuple[int, int],
     top_ngram_min_count: int,
     duplicate_n_gram_fraction_range: Tuple[int, int],
     vocab: Optional[Mapping],
     force: bool = True,
 ) -> Callable[[Doc], Doc]:
     """Allows Quality to be added to a spaCy pipe using
@@ -624,18 +620,14 @@
     text-to-text transformer. J. Mach. Learn. Res., 21(140), 1-67.
 
     Args:
         nlp (Language): spaCy language object, does not need to be specified in the
             nlp.add_pipe call.
         name (str): name of the component. Can be optionally specified in the
             nlp.add_pipe call, using the name argument.
-        symbols (List[str]): list of symbols for which to calculate the
-            proportion the ratio of symbols to words. Defaults to ["#"].
-        contains (List[str]): list of strings for which to check whether the
-            document contains them. Defaults to ["lorem ipsum"].
         top_ngram_range (Tuple[int]): range of n-grams to calculate the
             proportion of the top n-gram. Defaults to [2, 4].
         top_ngram_min_count (int): minimum number of times a n-gram must occur to
             be considered a top n-gram. Defaults to 3.
         duplicate_n_gram_fraction_range (Tuple[int]): range of n-grams to
             calculate the proportion of duplicate n-grams. Defaults to [5, 10].
         vocab (Optional[Mapping]): vocabulary to use for calculating the
@@ -648,27 +640,25 @@
 
     Returns:
         Callable[[Doc], Doc]: the Quality component
 
     Example:
         >>> import spacy
         >>> from spacy_quality import Quality
-        >>> nlp = spacy.blank(("en_core_web_sm")
+        >>> nlp = spacy.blank("en")
         >>> nlp.add_pipe("quality")
         >>> doc = nlp("This is a test")
         >>> # extract quality metrics
         >>> doc._.quality
         >>> # check whether the document passed the quality thresholds
         >>> doc._.passed_quality_check
     """
     return Quality(
         nlp,
         name=name,
-        symbols=symbols,
-        contains=contains,
         top_ngram_range=top_ngram_range,
         top_ngram_min_count=top_ngram_min_count,
         duplicate_n_gram_fraction_range=duplicate_n_gram_fraction_range,
         quality_thresholds=None,
         vocab=vocab,
         force=force,
     )
```

### Comparing `textdescriptives-2.8.0/src/textdescriptives/components/quality_data_classes.py` & `textdescriptives-2.8.1/src/textdescriptives/components/quality_data_classes.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/src/textdescriptives/components/readability.py` & `textdescriptives-2.8.1/src/textdescriptives/components/readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/src/textdescriptives/components/utils.py` & `textdescriptives-2.8.1/src/textdescriptives/components/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/src/textdescriptives/data/spam.csv` & `textdescriptives-2.8.1/src/textdescriptives/data/spam.csv`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/src/textdescriptives/extractors.py` & `textdescriptives-2.8.1/src/textdescriptives/extractors.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/src/textdescriptives/integrations/sklearn_featurizer.py` & `textdescriptives-2.8.1/src/textdescriptives/integrations/sklearn_featurizer.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/src/textdescriptives/load_components.py` & `textdescriptives-2.8.1/src/textdescriptives/load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/src/textdescriptives/utils.py` & `textdescriptives-2.8.1/src/textdescriptives/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/src/textdescriptives.egg-info/PKG-INFO` & `textdescriptives-2.8.1/src/textdescriptives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.8.0
+Version: 2.8.1
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -274,15 +274,15 @@
 
 # 🔧 Installation
 `pip install textdescriptives`
 
 # 📰 News
 
 * We now have a TextDescriptives-powered web-app so you can extract and downloads metrics without a single line of code! Check it out [here](https://huggingface.co/spaces/HLasse/textdescriptives)
-* Version 2.0 out with a new API, a new component, updated documentation, and tutorials! Components are now called by "`textdescriptives/{metric_name}`. New `coherence` component for calculating the semantic coherence between sentences. See the [documentation](https://github.com/HLasse/TextDescriptives) for tutorials and more information!  
+* Version 2.0 out with a new API, a new component, updated documentation, and tutorials! Components are now called by "`textdescriptives/{metric_name}`. New `coherence` component for calculating the semantic coherence between sentences. See the [documentation](https://hlasse.github.io/TextDescriptives/) for tutorials and more information!  
 
 
 
 # ⚡ Quick Start
 
 Use `extract_metrics` to quickly extract your desired metrics. To see available methods you can simply run:
 ```python
```

### Comparing `textdescriptives-2.8.0/src/textdescriptives.egg-info/SOURCES.txt` & `textdescriptives-2.8.1/src/textdescriptives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/tests/books.py` & `textdescriptives-2.8.1/tests/books.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/tests/test_coherence.py` & `textdescriptives-2.8.1/tests/test_coherence.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/tests/test_dependency_distance.py` & `textdescriptives-2.8.1/tests/test_dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/tests/test_descriptive_stats.py` & `textdescriptives-2.8.1/tests/test_descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/tests/test_extractors.py` & `textdescriptives-2.8.1/tests/test_extractors.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/tests/test_information.py` & `textdescriptives-2.8.1/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/tests/test_load_components.py` & `textdescriptives-2.8.1/tests/test_load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/tests/test_pos_proportions.py` & `textdescriptives-2.8.1/tests/test_pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/tests/test_quality.py` & `textdescriptives-2.8.1/tests/test_quality.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,14 @@
         contains={"lorem ipsum": False},
         oov_ratio=(None, 0.3),
     )
 
     quality_pipe = nlp.add_pipe(
         "textdescriptives/quality",
         config={
-            "symbols": ["."],
             "force": True,
         },
     )
     quality_pipe.set_quality_thresholds(quality_thresholds)
 
     doc = nlp("This is a test. This is a test. This is a test.")
     assert doc._.quality.n_stop_words == 9
```

### Comparing `textdescriptives-2.8.0/tests/test_readability.py` & `textdescriptives-2.8.1/tests/test_readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.0/tests/test_utils.py` & `textdescriptives-2.8.1/tests/test_utils.py`

 * *Files identical despite different names*

