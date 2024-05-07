# Comparing `tmp/menpofit-0.7.0.tar.gz` & `tmp/menpofit-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "menpofit-0.7.0.tar", last modified: Thu Jan 14 20:56:13 2021, max compression
+gzip compressed data, was "menpofit-0.7.1.tar", last modified: Tue May  7 11:02:53 2024, max compression
```

## Comparing `menpofit-0.7.0.tar` & `menpofit-0.7.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.961196 menpofit-0.7.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      480 2021-01-14 20:53:01.000000 menpofit-0.7.0/AUTHORS.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1643 2021-01-14 20:53:01.000000 menpofit-0.7.0/LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2021-01-14 20:53:01.000000 menpofit-0.7.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)      274 2021-01-14 20:56:13.961196 menpofit-0.7.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3337 2021-01-14 20:53:01.000000 menpofit-0.7.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.961196 menpofit-0.7.0/menpofit/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      333 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2021-01-14 20:56:13.965196 menpofit-0.7.0/menpofit/_static_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6088 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/_version.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.949196 menpofit-0.7.0/menpofit/aam/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      818 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aam/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.949196 menpofit-0.7.0/menpofit/aam/algorithm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      561 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aam/algorithm/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    59638 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aam/algorithm/lk.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19492 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aam/algorithm/sd.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    55755 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aam/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22434 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aam/fitter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1903 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aam/pretrained.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5427 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aam/result.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.953196 menpofit-0.7.0/menpofit/aps/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      113 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aps/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.953196 menpofit-0.7.0/menpofit/aps/algorithm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aps/algorithm/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23236 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aps/algorithm/gn.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35086 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aps/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8571 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aps/fitter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12842 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/aps/result.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.953196 menpofit-0.7.0/menpofit/atm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      186 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/atm/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14467 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/atm/algorithm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    43708 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/atm/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4472 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/atm/fitter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1123 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15759 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/builder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16617 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/checks.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.953196 menpofit-0.7.0/menpofit/clm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      253 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/clm/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.953196 menpofit-0.7.0/menpofit/clm/algorithm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       63 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/clm/algorithm/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14120 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/clm/algorithm/gd.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17910 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/clm/base.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.953196 menpofit-0.7.0/menpofit/clm/expert/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      128 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/clm/expert/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4956 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/clm/expert/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15624 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/clm/expert/ensemble.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4332 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/clm/fitter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3185 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/differentiable.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.957196 menpofit-0.7.0/menpofit/dlib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      168 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/dlib/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7089 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/dlib/algorithm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1368 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/dlib/conversion.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26465 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/dlib/fitter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.957196 menpofit-0.7.0/menpofit/error/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1025 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/error/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20913 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/error/base.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.957196 menpofit-0.7.0/menpofit/error/human/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      345 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/error/human/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15076 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/error/human/face.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4498 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/error/stats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35671 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/fitter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16345 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/io.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.957196 menpofit-0.7.0/menpofit/lk/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      252 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/lk/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16204 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/lk/algorithm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9468 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/lk/fitter.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    34565 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/lk/residual.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4664 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/lk/result.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.957196 menpofit-0.7.0/menpofit/math/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      194 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/math/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14354 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/math/correlationfilter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8323 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/math/fft_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12739 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/math/regression.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26958 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/modelinstance.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   118801 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/result.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.957196 menpofit-0.7.0/menpofit/sdm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1232 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/sdm/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.961196 menpofit-0.7.0/menpofit/sdm/algorithm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1279 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/sdm/algorithm/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25771 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/sdm/algorithm/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16364 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/sdm/algorithm/fullyparametric.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10542 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/sdm/algorithm/nonparametric.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11091 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/sdm/algorithm/parametricappearance.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12770 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/sdm/algorithm/parametricshape.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35099 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/sdm/fitter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.961196 menpofit-0.7.0/menpofit/transform/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      446 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/transform/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13711 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/transform/homogeneous.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22398 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/transform/modeldriven.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4601 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/transform/piecewiseaffine.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2789 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/transform/rbf.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.961196 menpofit-0.7.0/menpofit/transform/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/transform/test/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4541 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/transform/test/h_affine_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6324 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/transform/test/homogeneous_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2277 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/transform/test/rbf_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1523 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/transform/test/tps_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7008 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/transform/thinsplatesplines.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.961196 menpofit-0.7.0/menpofit/unified_aam_clm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      201 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/unified_aam_clm/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17178 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/unified_aam_clm/algorithm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23036 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/unified_aam_clm/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9448 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/unified_aam_clm/fitter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5503 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/unified_aam_clm/result.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.961196 menpofit-0.7.0/menpofit/visualize/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      161 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/visualize/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39484 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/visualize/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10112 2021-01-14 20:53:01.000000 menpofit-0.7.0/menpofit/visualize/textutils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-14 20:56:13.949196 menpofit-0.7.0/menpofit.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      274 2021-01-14 20:56:13.000000 menpofit-0.7.0/menpofit.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2566 2021-01-14 20:56:13.000000 menpofit-0.7.0/menpofit.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-01-14 20:56:13.000000 menpofit-0.7.0/menpofit.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2021-01-14 20:56:13.000000 menpofit-0.7.0/menpofit.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2021-01-14 20:56:13.000000 menpofit-0.7.0/menpofit.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      204 2021-01-14 20:56:13.961196 menpofit-0.7.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      947 2021-01-14 20:53:01.000000 menpofit-0.7.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.852250 menpofit-0.7.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      480 2024-05-07 11:00:37.000000 menpofit-0.7.1/AUTHORS.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1643 2024-05-07 11:00:37.000000 menpofit-0.7.1/LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2024-05-07 11:00:37.000000 menpofit-0.7.1/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      349 2024-05-07 11:02:53.852250 menpofit-0.7.1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3337 2024-05-07 11:00:37.000000 menpofit-0.7.1/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.852250 menpofit-0.7.1/menpofit/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      333 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2024-05-07 11:02:53.852250 menpofit-0.7.1/menpofit/_static_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6088 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/_version.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.840250 menpofit-0.7.1/menpofit/aam/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      818 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aam/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.840250 menpofit-0.7.1/menpofit/aam/algorithm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      561 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aam/algorithm/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    59634 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aam/algorithm/lk.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19492 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aam/algorithm/sd.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    55755 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aam/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22433 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aam/fitter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1900 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aam/pretrained.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5427 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aam/result.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.840250 menpofit-0.7.1/menpofit/aps/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      113 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aps/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.840250 menpofit-0.7.1/menpofit/aps/algorithm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aps/algorithm/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23233 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aps/algorithm/gn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35086 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aps/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8571 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aps/fitter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12842 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/aps/result.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.844250 menpofit-0.7.1/menpofit/atm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      186 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/atm/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14467 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/atm/algorithm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    43708 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/atm/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4472 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/atm/fitter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1123 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15759 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/builder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16623 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/checks.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.844250 menpofit-0.7.1/menpofit/clm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      253 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/clm/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.844250 menpofit-0.7.1/menpofit/clm/algorithm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       63 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/clm/algorithm/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14120 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/clm/algorithm/gd.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17910 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/clm/base.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.844250 menpofit-0.7.1/menpofit/clm/expert/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      128 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/clm/expert/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4956 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/clm/expert/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15624 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/clm/expert/ensemble.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4332 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/clm/fitter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3185 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/differentiable.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.844250 menpofit-0.7.1/menpofit/dlib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      168 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/dlib/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7089 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/dlib/algorithm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1368 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/dlib/conversion.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26465 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/dlib/fitter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.844250 menpofit-0.7.1/menpofit/error/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1025 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/error/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20913 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/error/base.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.844250 menpofit-0.7.1/menpofit/error/human/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      345 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/error/human/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15076 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/error/human/face.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4498 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/error/stats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35631 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/fitter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16345 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/io.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.844250 menpofit-0.7.1/menpofit/lk/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      252 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/lk/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16204 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/lk/algorithm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9468 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/lk/fitter.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    34565 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/lk/residual.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4664 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/lk/result.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.848250 menpofit-0.7.1/menpofit/math/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      194 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/math/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14354 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/math/correlationfilter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8323 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/math/fft_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12739 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/math/regression.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26958 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/modelinstance.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   118801 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/result.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.848250 menpofit-0.7.1/menpofit/sdm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1232 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/sdm/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.848250 menpofit-0.7.1/menpofit/sdm/algorithm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1279 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/sdm/algorithm/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25771 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/sdm/algorithm/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16364 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/sdm/algorithm/fullyparametric.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10542 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/sdm/algorithm/nonparametric.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11091 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/sdm/algorithm/parametricappearance.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12770 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/sdm/algorithm/parametricshape.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35099 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/sdm/fitter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.848250 menpofit-0.7.1/menpofit/transform/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      446 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/transform/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13705 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/transform/homogeneous.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22398 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/transform/modeldriven.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4601 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/transform/piecewiseaffine.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2789 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/transform/rbf.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.848250 menpofit-0.7.1/menpofit/transform/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/transform/test/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4541 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/transform/test/h_affine_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6324 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/transform/test/homogeneous_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2277 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/transform/test/rbf_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1523 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/transform/test/tps_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7008 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/transform/thinsplatesplines.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.848250 menpofit-0.7.1/menpofit/unified_aam_clm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      201 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/unified_aam_clm/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17178 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/unified_aam_clm/algorithm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23036 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/unified_aam_clm/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9448 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/unified_aam_clm/fitter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5503 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/unified_aam_clm/result.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.848250 menpofit-0.7.1/menpofit/visualize/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      161 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/visualize/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39484 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/visualize/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10112 2024-05-07 11:00:38.000000 menpofit-0.7.1/menpofit/visualize/textutils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:02:53.852250 menpofit-0.7.1/menpofit.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      349 2024-05-07 11:02:53.000000 menpofit-0.7.1/menpofit.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2566 2024-05-07 11:02:53.000000 menpofit-0.7.1/menpofit.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-07 11:02:53.000000 menpofit-0.7.1/menpofit.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2024-05-07 11:02:53.000000 menpofit-0.7.1/menpofit.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2024-05-07 11:02:53.000000 menpofit-0.7.1/menpofit.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      204 2024-05-07 11:02:53.852250 menpofit-0.7.1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      947 2024-05-07 11:00:38.000000 menpofit-0.7.1/setup.py
```

### Comparing `menpofit-0.7.0/LICENSE.txt` & `menpofit-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/README.md` & `menpofit-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/_version.py` & `menpofit-0.7.1/menpofit/_version.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/aam/__init__.py` & `menpofit-0.7.1/menpofit/aam/__init__.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/aam/algorithm/__init__.py` & `menpofit-0.7.1/menpofit/aam/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/aam/algorithm/lk.py` & `menpofit-0.7.1/menpofit/aam/algorithm/lk.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,19 +50,19 @@
         self._build_sampling_mask(sampling)
 
     def _build_sampling_mask(self, sampling):
         n_true_pixels = self.template.n_true_pixels()
         n_channels = self.template.n_channels
         n_parameters = self.transform.n_parameters
 
-        sampling_mask = np.zeros(n_true_pixels, dtype=np.bool)
+        sampling_mask = np.zeros(n_true_pixels, dtype=bool)
 
         if sampling is None:
             sampling = range(0, n_true_pixels, 1)
-        elif isinstance(sampling, np.int):
+        elif isinstance(sampling, np.int64):
             sampling = range(0, n_true_pixels, sampling)
 
         sampling_mask[sampling] = 1
 
         self.i_mask = np.nonzero(np.tile(
             sampling_mask[None, ...], (n_channels, 1)).flatten())[0]
         self.dW_dp_mask = np.nonzero(np.tile(
@@ -469,15 +469,15 @@
         self.patch_normalisation = patch_normalisation
 
         super(LucasKanadePatchBaseInterface, self).__init__(
             transform, template, sampling=sampling)
 
     def _build_sampling_mask(self, sampling):
         if sampling is None:
-            sampling = np.ones(self.patch_shape, dtype=np.bool)
+            sampling = np.ones(self.patch_shape, dtype=bool)
 
         image_shape = self.template.pixels.shape
         image_mask = np.tile(sampling[None, None, None, ...],
                              image_shape[:3] + (1, 1))
         self.i_mask = np.nonzero(image_mask.flatten())[0]
         self.gradient_mask = np.nonzero(np.tile(
             image_mask[None, ...], (2, 1, 1, 1, 1, 1)))
```

### Comparing `menpofit-0.7.0/menpofit/aam/algorithm/sd.py` & `menpofit-0.7.1/menpofit/aam/algorithm/sd.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/aam/base.py` & `menpofit-0.7.1/menpofit/aam/base.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/aam/fitter.py` & `menpofit-0.7.1/menpofit/aam/fitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,15 +447,15 @@
     """
     reference = aam.appearance_models[0].mean()
     scaled_reference = reference.rescale(scale)
 
     t = AlignmentUniformScale(scaled_reference.landmarks['source'],
                               reference.landmarks['source'])
     new_indices = np.require(np.round(t.apply(
-        scaled_reference.mask.true_indices())), dtype=np.int)
+        scaled_reference.mask.true_indices())), dtype=np.int64)
 
     modified_mask = deepcopy(reference.mask.pixels)
     modified_mask[:] = False
     modified_mask[:, new_indices[:, 0], new_indices[:, 1]] = True
 
     true_positions = np.nonzero(
         modified_mask[:, reference.mask.mask].ravel())[0]
@@ -481,15 +481,15 @@
         belong to the new mask.
     boolean_image : `menpo.image.BooleanImage`
         The boolean image of the mask.
     """
     reference = aam.appearance_models[0].mean()
 
     n_true_pixels = reference.n_true_pixels()
-    true_positions = np.zeros(n_true_pixels, dtype=np.bool)
+    true_positions = np.zeros(n_true_pixels, dtype=bool)
     sampling = range(0, n_true_pixels, step)
     true_positions[sampling] = True
 
     modified_mask = reference.mask.copy()
     new_indices = modified_mask.true_indices()[sampling, :]
     modified_mask.mask[:] = False
     modified_mask.mask[new_indices[:, 0], new_indices[:, 1]] = True
```

### Comparing `menpofit-0.7.0/menpofit/aam/pretrained.py` & `menpofit-0.7.1/menpofit/aam/pretrained.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     .. code-block:: python
 
       import numpy as np
 
       patch_shape = (13, 13)
       sampling_step = 4
 
-      sampling_grid = np.zeros(patch_shape, dtype=np.bool)
+      sampling_grid = np.zeros(patch_shape, dtype=bool)
       sampling_grid[::sampling_step, ::sampling_step] = True
       sampling = [sampling_grid, sampling_grid]
 
     Additionally, it is trained on LFPW trainset, HELEN trainset, IBUG and AFW
     datasets (3283 images in total), which are hosted in
     http://ibug.doc.ic.ac.uk/resources/facial-point-annotations/.
```

### Comparing `menpofit-0.7.0/menpofit/aam/result.py` & `menpofit-0.7.1/menpofit/aam/result.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/aps/algorithm/gn.py` & `menpofit-0.7.1/menpofit/aps/algorithm/gn.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self.template = template
 
         # build the sampling mask
         self._build_sampling_mask(sampling)
 
     def _build_sampling_mask(self, sampling):
         if sampling is None:
-            sampling = np.ones(self.patch_shape, dtype=np.bool)
+            sampling = np.ones(self.patch_shape, dtype=bool)
 
         image_shape = self.template.pixels.shape
         image_mask = np.tile(sampling[None, None, None, ...],
                              image_shape[:3] + (1, 1))
         self.i_mask = np.nonzero(image_mask.flatten())[0]
         self.gradient_mask = np.nonzero(np.tile(
             image_mask[None, ...], (2, 1, 1, 1, 1, 1)))
```

### Comparing `menpofit-0.7.0/menpofit/aps/base.py` & `menpofit-0.7.1/menpofit/aps/base.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/aps/fitter.py` & `menpofit-0.7.1/menpofit/aps/fitter.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/aps/result.py` & `menpofit-0.7.1/menpofit/aps/result.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/atm/algorithm.py` & `menpofit-0.7.1/menpofit/atm/algorithm.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/atm/base.py` & `menpofit-0.7.1/menpofit/atm/base.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/atm/fitter.py` & `menpofit-0.7.1/menpofit/atm/fitter.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/base.py` & `menpofit-0.7.1/menpofit/base.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/builder.py` & `menpofit-0.7.1/menpofit/builder.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/checks.py` & `menpofit-0.7.1/menpofit/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,15 +311,15 @@
     elif len(max_iters) == 1 and n_scales > 1:
         max_iters = [np.round(max_iters[0]/n_scales)
                      for _ in range(n_scales)]
     elif len(max_iters) != n_scales:
         raise ValueError('max_iters can be integer, integer list '
                          'containing 1 or {} elements or '
                          'None'.format(n_scales))
-    return np.require(max_iters, dtype=np.int)
+    return np.require(max_iters, dtype=np.int64)
 
 
 def check_sampling(sampling, n_scales):
     r"""
     Function that checks the value of a `sampling` parameter defined for
     multiple scales. It must be `int` or `ndarray` or `list` of those.
 
@@ -340,25 +340,25 @@
     ValueError
         A sampling list can only contain 1 element or {n_scales} elements
     ValueError
         sampling can be an integer or ndarray, a integer or ndarray list
         containing 1 or {n_scales} elements or None
     """
     if (isinstance(sampling, (list, tuple)) and
-        np.alltrue([isinstance(s, (np.ndarray, np.int)) or sampling is None
+        np.alltrue([isinstance(s, (np.ndarray, np.int64)) or sampling is None
                     for s in sampling])):
         if len(sampling) == 1:
             return sampling * n_scales
         elif len(sampling) == n_scales:
             return sampling
         else:
             raise ValueError('A sampling list can only '
                              'contain 1 element or {} '
                              'elements'.format(n_scales))
-    elif isinstance(sampling, (np.ndarray, np.int)) or sampling is None:
+    elif isinstance(sampling, (np.ndarray, np.int64)) or sampling is None:
         return [sampling] * n_scales
     else:
         raise ValueError('sampling can be an integer or ndarray, '
                          'a integer or ndarray list '
                          'containing 1 or {} elements or '
                          'None'.format(n_scales))
```

### Comparing `menpofit-0.7.0/menpofit/clm/algorithm/gd.py` & `menpofit-0.7.1/menpofit/clm/algorithm/gd.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/clm/base.py` & `menpofit-0.7.1/menpofit/clm/base.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/clm/expert/base.py` & `menpofit-0.7.1/menpofit/clm/expert/base.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/clm/expert/ensemble.py` & `menpofit-0.7.1/menpofit/clm/expert/ensemble.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/clm/fitter.py` & `menpofit-0.7.1/menpofit/clm/fitter.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/differentiable.py` & `menpofit-0.7.1/menpofit/differentiable.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/dlib/algorithm.py` & `menpofit-0.7.1/menpofit/dlib/algorithm.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/dlib/conversion.py` & `menpofit-0.7.1/menpofit/dlib/conversion.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/dlib/fitter.py` & `menpofit-0.7.1/menpofit/dlib/fitter.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/error/__init__.py` & `menpofit-0.7.1/menpofit/error/__init__.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/error/base.py` & `menpofit-0.7.1/menpofit/error/base.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/error/human/face.py` & `menpofit-0.7.1/menpofit/error/human/face.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/error/stats.py` & `menpofit-0.7.1/menpofit/error/stats.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/fitter.py` & `menpofit-0.7.1/menpofit/fitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,24 +67,24 @@
     elif len(noise_percentage) == 1:
         noise_percentage *= 3
 
     similarity = AlignmentSimilarity(source, target,
                                      rotation=allow_alignment_rotation)
 
     if noise_type is 'gaussian':
-        s = noise_percentage[0] * (0.5 / 3) * np.asscalar(np.random.randn(1))
-        r = noise_percentage[1] * (180 / 3) * np.asscalar(np.random.randn(1))
+        s = noise_percentage[0] * (0.5 / 3) * np.random.randn(1)[0]
+        r = noise_percentage[1] * (180 / 3) * np.random.randn(1)[0]
         t = noise_percentage[2] * (target.range() / 3) * np.random.randn(2)
 
         s = scale_about_centre(target, 1 + s)
         r = rotate_ccw_about_centre(target, r)
         t = Translation(t, source.n_dims)
     elif noise_type is 'uniform':
-        s = noise_percentage[0] * 0.5 * (2 * np.asscalar(np.random.randn(1)) - 1)
-        r = noise_percentage[1] * 180 * (2 * np.asscalar(np.random.rand(1)) - 1)
+        s = noise_percentage[0] * 0.5 * (2 * np.random.randn(1)[0] - 1)
+        r = noise_percentage[1] * 180 * (2 * np.random.rand(1)[0] - 1)
         t = noise_percentage[2] * target.range() * (2 * np.random.rand(2) - 1)
 
         s = scale_about_centre(target, 1. + s)
         r = rotate_ccw_about_centre(target, r)
         t = Translation(t, source.n_dims)
     else:
         raise ValueError('Unexpected noise type. '
```

### Comparing `menpofit-0.7.0/menpofit/io.py` & `menpofit-0.7.1/menpofit/io.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/lk/algorithm.py` & `menpofit-0.7.1/menpofit/lk/algorithm.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/lk/fitter.py` & `menpofit-0.7.1/menpofit/lk/fitter.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/lk/residual.py` & `menpofit-0.7.1/menpofit/lk/residual.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/lk/result.py` & `menpofit-0.7.1/menpofit/lk/result.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/math/correlationfilter.py` & `menpofit-0.7.1/menpofit/math/correlationfilter.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/math/fft_utils.py` & `menpofit-0.7.1/menpofit/math/fft_utils.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/math/regression.py` & `menpofit-0.7.1/menpofit/math/regression.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/modelinstance.py` & `menpofit-0.7.1/menpofit/modelinstance.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/result.py` & `menpofit-0.7.1/menpofit/result.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/sdm/__init__.py` & `menpofit-0.7.1/menpofit/sdm/__init__.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/sdm/algorithm/__init__.py` & `menpofit-0.7.1/menpofit/sdm/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/sdm/algorithm/base.py` & `menpofit-0.7.1/menpofit/sdm/algorithm/base.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/sdm/algorithm/fullyparametric.py` & `menpofit-0.7.1/menpofit/sdm/algorithm/fullyparametric.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/sdm/algorithm/nonparametric.py` & `menpofit-0.7.1/menpofit/sdm/algorithm/nonparametric.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/sdm/algorithm/parametricappearance.py` & `menpofit-0.7.1/menpofit/sdm/algorithm/parametricappearance.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/sdm/algorithm/parametricshape.py` & `menpofit-0.7.1/menpofit/sdm/algorithm/parametricshape.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/sdm/fitter.py` & `menpofit-0.7.1/menpofit/sdm/fitter.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/transform/homogeneous.py` & `menpofit-0.7.1/menpofit/transform/homogeneous.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
         raise ValueError(
             "Trying to sample jacobian in incorrect dimensions "
             "(transform is {0}D, sampling at {1}D)".format(
                 self.n_dims, points_n_dim))
     # prealloc the jacobian
     jac = np.zeros((n_points, self.n_parameters, self.n_dims))
     # a mask that we can apply at each iteration
-    dim_mask = np.eye(self.n_dims, dtype=np.bool)
+    dim_mask = np.eye(self.n_dims, dtype=bool)
 
     for i, s in enumerate(
             range(0, self.n_dims * self.n_dims, self.n_dims)):
         # i is current axis
         # s is slicing offset
         # make a mask for a single points jacobian
         full_mask = np.zeros((self.n_parameters, self.n_dims), dtype=bool)
@@ -379,13 +379,13 @@
     _apply_jacobian_mask(sim, jac, np.array([0, 1]), 3, ones)
 
     return jac
 
 
 def _apply_jacobian_mask(sim, jac, param_mask, row_index, points):
     # make a mask for a single points jacobian
-    full_mask = np.zeros((sim.n_parameters, sim.n_dims), dtype=np.bool)
+    full_mask = np.zeros((sim.n_parameters, sim.n_dims), dtype=bool)
     # fill the mask in for the ith axis
     full_mask[row_index] = [True, True]
     # assign the ith axis points to this mask, broadcasting over all
     # points
     jac[:, full_mask] = points * param_mask
```

### Comparing `menpofit-0.7.0/menpofit/transform/modeldriven.py` & `menpofit-0.7.1/menpofit/transform/modeldriven.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/transform/piecewiseaffine.py` & `menpofit-0.7.1/menpofit/transform/piecewiseaffine.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/transform/rbf.py` & `menpofit-0.7.1/menpofit/transform/rbf.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/transform/test/h_affine_test.py` & `menpofit-0.7.1/menpofit/transform/test/h_affine_test.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/transform/test/homogeneous_test.py` & `menpofit-0.7.1/menpofit/transform/test/homogeneous_test.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/transform/test/rbf_test.py` & `menpofit-0.7.1/menpofit/transform/test/rbf_test.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/transform/test/tps_test.py` & `menpofit-0.7.1/menpofit/transform/test/tps_test.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/transform/thinsplatesplines.py` & `menpofit-0.7.1/menpofit/transform/thinsplatesplines.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/unified_aam_clm/algorithm.py` & `menpofit-0.7.1/menpofit/unified_aam_clm/algorithm.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/unified_aam_clm/base.py` & `menpofit-0.7.1/menpofit/unified_aam_clm/base.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/unified_aam_clm/fitter.py` & `menpofit-0.7.1/menpofit/unified_aam_clm/fitter.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/unified_aam_clm/result.py` & `menpofit-0.7.1/menpofit/unified_aam_clm/result.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/visualize/base.py` & `menpofit-0.7.1/menpofit/visualize/base.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit/visualize/textutils.py` & `menpofit-0.7.1/menpofit/visualize/textutils.py`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/menpofit.egg-info/SOURCES.txt` & `menpofit-0.7.1/menpofit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `menpofit-0.7.0/setup.py` & `menpofit-0.7.1/setup.py`

 * *Files identical despite different names*

