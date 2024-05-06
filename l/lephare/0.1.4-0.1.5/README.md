# Comparing `tmp/lephare-0.1.4.tar.gz` & `tmp/lephare-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lephare-0.1.4.tar", last modified: Tue Apr 30 19:03:46 2024, max compression
+gzip compressed data, was "lephare-0.1.5.tar", last modified: Mon May  6 23:48:56 2024, max compression
```

## Comparing `lephare-0.1.4.tar` & `lephare-0.1.5.tar`

### file list

```diff
@@ -1,147 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.970774 lephare-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 19:03:40.000000 lephare-0.1.4/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-30 19:03:40.000000 lephare-0.1.4/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 19:03:40.000000 lephare-0.1.4/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-30 19:03:40.000000 lephare-0.1.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.950774 lephare-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.950774 lephare-0.1.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.954774 lephare-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/workflows/compile-cpp.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-30 19:03:40.000000 lephare-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 19:03:40.000000 lephare-0.1.4/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-30 19:03:40.000000 lephare-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-30 19:03:40.000000 lephare-0.1.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-30 19:03:40.000000 lephare-0.1.4/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-30 19:03:40.000000 lephare-0.1.4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-30 19:03:40.000000 lephare-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-30 19:03:46.970774 lephare-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-30 19:03:40.000000 lephare-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.954774 lephare-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.954774 lephare-0.1.4/docs/doxygen/
--rw-r--r--   0 runner    (1001) docker     (127)   112662 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/doxygen/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/keywords.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/legacy_install.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.954774 lephare-0.1.4/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Building_list_of_onesources.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Data_retrieval.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Example_SED_manipulation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Example_cosmo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Example_full_run.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Example_of_usage_of_magSvc.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.958774 lephare-0.1.4/docs/notebooks/data/
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/data/COSMOS.para
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/data/output.para
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.958774 lephare-0.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-04-30 19:03:40.000000 lephare-0.1.4/examples/color.py
--rw-r--r--   0 runner    (1001) docker     (127)    39348 2024-04-30 19:03:40.000000 lephare-0.1.4/examples/figuresLPP.py
--rw-r--r--   0 runner    (1001) docker     (127)    31984 2024-04-30 19:03:40.000000 lephare-0.1.4/examples/figuresLPZ.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-30 19:03:40.000000 lephare-0.1.4/examples/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-30 19:03:40.000000 lephare-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:03:46.970774 lephare-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-30 19:03:40.000000 lephare-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.946774 lephare-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.958774 lephare-0.1.4/src/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/_flt.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/_photoz.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/data_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/filterSvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/magSvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/mag_gal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/sedtolib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/zphota.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.970774 lephare-0.1.4/src/lephare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.966774 lephare-0.1.4/src/lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3003 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/PDF.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/PDF.h
--rw-r--r--   0 runner    (1001) docker     (127)    72115 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/SED.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/SED.h
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/SEDLib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/SEDLib.h
--rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/_bindings.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/cosmology.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/cosmology.h
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/ext.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/ext.h
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/ext_curv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/filter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/filter_extinc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20186 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/flt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/flt.h
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/globals.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/globals.h
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/keyword.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/keyword.h
--rw-r--r--   0 runner    (1001) docker     (127)    31598 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/mag.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/mag.h
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/mag_gal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/oneElLambda.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/oneElLambda.h
--rw-r--r--   0 runner    (1001) docker     (127)    80072 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/onesource.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/onesource.h
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/opa.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/opa.h
--rw-r--r--   0 runner    (1001) docker     (127)    61669 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/photoz_lib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/photoz_lib.h
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/sedtolib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/zphota.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.966774 lephare-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.966774 lephare-0.1.4/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)    41606 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/calzetti.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.966774 lephare-0.1.4/tests/data/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/examples/COSMOS.para
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.950774 lephare-0.1.4/tests/data/filt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.966774 lephare-0.1.4/tests/data/filt/subaru/
--rw-r--r--   0 runner    (1001) docker     (127)    25919 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/filt/subaru/IB527.pb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.966774 lephare-0.1.4/tests/data/sed/
--rw-r--r--   0 runner    (1001) docker     (127)    54522 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/sed/WDgd71.sed.ext
--rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/sed/o5v.sed.ext
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/tau10.out
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/test_data_registry.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/test_file_names.list
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.970774 lephare-0.1.4/tests/data/vega/
--rwxr-xr-x   0 runner    (1001) docker     (127)    24434 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/vega/SunLCB.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    24455 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/vega/VegaLCB.sed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.970774 lephare-0.1.4/tests/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_cosmology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_data_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_data_retrieval_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_keyword.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_oneElLambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_onesource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_sed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.045221 lephare-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-06 23:48:49.000000 lephare-0.1.5/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-06 23:48:49.000000 lephare-0.1.5/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 23:48:49.000000 lephare-0.1.5/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-06 23:48:49.000000 lephare-0.1.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.005221 lephare-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.005221 lephare-0.1.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.005221 lephare-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/workflows/compile-cpp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-06 23:48:49.000000 lephare-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-06 23:48:49.000000 lephare-0.1.5/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-06 23:48:49.000000 lephare-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-06 23:48:49.000000 lephare-0.1.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-06 23:48:49.000000 lephare-0.1.5/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-06 23:48:49.000000 lephare-0.1.5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-06 23:48:49.000000 lephare-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-06 23:48:56.045221 lephare-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-06 23:48:49.000000 lephare-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.005221 lephare-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.005221 lephare-0.1.5/docs/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (127)   112662 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/doxygen/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/keywords.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/legacy_install.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.009221 lephare-0.1.5/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Building_list_of_onesources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Data_retrieval.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Example_SED_manipulation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Example_cosmo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Example_full_run.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Example_of_usage_of_magSvc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Minimal_photoz_run.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.009221 lephare-0.1.5/docs/notebooks/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/data/COSMOS.para
+-rw-r--r--   0 runner    (1001) docker     (127)    66240 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/data/COSMOS_first100specz.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/data/output.para
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.009221 lephare-0.1.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-05-06 23:48:49.000000 lephare-0.1.5/examples/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39348 2024-05-06 23:48:49.000000 lephare-0.1.5/examples/figuresLPP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31984 2024-05-06 23:48:49.000000 lephare-0.1.5/examples/figuresLPZ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-06 23:48:49.000000 lephare-0.1.5/examples/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-06 23:48:49.000000 lephare-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 23:48:56.045221 lephare-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-06 23:48:49.000000 lephare-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.001221 lephare-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.013221 lephare-0.1.5/src/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/_flt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/_photoz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/filterSvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/magSvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/mag_gal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/sedtolib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/zphota.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.041221 lephare-0.1.5/src/lephare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.017221 lephare-0.1.5/src/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3003 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/PDF.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/PDF.h
+-rw-r--r--   0 runner    (1001) docker     (127)    72115 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/SED.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/SED.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/SEDLib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/SEDLib.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/_bindings.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/cosmology.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/cosmology.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/ext.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/ext.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/ext_curv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/filter_extinc.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20186 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/flt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/flt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/globals.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/globals.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/keyword.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/keyword.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31598 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/mag.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/mag.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/mag_gal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/oneElLambda.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/oneElLambda.h
+-rw-r--r--   0 runner    (1001) docker     (127)    80072 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/onesource.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/onesource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/opa.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/opa.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61669 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/photoz_lib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/photoz_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/sedtolib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/zphota.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.017221 lephare-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.021221 lephare-0.1.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/alloutputkeys.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41606 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/calzetti.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.021221 lephare-0.1.5/tests/data/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/examples/COSMOS.para
+-rw-r--r--   0 runner    (1001) docker     (127)    66240 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/examples/COSMOS_first100specz.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/examples/output.para
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.021221 lephare-0.1.5/tests/data/ext/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   104052 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/ext/MW_seaton.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72411 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/ext/SB_calzetti.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.001221 lephare-0.1.5/tests/data/filt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.021221 lephare-0.1.5/tests/data/filt/subaru/
+-rw-r--r--   0 runner    (1001) docker     (127)    25919 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/filt/subaru/IB527.pb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.037221 lephare-0.1.5/tests/data/opa/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1134 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/OPACITY.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau00.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau01.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau02.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau03.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau04.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau05.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau06.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau07.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau08.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau09.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau10.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau11.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau12.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau13.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau14.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau15.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau16.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau17.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau18.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau19.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau20.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau21.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau22.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau23.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau24.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau25.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau26.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau27.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau28.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau29.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau30.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau31.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau32.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau33.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau34.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau35.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau36.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau37.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau38.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau39.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau40.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau41.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau42.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau43.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau44.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau45.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau46.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau47.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau48.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau49.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau50.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau51.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau52.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau53.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau54.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau55.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau56.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau57.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau58.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau59.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau60.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau61.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau62.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau63.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau64.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau65.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau66.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau67.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau68.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau69.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau70.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau71.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau72.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau73.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau74.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau75.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau76.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau77.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau78.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau79.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau80.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.037221 lephare-0.1.5/tests/data/sed/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.037221 lephare-0.1.5/tests/data/sed/GAL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.037221 lephare-0.1.5/tests/data/sed/GAL/BETHERMIN12/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/GAL/BETHERMIN12/BETHERMIN12_MOD.list
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/GAL/BETHERMIN12/sed_z1_MS.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/GAL/ONE_SED.list
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/GAL/o5v.sed.ext
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.037221 lephare-0.1.5/tests/data/sed/QSO/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/QSO/ONE_SED.list
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/QSO/o5v.sed.ext
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.037221 lephare-0.1.5/tests/data/sed/STAR/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/STAR/ONE_SED.list
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/STAR/o5v.sed.ext
+-rw-r--r--   0 runner    (1001) docker     (127)    54522 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/WDgd71.sed.ext
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/o5v.sed.ext
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/tau10.out
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/test_data_registry.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/test_file_names.list
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.041221 lephare-0.1.5/tests/data/vega/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1592 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/vega/BD+17.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3957 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/vega/BD+17o4708.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24434 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/vega/SunLCB.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24455 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/vega/VegaLCB.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   100244 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/vega/a0v.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    93156 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/vega/a0v_n.sed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.041221 lephare-0.1.5/tests/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_data_retrieval_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_oneElLambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_onesource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_sed.py
```

### Comparing `lephare-0.1.4/.copier-answers.yml` & `lephare-0.1.5/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.gitattributes` & `lephare-0.1.5/.gitattributes`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md` & `lephare-0.1.5/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md` & `lephare-0.1.5/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.github/pull_request_template.md` & `lephare-0.1.5/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.github/workflows/build-documentation.yml` & `lephare-0.1.5/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.github/workflows/compile-cpp.yml` & `lephare-0.1.5/.github/workflows/compile-cpp.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.github/workflows/pre-commit-ci.yml` & `lephare-0.1.5/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.github/workflows/publish-to-pypi.yml` & `lephare-0.1.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.github/workflows/smoke-test.yml` & `lephare-0.1.5/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.github/workflows/testing-and-coverage.yml` & `lephare-0.1.5/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.gitignore` & `lephare-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.pre-commit-config.yaml` & `lephare-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.readthedocs.yml` & `lephare-0.1.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/.setup_dev.sh` & `lephare-0.1.5/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/CMakeLists.txt` & `lephare-0.1.5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/LICENSE` & `lephare-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/PKG-INFO` & `lephare-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lephare
-Version: 0.1.4
+Version: 0.1.5
 Summary: LEPHARE photometric redshift estimator
 Home-page: https://gitlab.lam.fr/Galaxies/LEPHARE
 Author: Johann Cohen-Tanugi
 Author-email: Stéphane Arnouts <stephane.arnouts@lam.fr>, Olivier Ilbert <olivier.ilbert@lam.fr>, Johann Cohen-Tanugi <johann.cohen-tanugi@in2p3.fr>, Raphael Shirley <rshirley@mpe.mpg.de>
 License: MIT License
         
         Copyright (c) 2023 Johann Cohen-Tanugi
```

### Comparing `lephare-0.1.4/README.md` & `lephare-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/Makefile` & `lephare-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/conf.py` & `lephare-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/doxygen/Doxyfile` & `lephare-0.1.5/docs/doxygen/Doxyfile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/index.rst` & `lephare-0.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/keywords.rst` & `lephare-0.1.5/docs/keywords.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/legacy_install.rst` & `lephare-0.1.5/docs/legacy_install.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/notebooks/Building_list_of_onesources.ipynb` & `lephare-0.1.5/docs/notebooks/Building_list_of_onesources.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/notebooks/Data_retrieval.ipynb` & `lephare-0.1.5/docs/notebooks/Data_retrieval.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/notebooks/Example_SED_manipulation.ipynb` & `lephare-0.1.5/docs/notebooks/Example_SED_manipulation.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/notebooks/Example_cosmo.ipynb` & `lephare-0.1.5/docs/notebooks/Example_cosmo.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/notebooks/Example_full_run.ipynb` & `lephare-0.1.5/docs/notebooks/Example_full_run.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/notebooks/Example_of_usage_of_magSvc.ipynb` & `lephare-0.1.5/docs/notebooks/Example_of_usage_of_magSvc.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/notebooks/README.md` & `lephare-0.1.5/docs/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb` & `lephare-0.1.5/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/notebooks/data/COSMOS.para` & `lephare-0.1.5/docs/notebooks/data/COSMOS.para`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/docs/notebooks/data/output.para` & `lephare-0.1.5/docs/notebooks/data/output.para`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/examples/color.py` & `lephare-0.1.5/examples/color.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/examples/figuresLPP.py` & `lephare-0.1.5/examples/figuresLPP.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/examples/figuresLPZ.py` & `lephare-0.1.5/examples/figuresLPZ.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/examples/spec.py` & `lephare-0.1.5/examples/spec.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/pyproject.toml` & `lephare-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,20 @@
     "astropy",
     "scipy",
     "requests",
     "pooch",
     "platformdirs",
 ]
 
+[project.scripts]
+filter = "lephare.filter:main"
+sedtolib = "lephare.sedtolib:main"
+mag_gal = "lephare.mag_gal:main"
+zphota = "lephare.zphota:main"
+
 [project.urls]
 "Source Code" = "https://github.com/lincc-frameworks/lephare"
 
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
 dev = [
     "jupyter", # Clears output from Jupyter notebooks
```

### Comparing `lephare-0.1.4/setup.py` & `lephare-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lephare/__init__.py` & `lephare-0.1.5/src/lephare/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,9 +22,11 @@
 from ._photoz import *
 from ._spec import *
 from .data_retrieval import *
 from .filter import *
 from .filterSvc import *
 from .mag_gal import *
 from .magSvc import *
+from .prepare import *
+from .process import *
 from .sedtolib import *
 from .zphota import *
```

### Comparing `lephare-0.1.4/src/lephare/_flt.py` & `lephare-0.1.5/src/lephare/_flt.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lephare/_pdf.py` & `lephare-0.1.5/src/lephare/_pdf.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lephare/_photoz.py` & `lephare-0.1.5/src/lephare/_photoz.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lephare/_spec.py` & `lephare-0.1.5/src/lephare/_spec.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lephare/_utils.py` & `lephare-0.1.5/src/lephare/_utils.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lephare/data_manager.py` & `lephare-0.1.5/src/lephare/data_manager.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lephare/data_retrieval.py` & `lephare-0.1.5/src/lephare/data_retrieval.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lephare/filter.py` & `lephare-0.1.5/src/lephare/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,11 +63,15 @@
             one_filt = flt(k, f, t, c)
             one_filt.read(flt_file)
             vec_flt.append(one_filt)
 
         write_output_filter(filtfile, filtdoc, vec_flt)
 
 
-if __name__ == "__main__":
+def main():
     runner = Filter()
     runner.run()
     runner.end()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `lephare-0.1.4/src/lephare/filterSvc.py` & `lephare-0.1.5/src/lephare/filterSvc.py`

 * *Files 11% similar despite different names*

```diff
@@ -216,7 +216,41 @@
         # avoid exposing trans and clean methods.
         flt_obj = flt(counter, "./" + name, trans_type, 0)
         # flt_obj.read("dummy")
         os.remove(name)
         # save the SVO additional info in an instance property
         flt_obj.svo_params = param_dict
         return flt_obj
+
+    @classmethod
+    def from_keymap(cls, keymap):
+        """Load filter from a config keymap.
+
+        Parameters
+        ----------
+        keymap : dict of lephare.keyword
+            The config keymap
+
+        Returns
+        -------
+        flt_array : list of `lephare.flt`
+            List of filters.
+        """
+        keymap["FILTER_REP"].value = keymap["FILTER_REP"].value.replace("$LEPHAREDIR", LEPHAREDIR)
+
+        filter_list = keymap["FILTER_LIST"].value.split(",")
+        filter_calib = keymap["FILTER_CALIB"].value.split(",")
+        filter_trans = keymap["TRANS_TYPE"].value.split(",")
+        if len(filter_trans) == 1:
+            filter_trans = len(filter_list) * filter_trans
+        elif len(filter_trans) != len(filter_list):
+            raise RuntimeError("FILTER_LIST and FILTER_TRANS do not have the same size")
+        if len(filter_calib) == 1:
+            filter_calib = len(filter_list) * filter_calib
+        elif len(filter_calib) != len(filter_list):
+            raise RuntimeError("FILTER_LIST and FILTER_CALIB do not have the same size")
+        flt_array = []
+        for i in range(len(filter_list)):
+            name = os.path.join(keymap["FILTER_REP"].value, filter_list[i])
+            oneflt = flt(i, name, int(filter_trans[i]), int(filter_calib[i]))
+            flt_array.append(oneflt)
+        return flt_array
```

### Comparing `lephare-0.1.4/src/lephare/magSvc.py` & `lephare-0.1.5/src/lephare/magSvc.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lephare/mag_gal.py` & `lephare-0.1.5/src/lephare/mag_gal.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,11 +93,15 @@
         # be called within a python session that stays alive afterwards
         mag.close_files()
 
         self.Mag = mag
         return
 
 
-if __name__ == "__main__":
+def main():
     runner = MagGal()
     runner.run()
     runner.end()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `lephare-0.1.4/src/lephare/runner.py` & `lephare-0.1.5/src/lephare/runner.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lephare/sedtolib.py` & `lephare-0.1.5/src/lephare/sedtolib.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "AGE_RANGE",
     "QSO_SED",
     "QSO_FSCALE",
     "QSO_LIB",
     "STAR_SED",
     "STAR_LIB",
     "STAR_FSCALE",
+    "LIB_ASCII",
 ]
 
 
 class Sedtolib(Runner):
     """Read a configurable set of SED, compute extinction corrections, and store the
     results into a binary library for later use.
 
@@ -81,11 +82,15 @@
         # be called within a python session that stays alive afterwards
         sed_library.close_output_files()
 
         self.SEDLib = sed_library
         return
 
 
-if __name__ == "__main__":
+def main():
     runner = Sedtolib()
     runner.run()
     runner.end()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `lephare-0.1.4/src/lephare/zphota.py` & `lephare-0.1.5/src/lephare/zphota.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "INP_TYPE",
     "CAT_MAG",
     "CAT_FMT",
     "CAT_LINES",
     "ZPHOTLIB",
     "PARA_OUT",
     "CAT_OUT",
+    "VERBOSE",
     "CAT_TYPE",
     "ERR_SCALE",
     "ERR_FACTOR",
     "BD_SCALE",
     "GLB_CONTEXT",
     "FORB_CONTEXT",
     "MASS_SCALE",
@@ -66,15 +67,14 @@
     "ADD_EMLINES",
     "ADDITIONAL_MAG",
     "LIMITS_ZBIN",
     "LIMITS_MAPP_REF",
     "LIMITS_MAPP_SEL",
     "LIMITS_MAPP_CUT",
     "Z_STEP",
-    "VERBOSE",
 ]
 
 nonestring = "NONE"
 
 
 class Zphota(Runner):
     """Performs chisquare minimization in order to derive photometric redshifts and
@@ -102,42 +102,40 @@
             # if k == "config":
             #     self.config = config_file
             #     continue
             if k.upper() in self.keymap:
                 self.keymap[k.upper()] = keyword(k.upper(), str(v))
         self.keymap["c"] = keyword("c", self.config)
 
-        print(self.keymap["Z_STEP"])
-        print(self.keymap["COSMOLOGY"])
-        print(self.keymap["Z_STEP"].split_double("0.1", 3))
-
         photoz = PhotoZ(self.keymap)
-        autoadapt = (self.keymap["AUTO_ADAPT"]).split_string("YES", 1)[0]
-        if autoadapt == "YES":
+        autoadapt = (self.keymap["AUTO_ADAPT"]).split_bool("NO", 1)[0]
+        if autoadapt:
             adapt_srcs = photoz.read_autoadapt_sources()
-            photoz.prep_data(adapt_srcs)
             a0, a1 = photoz.run_autoadapt(adapt_srcs)
             offsets = ",".join(np.array(a0).astype(str))
             offsets = "# Offsets from auto-adapt: " + offsets + "\n"
             photoz.outputHeader += offsets
         else:
             a0 = []
             a1 = []
             for _ in range(photoz.imagm):
                 a0.append(0.0)
                 a1.append(0.0)
 
         opa_out = GalMag.read_opa()  # noqa: F841
 
         fit_srcs = photoz.read_photoz_sources()
-        photoz.prep_data(fit_srcs)
         photoz.run_photoz(fit_srcs, a0, a1)
         photoz.write_outputs(fit_srcs, int(time.time()))
 
     def end(self):
         super().end()
 
 
-if __name__ == "__main__":
+def main():
     runner = Zphota()
     runner.run()
     runner.end()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `lephare-0.1.4/src/lephare.egg-info/PKG-INFO` & `lephare-0.1.5/src/lephare.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lephare
-Version: 0.1.4
+Version: 0.1.5
 Summary: LEPHARE photometric redshift estimator
 Home-page: https://gitlab.lam.fr/Galaxies/LEPHARE
 Author: Johann Cohen-Tanugi
 Author-email: Stéphane Arnouts <stephane.arnouts@lam.fr>, Olivier Ilbert <olivier.ilbert@lam.fr>, Johann Cohen-Tanugi <johann.cohen-tanugi@in2p3.fr>, Raphael Shirley <rshirley@mpe.mpg.de>
 License: MIT License
         
         Copyright (c) 2023 Johann Cohen-Tanugi
```

### Comparing `lephare-0.1.4/src/lib/Makefile` & `lephare-0.1.5/src/lib/Makefile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/PDF.cpp` & `lephare-0.1.5/src/lib/PDF.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/PDF.h` & `lephare-0.1.5/src/lib/PDF.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/SED.cpp` & `lephare-0.1.5/src/lib/SED.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/SED.h` & `lephare-0.1.5/src/lib/SED.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/SEDLib.cpp` & `lephare-0.1.5/src/lib/SEDLib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/SEDLib.h` & `lephare-0.1.5/src/lib/SEDLib.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/_bindings.cc` & `lephare-0.1.5/src/lib/_bindings.cc`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/cosmology.cpp` & `lephare-0.1.5/src/lib/cosmology.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/cosmology.h` & `lephare-0.1.5/src/lib/cosmology.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/ext.cpp` & `lephare-0.1.5/src/lib/ext.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/ext.h` & `lephare-0.1.5/src/lib/ext.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/ext_curv.cpp` & `lephare-0.1.5/src/lib/ext_curv.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/filter.cpp` & `lephare-0.1.5/src/lib/filter.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/filter_extinc.cpp` & `lephare-0.1.5/src/lib/filter_extinc.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/flt.cpp` & `lephare-0.1.5/src/lib/flt.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/flt.h` & `lephare-0.1.5/src/lib/flt.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/globals.cpp` & `lephare-0.1.5/src/lib/globals.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/globals.h` & `lephare-0.1.5/src/lib/globals.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/keyword.cpp` & `lephare-0.1.5/src/lib/keyword.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/keyword.h` & `lephare-0.1.5/src/lib/keyword.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/mag.cpp` & `lephare-0.1.5/src/lib/mag.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/mag.h` & `lephare-0.1.5/src/lib/mag.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/mag_gal.cpp` & `lephare-0.1.5/src/lib/mag_gal.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/oneElLambda.cpp` & `lephare-0.1.5/src/lib/oneElLambda.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/oneElLambda.h` & `lephare-0.1.5/src/lib/oneElLambda.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/onesource.cpp` & `lephare-0.1.5/src/lib/onesource.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/onesource.h` & `lephare-0.1.5/src/lib/onesource.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/opa.cpp` & `lephare-0.1.5/src/lib/opa.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/opa.h` & `lephare-0.1.5/src/lib/opa.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/photoz_lib.cpp` & `lephare-0.1.5/src/lib/photoz_lib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/photoz_lib.h` & `lephare-0.1.5/src/lib/photoz_lib.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/sedtolib.cpp` & `lephare-0.1.5/src/lib/sedtolib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/src/lib/zphota.cpp` & `lephare-0.1.5/src/lib/zphota.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/conftest.py` & `lephare-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/data/calzetti.dat` & `lephare-0.1.5/tests/data/calzetti.dat`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/data/examples/COSMOS.para` & `lephare-0.1.5/tests/data/examples/COSMOS.para`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 ##############################################################################################
 ###########               CREATION OF LIBRARIES FROM SEDs List                   #############
 ########### Run : $ZPHOTDIR/source/sedtolib -t (S/Q/G) -c zphot.para             #############
 ##############################################################################################
 #
 #-------------------    STELLAR LIBRARY (ASCII SEDs)        ---------------------------       
-STAR_SED        STAR_SWIRE.list         # STAR list (full path)
+STAR_SED        sed/STAR/ONE_SED.list         # STAR list (full path)
+#STAR_SED        sed/STAR/STAR_MOD_ALL.list         # STAR list (full path)
 STAR_LIB	LIB_STAR		# Binary STAR LIBRARY (-> $ZPHOTWORK/lib_bin/*)
 STAR_FSCALE	3.432E-09		# Arbitrary Flux Scale 
 #
 #-------------------    QSO LIBRARY (ASCII SEDs)            ---------------------------  
-QSO_SED		AGN_LONSDALE.list       # QSO list (full path)
+QSO_SED		sed/QSO/ONE_SED.list       # QSO list (full path)
+#QSO_SED		sed/QSO/SALVATO09/AGN_MOD.list       # QSO list (full path)
 QSO_LIB		LIB_QSO			# Binary QSO LIBRARY (-> $ZPHOTWORK/lib_bin/*)
 QSO_FSCALE	1.			# Arbitrary Flux Scale 
 #
 #-------------------  GALAXY LIBRARY (ASCII or BINARY SEDs) ---------------------------
-GAL_SED		 CE_MOD.list            # GALAXMuzzin09_SEDY list (full path)
+GAL_SED		 sed/GAL/ONE_SED.list            # GALAXMuzzin09_SEDY list (full path)
+#GAL_SED		 examples/COSMOS_MOD.list            # GALAXMuzzin09_SEDY list (full path)
 GAL_LIB	         LIB_CE	                # Binary GAL LIBRARY (-> $ZPHOTWORK/lib_bin/*)
 GAL_FSCALE      1.                      # Arbitrary Flux Scale
 #SEL_AGE 	/data/zphot_vers25_03_03/sed/GAL/HYPERZ/AGE_GISSEL_HZ.dat	# List of Age for GISSEL(full path)
 AGE_RANGE  0.,15.e9                                     # Age Min-Max in yr
 
+                       
 
 #
 ##############################################################################################
 ###########                          FILTERS                                     #############
 ########### Run : $ZPHOTDIR/source/filter  -c zphot.para                         #############
 ##############################################################################################
 
 # 
 FILTER_REP   $LEPHAREDIR/filt           # Repository in which the filters are stored
-FILTER_LIST   subaru/IB527.pb
+FILTER_LIST   subaru/IB527.pb 
 # FILTER_LIST   cosmos/u_cfht.lowres,cosmos/u_new.pb,hsc/gHSC.pb,hsc/rHSC.pb,hsc/iHSC.pb,hsc/zHSC.pb,hsc/yHSC.pb,vista/Y.lowres,vista/J.lowres,vista/H.lowres,vista/K.lowres,cosmos/IB427.lowres,cosmos/IB464.lowres,cosmos/IB484.lowres,cosmos/IB505.lowres,cosmos/IB527.lowres,cosmos/IB574.lowres,cosmos/IB624.lowres,cosmos/IB679.lowres,cosmos/IB709.lowres,cosmos/IB738.lowres,cosmos/IB767.lowres,cosmos/IB827.lowres,cosmos/NB711.lowres,cosmos/NB816.lowres,vista/NB118.lowres,cosmos/irac_ch1.lowres,cosmos/irac_ch2.lowres,cosmos/irac_ch3.lowres,cosmos/irac_ch4.lowres 
 TRANS_TYPE	 1			# TRANSMISSION TYPE
                                         # 0[-def]: Energy, 1: Nb of photons
 FILTER_CALIB    0
 					# 0[-def]:  fnu=ctt 
                                         # 1      :  nu.fnu=ctt 
                                         # 2      :  fnu=nu 
@@ -59,15 +63,15 @@
 #-------------------      From GALAXY LIBRARY            ------------------------------
 GAL_LIB_IN	LIB_CE 	        # Input GALAXY LIBRARY   (in $ZPHOTWORK/lib_bin/*)
 GAL_LIB_OUT	CE_COSMOS	# Output GALAXY LIBRARY  (-> $ZPHOTWORK/lib_mag/*) 
 #
 #------------------   MAG + Z_STEP + COSMO + EXTINCTION   -----------------------------
 MAGTYPE         AB		# Magnitude type (AB or VEGA)
 ZGRID_TYPE      0               # Define the kind of redshift grid (0: linear ; 1: dz*(1+z)) 
-Z_STEP 		0.01,0.,7. 	# dz, zmin, zmax 
+Z_STEP 		0.1,0.,5. 	# dz, zmin, zmax 
 COSMOLOGY	70,0.3,0.7	# H0,om0,lbd0    (if lb0>0->om0+lbd0=1)
 MOD_EXTINC 	0,0		# model range for extinction 
 EXTINC_LAW	SB_calzetti.dat	# ext. law (in  $ZPHOTDIR/ext/*)
 EB_V            0.,0.05,0.1,0.15,0.2,0.25,0.3,0.35,0.4,0.5 # E(B-V) (<50 values)
 EM_LINES        EMP_UV          # [NO/EMP_UV/EMP_SFR/PHYS] choice between emission line prescription  
 EM_DISPERSION   0.5,0.75,1.,1.5,2. # Dispersion allowed in the emission line flux factor
 ADD_DUSTEM      NO               # Add the dust emission in templates when missing 
@@ -88,15 +92,15 @@
 CAT_MAG         AB               # Input Magnitude (AB or VEGA)
 CAT_FMT         MEME  	         # MEME: (Mag,Err)i  
   		                 # MMEE: (Mag)i,(Err)i  
 CAT_LINES       0,1000000000     #  MIN and MAX RANGE of ROWS used in input cat [def:-99,-99]
 CAT_TYPE	LONG	  	 # Input Format    (LONG,SHORT-def)
 GLB_CONTEXT	0		 # Overwrite Context (Sum 2^n; n=0->nbd-1, 0->all bands, -1[-def] used context per object) 
 FORB_CONTEXT	-1		 # Not consider these filters in the fit  (Sum 2^n; n=0->nbd-1) 
-ERR_SCALE       0.02,0.02,0.02,0.02,0.02,0.02,0.02,0.05,0.05,0.05,0.05,0.02,0.02,0.02,0.02,0.02,0.02,0.02,0.02,0.02,0.02,0.02,0.02,0.05,0.05,0.05,0.05,0.1,0.2,0.3  # Systematic errors per band
+ERR_SCALE       0.02 # Systematic errors per band
 ERR_FACTOR      1.5              # Multiply all the flux uncertainties by this factor
 ADD_EMLINES     0,10000          # Range of template in which we add emission lines
 
 #
 #------------------    Theoretical libraries           --------------------------------
 ZPHOTLIB	CE_COSMOS,STAR_COSMOS,QSO_COSMOS  # Library used for Chi2 (max:3)
 
@@ -115,15 +119,15 @@
 #--------------------  Checks  -----------------------------------------------------
 RM_DISCREPANT_BD 500             # Threshold in chi2 to consider. Remove <3 bands, stop when below this chi2 threshold  
 
 #
 #------------------      Priors                       --------------------------------- 
 MAG_ABS 	-24,-5  	# Mabs_min , Mabs_max [0,0-def]
 MAG_ABS_QSO 	-30,-10  	# Mabs_min , Mabs_max for QSO library [0,0-def]
-MAG_REF 	3		# Reference number for band used by Mag_abs
+MAG_REF 	1		# Reference number for band used by Mag_abs
 Z_RANGE        0.,99.99          # Z min-max used for the Galaxy library 
 EBV_RANGE      0,9               # E(B-V) MIN-MAX RANGE of E(B-V) used  
 #NZ_PRIOR       4,5                # I Band for prior on N(z), the second number is the band to be used if the first is missing.
 
 #
 #------------------  Fixed Z   (need format LONG for input Cat)  ----------------------
 ZFIX		NO		# fixed z and search best model  [YES,NO-def]
@@ -158,15 +162,15 @@
                                  # used only if number of shifts matches
                                  # with number of filters in the library    
 
 #
 #-------------------   ADAPTIVE METHOD using Z spectro sample -----------------
 #
 AUTO_ADAPT	NO		 # Adapting method with spectro [NO-def]
-ADAPT_BAND 	5		 # Reference band, band1, band2 for color 
+ADAPT_BAND 	1		 # Reference band, band1, band2 for color 
 ADAPT_LIM       1.5,23.0         # Mag limits for spectro in Ref band [18,21.5-def]
 ADAPT_CONTEXT  -1                # Context for bands used for training
                                  # If -1[-def] the ones given by the normal context
 ADAPT_ZBIN     0.01,6            # Redshift's interval used for training
                                  # [0.001,6-Def]
 ADAPT_MODBIN   1,1000            # Model's interval    used for training
                                  # [1,1000-Def]
```

### Comparing `lephare-0.1.4/tests/data/filt/subaru/IB527.pb` & `lephare-0.1.5/tests/data/filt/subaru/IB527.pb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/data/sed/WDgd71.sed.ext` & `lephare-0.1.5/tests/data/sed/WDgd71.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/data/sed/o5v.sed.ext` & `lephare-0.1.5/tests/data/sed/GAL/o5v.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/data/tau10.out` & `lephare-0.1.5/tests/data/opa/tau10.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/data/vega/SunLCB.sed` & `lephare-0.1.5/tests/data/vega/SunLCB.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/data/vega/VegaLCB.sed` & `lephare-0.1.5/tests/data/vega/VegaLCB.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/lephare/test_cosmology.py` & `lephare-0.1.5/tests/lephare/test_cosmology.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/lephare/test_data_manager.py` & `lephare-0.1.5/tests/lephare/test_data_manager.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/lephare/test_data_retrieval.py` & `lephare-0.1.5/tests/lephare/test_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/lephare/test_data_retrieval_registry.py` & `lephare-0.1.5/tests/lephare/test_data_retrieval_registry.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/lephare/test_filter.py` & `lephare-0.1.5/tests/lephare/test_filter.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/lephare/test_keyword.py` & `lephare-0.1.5/tests/lephare/test_keyword.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/lephare/test_oneElLambda.py` & `lephare-0.1.5/tests/lephare/test_oneElLambda.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/lephare/test_onesource.py` & `lephare-0.1.5/tests/lephare/test_onesource.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.4/tests/lephare/test_sed.py` & `lephare-0.1.5/tests/lephare/test_sed.py`

 * *Files identical despite different names*

