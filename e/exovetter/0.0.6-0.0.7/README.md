# Comparing `tmp/exovetter-0.0.6.tar.gz` & `tmp/exovetter-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exovetter-0.0.6.tar", last modified: Wed Mar  6 15:20:56 2024, max compression
+gzip compressed data, was "exovetter-0.0.7.tar", last modified: Mon May  6 22:56:01 2024, max compression
```

## Comparing `exovetter-0.0.6.tar` & `exovetter-0.0.7.tar`

### file list

```diff
@@ -1,83 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:20:56.287412 exovetter-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-06 15:20:41.000000 exovetter-0.0.6/.bandit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:20:56.263413 exovetter-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:20:56.267413 exovetter-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-06 15:20:41.000000 exovetter-0.0.6/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-06 15:20:41.000000 exovetter-0.0.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-06 15:20:41.000000 exovetter-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-06 15:20:41.000000 exovetter-0.0.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-06 15:20:41.000000 exovetter-0.0.6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-06 15:20:41.000000 exovetter-0.0.6/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-06 15:20:41.000000 exovetter-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-03-06 15:20:56.287412 exovetter-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-03-06 15:20:41.000000 exovetter-0.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:20:56.271412 exovetter-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-03-06 15:20:41.000000 exovetter-0.0.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-03-06 15:20:41.000000 exovetter-0.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-06 15:20:41.000000 exovetter-0.0.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-06 15:20:41.000000 exovetter-0.0.6/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-03-06 15:20:41.000000 exovetter-0.0.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-06 15:20:41.000000 exovetter-0.0.6/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-06 15:20:41.000000 exovetter-0.0.6/docs/vetters.rst
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-06 15:20:41.000000 exovetter-0.0.6/docs/vetters_low_level.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:20:56.271412 exovetter-0.0.6/exovetter/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:20:56.275412 exovetter-0.0.6/exovetter/centroid/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/centroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/centroid/centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/centroid/covar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/centroid/disp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/centroid/fastpsffit.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/leo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/lightkurve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/lpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:20:56.275412 exovetter-0.0.6/exovetter/modshift/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/modshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/modshift/modshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/modshift/plotmodshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/odd_even.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/sweet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/tce.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/transit_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)    31097 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/trapezoid_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    18430 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-06 15:20:56.000000 exovetter-0.0.6/exovetter/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    35132 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/vetters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-03-06 15:20:41.000000 exovetter-0.0.6/exovetter/viz_transits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:20:56.283412 exovetter-0.0.6/exovetter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-03-06 15:20:56.000000 exovetter-0.0.6/exovetter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-06 15:20:56.000000 exovetter-0.0.6/exovetter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 15:20:56.000000 exovetter-0.0.6/exovetter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 15:20:56.000000 exovetter-0.0.6/exovetter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-06 15:20:56.000000 exovetter-0.0.6/exovetter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-06 15:20:56.000000 exovetter-0.0.6/exovetter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:20:56.275412 exovetter-0.0.6/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-06 15:20:41.000000 exovetter-0.0.6/licenses/DAVE_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-06 15:20:41.000000 exovetter-0.0.6/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-06 15:20:41.000000 exovetter-0.0.6/licenses/TEMPLATE_LICENCE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-06 15:20:41.000000 exovetter-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-06 15:20:41.000000 exovetter-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-06 15:20:56.287412 exovetter-0.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1958 2024-03-06 15:20:41.000000 exovetter-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:20:56.283412 exovetter-0.0.6/tutorial_notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)   278575 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/Centroid.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   160061 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/LPP.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    70192 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/LeoTransitEvents.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   219164 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/OddEven.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   251796 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/SWEET.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/TCEs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   131489 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/TransitPhaseCoverage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   224308 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/VizTransits.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   241212 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/lightcurves.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   235866 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/modshift.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    66058 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/run_all.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:20:56.283412 exovetter-0.0.6/tutorial_notebooks/run_all_plots/
--rw-r--r--   0 runner    (1001) docker     (127)   178587 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/run_all_plots/TOI_1000.01.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   178796 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/run_all_plots/TOI_1001.01.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   273972 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/run_all_plots/TOI_1004.01.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   172989 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/run_all_plots/TOI_1007.01.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   179649 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/run_all_plots/TOI_1011.01.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   740160 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/wasp18b.fits
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-06 15:20:41.000000 exovetter-0.0.6/tutorial_notebooks/wasp18b_tce
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.105566 exovetter-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 22:55:52.000000 exovetter-0.0.7/.bandit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.085566 exovetter-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.089566 exovetter-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-06 22:55:52.000000 exovetter-0.0.7/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-06 22:55:52.000000 exovetter-0.0.7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-06 22:55:52.000000 exovetter-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-06 22:55:52.000000 exovetter-0.0.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-06 22:55:52.000000 exovetter-0.0.7/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-06 22:55:52.000000 exovetter-0.0.7/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 22:55:52.000000 exovetter-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-06 22:56:01.105566 exovetter-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-06 22:55:52.000000 exovetter-0.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.089566 exovetter-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/vetters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/vetters_low_level.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.093566 exovetter-0.0.7/exovetter/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.097566 exovetter-0.0.7/exovetter/centroid/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/centroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/centroid/centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/centroid/covar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/centroid/disp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/centroid/fastpsffit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/leo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/lightkurve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/lpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.097566 exovetter-0.0.7/exovetter/modshift/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/modshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/modshift/modshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/modshift/plotmodshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/odd_even.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/sweet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/tce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/transit_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31097 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/trapezoid_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24909 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-06 22:56:00.000000 exovetter-0.0.7/exovetter/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37423 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/vetters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/viz_transits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.105566 exovetter-0.0.7/exovetter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-06 22:56:01.000000 exovetter-0.0.7/exovetter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-06 22:56:01.000000 exovetter-0.0.7/exovetter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 22:56:01.000000 exovetter-0.0.7/exovetter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 22:56:01.000000 exovetter-0.0.7/exovetter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-06 22:56:01.000000 exovetter-0.0.7/exovetter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 22:56:01.000000 exovetter-0.0.7/exovetter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.097566 exovetter-0.0.7/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-06 22:55:52.000000 exovetter-0.0.7/licenses/DAVE_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-06 22:55:52.000000 exovetter-0.0.7/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-06 22:55:52.000000 exovetter-0.0.7/licenses/TEMPLATE_LICENCE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-06 22:55:52.000000 exovetter-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-06 22:55:52.000000 exovetter-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-06 22:56:01.105566 exovetter-0.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1958 2024-05-06 22:55:52.000000 exovetter-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.105566 exovetter-0.0.7/tutorial_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)  1714508 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/100100827.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   278575 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/Centroid.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   160061 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/LPP.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    70192 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/LeoTransitEvents.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   219164 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/OddEven.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   251796 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/SWEET.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/TCEs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   131489 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/TransitPhaseCoverage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   224308 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/VizTransits.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   241212 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/lightcurves.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   235866 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/modshift.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    86880 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/run_all.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   740160 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/wasp18b.fits
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/wasp18b_tce
```

### Comparing `exovetter-0.0.6/.github/workflows/ci_workflows.yml` & `exovetter-0.0.7/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/.github/workflows/publish.yml` & `exovetter-0.0.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/.gitignore` & `exovetter-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/.readthedocs.yml` & `exovetter-0.0.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/LICENSE.rst` & `exovetter-0.0.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/PKG-INFO` & `exovetter-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exovetter
-Version: 0.0.6
+Version: 0.0.7
 Summary: Exoplanet vetting package
 Home-page: https://github.com/spacetelescope/exovetter
 Author: Susan Mullally et al.
 Author-email: smullally@stsci.edu
 License: BSD 3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `exovetter-0.0.6/README.rst` & `exovetter-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/docs/Makefile` & `exovetter-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/docs/conf.py` & `exovetter-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/docs/install.rst` & `exovetter-0.0.7/docs/install.rst`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/docs/make.bat` & `exovetter-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/docs/vetters_low_level.rst` & `exovetter-0.0.7/docs/vetters_low_level.rst`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/centroid/centroid.py` & `exovetter-0.0.7/exovetter/centroid/centroid.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/centroid/covar.py` & `exovetter-0.0.7/exovetter/centroid/covar.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/centroid/disp.py` & `exovetter-0.0.7/exovetter/centroid/disp.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/centroid/fastpsffit.py` & `exovetter-0.0.7/exovetter/centroid/fastpsffit.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/const.py` & `exovetter-0.0.7/exovetter/const.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/leo.py` & `exovetter-0.0.7/exovetter/leo.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/lightkurve_utils.py` & `exovetter-0.0.7/exovetter/lightkurve_utils.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/lpp.py` & `exovetter-0.0.7/exovetter/lpp.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/model.py` & `exovetter-0.0.7/exovetter/model.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/modshift/modshift.py` & `exovetter-0.0.7/exovetter/modshift/modshift.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/modshift/plotmodshift.py` & `exovetter-0.0.7/exovetter/modshift/plotmodshift.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/odd_even.py` & `exovetter-0.0.7/exovetter/odd_even.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/sweet.py` & `exovetter-0.0.7/exovetter/sweet.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/tce.py` & `exovetter-0.0.7/exovetter/tce.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/transit_coverage.py` & `exovetter-0.0.7/exovetter/transit_coverage.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/trapezoid_fit.py` & `exovetter-0.0.7/exovetter/trapezoid_fit.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter/utils.py` & `exovetter-0.0.7/exovetter/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 """Utility functions."""
 
 import sys
 import warnings
-
+from exovetter import lightkurve_utils
+from exovetter import utils
+from exovetter import const as exo_const
+import astropy.units as u
+from exovetter import vetters as vet
+from matplotlib.backends.backend_pdf import PdfPages
+import matplotlib.pyplot as plt
 import numpy as np
+import os
 
 __all__ = ['sine', 'estimate_scatter', 'mark_transit_cadences', 'median_detrend', 
            'plateau', 'set_median_flux_to_zero', 'set_median_flux_to_one', 'sigmaClip', 
-           'get_mast_tce', 'WqedLSF', 'compute_phases', 'first_epoch']
+           'get_mast_tce', 'WqedLSF', 'compute_phases', 'first_epoch', 'run_all']
 
 def sine(x, order, period=1):
     """Sine function for SWEET vetter."""
     w = 2 * np.pi / period
     if order == 0:
         return np.sin(w * x)
     elif order == 1:
@@ -649,7 +656,168 @@
         N = np.floor((epoch.value-lc.time.value[0])/period.value)
         first_epoch = epoch - N*period
     else:
         N = np.ceil((lc.time.value[0]-epoch.value)/period.value)
         first_epoch = epoch + N*period
 
     return first_epoch
+
+def run_all(tce, lc, tpf=None, vetters=None, remove_metrics=None, plot=False, plot_dir=None):
+    """Run a set of vetters on a tce and lc, returning a dictionary of all metrics collected
+    
+    Parameters
+    ----------
+    tce : tce object
+        tce object is a dictionary that contains information about the tce
+        to vet, like period, epoch, duration, depth
+
+    lc : lightkurve object
+        lightkurve object with the time and flux to use for vetting.
+
+    tpf : obj
+        ``lightkurve`` target pixel file object with pixels in column lc_name
+
+    vetters : list
+        list of vetter objects to run on, ie [vet.ModShift(), vet.OddEven(dur_frac=0.75)]
+        Defaults to all vetters
+    
+    remove_metrics : list
+        metrics to not store, defaults to removing plotting values
+
+    plot : bool
+        Option to return a pdf of the vetting diagnostic plots, defaults to False
+
+    plot_dir : str
+        Path to store diagnostic pdfs in, defaults to current working directory
+
+    Returns
+    -------
+    results_dict : dictionary
+        Dictionary of the kept vetting metrics
+    """
+    
+    # Set initial parameters
+    if not vetters:
+        vetters = [vet.VizTransits(), vet.ModShift(), vet.Lpp(), vet.OddEven(), vet.TransitPhaseCoverage(), vet.Sweet(), vet.LeoTransitEvents(), vet.Centroid()]
+
+    if not remove_metrics:
+        remove_metrics = ['plot_data']
+
+    if not plot_dir:
+        plot_dir = os.getcwd()+'/'
+
+    if not tpf:
+        if any(vetter.__class__.__name__ == 'Centroid' for vetter in vetters):
+            raise Exception("TPF file required while running centroid")
+
+    # Run all listed vetters
+    results_list = []
+
+    if not plot:
+        for vetter in vetters:
+            if vetter.__class__.__name__ != 'Centroid':
+                vetter_results = vetter.run(tce, lc, plot=False) # dictionary returned from each vetter
+                results_list.append(vetter_results)
+            else:
+                vetter_results = vetter.run(tce, tpf, plot=False) # centroid uses tpf rather than lc
+                results_list.append(vetter_results)
+
+    else:
+        plot_name = lc.LABEL
+
+        diagnostic_plot = PdfPages(plot_dir+plot_name+'.pdf') # initialize a pdf to save each figure into
+        plot_figures = []
+        
+        # Manually run viz transits with an extra mark cadences plot
+        cadences_plot = mark_cadences_plot(lc, tce)
+        diagnostic_plot.savefig(cadences_plot)
+
+        for vetter in vetters:
+            if vetter.__class__.__name__ not in ['VizTransits', 'Centroid', 'LeoTransitEvents']: # viz_transits and Centroid generate more than one figures so handle later
+                vetter_results = vetter.run(tce, lc, plot=True) # dictionary returned from each vetter
+                plot_figures.append(plt.gcf())
+                plt.close() # Make them not show up if running in a notebook
+                results_list.append(vetter_results)
+
+            if vetter.__class__.__name__ == 'Centroid': # centroid produces 2 plots, the second of which is the most useful so just collect that one
+                vetter_results = vet.Centroid(lc_name=vetter.lc_name, diff_plots=False, centroid_plots=True).run(tce, tpf)
+                plot_figures.append(plt.gcf())
+                plt.close()
+                results_list.append(vetter_results)
+                
+        # run viz_transits plots
+        transit = vet.VizTransits(transit_plot=True, folded_plot=False).run(tce, lc)
+        transit_plot = plt.gcf()
+        transit_plot.suptitle(plot_name+' Transits')
+        transit_plot.tight_layout()
+        plt.close()
+        diagnostic_plot.savefig(transit_plot)
+
+        folded = vet.VizTransits(transit_plot=False, folded_plot=True).run(tce, lc)
+        folded_plot = plt.gcf()
+        folded_plot.suptitle(plot_name+' Folded Transits')
+        folded_plot.tight_layout()
+        plt.close()
+        diagnostic_plot.savefig(folded_plot)
+        
+        # Save each diagnostic plot stored in plot_figures to diagnostic_plot pdf file
+        for plot in plot_figures:
+            diagnostic_plot.savefig(plot)
+
+        diagnostic_plot.close()
+    
+    # Convert to a single dictionary output
+    results_dict = {k: v for d in results_list for k, v in d.items()} # Combine all dictionaries returned from vetters
+
+    # delete specified metrics
+    for key in remove_metrics:
+        if results_dict.get(key):
+            del results_dict[key]
+    
+    return results_dict
+
+
+def mark_cadences_plot(lc, tce):
+    """return figure object of the lightcurve with epochs oeverplotted"""
+    
+    fig, ax1 = plt.subplots(nrows=1, ncols=1, figsize=(9,5))
+
+    # Get lightcurve data
+    time, flux, time_offset_str = lightkurve_utils.unpack_lk_version(lc, "flux")  # noqa: E50
+    time_offset_q = getattr(exo_const, time_offset_str)
+    epoch = tce.get_epoch(time_offset_q).to_value(u.day)
+    
+    # Get points of lightcurve found to be in transit
+    period = tce["period"].to_value(u.day)
+    dur = tce["duration"].to_value(u.day)
+    intransit = mark_transit_cadences(time, period, epoch, dur)
+
+    # Plot epoch
+    ax1.axvline(x=epoch, lw='0.6', color='r', label='epoch', alpha=0.5)
+
+    # Plot transit train
+    ax1.plot(time, flux, lw=0.72, alpha=0.9)
+    ax1.scatter(time, flux, color='k', s=3, label='cadences', alpha=0.5)
+    
+    # TODO This only plots forward in time from the epoch, works fine assuming tce epoch is first in light curve but not robust
+    transit_epochs = epoch-dur/2
+    while transit_epochs <= time[-1]:
+        ax1.axvline(x=transit_epochs, lw='0.6', color='r', alpha=0.3, ls='--')
+        transit_epochs = transit_epochs+dur
+        ax1.axvline(x=transit_epochs, lw='0.6', color='r', alpha=0.3, ls='--')
+        transit_epochs = transit_epochs-dur + period
+        
+    # Plot cadences in transit
+    ax1.scatter(time[intransit], flux[intransit], color='r', s=4, label='cadences in transit');
+
+    # Plotting params
+    ax1.set_ylabel('Flux')
+    ax1.set_xlabel('Time '+time_offset_str)
+    ax1.set_title(lc.label+' period='+'{0:.2f}'.format(period)+'d, dur='+'{0:.2f}'.format(dur)+'d')
+    ax1.legend();
+
+    cadences_plot = plt.gcf()
+    plt.close()
+
+    return cadences_plot
+
+
```

### Comparing `exovetter-0.0.6/exovetter/vetters.py` & `exovetter-0.0.7/exovetter/vetters.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import pprint
 from abc import ABC, abstractmethod
 
 import astropy.units as u
 import numpy as np
 import pandas as pd
-import time as py_time
+# import time as py_time
 import os
-import matplotlib.pyplot as plt
-from matplotlib.backends.backend_pdf import PdfPages
+# import matplotlib.pyplot as plt
+# from matplotlib.backends.backend_pdf import PdfPages
 
 from exovetter.centroid import centroid as cent
 from exovetter import transit_coverage
 from exovetter import modshift
 from exovetter import odd_even
 from exovetter import sweet
 from exovetter import lpp
@@ -22,15 +22,15 @@
 from exovetter import utils
 from exovetter import model
 from exovetter import viz_transits
 from exovetter import leo
 
 __all__ = ['BaseVetter', 'ModShift', 'Lpp', 'OddEven', 
            'TransitPhaseCoverage', 'Sweet', 'Centroid',
-           'VizTransits', 'LeoTransitEvents', 'run_all']
+           'VizTransits', 'LeoTransitEvents']
 
 class BaseVetter(ABC):
     """Base class for vetters.
 
     Each vetting test should be a subclass of this class.
 
     Parameters
@@ -581,21 +581,27 @@
     def plot(self):  # pragma: no cover
         self.run(self.tce, self.lc, plot=True)
 
 
 class Centroid(BaseVetter):
     """Class to handle centroid vetting"""
 
-    def __init__(self, lc_name="flux"):
+    def __init__(self, lc_name="flux", diff_plots=False, centroid_plots=False):
         """
         Parameters
         ----------
         lc_name : str
             Name of the flux array in the ``lightkurve`` object.
 
+        diff_plots : bool
+            Show centroid difference plots
+
+        centroid_plots : bool
+            Show centroid summary plot
+
         Attributes
         ----------
         tce : tce object
             tce object is a dictionary that contains information about the tce
             to vet, like period, epoch, duration, depth.
 
         tpf : obj
@@ -604,14 +610,16 @@
         metrics : dict
             Centroid result dictionary populated by :meth:`run`."""
 
         self.lc_name = lc_name
         self.tce = None
         self.tpf = None
         self.metrics = None
+        self.diff_plots = diff_plots
+        self.centroid_plots = centroid_plots
 
     def run(self, tce, lk_tpf, plot=False, remove_transits=None):
         """Runs cent.compute_diff_image_centroids and cent.measure_centroid_shift
         to populate the vetter object.
 
         Parameters
         ----------
@@ -638,31 +646,35 @@
                 Values close to 1 mean the transit is likely on the target star.
                 Values less than ~1e-3 suggest the target is not the source of the transit.
         """
 
         self.tce = tce
         self.tpf = lk_tpf
 
+        if plot:
+            self.diff_plots = True
+            self.centroid_plots = True
+
         time, cube, time_offset_str = lightkurve_utils.unpack_tpf(
             self.tpf, self.lc_name
         )  # noqa: E50
 
         period_days = tce["period"].to_value(u.day)
         time_offset_q = getattr(exo_const, time_offset_str)
         epoch = tce.get_epoch(time_offset_q).to_value(u.day)
         duration_days = tce["duration"].to_value(u.day)
 
         if remove_transits is None: # reformat to be a blank list
             remove_transits = []
         
         centroids, figs, kept_transits = cent.compute_diff_image_centroids(
             time, cube, period_days, epoch, duration_days, 
-            remove_transits, plot=plot)
+            remove_transits, plot=self.diff_plots)
         
-        offset, signif, fig = cent.measure_centroid_shift(centroids, kept_transits, plot)
+        offset, signif, fig = cent.measure_centroid_shift(centroids, kept_transits, self.centroid_plots)
         figs.append(fig)
 
         # TODO: If plot=True, figs is a list of figure handles.
         # Do I save those figures, put them in a single pdf,
         # close them all?
 
         self.metrics = dict(offset=offset, significance=signif)
@@ -897,147 +909,199 @@
 
         if plot:
             pass
 
     def plot(self):
         pass
 
-def run_all(tces, lcs, vetters=[VizTransits(), ModShift(), Lpp(), OddEven(), TransitPhaseCoverage(), Sweet(), LeoTransitEvents()], plot=False, verbose=False, plot_dir=None):
-    # TODO Add centroid, maybe rething plotting in general since plotting uses vetter.plot which essentially doubles runtime, 
-    # probably should run initially with vet.run(plot=True) and not store them unless run_all plot=True
-    """Runs vetters and packs results into a dataframe.
+def run_all(tce, lc, vetters=[VizTransits(), ModShift(), Lpp(), OddEven(), TransitPhaseCoverage(), Sweet(), LeoTransitEvents()], remove_metrics = ['plot_data'], plot=False, plot_dir='', plot_name=None ,verbose=False):
+    """Runs vetters on a tce and lc and packs results into a dictionary.
 
     Parameters
     ----------
-    tces: list of tce objects to vet on
+    tces: tce object to vet on
 
-    lc: list of lightkurve objects to vet on
+    lc: lightkurve object to vet on
     
     vetters : list
         List of vetter classes to run
 
     plot : bool
         Toggle diagnostic plots
     
-    plot_dir : str
-        path to store plots in, defaults to current working directory
-    
     verbose : bool
         Toggle timing info and other print statements
 
     Returns
     ------------
-    results : dataframe
-        Pandas dataframe of all the numerical results from the vetters
+    results : dictionary
+        Dictionary of all the numerical results from the vetters
           
     """
 
-    results_dicts = [] # initialize a list to pack results from each tce into
-    tce_names = []
-    run_start = py_time.time()
+    results = run_vetters.run_all(tce, lc, vetters, remove_metrics, plot, plot_dir, plot_name, verbose)
+
+    return results
+
+    # results_list = []
+
+    # if plot == False:
+    #     for vetter in vetters:
+    #         vetter_results = vetter.run(tce, lc, plot=False) # dictionary returned from each vetter
+    #         results_list.append(vetter_results)
+
+    # else:
+    #     
+    #     if plot_name is None:
+    #         plot_name = tce['target'] 
+    #     diagnostic_plot = PdfPages(plot_dir+plot_name+'.pdf') # initialize a pdf to save each figure into
+    #     plot_figures = []
+
+    #     for vetter in vetters:
+    #         vetter_results = vetter.run(tce, lc, plot=True)
+    #         plot_figures.append(plt.gcf())
+    #         plt.close()
+    #         results_list.append(vetter_results)
+
+    #     # Save each diagnostic plot ran on that tce/lc
+    #     for plot in plot_figures:
+    #         diagnostic_plot.savefig(plot)
+
+    #     diagnostic_plot.close()
+
+    # results_dict = {k: v for d in results_list for k, v in d.items()}
+
+    # # delete dictionary entries that are huge arrays to save space
+    # for key in remove_metrics:
+    #     if results_dict.get(key):
+    #         del results_dict[key]
+
+    # return results_dict
+        
+    # OLDER CODE
+        # if plot:
+        #     if vetter.__class__.__name__ != 'VizTransits' and vetter.__class__.__name__ != 'LeoTransitEvents': 
+        #         # viz_transits generates 2 figures so it's handled later, LeoTransitEvents just doesn't have a plot
+        #         vetter.plot()
+        #         vetter_plot = plt.gcf()
+        #         vetter_plot.suptitle(tce['target']+' '+vetter.__class__.__name__)
+        #         vetter_plot.tight_layout()
+        #         plt.close()
+        #         plot_figures.append(vetter_plot)
+
+        # if verbose:
+        #     time_end = py_time.time()
+        #     print(vetter.__class__.__name__, 'finished in', time_end - time_start, 's.')
+        
+        # results_list.append(vetter_results)
+    
+
+    # results_dicts = [] # initialize a list to pack results from each tce into
+    # tce_names = []
+    # run_start = py_time.time()
 
-    if plot_dir is None:
-        plot_dir = os.getcwd()
+    # if plot_dir is None:
+    #     plot_dir = os.getcwd()
     
-    if plot or verbose: 
-        for tce in tces:
-            if 'target' not in tce.keys():
-                print("ERROR: Please supply a 'target' key to all input tces to use the plot or verbose parameters")
-                return
-
-    for tce, lc in zip(tces, lcs):
-        if verbose:
-            print('Vetting', tce['target'], ':')
+    # if plot or verbose: 
+    #     for tce in tces:
+    #         if 'target' not in tce.keys():
+    #             print("ERROR: Please supply a 'target' key to all input tces to use the plot or verbose parameters")
+    #             return
+
+    # for tce, lc in zip(tces, lcs):
+    #     if verbose:
+    #         print('Vetting', tce['target'], ':')
 
-        tce_names.append(tce['target'])
-        results_list = [] # initialize a list to pack result dictionaries into
+    #     tce_names.append(tce['target'])
+    #     results_list = [] # initialize a list to pack result dictionaries into
         
-        # run each vetter, if plotting is true fill the figures into a list to save later
-        plot_figures = []
-        for vetter in vetters:
-            time_start = py_time.time()
-            vetter_results = vetter.run(tce, lc)
+    #     # run each vetter, if plotting is true fill the figures into a list to save later
+    #     plot_figures = []
+    #     for vetter in vetters:
+    #         time_start = py_time.time()
+    #         vetter_results = vetter.run(tce, lc)
             
-            if plot:
-                if vetter.__class__.__name__ != 'VizTransits' and vetter.__class__.__name__ != 'LeoTransitEvents': 
-                    # viz_transits generates 2 figures so it's handled later, LeoTransitEvents just doesn't have a plot
-                    vetter.plot()
-                    vetter_plot = plt.gcf()
-                    vetter_plot.suptitle(tce['target']+' '+vetter.__class__.__name__)
-                    vetter_plot.tight_layout()
-                    plt.close()
-                    plot_figures.append(vetter_plot)
-
-            if verbose:
-                time_end = py_time.time()
-                print(vetter.__class__.__name__, 'finished in', time_end - time_start, 's.')
+    #         if plot:
+    #             if vetter.__class__.__name__ != 'VizTransits' and vetter.__class__.__name__ != 'LeoTransitEvents': 
+    #                 # viz_transits generates 2 figures so it's handled later, LeoTransitEvents just doesn't have a plot
+    #                 vetter.plot()
+    #                 vetter_plot = plt.gcf()
+    #                 vetter_plot.suptitle(tce['target']+' '+vetter.__class__.__name__)
+    #                 vetter_plot.tight_layout()
+    #                 plt.close()
+    #                 plot_figures.append(vetter_plot)
+
+    #         if verbose:
+    #             time_end = py_time.time()
+    #             print(vetter.__class__.__name__, 'finished in', time_end - time_start, 's.')
             
-            results_list.append(vetter_results)
+    #         results_list.append(vetter_results)
         
-        if verbose: # add some whitespace for readability
-            print()
+    #     if verbose: # add some whitespace for readability
+    #         print()
 
-        if plot: # save a pdf of each figure made for that vetter
-            diagnostic_plot = PdfPages(plot_dir+tce['target']+'.pdf') # initialize a pdf to save each figure into
+    #     if plot: # save a pdf of each figure made for that vetter
+    #         diagnostic_plot = PdfPages(plot_dir+tce['target']+'.pdf') # initialize a pdf to save each figure into
 
-            # plot the lightcurve with epochs oeverplotted
-            time, flux, time_offset_str = lightkurve_utils.unpack_lk_version(lc, "flux")  # noqa: E50
-            period = tce["period"].to_value(u.day)
-            dur = tce["duration"].to_value(u.day)
-
-            time_offset_q = getattr(exo_const, time_offset_str)
-            epoch = tce.get_epoch(time_offset_q).to_value(u.day)
-            intransit = utils.mark_transit_cadences(time, period, epoch, dur, num_durations=3, flags=None)
-
-            fig, ax1 = plt.subplots(nrows=1, ncols=1, figsize=(9,5))
-            ax1.plot(time, flux, lw=0.4);
-            ax1.axvline(x=epoch, lw='0.6', color='r', label='epoch');
-            ax1.fill_between(time, 0,1, where=intransit, transform=ax1.get_xaxis_transform(), color='r', alpha=0.15, label='in transit')
-
-            ax1.set_ylabel('Flux')
-            ax1.set_xlabel('Time '+time_offset_str)
-            if 'target' in tce:
-                ax1.set_title(tce['target']);
-
-            ax1.legend();
-            lightcurve_plot = plt.gcf()
-            plt.close()
-            diagnostic_plot.savefig(lightcurve_plot)
-
-            # run viz_transits plots
-            transit = VizTransits(transit_plot=True, folded_plot=False).run(tce, lc)
-            transit_plot = plt.gcf()
-            transit_plot.suptitle(tce['target']+' Transits')
-            transit_plot.tight_layout()
-            plt.close()
-            diagnostic_plot.savefig(transit_plot)
-
-            folded = VizTransits(transit_plot=False, folded_plot=True).run(tce, lc)
-            folded_plot = plt.gcf()
-            folded_plot.suptitle(tce['target']+' Folded Transits')
-            folded_plot.tight_layout()
-            plt.close()
-            diagnostic_plot.savefig(folded_plot)
-
-            # Save each diagnostic plot ran on that tce/lc
-            for plot in plot_figures:
-                diagnostic_plot.savefig(plot)
+    #         # plot the lightcurve with epochs oeverplotted
+    #         time, flux, time_offset_str = lightkurve_utils.unpack_lk_version(lc, "flux")  # noqa: E50
+    #         period = tce["period"].to_value(u.day)
+    #         dur = tce["duration"].to_value(u.day)
+
+    #         time_offset_q = getattr(exo_const, time_offset_str)
+    #         epoch = tce.get_epoch(time_offset_q).to_value(u.day)
+    #         intransit = utils.mark_transit_cadences(time, period, epoch, dur, num_durations=3, flags=None)
+
+    #         fig, ax1 = plt.subplots(nrows=1, ncols=1, figsize=(9,5))
+    #         ax1.plot(time, flux, lw=0.4);
+    #         ax1.axvline(x=epoch, lw='0.6', color='r', label='epoch');
+    #         ax1.fill_between(time, 0,1, where=intransit, transform=ax1.get_xaxis_transform(), color='r', alpha=0.15, label='in transit')
+
+    #         ax1.set_ylabel('Flux')
+    #         ax1.set_xlabel('Time '+time_offset_str)
+    #         if 'target' in tce:
+    #             ax1.set_title(tce['target']);
+
+    #         ax1.legend();
+    #         lightcurve_plot = plt.gcf()
+    #         plt.close()
+    #         diagnostic_plot.savefig(lightcurve_plot)
+
+    #         # run viz_transits plots
+    #         transit = VizTransits(transit_plot=True, folded_plot=False).run(tce, lc)
+    #         transit_plot = plt.gcf()
+    #         transit_plot.suptitle(tce['target']+' Transits')
+    #         transit_plot.tight_layout()
+    #         plt.close()
+    #         diagnostic_plot.savefig(transit_plot)
+
+    #         folded = VizTransits(transit_plot=False, folded_plot=True).run(tce, lc)
+    #         folded_plot = plt.gcf()
+    #         folded_plot.suptitle(tce['target']+' Folded Transits')
+    #         folded_plot.tight_layout()
+    #         plt.close()
+    #         diagnostic_plot.savefig(folded_plot)
+
+    #         # Save each diagnostic plot ran on that tce/lc
+    #         for plot in plot_figures:
+    #             diagnostic_plot.savefig(plot)
 
-            diagnostic_plot.close()
+    #         diagnostic_plot.close()
         
-        # put all values from each results dictionary into a single dictionary
-        results_dict = {k: v for d in results_list for k, v in d.items()}
+    #     # put all values from each results dictionary into a single dictionary
+    #     results_dict = {k: v for d in results_list for k, v in d.items()}
         
-        # delete dictionary entries that are huge arrays to save space
-        if results_dict.get('plot_data'):
-            del results_dict['plot_data']
+    #     # delete dictionary entries that are huge arrays to save space
+    #     if results_dict.get('plot_data'):
+    #         del results_dict['plot_data']
         
-        # add the dictionary to the final list
-        results_dicts.append(results_dict)
+    #     # add the dictionary to the final list
+    #     results_dicts.append(results_dict)
 
-    results_df = pd.DataFrame(results_dicts) # Put the values from each result dictionary into a dataframe
+    # results_df = pd.DataFrame(results_dicts) # Put the values from each result dictionary into a dataframe
     
-    results_df.insert(loc=0, column='tce', value=tce_names)
-    if verbose:
-        print('Execution time:', (py_time.time() - run_start), 's')
+    # results_df.insert(loc=0, column='tce', value=tce_names)
+    # if verbose:
+    #     print('Execution time:', (py_time.time() - run_start), 's')
 
-    return results_df
+    # return results_df
```

### Comparing `exovetter-0.0.6/exovetter/viz_transits.py` & `exovetter-0.0.7/exovetter/viz_transits.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/exovetter.egg-info/PKG-INFO` & `exovetter-0.0.7/exovetter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exovetter
-Version: 0.0.6
+Version: 0.0.7
 Summary: Exoplanet vetting package
 Home-page: https://github.com/spacetelescope/exovetter
 Author: Susan Mullally et al.
 Author-email: smullally@stsci.edu
 License: BSD 3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `exovetter-0.0.6/exovetter.egg-info/SOURCES.txt` & `exovetter-0.0.7/exovetter.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -47,25 +47,21 @@
 exovetter/centroid/fastpsffit.py
 exovetter/modshift/__init__.py
 exovetter/modshift/modshift.py
 exovetter/modshift/plotmodshift.py
 licenses/DAVE_LICENSE
 licenses/README.rst
 licenses/TEMPLATE_LICENCE.rst
+tutorial_notebooks/100100827.pdf
 tutorial_notebooks/Centroid.ipynb
 tutorial_notebooks/LPP.ipynb
 tutorial_notebooks/LeoTransitEvents.ipynb
 tutorial_notebooks/OddEven.ipynb
 tutorial_notebooks/SWEET.ipynb
 tutorial_notebooks/TCEs.ipynb
 tutorial_notebooks/TransitPhaseCoverage.ipynb
 tutorial_notebooks/VizTransits.ipynb
 tutorial_notebooks/lightcurves.ipynb
 tutorial_notebooks/modshift.ipynb
 tutorial_notebooks/run_all.ipynb
 tutorial_notebooks/wasp18b.fits
-tutorial_notebooks/wasp18b_tce
-tutorial_notebooks/run_all_plots/TOI_1000.01.pdf
-tutorial_notebooks/run_all_plots/TOI_1001.01.pdf
-tutorial_notebooks/run_all_plots/TOI_1004.01.pdf
-tutorial_notebooks/run_all_plots/TOI_1007.01.pdf
-tutorial_notebooks/run_all_plots/TOI_1011.01.pdf
+tutorial_notebooks/wasp18b_tce
```

### Comparing `exovetter-0.0.6/licenses/DAVE_LICENSE` & `exovetter-0.0.7/licenses/DAVE_LICENSE`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/licenses/TEMPLATE_LICENCE.rst` & `exovetter-0.0.7/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/setup.cfg` & `exovetter-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/setup.py` & `exovetter-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/tutorial_notebooks/Centroid.ipynb` & `exovetter-0.0.7/tutorial_notebooks/Centroid.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/tutorial_notebooks/LPP.ipynb` & `exovetter-0.0.7/tutorial_notebooks/LPP.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/tutorial_notebooks/LeoTransitEvents.ipynb` & `exovetter-0.0.7/tutorial_notebooks/LeoTransitEvents.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/tutorial_notebooks/OddEven.ipynb` & `exovetter-0.0.7/tutorial_notebooks/OddEven.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/tutorial_notebooks/SWEET.ipynb` & `exovetter-0.0.7/tutorial_notebooks/SWEET.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/tutorial_notebooks/TCEs.ipynb` & `exovetter-0.0.7/tutorial_notebooks/TCEs.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/tutorial_notebooks/TransitPhaseCoverage.ipynb` & `exovetter-0.0.7/tutorial_notebooks/TransitPhaseCoverage.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/tutorial_notebooks/VizTransits.ipynb` & `exovetter-0.0.7/tutorial_notebooks/VizTransits.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/tutorial_notebooks/lightcurves.ipynb` & `exovetter-0.0.7/tutorial_notebooks/lightcurves.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/tutorial_notebooks/modshift.ipynb` & `exovetter-0.0.7/tutorial_notebooks/modshift.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.6/tutorial_notebooks/wasp18b.fits` & `exovetter-0.0.7/tutorial_notebooks/wasp18b.fits`

 * *Files identical despite different names*

