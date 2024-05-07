# Comparing `tmp/pyswipe-0.9.6.tar.gz` & `tmp/pyswipe-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyswipe-0.9.6.tar", last modified: Fri May  3 06:12:18 2024, max compression
+gzip compressed data, was "pyswipe-0.9.7.tar", last modified: Tue May  7 04:51:57 2024, max compression
```

## Comparing `pyswipe-0.9.6.tar` & `pyswipe-0.9.7.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.213415 pyswipe-0.9.6/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       68 2024-03-04 09:30:57.000000 pyswipe-0.9.6/.coveragerc
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      136 2024-03-04 09:30:57.000000 pyswipe-0.9.6/.gitignore
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1241 2024-03-04 09:30:57.000000 pyswipe-0.9.6/.travis.yml
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       59 2024-03-04 09:30:57.000000 pyswipe-0.9.6/CHANGELOG.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      518 2024-03-04 09:30:57.000000 pyswipe-0.9.6/CITATION.cff
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      281 2024-03-04 09:30:57.000000 pyswipe-0.9.6/CITATION_old.cff
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1072 2024-03-04 09:30:57.000000 pyswipe-0.9.6/LICENSE
--rw-r--r--   0 spencerh  (1000) spencerh  (1000)     6588 2024-05-03 06:12:18.213415 pyswipe-0.9.6/PKG-INFO
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     4008 2024-04-10 07:18:07.000000 pyswipe-0.9.6/README.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      189 2024-03-04 09:30:57.000000 pyswipe-0.9.6/TODO.md
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.197415 pyswipe-0.9.6/docs/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      676 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/Makefile
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.197415 pyswipe-0.9.6/docs/source/
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.197415 pyswipe-0.9.6/docs/source/.templates/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      157 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/.templates/layout.html
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       32 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/changelog.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     6212 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/conf.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      476 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/index.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      632 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/installation.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     2874 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/model_coefficients.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       29 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/readme.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1046 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/reference.rst
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8103 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/source/usage.rst
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.205415 pyswipe-0.9.6/docs/static/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)  6334764 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/static/animation.gif
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       47 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/static/custom.css
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   220149 2024-03-04 09:30:57.000000 pyswipe-0.9.6/docs/static/example_plot.png
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1466 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyproject.toml
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.209415 pyswipe-0.9.6/pyswipe/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      305 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/__init__.py
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.213415 pyswipe-0.9.6/pyswipe/coefficients/
--rw-r--r--   0 spencerh  (1000) spencerh  (1000)   106628 2024-03-04 09:27:34.000000 pyswipe-0.9.6/pyswipe/coefficients/SW_OPER_EIO_SWI_2E_00000000T000000_99999999T999999_0101.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      144 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/constants.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   310000 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/mlat_scalargrid.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   300000 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/mlt_scalargrid.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    13152 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/mlt_utils.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    10843 2024-05-03 05:57:04.000000 pyswipe-0.9.6/pyswipe/model_utils.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     4406 2024-05-03 06:02:49.000000 pyswipe-0.9.6/pyswipe/model_vector_to_txt.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    48412 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/plot_utils.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   312289 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/potential.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    40562 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/sh_utils.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   158608 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/swipe.py
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.213415 pyswipe-0.9.6/pyswipe/tests/
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8557 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/01__plot_cpcp_vs_hemi_bt_and_clockangle.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8061 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/02__E_at_lowlatboundary.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    10936 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/03__hi-c_cpcp_vs_other_studies.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     9022 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/04__potential_dial_plots.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    11467 2024-05-03 06:05:31.000000 pyswipe-0.9.6/pyswipe/tests/04__potential_dial_plots__alternative_levels.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8162 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/05__emwork_dial_plots.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     9136 2024-05-03 06:05:45.000000 pyswipe-0.9.6/pyswipe/tests/05__emwork_dial_plots__alternative_levels.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     9489 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/06__plot_emwork_vs_hemi_bt_and_clockangle.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8325 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/08__conductance_dial_plots__filledcell.py
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     4853 2024-03-04 09:30:57.000000 pyswipe-0.9.6/pyswipe/tests/09__dask_functions_for_large_input.py
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.213415 pyswipe-0.9.6/pyswipe.egg-info/
--rw-r--r--   0 spencerh  (1000) spencerh  (1000)     6588 2024-05-03 06:12:18.000000 pyswipe-0.9.6/pyswipe.egg-info/PKG-INFO
--rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     1641 2024-05-03 06:12:18.000000 pyswipe-0.9.6/pyswipe.egg-info/SOURCES.txt
--rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)        1 2024-05-03 06:12:18.000000 pyswipe-0.9.6/pyswipe.egg-info/dependency_links.txt
--rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)      156 2024-05-03 06:12:18.000000 pyswipe-0.9.6/pyswipe.egg-info/requires.txt
--rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)        8 2024-05-03 06:12:18.000000 pyswipe-0.9.6/pyswipe.egg-info/top_level.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      106 2024-03-04 09:31:09.000000 pyswipe-0.9.6/requirements.txt
--rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       38 2024-05-03 06:12:18.217415 pyswipe-0.9.6/setup.cfg
-drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-03 06:12:18.213415 pyswipe-0.9.6/tests/
--rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)      541 2021-08-20 11:22:35.000000 pyswipe-0.9.6/tests/test_basic.py
--rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     4231 2021-08-20 11:22:35.000000 pyswipe-0.9.6/tests/test_mlt_utils.py
--rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     1042 2021-08-20 11:22:35.000000 pyswipe-0.9.6/tests/test_model_utils.py
--rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)      804 2021-08-20 11:22:35.000000 pyswipe-0.9.6/tests/test_model_vector_to_txt.py
--rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     3653 2021-08-20 11:22:35.000000 pyswipe-0.9.6/tests/test_plot_utils.py
--rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     6350 2021-08-20 11:22:35.000000 pyswipe-0.9.6/tests/test_sh_utils.py
--rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)    17380 2023-09-14 05:36:06.000000 pyswipe-0.9.6/tests/test_swipe.py
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-07 04:51:57.196206 pyswipe-0.9.7/
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       68 2024-03-04 09:30:57.000000 pyswipe-0.9.7/.coveragerc
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      136 2024-03-04 09:30:57.000000 pyswipe-0.9.7/.gitignore
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1241 2024-03-04 09:30:57.000000 pyswipe-0.9.7/.travis.yml
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       59 2024-03-04 09:30:57.000000 pyswipe-0.9.7/CHANGELOG.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      518 2024-03-04 09:30:57.000000 pyswipe-0.9.7/CITATION.cff
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      281 2024-03-04 09:30:57.000000 pyswipe-0.9.7/CITATION_old.cff
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1072 2024-03-04 09:30:57.000000 pyswipe-0.9.7/LICENSE
+-rw-r--r--   0 spencerh  (1000) spencerh  (1000)     6588 2024-05-07 04:51:57.196206 pyswipe-0.9.7/PKG-INFO
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     4008 2024-04-10 07:18:07.000000 pyswipe-0.9.7/README.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      189 2024-03-04 09:30:57.000000 pyswipe-0.9.7/TODO.md
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-07 04:51:57.180207 pyswipe-0.9.7/docs/
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      676 2024-03-04 09:30:57.000000 pyswipe-0.9.7/docs/Makefile
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-07 04:51:57.180207 pyswipe-0.9.7/docs/source/
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-07 04:51:57.180207 pyswipe-0.9.7/docs/source/.templates/
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      157 2024-03-04 09:30:57.000000 pyswipe-0.9.7/docs/source/.templates/layout.html
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       32 2024-03-04 09:30:57.000000 pyswipe-0.9.7/docs/source/changelog.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     6212 2024-03-04 09:30:57.000000 pyswipe-0.9.7/docs/source/conf.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      476 2024-03-04 09:30:57.000000 pyswipe-0.9.7/docs/source/index.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      632 2024-03-04 09:30:57.000000 pyswipe-0.9.7/docs/source/installation.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     2874 2024-03-04 09:30:57.000000 pyswipe-0.9.7/docs/source/model_coefficients.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       29 2024-03-04 09:30:57.000000 pyswipe-0.9.7/docs/source/readme.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1046 2024-03-04 09:30:57.000000 pyswipe-0.9.7/docs/source/reference.rst
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8103 2024-03-04 09:30:57.000000 pyswipe-0.9.7/docs/source/usage.rst
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-07 04:51:57.188207 pyswipe-0.9.7/docs/static/
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)  6334764 2024-03-04 09:30:57.000000 pyswipe-0.9.7/docs/static/animation.gif
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       47 2024-03-04 09:30:57.000000 pyswipe-0.9.7/docs/static/custom.css
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   220149 2024-03-04 09:30:57.000000 pyswipe-0.9.7/docs/static/example_plot.png
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     1466 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyproject.toml
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-07 04:51:57.192206 pyswipe-0.9.7/pyswipe/
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      305 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/__init__.py
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-07 04:51:57.192206 pyswipe-0.9.7/pyswipe/coefficients/
+-rw-r--r--   0 spencerh  (1000) spencerh  (1000)   106628 2024-03-04 09:27:34.000000 pyswipe-0.9.7/pyswipe/coefficients/SW_OPER_EIO_SHA_2E_00000000T000000_99999999T999999_0101.txt
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      144 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/constants.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   310000 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/mlat_scalargrid.txt
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   300000 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/mlt_scalargrid.txt
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    13152 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/mlt_utils.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    10843 2024-05-07 04:43:17.000000 pyswipe-0.9.7/pyswipe/model_utils.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     4406 2024-05-03 06:02:49.000000 pyswipe-0.9.7/pyswipe/model_vector_to_txt.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    48412 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/plot_utils.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   312289 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/potential.txt
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    40562 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/sh_utils.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)   158608 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/swipe.py
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-07 04:51:57.196206 pyswipe-0.9.7/pyswipe/tests/
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8557 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/tests/01__plot_cpcp_vs_hemi_bt_and_clockangle.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8061 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/tests/02__E_at_lowlatboundary.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    10936 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/tests/03__hi-c_cpcp_vs_other_studies.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     9022 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/tests/04__potential_dial_plots.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)    11467 2024-05-03 06:05:31.000000 pyswipe-0.9.7/pyswipe/tests/04__potential_dial_plots__alternative_levels.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8162 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/tests/05__emwork_dial_plots.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     9136 2024-05-03 06:05:45.000000 pyswipe-0.9.7/pyswipe/tests/05__emwork_dial_plots__alternative_levels.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     9489 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/tests/06__plot_emwork_vs_hemi_bt_and_clockangle.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     8325 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/tests/08__conductance_dial_plots__filledcell.py
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)     4853 2024-03-04 09:30:57.000000 pyswipe-0.9.7/pyswipe/tests/09__dask_functions_for_large_input.py
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-07 04:51:57.196206 pyswipe-0.9.7/pyswipe.egg-info/
+-rw-r--r--   0 spencerh  (1000) spencerh  (1000)     6588 2024-05-07 04:51:57.000000 pyswipe-0.9.7/pyswipe.egg-info/PKG-INFO
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     1641 2024-05-07 04:51:57.000000 pyswipe-0.9.7/pyswipe.egg-info/SOURCES.txt
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)        1 2024-05-07 04:51:57.000000 pyswipe-0.9.7/pyswipe.egg-info/dependency_links.txt
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)      156 2024-05-07 04:51:57.000000 pyswipe-0.9.7/pyswipe.egg-info/requires.txt
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)        8 2024-05-07 04:51:57.000000 pyswipe-0.9.7/pyswipe.egg-info/top_level.txt
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)      106 2024-03-04 09:31:09.000000 pyswipe-0.9.7/requirements.txt
+-rw-rw-r--   0 spencerh  (1000) spencerh  (1000)       38 2024-05-07 04:51:57.196206 pyswipe-0.9.7/setup.cfg
+drwxrwxr-x   0 spencerh  (1000) spencerh  (1000)        0 2024-05-07 04:51:57.196206 pyswipe-0.9.7/tests/
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)      541 2021-08-20 11:22:35.000000 pyswipe-0.9.7/tests/test_basic.py
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     4231 2021-08-20 11:22:35.000000 pyswipe-0.9.7/tests/test_mlt_utils.py
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     1042 2021-08-20 11:22:35.000000 pyswipe-0.9.7/tests/test_model_utils.py
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)      804 2021-08-20 11:22:35.000000 pyswipe-0.9.7/tests/test_model_vector_to_txt.py
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     3653 2021-08-20 11:22:35.000000 pyswipe-0.9.7/tests/test_plot_utils.py
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)     6350 2021-08-20 11:22:35.000000 pyswipe-0.9.7/tests/test_sh_utils.py
+-rwxr-xr-x   0 spencerh  (1000) spencerh  (1000)    17380 2023-09-14 05:36:06.000000 pyswipe-0.9.7/tests/test_swipe.py
```

### Comparing `pyswipe-0.9.6/.travis.yml` & `pyswipe-0.9.7/.travis.yml`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/CITATION.cff` & `pyswipe-0.9.7/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/LICENSE` & `pyswipe-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/PKG-INFO` & `pyswipe-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswipe
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python implementation of the Swarm Ionospheric Polar Electrodynamics (Swipe) model
 Author: Karl M. Laundal
 Author-email: "Spencer M. Hatch" <spencer.hatch@ift.uib.no>
 Maintainer-email: "Spencer M. Hatch" <spencer.hatch@ift.uib.no>
 License: MIT License
         
         Copyright (c) 2023 Spencer M Hatch
```

### Comparing `pyswipe-0.9.6/README.rst` & `pyswipe-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/docs/Makefile` & `pyswipe-0.9.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/docs/source/conf.py` & `pyswipe-0.9.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/docs/source/installation.rst` & `pyswipe-0.9.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/docs/source/model_coefficients.rst` & `pyswipe-0.9.7/docs/source/model_coefficients.rst`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/docs/source/reference.rst` & `pyswipe-0.9.7/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/docs/source/usage.rst` & `pyswipe-0.9.7/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/docs/static/animation.gif` & `pyswipe-0.9.7/docs/static/animation.gif`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/docs/static/example_plot.png` & `pyswipe-0.9.7/docs/static/example_plot.png`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyproject.toml` & `pyswipe-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/coefficients/SW_OPER_EIO_SWI_2E_00000000T000000_99999999T999999_0101.txt` & `pyswipe-0.9.7/pyswipe/coefficients/SW_OPER_EIO_SHA_2E_00000000T000000_99999999T999999_0101.txt`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/mlat_scalargrid.txt` & `pyswipe-0.9.7/pyswipe/mlat_scalargrid.txt`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/mlt_scalargrid.txt` & `pyswipe-0.9.7/pyswipe/mlt_scalargrid.txt`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/mlt_utils.py` & `pyswipe-0.9.7/pyswipe/mlt_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/model_utils.py` & `pyswipe-0.9.7/pyswipe/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import reduce
 from .sh_utils import get_A_matrix__Ephizero, get_A_matrix__potzero, SHkeys
 from .constants import REFRE,d2r
 
 basepath = os.path.dirname(__file__)
 # basepath = '/SPENCEdata/Research/database/SHEIC/matrices/10k_points/'
 
-default_coeff_fn = os.path.abspath(os.path.join(basepath,'coefficients','SW_OPER_EIO_SWI_2E_00000000T000000_99999999T999999_0101.txt'))
+default_coeff_fn = os.path.abspath(os.path.join(basepath,'coefficients','SW_OPER_EIO_SHA_2E_00000000T000000_99999999T999999_0101.txt'))
 
 # read coefficient file and store in pandas DataFrame - with column names from last row of header:
 colnames = ([x for x in open(default_coeff_fn).readlines() if x.startswith('#')][-1][1:]).strip().split(' ') 
 
 get_coeffs = lambda fn: pd.read_table(fn, skipinitialspace = True, comment = '#', sep = ' ', names = colnames, index_col = [0, 1])
```

### Comparing `pyswipe-0.9.6/pyswipe/model_vector_to_txt.py` & `pyswipe-0.9.7/pyswipe/model_vector_to_txt.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/plot_utils.py` & `pyswipe-0.9.7/pyswipe/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/potential.txt` & `pyswipe-0.9.7/pyswipe/potential.txt`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/sh_utils.py` & `pyswipe-0.9.7/pyswipe/sh_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/swipe.py` & `pyswipe-0.9.7/pyswipe/swipe.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/tests/01__plot_cpcp_vs_hemi_bt_and_clockangle.py` & `pyswipe-0.9.7/pyswipe/tests/01__plot_cpcp_vs_hemi_bt_and_clockangle.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/tests/02__E_at_lowlatboundary.py` & `pyswipe-0.9.7/pyswipe/tests/02__E_at_lowlatboundary.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/tests/03__hi-c_cpcp_vs_other_studies.py` & `pyswipe-0.9.7/pyswipe/tests/03__hi-c_cpcp_vs_other_studies.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/tests/04__potential_dial_plots.py` & `pyswipe-0.9.7/pyswipe/tests/04__potential_dial_plots.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/tests/04__potential_dial_plots__alternative_levels.py` & `pyswipe-0.9.7/pyswipe/tests/04__potential_dial_plots__alternative_levels.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/tests/05__emwork_dial_plots.py` & `pyswipe-0.9.7/pyswipe/tests/05__emwork_dial_plots.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/tests/05__emwork_dial_plots__alternative_levels.py` & `pyswipe-0.9.7/pyswipe/tests/05__emwork_dial_plots__alternative_levels.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/tests/06__plot_emwork_vs_hemi_bt_and_clockangle.py` & `pyswipe-0.9.7/pyswipe/tests/06__plot_emwork_vs_hemi_bt_and_clockangle.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/tests/08__conductance_dial_plots__filledcell.py` & `pyswipe-0.9.7/pyswipe/tests/08__conductance_dial_plots__filledcell.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe/tests/09__dask_functions_for_large_input.py` & `pyswipe-0.9.7/pyswipe/tests/09__dask_functions_for_large_input.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/pyswipe.egg-info/PKG-INFO` & `pyswipe-0.9.7/pyswipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswipe
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python implementation of the Swarm Ionospheric Polar Electrodynamics (Swipe) model
 Author: Karl M. Laundal
 Author-email: "Spencer M. Hatch" <spencer.hatch@ift.uib.no>
 Maintainer-email: "Spencer M. Hatch" <spencer.hatch@ift.uib.no>
 License: MIT License
         
         Copyright (c) 2023 Spencer M Hatch
```

### Comparing `pyswipe-0.9.6/pyswipe.egg-info/SOURCES.txt` & `pyswipe-0.9.7/pyswipe.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 pyswipe/sh_utils.py
 pyswipe/swipe.py
 pyswipe.egg-info/PKG-INFO
 pyswipe.egg-info/SOURCES.txt
 pyswipe.egg-info/dependency_links.txt
 pyswipe.egg-info/requires.txt
 pyswipe.egg-info/top_level.txt
-pyswipe/coefficients/SW_OPER_EIO_SWI_2E_00000000T000000_99999999T999999_0101.txt
+pyswipe/coefficients/SW_OPER_EIO_SHA_2E_00000000T000000_99999999T999999_0101.txt
 pyswipe/tests/01__plot_cpcp_vs_hemi_bt_and_clockangle.py
 pyswipe/tests/02__E_at_lowlatboundary.py
 pyswipe/tests/03__hi-c_cpcp_vs_other_studies.py
 pyswipe/tests/04__potential_dial_plots.py
 pyswipe/tests/04__potential_dial_plots__alternative_levels.py
 pyswipe/tests/05__emwork_dial_plots.py
 pyswipe/tests/05__emwork_dial_plots__alternative_levels.py
```

### Comparing `pyswipe-0.9.6/tests/test_basic.py` & `pyswipe-0.9.7/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/tests/test_mlt_utils.py` & `pyswipe-0.9.7/tests/test_mlt_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/tests/test_model_utils.py` & `pyswipe-0.9.7/tests/test_model_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/tests/test_model_vector_to_txt.py` & `pyswipe-0.9.7/tests/test_model_vector_to_txt.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/tests/test_plot_utils.py` & `pyswipe-0.9.7/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/tests/test_sh_utils.py` & `pyswipe-0.9.7/tests/test_sh_utils.py`

 * *Files identical despite different names*

### Comparing `pyswipe-0.9.6/tests/test_swipe.py` & `pyswipe-0.9.7/tests/test_swipe.py`

 * *Files identical despite different names*

