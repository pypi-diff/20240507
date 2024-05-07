# Comparing `tmp/latexmlsuite-0.4.0.tar.gz` & `tmp/latexmlsuite-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latexmlsuite-0.4.0.tar", last modified: Fri Mar  8 20:43:52 2024, max compression
+gzip compressed data, was "latexmlsuite-0.4.1.tar", last modified: Tue May  7 14:13:17 2024, max compression
```

## Comparing `latexmlsuite-0.4.0.tar` & `latexmlsuite-0.4.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.436334 latexmlsuite-0.4.0/
--rw-rw-rw-   0        0        0      623 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/.coveragerc
--rw-rw-rw-   0        0        0      831 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/.gitignore
--rw-rw-rw-   0        0        0      513 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/.readthedocs.yml
--rw-rw-rw-   0        0        0       66 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/AUTHORS.rst
--rw-rw-rw-   0        0        0      587 2024-03-08 20:34:59.000000 latexmlsuite-0.4.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0    14233 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1103 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3049 2024-03-08 20:43:52.433000 latexmlsuite-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1754 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.039371 latexmlsuite-0.4.0/docs/
--rw-rw-rw-   0        0        0     1183 2024-03-08 07:55:19.000000 latexmlsuite-0.4.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.043392 latexmlsuite-0.4.0/docs/_static/
--rw-rw-rw-   0        0        0       19 2024-03-08 07:55:19.000000 latexmlsuite-0.4.0/docs/_static/.gitignore
--rw-rw-rw-   0        0        0       43 2024-03-08 07:55:19.000000 latexmlsuite-0.4.0/docs/authors.rst
--rw-rw-rw-   0        0        0       45 2024-03-08 07:55:19.000000 latexmlsuite-0.4.0/docs/changelog.rst
--rw-rw-rw-   0        0        0    10051 2024-03-08 07:55:19.000000 latexmlsuite-0.4.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2024-03-08 07:55:19.000000 latexmlsuite-0.4.0/docs/contributing.rst
--rw-rw-rw-   0        0        0     2394 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/docs/index.rst
--rw-rw-rw-   0        0        0       74 2024-03-08 07:55:19.000000 latexmlsuite-0.4.0/docs/license.rst
--rw-rw-rw-   0        0        0       41 2024-03-08 07:55:19.000000 latexmlsuite-0.4.0/docs/readme.rst
--rw-rw-rw-   0        0        0      238 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:51.894167 latexmlsuite-0.4.0/examples/
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.100045 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/
--rw-rw-rw-   0        0        0     3591 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/.gitignore
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.116125 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/data/
--rw-rw-rw-   0        0        0      143 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/data/afmetingen_bloem.csv
--rw-rw-rw-   0        0        0      459 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/data/afmetingen_bloem.tex
--rw-rw-rw-   0        0        0     1374 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/data/maak_iris_data.py
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:51.904906 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.179000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/
--rw-rw-rw-   0        0        0     1344 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/Makefile
--rw-rw-rw-   0        0        0      797 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/gemiddelde_afmeting.tex
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:51.901385 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/highcharts/
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:51.902895 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/highcharts/hoofdstuk2/
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.192991 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/highcharts/hoofdstuk2/Fig_2_2_2/
--rw-rw-rw-   0        0        0    17943 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/highcharts/hoofdstuk2/Fig_2_2_2/afmetingen_bloem.html
--rw-rw-rw-   0        0        0     4069 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/plot_afmeting.py
--rw-rw-rw-   0        0        0     4473 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/readme.md
--rw-rw-rw-   0        0        0      225 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/sync_htmls.ps1
--rw-rw-rw-   0        0        0      206 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/sync_htmls.sh
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.277386 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/
--rw-rw-rw-   0        0        0    13478 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/2.2.1 Gemiddelde afmeting per bloemonderdeel, plaatje gemaakt met highcharts.svg
--rw-rw-rw-   0        0        0     4629 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/221 Gemiddelde afmeting per bloemonderdeel plaatje gemaakt met highcharts.json
--rw-rw-rw-   0        0        0    11580 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/afmetingen_bloem_hc.pdf
--rw-rw-rw-   0        0        0    19874 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/afmetingen_bloem_hc.svg
--rw-rw-rw-   0        0        0      832 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/gemiddelde_afmeting_hc.tex
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:51.907423 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/highcharts/
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:51.909420 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/highcharts/hoofdstuk2/
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.290410 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/highcharts/hoofdstuk2/Fig_2_2_1/
--rw-rw-rw-   0        0        0    17977 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/highcharts/hoofdstuk2/Fig_2_2_1/afmetingen_bloem_hc.html
--rw-rw-rw-   0        0        0     3337 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/readme.md
--rw-rw-rw-   0        0        0      231 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/sync_htmls.ps1
--rw-rw-rw-   0        0        0      224 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/sync_htmls.sh
--rw-rw-rw-   0        0        0     2397 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/maak_ccn_kopij.ps1
--rw-rw-rw-   0        0        0     1803 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/main.tex
--rw-rw-rw-   0        0        0      446 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/rapport_settings.yml
--rw-rw-rw-   0        0        0     4007 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/readme.md
--rw-rw-rw-   0        0        0     2039 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/references.bib
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.320025 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/sections/
--rw-rw-rw-   0        0        0     2071 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/sections/01_introductie.tex
--rw-rw-rw-   0        0        0     4696 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/sections/02_latex_voorbeelden.tex
--rw-rw-rw-   0        0        0      184 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/sections/03_conclusies.tex
--rw-rw-rw-   0        0        0      202 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/sections/A_tabellen.tex
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.333230 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/tables/
--rw-rw-rw-   0        0        0      622 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/tables/Makefile
--rw-rw-rw-   0        0        0      669 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/tables/iris_data.tex
--rw-rw-rw-   0        0        0      501 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/tables/iris_data_tabular.tex
--rw-rw-rw-   0        0        0      364 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       65 2024-03-08 19:39:58.000000 latexmlsuite-0.4.0/requirements.txt
--rw-rw-rw-   0        0        0     1446 2024-03-08 20:43:52.440852 latexmlsuite-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      728 2024-03-08 07:55:19.000000 latexmlsuite-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:51.916939 latexmlsuite-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.351955 latexmlsuite-0.4.0/src/latexmlsuite/
--rw-rw-rw-   0        0        0      593 2024-03-08 07:55:19.000000 latexmlsuite-0.4.0/src/latexmlsuite/__init__.py
--rw-rw-rw-   0        0        0    31960 2024-03-08 19:59:52.000000 latexmlsuite-0.4.0/src/latexmlsuite/main_suite.py
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.425736 latexmlsuite-0.4.0/src/latexmlsuite.egg-info/
--rw-rw-rw-   0        0        0     3049 2024-03-08 20:43:51.000000 latexmlsuite-0.4.0/src/latexmlsuite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2899 2024-03-08 20:43:51.000000 latexmlsuite-0.4.0/src/latexmlsuite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 20:43:51.000000 latexmlsuite-0.4.0/src/latexmlsuite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-03-08 20:43:51.000000 latexmlsuite-0.4.0/src/latexmlsuite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-08 20:43:48.000000 latexmlsuite-0.4.0/src/latexmlsuite.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      239 2024-03-08 20:43:51.000000 latexmlsuite-0.4.0/src/latexmlsuite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-08 20:43:51.000000 latexmlsuite-0.4.0/src/latexmlsuite.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-08 20:43:52.414976 latexmlsuite-0.4.0/tests/
--rw-rw-rw-   0        0        0      290 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/tests/conftest.py
--rw-rw-rw-   0        0        0      337 2024-03-08 20:15:25.000000 latexmlsuite-0.4.0/tests/test_main_suite.py
--rw-rw-rw-   0        0        0     2659 2023-01-27 08:57:43.000000 latexmlsuite-0.4.0/tox.ini
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.638871 latexmlsuite-0.4.1/
+-rw-rw-rw-   0        0        0      623 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/.coveragerc
+-rw-rw-rw-   0        0        0      831 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/.gitignore
+-rw-rw-rw-   0        0        0      513 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/.readthedocs.yml
+-rw-rw-rw-   0        0        0       66 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0      805 2024-05-07 13:58:11.000000 latexmlsuite-0.4.1/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    14233 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1103 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3049 2024-05-07 14:13:17.636307 latexmlsuite-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1754 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.062397 latexmlsuite-0.4.1/docs/
+-rw-rw-rw-   0        0        0     1183 2024-03-08 07:55:19.000000 latexmlsuite-0.4.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.069194 latexmlsuite-0.4.1/docs/_static/
+-rw-rw-rw-   0        0        0       19 2024-03-08 07:55:19.000000 latexmlsuite-0.4.1/docs/_static/.gitignore
+-rw-rw-rw-   0        0        0       43 2024-03-08 07:55:19.000000 latexmlsuite-0.4.1/docs/authors.rst
+-rw-rw-rw-   0        0        0       45 2024-03-08 07:55:19.000000 latexmlsuite-0.4.1/docs/changelog.rst
+-rw-rw-rw-   0        0        0     9999 2024-05-07 13:58:11.000000 latexmlsuite-0.4.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2024-03-08 07:55:19.000000 latexmlsuite-0.4.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0     2394 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/docs/index.rst
+-rw-rw-rw-   0        0        0       74 2024-03-08 07:55:19.000000 latexmlsuite-0.4.1/docs/license.rst
+-rw-rw-rw-   0        0        0       41 2024-03-08 07:55:19.000000 latexmlsuite-0.4.1/docs/readme.rst
+-rw-rw-rw-   0        0        0      301 2024-05-07 13:58:11.000000 latexmlsuite-0.4.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:16.874743 latexmlsuite-0.4.1/examples/
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.110786 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/
+-rw-rw-rw-   0        0        0     3591 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.172839 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/data/
+-rw-rw-rw-   0        0        0      143 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/data/afmetingen_bloem.csv
+-rw-rw-rw-   0        0        0      459 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/data/afmetingen_bloem.tex
+-rw-rw-rw-   0        0        0     1374 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/data/maak_iris_data.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:16.886366 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.273320 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/
+-rw-rw-rw-   0        0        0     1344 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/Makefile
+-rw-rw-rw-   0        0        0      797 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/gemiddelde_afmeting.tex
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:16.883348 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/highcharts/
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:16.884869 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/highcharts/hoofdstuk2/
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.281822 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/highcharts/hoofdstuk2/Fig_2_2_2/
+-rw-rw-rw-   0        0        0    17943 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/highcharts/hoofdstuk2/Fig_2_2_2/afmetingen_bloem.html
+-rw-rw-rw-   0        0        0     4069 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/plot_afmeting.py
+-rw-rw-rw-   0        0        0     4473 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/readme.md
+-rw-rw-rw-   0        0        0      225 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/sync_htmls.ps1
+-rw-rw-rw-   0        0        0      206 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/sync_htmls.sh
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.347822 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/
+-rw-rw-rw-   0        0        0    13478 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/2.2.1 Gemiddelde afmeting per bloemonderdeel, plaatje gemaakt met highcharts.svg
+-rw-rw-rw-   0        0        0     4629 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/221 Gemiddelde afmeting per bloemonderdeel plaatje gemaakt met highcharts.json
+-rw-rw-rw-   0        0        0    11580 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/afmetingen_bloem_hc.pdf
+-rw-rw-rw-   0        0        0    19874 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/afmetingen_bloem_hc.svg
+-rw-rw-rw-   0        0        0      832 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/gemiddelde_afmeting_hc.tex
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:16.889667 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/highcharts/
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:16.890659 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/highcharts/hoofdstuk2/
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.357834 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/highcharts/hoofdstuk2/Fig_2_2_1/
+-rw-rw-rw-   0        0        0    17977 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/highcharts/hoofdstuk2/Fig_2_2_1/afmetingen_bloem_hc.html
+-rw-rw-rw-   0        0        0     3337 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/readme.md
+-rw-rw-rw-   0        0        0      231 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/sync_htmls.ps1
+-rw-rw-rw-   0        0        0      224 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/sync_htmls.sh
+-rw-rw-rw-   0        0        0     2397 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/maak_ccn_kopij.ps1
+-rw-rw-rw-   0        0        0     1803 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/main.tex
+-rw-rw-rw-   0        0        0      446 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/rapport_settings.yml
+-rw-rw-rw-   0        0        0     4007 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/readme.md
+-rw-rw-rw-   0        0        0     2039 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/references.bib
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.386580 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/sections/
+-rw-rw-rw-   0        0        0     2071 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/sections/01_introductie.tex
+-rw-rw-rw-   0        0        0     4696 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/sections/02_latex_voorbeelden.tex
+-rw-rw-rw-   0        0        0      184 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/sections/03_conclusies.tex
+-rw-rw-rw-   0        0        0      202 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/sections/A_tabellen.tex
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.403651 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/tables/
+-rw-rw-rw-   0        0        0      622 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/tables/Makefile
+-rw-rw-rw-   0        0        0      669 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/tables/iris_data.tex
+-rw-rw-rw-   0        0        0      501 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/tables/iris_data_tabular.tex
+-rw-rw-rw-   0        0        0      364 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       65 2024-03-08 19:39:58.000000 latexmlsuite-0.4.1/requirements.txt
+-rw-rw-rw-   0        0        0     1446 2024-05-07 14:13:17.644873 latexmlsuite-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      728 2024-03-08 07:55:19.000000 latexmlsuite-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:16.900692 latexmlsuite-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.442736 latexmlsuite-0.4.1/src/latexmlsuite/
+-rw-rw-rw-   0        0        0      593 2024-03-08 07:55:19.000000 latexmlsuite-0.4.1/src/latexmlsuite/__init__.py
+-rw-rw-rw-   0        0        0    34202 2024-05-07 13:58:11.000000 latexmlsuite-0.4.1/src/latexmlsuite/main_suite.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.631642 latexmlsuite-0.4.1/src/latexmlsuite.egg-info/
+-rw-rw-rw-   0        0        0     3049 2024-05-07 14:13:16.000000 latexmlsuite-0.4.1/src/latexmlsuite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2899 2024-05-07 14:13:16.000000 latexmlsuite-0.4.1/src/latexmlsuite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:13:16.000000 latexmlsuite-0.4.1/src/latexmlsuite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-07 14:13:16.000000 latexmlsuite-0.4.1/src/latexmlsuite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-07 14:13:14.000000 latexmlsuite-0.4.1/src/latexmlsuite.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      239 2024-05-07 14:13:16.000000 latexmlsuite-0.4.1/src/latexmlsuite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-07 14:13:16.000000 latexmlsuite-0.4.1/src/latexmlsuite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 14:13:17.618993 latexmlsuite-0.4.1/tests/
+-rw-rw-rw-   0        0        0      290 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/tests/conftest.py
+-rw-rw-rw-   0        0        0      337 2024-03-08 20:15:25.000000 latexmlsuite-0.4.1/tests/test_main_suite.py
+-rw-rw-rw-   0        0        0     2659 2023-01-27 08:57:43.000000 latexmlsuite-0.4.1/tox.ini
```

### Comparing `latexmlsuite-0.4.0/.coveragerc` & `latexmlsuite-0.4.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/.gitignore` & `latexmlsuite-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/.readthedocs.yml` & `latexmlsuite-0.4.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/CONTRIBUTING.rst` & `latexmlsuite-0.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/LICENSE.txt` & `latexmlsuite-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/PKG-INFO` & `latexmlsuite-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latexmlsuite
-Version: 0.4.0
+Version: 0.4.1
 Summary: A tool to create a latex publication using latexml
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `latexmlsuite-0.4.0/README.rst` & `latexmlsuite-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/docs/Makefile` & `latexmlsuite-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/docs/conf.py` & `latexmlsuite-0.4.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,22 +149,20 @@
 todo_emit_warnings = True
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "alabaster"
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
-    "sidebar_width": "300px",
-    "page_width": "1200px"
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
```

### Comparing `latexmlsuite-0.4.0/docs/index.rst` & `latexmlsuite-0.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/.gitignore` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/.gitignore`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/data/maak_iris_data.py` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/data/maak_iris_data.py`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/Makefile` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/Makefile`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/gemiddelde_afmeting.tex` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/gemiddelde_afmeting.tex`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/highcharts/hoofdstuk2/Fig_2_2_2/afmetingen_bloem.html` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/highcharts/hoofdstuk2/Fig_2_2_2/afmetingen_bloem.html`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/plot_afmeting.py` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/plot_afmeting.py`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris/readme.md` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris/readme.md`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/2.2.1 Gemiddelde afmeting per bloemonderdeel, plaatje gemaakt met highcharts.svg` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/2.2.1 Gemiddelde afmeting per bloemonderdeel, plaatje gemaakt met highcharts.svg`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/221 Gemiddelde afmeting per bloemonderdeel plaatje gemaakt met highcharts.json` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/221 Gemiddelde afmeting per bloemonderdeel plaatje gemaakt met highcharts.json`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/afmetingen_bloem_hc.pdf` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/afmetingen_bloem_hc.pdf`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/afmetingen_bloem_hc.svg` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/afmetingen_bloem_hc.svg`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/gemiddelde_afmeting_hc.tex` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/gemiddelde_afmeting_hc.tex`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/highcharts/hoofdstuk2/Fig_2_2_1/afmetingen_bloem_hc.html` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/highcharts/hoofdstuk2/Fig_2_2_1/afmetingen_bloem_hc.html`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/readme.md` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/figures/iris_via_hc/readme.md`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/maak_ccn_kopij.ps1` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/maak_ccn_kopij.ps1`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/main.tex` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/main.tex`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/readme.md` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/readme.md`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/references.bib` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/references.bib`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/sections/01_introductie.tex` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/sections/01_introductie.tex`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/sections/02_latex_voorbeelden.tex` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/sections/02_latex_voorbeelden.tex`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/tables/Makefile` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/tables/Makefile`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/examples/voorbeeld_cbs_publicatie/tables/iris_data.tex` & `latexmlsuite-0.4.1/examples/voorbeeld_cbs_publicatie/tables/iris_data.tex`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/setup.cfg` & `latexmlsuite-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/setup.py` & `latexmlsuite-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/src/latexmlsuite/__init__.py` & `latexmlsuite-0.4.1/src/latexmlsuite/__init__.py`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/src/latexmlsuite/main_suite.py` & `latexmlsuite-0.4.1/src/latexmlsuite/main_suite.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from pathlib import Path
 
 import path
 import yaml
 
 from latexmlsuite import __version__
 
-MODES = ("all", "html", "latex", "clean", "xml", "none")
+MODES = ("all", "html", "latex", "clean", "xml", "none", "docx")
 DEFAULT_MAIN = "main"
 DEFAULT_MODE = "all"
 
 FOREGROUND_COLOR_OPTIONS = set([c for c in dir(AnsiFore) if "__" not in c])
 BACKGROUND_COLOR_OPTIONS = set([c for c in dir(AnsiBack) if "__" not in c])
 # dit is nodig om kleuren in een powershell te kunnen gebruiken
 colorama.init(True)
@@ -46,22 +46,25 @@
 
 
 # ---- CLI ----
 # The functions defined in this section are wrappers around the main Python
 # API allowing them to be called directly from the terminal as a CLI
 # executable/script.
 
+
 def check_make_was_clean(make_result):
     make_was_clean = True
     try:
         first_line = make_result[0]
     except IndexError:
         pass
     else:
-        if not ("Nothing to be done" in first_line or "Er is niets te doen" in first_line):
+        if not (
+            "Nothing to be done" in first_line or "Er is niets te doen" in first_line
+        ):
             make_was_clean = False
     return make_was_clean
 
 
 def parse_args(args):
     """Parse command line parameters
 
@@ -81,95 +84,150 @@
     parser.add_argument(
         "-v",
         "--verbose",
         dest="loglevel",
         help="set loglevel to INFO",
         action="store_const",
         const=logging.INFO,
-        default=logging.WARNING
+        default=logging.WARNING,
     )
     parser.add_argument(
         "-vv",
         "--debug",
         dest="loglevel",
         help="set loglevel to DEBUG",
         action="store_const",
         const=logging.DEBUG,
     )
     parser.add_argument(
-        "--settings_filename", help="Extra input yaml file to pass extra parameters",
-        default="rapport_settings.yml"
+        "--settings_filename",
+        help="Extra input yaml file to pass extra parameters",
+        default="rapport_settings.yml",
+    )
+    parser.add_argument(
+        "--make_exe",
+        help="executable naam om Makefile te runnen. Default 'make'",
+        default="make",
+    )
+    parser.add_argument(
+        "--no_make",
+        help="Sla het runnen van de makefiles over",
+        action="store_false",
+        default=True,
+        dest="do_make",
+    )
+    parser.add_argument(
+        "--no_scripts",
+        help="Sla het runnen van de alle scripts over",
+        action="store_false",
+        default=True,
+        dest="do_scripts",
     )
     parser.add_argument(
-        "--make_exe", help="executable naam om Makefile te runnen. Default 'make'",
-        default="make"
+        "--no_post_scripts",
+        help="Sla het runnen van de postscripts over",
+        action="store_false",
+        default=True,
+        dest="do_postscripts",
     )
     parser.add_argument(
-        "--no_make", help="Sla het runnen van de makefiles over",
-        action="store_false", default=True, dest="do_make"
+        "--no_pre_scripts",
+        help="Sla het runnen van de prescripts over",
+        action="store_false",
+        default=True,
+        dest="do_prescripts",
     )
     parser.add_argument(
-        "--no_scripts", help="Sla het runnen van de alle scripts over",
-        action="store_false", default=True, dest="do_scripts"
+        "--no_latexml",
+        help="Sla het runnen van alle latexml scripts over",
+        action="store_false",
+        default=True,
+        dest="do_latexml",
     )
     parser.add_argument(
-        "--no_post_scripts", help="Sla het runnen van de postscripts over",
-        action="store_false", default=True, dest="do_postscripts"
+        "--no_colors",
+        help="Geef geen kleur aan de commando's die naar terminal geschreven worden",
+        action="store_false",
+        default=True,
+        dest="use_terminal_colors",
     )
     parser.add_argument(
-        "--no_pre_scripts", help="Sla het runnen van de prescripts over",
-        action="store_false", default=True, dest="do_prescripts"
+        "--foreground_color",
+        help="Voorgrondkleur van commando's",
+        choices=FOREGROUND_COLOR_OPTIONS,
+        default="GREEN",
     )
     parser.add_argument(
-        "--no_latexml", help="Sla het runnen van alle latexml scripts over",
-        action="store_false", default=True, dest="do_latexml"
+        "--background_color",
+        help="Achtergrondkleur van commando's",
+        choices=BACKGROUND_COLOR_OPTIONS,
+        default=None,
     )
     parser.add_argument(
-        "--no_colors", help="Geef geen kleur aan de commando's die naar terminal geschreven worden",
-        action="store_false", default=True, dest="use_terminal_colors"
+        "--test",
+        help="Doe een droge run, dus laat alleen commando's zien",
+        action="store_true",
+        default=False,
     )
     parser.add_argument(
-        "--foreground_color", help="Voorgrondkleur van commando's",
-        choices=FOREGROUND_COLOR_OPTIONS, default="GREEN"
+        "--include_graphs",
+        help="Plot ook de tabellen en grafieken in de html output",
+        action="store_true",
+        default=False,
     )
     parser.add_argument(
-        "--background_color", help="Achtergrondkleur van commando's",
-        choices=BACKGROUND_COLOR_OPTIONS, default=None
+        "--include_hyperref",
+        help="Genereer CCN html met hyperrefs",
+        action="store_true",
+        default=True,
     )
     parser.add_argument(
-        "--test", help="Doe een droge run, dus laat alleen commando's zien",
-        action="store_true", default=False
+        "--include_nohyperref",
+        help="Genereer CCN html zonder hyperrefs",
+        action="store_false",
+        default=True,
+        dest="include_hyperref",
     )
     parser.add_argument(
-        "--include_graphs", help="Plot ook de tabellen en grafieken in de html output",
-        action="store_true", default=False
+        "--include_json",
+        help="Naast de highcharts html files worden ook de json files gesynchroniseerd in het "
+        "geval je die ook naar CCN wilt meeleveren",
+        action="store_true",
+        default=False,
     )
     parser.add_argument(
-        "--force_html", help="Forceer het compileren van de html files met latexml, ook al is er"
-                             "geen update geweest",
-        action="store_true", default=False
+        "--force_html",
+        help="Forceer het compileren van de html files met latexml, ook al is er"
+        "geen update geweest",
+        action="store_true",
+        default=False,
     )
     parser.add_argument(
-        "--mode", help="Welke type document wil je maken?",
-        choices=MODES, default=DEFAULT_MODE
+        "--mode",
+        help="Welke type document wil je maken?",
+        choices=MODES,
+        default=DEFAULT_MODE,
     )
     parser.add_argument(
-        "--no_overwrite", help="Schrijf de schoongemaakte html's naar een nieuwe file",
-        action="store_false", default=True, dest="overwrite"
+        "--no_overwrite",
+        help="Schrijf de schoongemaakte html's naar een nieuwe file",
+        action="store_false",
+        default=True,
+        dest="overwrite",
     )
     return parser.parse_args(args)
 
 
 def setup_logging(loglevel):
     """Setup basic logging
 
     Args:
       loglevel (int): minimum loglevel for emitting messages
     """
-    logformat = '%(levelname)-8s [%(filename)s:%(lineno)4d] %(message)s'
+    logformat = "%(levelname)-8s [%(filename)s:%(lineno)4d] %(message)s"
     logging.basicConfig(
         level=loglevel, stream=sys.stdout, format=logformat, datefmt="%Y-%m-%d %H:%M:%S"
     )
 
 
 def update_target_compared_to_source(source_file: Path, target_file: Path):
     """
@@ -184,49 +242,62 @@
             Name of the target file
 
     Returns: bool
         Flag indicating that the target must be updated
     """
     source_file = Path(source_file)
     target_file = Path(target_file)
-    time0 = datetime.datetime.fromtimestamp(source_file.stat().st_mtime, tz=datetime.timezone.utc)
+    time0 = datetime.datetime.fromtimestamp(
+        source_file.stat().st_mtime, tz=datetime.timezone.utc
+    )
     update_target = True
     if target_file.exists():
-        time1 = datetime.datetime.fromtimestamp(target_file.stat().st_mtime,
-                                                tz=datetime.timezone.utc)
+        time1 = datetime.datetime.fromtimestamp(
+            target_file.stat().st_mtime, tz=datetime.timezone.utc
+        )
         update_target = time1 < time0
     return update_target
 
 
-def copy_main_for_latexml(tex_input_file: Path, tex_output_file: Path,
-                          include_graphics: bool = False):
+def copy_main_for_latexml(
+    tex_input_file: Path,
+    tex_output_file: Path,
+    include_graphics: bool = False,
+    include_hyperref: bool = False,
+):
     # lees de inhoud van main en pas de opties aan om grafieken en tabellen weg te laten
     _logger.debug(f"Reading {tex_input_file}")
     with open(tex_input_file, "r") as in_stream:
         tex_content = in_stream.read()
 
     _logger.debug(f"Writing {tex_output_file}")
 
     options = ""
     if not include_graphics:
-        options += ",nographs,notables,nohyperrefs"
-    else:
+        options += ",nographs,notables"
+    if not include_hyperref:
         options += ",nohyperrefs"
     cbsdocs = "]{cbsdocs}"
 
     tex_content_new = re.sub(cbsdocs, options + cbsdocs, tex_content)
     with open(tex_output_file, "w") as out_stream:
         out_stream.write(tex_content_new)
 
 
 class TerminalColors:
-    def __init__(self, foreground_color=None, background_color=None, use_terminal_colors=False):
+    def __init__(
+        self, foreground_color=None, background_color=None, use_terminal_colors=False
+    ):
         self.use_terminal_colors = use_terminal_colors
-        self.foreground_color = self.set_color(color_name=foreground_color, foreground=True)
-        self.background_color = self.set_color(color_name=background_color, foreground=False)
+        self.foreground_color = self.set_color(
+            color_name=foreground_color, foreground=True
+        )
+        self.background_color = self.set_color(
+            color_name=background_color, foreground=False
+        )
         if use_terminal_colors:
             self.reset_colors = Style.RESET_ALL
         else:
             self.reset_colors = ""
 
     def set_color(self, color_name, foreground=True):
         if color_name is not None and self.use_terminal_colors:
@@ -237,65 +308,73 @@
         else:
             color = ""
 
         return color
 
 
 class LaTeXMLSuite:
-    def __init__(self,
-                 main_file_name="main",
-                 make_exe="make",
-                 do_make=True,
-                 do_postscripts=True,
-                 do_prescripts=True,
-                 do_latexml=True,
-                 overwrite=True,
-                 bibtex_file=None,
-                 output_directory=None,
-                 output_directory_html=None,
-                 output_directory_highcharts=None,
-                 output_directory_tabellen=None,
-                 output_filename=None,
-                 ccn_output_directory=None,
-                 makefile_directories=None,
-                 pre_scripts=None,
-                 post_scripts=None,
-                 mode=None,
-                 test=False,
-                 merge_chapters=False,
-                 include_graphs=False,
-                 platform_is_windows=False,
-                 foreground_color=None,
-                 background_color=None,
-                 use_terminal_colors=False,
-                 force_html=False
-                 ):
-
-        self.terminal_colors = TerminalColors(foreground_color=foreground_color,
-                                              background_color=background_color,
-                                              use_terminal_colors=use_terminal_colors)
+    def __init__(
+        self,
+        main_file_name="main",
+        make_exe="make",
+        do_make=True,
+        do_postscripts=True,
+        do_prescripts=True,
+        do_latexml=True,
+        overwrite=True,
+        bibtex_file=None,
+        output_directory=None,
+        output_directory_html=None,
+        output_directory_highcharts=None,
+        output_directory_tabellen=None,
+        output_filename=None,
+        ccn_output_directory=None,
+        makefile_directories=None,
+        pre_scripts=None,
+        post_scripts=None,
+        mode=None,
+        test=False,
+        merge_chapters=False,
+        include_graphs=False,
+        include_hyperref=False,
+        platform_is_windows=False,
+        foreground_color=None,
+        background_color=None,
+        use_terminal_colors=False,
+        force_html=False,
+        include_json=False,
+    ):
+
+        self.terminal_colors = TerminalColors(
+            foreground_color=foreground_color,
+            background_color=background_color,
+            use_terminal_colors=use_terminal_colors,
+        )
         self.force_html = force_html
         self.output_filename = output_filename
         if ccn_output_directory is not None:
             self.ccn_output_directory = Path(ccn_output_directory)
         else:
             self.ccn_output_directory = Path("ccn")
         self.ccn_html_dir = self.ccn_output_directory / Path("html")
+        self.ccn_docx_dir = self.ccn_output_directory / Path("docx")
         self.overwrite = overwrite
         self.makefile_directories = makefile_directories
         self.pre_scripts = pre_scripts
         self.post_scripts = post_scripts
         self.platform_is_windows = platform_is_windows
         self.make_exe = make_exe
         self.include_graphs = include_graphs
+        self.include_hyperref = include_hyperref
         self.test = test
         self.do_make = do_make
         self.do_prescripts = do_prescripts
         self.do_postscripts = do_postscripts
         self.do_latexml = do_latexml
+        self.include_json = include_json
         if main_file_name is None:
             self.main_file_name = Path("main.tex")
         else:
             self.main_file_name = Path(main_file_name)
 
         self.bibtex_file = bibtex_file
 
@@ -308,20 +387,24 @@
             self.output_directory_html = Path("out_html")
         else:
             self.output_directory_html = Path(output_directory_html)
 
         if output_directory_highcharts is None:
             self.ccn_highcharts_dir = self.ccn_output_directory / Path("highcharts")
         else:
-            self.ccn_highcharts_dir = self.ccn_output_directory / Path(output_directory_highcharts)
+            self.ccn_highcharts_dir = self.ccn_output_directory / Path(
+                output_directory_highcharts
+            )
 
         if output_directory_tabellen is None:
             self.ccn_tables_dir = self.ccn_output_directory / Path("tabellen")
         else:
-            self.ccn_tables_dir = self.ccn_output_directory / Path(output_directory_tabellen)
+            self.ccn_tables_dir = self.ccn_output_directory / Path(
+                output_directory_tabellen
+            )
 
         self.xml_refs = None
         self.updated_references = False
         self.merge_chapters = merge_chapters
 
         if mode is None:
             self.mode = "all"
@@ -345,33 +428,35 @@
         if self.pre_scripts is not None and self.do_prescripts and self.mode != "clean":
             self.launch_scripts(self.pre_scripts)
 
         if self.mode == "none":
             # met none maken we de documenten niet, alleen de make files worden gerund
             return
 
-        if self.mode in ("clean", "latex", "all"):
+        if self.mode in ("clean", "latex", "all", "docx"):
             self.launch_latexmk()
             if self.mode == "clean":
                 self.clean_log()
-        if self.mode in ("xml", "all"):
+        if self.mode in ("xml", "all", "docx"):
             self.launch_latexmk_for_html()
             self.copy_pdf()
             if self.do_latexml:
                 if self.bibtex_file is not None:
                     self.launch_latexml_bibtex()
                 self.launch_latexml()
-        if self.mode in ("html", "all"):
+        if self.mode in ("html", "all", "docx"):
             if self.do_latexml:
                 # This only works if you have installed latexml
                 self.launch_latexml_post()
                 self.rename_and_clean_html()
                 self.clean_ccs()
             if self.post_scripts is not None and self.do_postscripts:
                 self.launch_scripts(self.post_scripts)
+            if self.mode == "docx":
+                self.launch_html_to_docx()
 
     def clean_ccs(self):
 
         pattern = f"{self.ccn_html_dir.as_posix()}/*.css"
         css_files = glob.glob(pattern)
         if len(css_files) == 0:
             _logger.debug("No css files found.")
@@ -497,24 +582,32 @@
             if self.test:
                 cmd.append("echo")
             cmd.append(self.make_exe)
             if self.mode == "clean":
                 cmd.append("clean")
             print(f"{fc}{bc}cd {makefile_dir}{rs}", end="; ")
             with path.Path(makefile_dir) as pp:
-                make_result = run_command(command=cmd, terminal_colors=self.terminal_colors)
-                if not check_make_was_clean(make_result=make_result) and self.mode != "clean":
+                make_result = run_command(
+                    command=cmd, terminal_colors=self.terminal_colors
+                )
+                if (
+                    not check_make_was_clean(make_result=make_result)
+                    and self.mode != "clean"
+                ):
                     for sync_dir in self.synchronise_directories:
                         sync_dir_base = Path(sync_dir.stem)
                         # als we de make file inderdaad gedraaid hebben en we hebben een sync
                         # directory, sync deze dan met de ccn output directory
                         if sync_dir_base.exists():
-                            sync_cmd = self.make_sync_command(parent_path=pp,
-                                                              synchronize_directory=sync_dir_base)
-                            run_command(command=sync_cmd, terminal_colors=self.terminal_colors)
+                            sync_cmd = self.make_sync_command(
+                                parent_path=pp, synchronize_directory=sync_dir_base
+                            )
+                            run_command(
+                                command=sync_cmd, terminal_colors=self.terminal_colors
+                            )
 
     def make_sync_command(self, parent_path, synchronize_directory):
         """
         Maak een commando om een highcharts directory te synchroniseren met de ccn output
 
         Args:
             parent_path: Path
@@ -547,19 +640,23 @@
         sync_cmd.append(synchronize_directory.as_posix() + "/")
         sync_cmd.append((n_up_dir / ccn_sync_dir).as_posix())
 
         # Either Robocopy switches or rsync switches to exclude json
         if self.platform_is_windows:
             sync_cmd.append("/E")
             sync_cmd.append("/NDL")
-            sync_cmd.append("/XF")
-        else:
-            sync_cmd.append("--exclude")
 
-        sync_cmd.append("*.json")
+        if not self.include_json:
+            # robocopy switches of rsync switches om json te excluden
+            if self.platform_is_windows:
+                sync_cmd.append("/XF")
+            else:
+                sync_cmd.append("--exclude")
+
+            sync_cmd.append("*.json")
 
         return sync_cmd
 
     def launch_latexmk_for_html(self):
         """
         Run latexmk voor de tex file in de html output directory
         """
@@ -575,21 +672,48 @@
         cmd.append(f"{main_file}")
         cmd.append("-xelatex")
         cmd.append("-shell-escape")
         cmd.append(f"-output-directory={out_dir}")
 
         # lees de inhoud van main en pas de opties aan om grafieken en tabellen weg te laten
         if update_target_compared_to_source(self.main_file_name, main_file):
-            copy_main_for_latexml(tex_input_file=self.main_file_name, tex_output_file=main_file,
-                                  include_graphics=self.include_graphs)
-        else:
-            _logger.debug(f"No update need for {self.main_file_name} compared to {main_file}")
+            copy_main_for_latexml(
+                tex_input_file=self.main_file_name,
+                tex_output_file=main_file,
+                include_graphics=self.include_graphs,
+                include_hyperref=self.include_hyperref,
+            )
+        else:
+            _logger.debug(
+                f"No update need for {self.main_file_name} compared to {main_file}"
+            )
 
         run_command(command=cmd, terminal_colors=self.terminal_colors)
 
+    def launch_html_to_docx(self):
+
+        html_files = glob.glob(f"{self.ccn_html_dir.as_posix()}/*.html")
+        self.ccn_docx_dir.mkdir(exist_ok=True, parents=True)
+
+        for html_file_str in html_files:
+            html_file = Path(html_file_str)
+            cmd = []
+            if self.test:
+                cmd.append("echo")
+            docx_file = self.ccn_docx_dir / Path(html_file.stem + ".docx")
+
+            if update_target_compared_to_source(self.main_file_name, docx_file):
+                cmd.append("pandoc")
+                cmd.append(html_file.as_posix())
+                cmd.append("-o")
+                cmd.append(docx_file.as_posix())
+                run_command(command=cmd, terminal_colors=self.terminal_colors)
+            else:
+                _logger.info(f"docx file {docx_file} already up to date ")
+
     def copy_pdf(self):
         """
         Kopieer de volledige pdf voor ccn (dus met de plaatjes)
         """
         out_dir = Path(self.output_directory)
         main_file = out_dir / Path(self.main_file_name)
 
@@ -624,15 +748,17 @@
             cmd.append(f"--dest={self.xml_refs.as_posix()}")
             cmd.append(f"--preload=hyperref.sty")
             cmd.append(f"{references}")
 
             run_command(command=cmd, terminal_colors=self.terminal_colors)
             self.updated_references = True
         else:
-            _logger.debug(f"No update need for {self.xml_refs} compared to {references}")
+            _logger.debug(
+                f"No update need for {self.xml_refs} compared to {references}"
+            )
             self.updated_references = False
 
     def launch_latexml(self):
         cmd = []
 
         if self.test:
             cmd.append("echo")
@@ -644,16 +770,19 @@
         out_dir = Path(self.output_directory_html)
         main_file = out_dir / Path(self.main_file_name)
         xml_file = main_file.with_suffix(".xml")
 
         cmd.append(f"--dest={xml_file.as_posix()}")
         cmd.append(f"{main_file.as_posix()}")
 
-        if update_target_compared_to_source(main_file, xml_file) or self.updated_references or \
-                self.force_html:
+        if (
+            update_target_compared_to_source(main_file, xml_file)
+            or self.updated_references
+            or self.force_html
+        ):
             run_command(command=cmd, terminal_colors=self.terminal_colors)
         else:
             _logger.info(f"No update need for {xml_file} compared to {main_file}")
 
     def launch_latexml_post(self):
         cmd = []
 
@@ -690,15 +819,15 @@
         main_base = self.main_file_name.stem
         if self.test:
             cmd.append("echo")
 
         cmd.append("latexmk")
         cmd.append(f"-output-directory={self.output_directory.as_posix()}")
 
-        if self.mode in ("latex", "all"):
+        if self.mode in ("latex", "all", "docx"):
             cmd.append(f"{main_base}.tex")
             cmd.append("-xelatex")
             cmd.append("-shell-escape")
 
         elif self.mode == "clean":
             cmd.append("-c")
         else:
@@ -716,26 +845,28 @@
         fc = ""
         bc = ""
         rs = ""
     all_output_lines = list()
     if command[0] != "echo":
         print(f"{fc}{bc}" + " ".join(command) + f"{rs}")
     try:
-        process = subprocess.Popen(command,
-                                   stdout=subprocess.PIPE,
-                                   stderr=subprocess.STDOUT,
-                                   env=os.environ,
-                                   shell=shell)
+        process = subprocess.Popen(
+            command,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+            env=os.environ,
+            shell=shell,
+        )
 
     except FileNotFoundError as err:
         _logger.warning(f"Failed for '{command}' with error:\n{err}")
     else:
-        for line in iter(process.stdout.readline, b''):
+        for line in iter(process.stdout.readline, b""):
             try:
-                clean_line = line.decode('utf-8').strip()
+                clean_line = line.decode("utf-8").strip()
             except UnicodeDecodeError as err:
                 _logger.warning(err)
                 _logger.warning(line)
             else:
                 print(clean_line)
                 all_output_lines.append(clean_line)
 
@@ -770,15 +901,17 @@
         self.makefile_directories = settings.get("makefiles")
         self.post_scripts = settings.get("postscripts")
         self.pre_scripts = settings.get("prescripts")
         out_def = Path(self.main_name).with_suffix(".pdf")
         self.output_filename = general_settings.get("output_filename", out_def)
         if cache_settings is not None:
             self.output_directory = cache_settings.get("output_directory", "out")
-            self.output_directory_html = cache_settings.get("output_directory_html", "out_html")
+            self.output_directory_html = cache_settings.get(
+                "output_directory_html", "out_html"
+            )
         else:
             self.output_directory = "out"
             self.output_directory_html = "out_html"
 
     def report_settings(self):
         message = "{:40s} : {}"
         _logger.debug(message.format("main_file_name", self.main_name))
@@ -810,38 +943,41 @@
     else:
         platform_is_windows = False
 
     if not args.do_scripts:
         args.do_prescripts = False
         args.do_postscripts = False
 
-    suite = LaTeXMLSuite(mode=args.mode,
-                         test=args.test,
-                         make_exe=args.make_exe,
-                         do_make=args.do_make,
-                         do_postscripts=args.do_postscripts,
-                         do_prescripts=args.do_prescripts,
-                         do_latexml=args.do_latexml,
-                         overwrite=args.overwrite,
-                         main_file_name=settings.main_name,
-                         bibtex_file=settings.bibtex_file,
-                         output_directory=settings.output_directory,
-                         output_directory_html=settings.output_directory_html,
-                         output_filename=settings.output_filename,
-                         ccn_output_directory=settings.ccn_output_directory,
-                         makefile_directories=settings.makefile_directories,
-                         pre_scripts=settings.pre_scripts,
-                         post_scripts=settings.post_scripts,
-                         include_graphs=args.include_graphs,
-                         platform_is_windows=platform_is_windows,
-                         foreground_color=args.foreground_color,
-                         background_color=args.background_color,
-                         use_terminal_colors=args.use_terminal_colors,
-                         force_html=args.force_html
-                         )
+    suite = LaTeXMLSuite(
+        mode=args.mode,
+        test=args.test,
+        make_exe=args.make_exe,
+        do_make=args.do_make,
+        do_postscripts=args.do_postscripts,
+        do_prescripts=args.do_prescripts,
+        do_latexml=args.do_latexml,
+        overwrite=args.overwrite,
+        main_file_name=settings.main_name,
+        bibtex_file=settings.bibtex_file,
+        output_directory=settings.output_directory,
+        output_directory_html=settings.output_directory_html,
+        output_filename=settings.output_filename,
+        ccn_output_directory=settings.ccn_output_directory,
+        makefile_directories=settings.makefile_directories,
+        pre_scripts=settings.pre_scripts,
+        post_scripts=settings.post_scripts,
+        include_graphs=args.include_graphs,
+        include_hyperref=args.include_hyperref,
+        platform_is_windows=platform_is_windows,
+        foreground_color=args.foreground_color,
+        background_color=args.background_color,
+        use_terminal_colors=args.use_terminal_colors,
+        force_html=args.force_html,
+        include_json=args.include_json,
+    )
 
     suite.run()
 
     _logger.info("Script ends here")
 
 
 def run():
```

### Comparing `latexmlsuite-0.4.0/src/latexmlsuite.egg-info/PKG-INFO` & `latexmlsuite-0.4.1/src/latexmlsuite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latexmlsuite
-Version: 0.4.0
+Version: 0.4.1
 Summary: A tool to create a latex publication using latexml
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `latexmlsuite-0.4.0/src/latexmlsuite.egg-info/SOURCES.txt` & `latexmlsuite-0.4.1/src/latexmlsuite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `latexmlsuite-0.4.0/tox.ini` & `latexmlsuite-0.4.1/tox.ini`

 * *Files identical despite different names*

