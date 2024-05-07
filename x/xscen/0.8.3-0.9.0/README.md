# Comparing `tmp/xscen-0.8.3.tar.gz` & `tmp/xscen-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xscen-0.8.3.tar", last modified: Wed Feb 28 15:26:32 2024, max compression
+gzip compressed data, was "xscen-0.9.0.tar", last modified: Tue May  7 19:23:24 2024, max compression
```

## Comparing `xscen-0.8.3.tar` & `xscen-0.9.0.tar`

### file list

```diff
@@ -1,105 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.094024 xscen-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-02-28 15:26:18.000000 xscen-0.8.3/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-28 15:26:18.000000 xscen-0.8.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    32857 2024-02-28 15:26:18.000000 xscen-0.8.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-02-28 15:26:18.000000 xscen-0.8.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    12179 2024-02-28 15:26:18.000000 xscen-0.8.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-28 15:26:18.000000 xscen-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-28 15:26:18.000000 xscen-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-02-28 15:26:18.000000 xscen-0.8.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-02-28 15:26:32.094024 xscen-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-02-28 15:26:18.000000 xscen-0.8.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-02-28 15:26:18.000000 xscen-0.8.3/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.070024 xscen-0.8.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.062024 xscen-0.8.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.070024 xscen-0.8.3/docs/_static/_images/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/_static/_images/xscen-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/_static/_images/xscen-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/columns.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     8626 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/goodtoknow.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.074024 xscen-0.8.3/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    43387 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/notebooks/1_catalog.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    60514 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/notebooks/2_getting_started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18362 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/notebooks/3_diagnostics.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/notebooks/4_ensembles.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20154 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/notebooks/5_warminglevels.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13575 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/notebooks/6_config.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/notebooks/global_tas_average_obs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/notebooks/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.074024 xscen-0.8.3/docs/notebooks/samples/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/notebooks/samples/indicators.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11432 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/notebooks/samples/pangeo-cmip6.csv
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/notebooks/samples/pangeo-cmip6.json
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/notebooks/samples/properties.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/security.rst
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-28 15:26:18.000000 xscen-0.8.3/docs/templates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-02-28 15:26:18.000000 xscen-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-28 15:26:18.000000 xscen-0.8.3/requirements_upstream.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-28 15:26:32.094024 xscen-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-28 15:26:18.000000 xscen-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.078024 xscen-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-28 15:26:18.000000 xscen-0.8.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    25202 2024-02-28 15:26:18.000000 xscen-0.8.3/tests/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-02-28 15:26:18.000000 xscen-0.8.3/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-02-28 15:26:18.000000 xscen-0.8.3/tests/test_catutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18080 2024-02-28 15:26:18.000000 xscen-0.8.3/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    43493 2024-02-28 15:26:18.000000 xscen-0.8.3/tests/test_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-02-28 15:26:18.000000 xscen-0.8.3/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-02-28 15:26:18.000000 xscen-0.8.3/tests/test_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-02-28 15:26:18.000000 xscen-0.8.3/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-02-28 15:26:18.000000 xscen-0.8.3/tests/test_regrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-02-28 15:26:18.000000 xscen-0.8.3/tests/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-02-28 15:26:18.000000 xscen-0.8.3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.082024 xscen-0.8.3/xscen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.086024 xscen-0.8.3/xscen/CVs/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/CVs/frequency_to_timedelta.json
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/CVs/frequency_to_xrfreq.json
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/CVs/infer_resolution.json
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/CVs/resampling_methods.json
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/CVs/variable_names.json
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/CVs/xrfreq_to_frequency.json
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/CVs/xrfreq_to_timedelta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47875 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11221 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/biasadjust.py
--rw-r--r--   0 runner    (1001) docker     (127)    38431 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    45168 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/catutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.086024 xscen-0.8.3/xscen/data/
--rw-r--r--   0 runner    (1001) docker     (127)   649378 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/data/IPCC_annual_global_tas.nc
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/data/file_schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.062024 xscen-0.8.3/xscen/data/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.086024 xscen-0.8.3/xscen/data/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-02-28 15:26:24.000000 xscen-0.8.3/xscen/data/fr/LC_MESSAGES/xscen.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/data/fr/LC_MESSAGES/xscen.po
--rw-r--r--   0 runner    (1001) docker     (127)    23019 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    32997 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/ensembles.py
--rw-r--r--   0 runner    (1001) docker     (127)    70096 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)    34617 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/regrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/scripting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    51976 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.090024 xscen-0.8.3/xscen/xclim_modules/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/xclim_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/xclim_modules/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-02-28 15:26:18.000000 xscen-0.8.3/xscen/xclim_modules/conversions.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:26:32.090024 xscen-0.8.3/xscen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-02-28 15:26:31.000000 xscen-0.8.3/xscen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-02-28 15:26:32.000000 xscen-0.8.3/xscen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 15:26:31.000000 xscen-0.8.3/xscen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-28 15:26:31.000000 xscen-0.8.3/xscen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-28 15:26:31.000000 xscen-0.8.3/xscen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.433730 xscen-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-07 19:23:13.000000 xscen-0.9.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-07 19:23:13.000000 xscen-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    36131 2024-05-07 19:23:13.000000 xscen-0.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-07 19:23:13.000000 xscen-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-05-07 19:23:13.000000 xscen-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 19:23:13.000000 xscen-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-07 19:23:13.000000 xscen-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-07 19:23:13.000000 xscen-0.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-07 19:23:24.433730 xscen-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-07 19:23:13.000000 xscen-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-07 19:23:13.000000 xscen-0.9.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.409730 xscen-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.401730 xscen-0.9.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.409730 xscen-0.9.0/docs/_static/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/_static/_images/xscen-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/_static/_images/xscen-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/columns.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8599 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/goodtoknow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.413730 xscen-0.9.0/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    42663 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/notebooks/1_catalog.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    60613 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/notebooks/2_getting_started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18525 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/notebooks/3_diagnostics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/notebooks/4_ensembles.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20205 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/notebooks/5_warminglevels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13000 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/notebooks/6_config.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/notebooks/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.413730 xscen-0.9.0/docs/notebooks/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/notebooks/samples/indicators.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11432 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/notebooks/samples/pangeo-cmip6.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/notebooks/samples/pangeo-cmip6.json
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/notebooks/samples/properties.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/security.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 19:23:13.000000 xscen-0.9.0/docs/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-05-07 19:23:13.000000 xscen-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 19:23:13.000000 xscen-0.9.0/requirements_upstream.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.413730 xscen-0.9.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    14992 2024-05-07 19:23:13.000000 xscen-0.9.0/scripts/global_tas_average_obs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-07 19:23:24.433730 xscen-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-07 19:23:13.000000 xscen-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.417730 xscen-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25202 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_biasadjust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_catutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18080 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45474 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19730 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-07 19:23:13.000000 xscen-0.9.0/tests/test_xclimmod_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.421730 xscen-0.9.0/xscen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.425730 xscen-0.9.0/xscen/CVs/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/CVs/frequency_to_timedelta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/CVs/frequency_to_xrfreq.json
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/CVs/infer_resolution.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/CVs/resampling_methods.json
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/CVs/variable_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/CVs/xrfreq_to_frequency.json
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/CVs/xrfreq_to_timedelta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47875 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/biasadjust.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38511 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45122 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/catutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.425730 xscen-0.9.0/xscen/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   649378 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/data/IPCC_annual_global_tas.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/data/file_schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.401730 xscen-0.9.0/xscen/data/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.429730 xscen-0.9.0/xscen/data/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-07 19:23:21.000000 xscen-0.9.0/xscen/data/fr/LC_MESSAGES/xscen.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/data/fr/LC_MESSAGES/xscen.po
+-rw-r--r--   0 runner    (1001) docker     (127)    23287 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36316 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68987 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35090 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52884 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.429730 xscen-0.9.0/xscen/xclim_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/xclim_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/xclim_modules/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-07 19:23:13.000000 xscen-0.9.0/xscen/xclim_modules/conversions.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:23:24.429730 xscen-0.9.0/xscen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-07 19:23:24.000000 xscen-0.9.0/xscen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-07 19:23:24.000000 xscen-0.9.0/xscen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:23:24.000000 xscen-0.9.0/xscen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-07 19:23:24.000000 xscen-0.9.0/xscen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 19:23:24.000000 xscen-0.9.0/xscen.egg-info/top_level.txt
```

### Comparing `xscen-0.8.3/.zenodo.json` & `xscen-0.9.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/AUTHORS.rst` & `xscen-0.9.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/CHANGES.rst` & `xscen-0.9.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,54 @@
 =========
 Changelog
 =========
 
+v0.9.0 (2024-05-07)
+-------------------
+Contributors to this version: Trevor James Smith (:user:`Zeitsperre`), Pascal Bourgault (:user:`aulemahal`), Gabriel Rondeau-Genesse (:user:`RondeauG`), Juliette Lavoie (:user:`juliettelavoie`), Marco Braun (:user:`vindelico`).
+
+New features and enhancements
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+* ``xs.reduce_ensemble`` will now call ``xclim.ensembles.create_ensemble`` and ``xclim.ensembles.make_critera`` if required. (:pull:`386`).
+
+Breaking changes
+^^^^^^^^^^^^^^^^
+* Removed support for the old instances of the `region` argument in ``spatial_mean``, ``extract_dataset``, and ``subset``. (:pull:`367`).
+* Removed ``xscen.extract.clisops_subset``. (:pull:`367`).
+* ``dtr`` (the function) was renamed to ``dtr_from_minmax`` to avoid confusion with the `dtr` variable. (:pull:`372`).
+* The ``xscen.reduce`` module has been abandoned. (:pull:`386`).
+    * ``build_reduction_data`` has been made redundant by ``xclim.ensembles.make_critera`` and will be removed in a future release.
+    * ``xscen.reduce.reduce_ensemble`` has been moved to ``xscen.ensembles.reduce_ensemble``, as a module was no longer necessary.
+
+Internal changes
+^^^^^^^^^^^^^^^^
+* Modified ``xscen.utils.change_unit`` to always adopt the name from the `variables_and_units dictionary` if the physical units are equal but their names are not (ex. degC <-> ˚C) (:pull:`373`).
+* Updated the `cookiecutter` template to the latest version. (:pull:`358`):
+    * Addresses a handful of misconfigurations in the GitHub Workflows.
+    * Added a few free `grep`-based hooks for finding unwanted artifacts in the code base.
+    * Updated `ruff` to v0.2.0 and `black` to v24.2.0.
+* Added more tests. (:pull:`366`, :pull:`367`, :pull:`372`).
+* Refactored ``xs.spatial.subset`` into smaller functions. (:pull:`367`).
+* An `encoding` argument was added to ``xs.config.load_config``. (:pull:`370`).
+* Various small fixes to the code to address FutureWarnings. (:pull:`380`).
+* ``xs.spatial.subset`` will try to guess CF coordinate if it can't find "latitude" or "longitude" in ``ds.cf``. (:pull:`384`).
+* ``xs.extract_dataset`` and ``xs.DataCatalog.to_dataset`` will now default to opening datasets with option ``chunks={}``, which tries to respect chunking on disk. (:pull:`398`, :issue:`368`).
+
+Bug fixes
+^^^^^^^^^
+* Fix ``unstack_dates`` for the new frequency syntax introduced by pandas v2.2. (:pull:`359`).
+* ``subset_warming_level`` will not return partial subsets if the warming level is reached at the end of the timeseries. (:issue:`360`, :pull:`359`).
+* Loading of training in `adjust` is now done outside of the periods loop. (:pull:`366`).
+* Fixed bug for adding the preprocessing attributes inside the `adjust` function. (:pull:`366`).
+* Fixed a bug to accept `group = False` in `adjust` function. (:pull:`366`).
+* `creep_weights` now correctly handles the case where the grid is small, `n` is large, and `mode=wrap`. (:issue:`367`).
+* Fixed a bug in ``tasmin_from_dtr`` and ``tasmax_from_dtr``, when `dtr` units differed from tasmin/max. (:pull:`372`).
+* Fixed a bug where the requested chunking would be ignored when saving a dataset (:pull:`379`).
+* The missing value check in ``health_checks`` will no longer crasg if a variable has no time dimension. (:pull:`382`).
+
 v0.8.3 (2024-02-28)
 -------------------
 Contributors to this version: Juliette Lavoie (:user:`juliettelavoie`), Trevor James Smith (:user:`Zeitsperre`), Gabriel Rondeau-Genesse (:user:`RondeauG`), Pascal Bourgault (:user:`aulemahal`).
 
 Announcements
 ^^^^^^^^^^^^^
 * `xscen` now has a `security disclosure policy <https://github.com/Ouranosinc/xscen/tree/main?tab=security-ov-file#security-ov-file>`_. (:pull:`353`).
```

### Comparing `xscen-0.8.3/CODE_OF_CONDUCT.md` & `xscen-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/CONTRIBUTING.rst` & `xscen-0.9.0/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 The best way to send feedback is to file an issue at https://github.com/Ouranosinc/xscen/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
+  are welcome. :)
 
 Get Started!
 ------------
 
 .. note::
 
     If you are new to using GitHub and `git`, please read `this guide <https://guides.github.com/activities/hello-world/>`_ first.
@@ -200,15 +200,15 @@
 
 #. The pull request should include tests and should aim to provide `code coverage <https://en.wikipedia.org/wiki/Code_coverage>`_ for all new lines of code. You can use the ``--cov-report html --cov xscen`` flags during the call to ``pytest`` to generate an HTML report and analyse the current test coverage.
 
 #. If the pull request adds functionality, the docs should also be updated. Put your new functionality into a function with a docstring, and add the feature to the list in ``README.rst``.
 
 #. The pull request should not break the templates.
 
-#. The pull request should work for Python 3.9, 3.10, and 3.11. Check that the tests pass for all supported Python versions.
+#. The pull request should work for Python 3.9, 3.10, 3.11, and 3.12. Check that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
 
 $ pytest tests.test_xscen
```

### Comparing `xscen-0.8.3/LICENSE` & `xscen-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/MANIFEST.in` & `xscen-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/Makefile` & `xscen-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/PKG-INFO` & `xscen-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xscen
-Version: 0.8.3
+Version: 0.9.0
 Summary: A climate change scenario-building analysis framework, built with xclim/xarray.
 Author-email: Gabriel Rondeau-Genesse <rondeau-genesse.gabriel@ouranos.ca>
 Project-URL: About Ouranos, https://www.ouranos.ca/en/
 Project-URL: Changelog, https://xscen.readthedocs.io/en/stable/changes.html
 Project-URL: Homepage, https://xscen.readthedocs.io/
 Project-URL: Issue tracker, https://github.com/Ouranosinc/xscen/issues
 Project-URL: Source, https://github.com/Ouranosinc/xscen
@@ -41,29 +41,29 @@
 Requires-Dist: intake-esm>=2023.07.07; python_version >= "3.10"
 Requires-Dist: matplotlib
 Requires-Dist: netCDF4
 Requires-Dist: numcodecs
 Requires-Dist: numpy
 Requires-Dist: pandas>=2.2
 Requires-Dist: parse
-Requires-Dist: pyarrow
+Requires-Dist: pyarrow>=10.0.1
 Requires-Dist: pyyaml
 Requires-Dist: rechunker
 Requires-Dist: scipy
 Requires-Dist: shapely>=2.0
 Requires-Dist: sparse
 Requires-Dist: toolz
 Requires-Dist: xarray>=2023.11.0
 Requires-Dist: xclim>=0.48.2
 Requires-Dist: zarr
 Provides-Extra: dev
 Requires-Dist: pip>=23.3.0; extra == "dev"
-Requires-Dist: black==24.2.0; extra == "dev"
+Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: blackdoc==0.3.9; extra == "dev"
-Requires-Dist: bump-my-version>=0.17.1; extra == "dev"
+Requires-Dist: bump-my-version>=0.18.3; extra == "dev"
 Requires-Dist: coverage<8.0.0,>=6.2.2; extra == "dev"
 Requires-Dist: coveralls>=3.3.1; extra == "dev"
 Requires-Dist: flake8-alphabetize>=0.0.21; extra == "dev"
 Requires-Dist: flake8-rst-docstrings>=0.3.0; extra == "dev"
 Requires-Dist: flake8>=6.1.0; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
 Requires-Dist: pooch; extra == "dev"
```

### Comparing `xscen-0.8.3/README.rst` & `xscen-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/SECURITY.md` & `xscen-0.9.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/docs/Makefile` & `xscen-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/docs/_static/_images/xscen-logo-small.png` & `xscen-0.9.0/docs/_static/_images/xscen-logo-small.png`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/docs/_static/_images/xscen-logo.png` & `xscen-0.9.0/docs/_static/_images/xscen-logo.png`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/docs/api.rst` & `xscen-0.9.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/docs/columns.rst` & `xscen-0.9.0/docs/columns.rst`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/docs/conf.py` & `xscen-0.9.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 import sys
 import warnings
 from datetime import datetime
 from pathlib import Path
 
 sys.path.insert(0, os.path.abspath(".."))
 if os.environ.get("READTHEDOCS") and "ESMFMKFILE" not in os.environ:
-    # RTD doesn't activate the env, and esmpy depends on a env var set there
+    # RTD doesn't activate the env, and esmpy depends on an env var set there
     # We assume the `os` package is in {ENV}/lib/pythonX.X/os.py
     # See conda-forge/esmf-feedstock#91 and readthedocs/readthedocs.org#4067
     os.environ["ESMFMKFILE"] = str(Path(os.__file__).parent.parent / "esmf.mk")
 
-import xscen  # noqa
-import xarray  # noqa
+import xscen  # noqa: E402,F401
+import xarray  # noqa: E402
 
 xarray.DataArray.__module__ = "xarray"
 xarray.Dataset.__module__ = "xarray"
 
 # -- General configuration ---------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
@@ -177,15 +177,14 @@
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = [
     "_build",
     "Thumbs.db",
     ".DS_Store",
-    "notebooks/global_tas_average_obs.ipynb"
 ]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
```

### Comparing `xscen-0.8.3/docs/goodtoknow.rst` & `xscen-0.9.0/docs/goodtoknow.rst`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/docs/index.rst` & `xscen-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/docs/installation.rst` & `xscen-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/docs/make.bat` & `xscen-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/docs/notebooks/1_catalog.ipynb` & `xscen-0.9.0/docs/notebooks/1_catalog.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9872159090909091%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2'}, 3: {'id': '3'}, 4: {'id': '4'}, 5: "*

 * *            "{'id': '5'}, 6: {'id': '6'}, 7: {'id': '7'}, 8: {'id': '8'}, 9: {'id': '9'}, 10: "*

 * *            "{'id': '10'}, 11: {'id': '11'}, 12: {'id': '12'}, 13: {'id': '13'}, 14: {'id': '14'}, "*

 * *            "15: {'id': '15'}, 16: {'id': '16'}, 17: {'id': '17'}, 18: {'id': '18'}, 19: {'id': "*

 * *            "'19'}, 20: {'id': '20'}, 21: {'id': '21'}, 22: {'id': '22'}, 23: {'id': '23'}, 24: "*

 * *            "{'id':  […]*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "c9ec1e3c",
+            "id": "0",
             "metadata": {},
             "source": [
                 "# Using and understanding Catalogs\n",
                 "\n",
                 "<div class=\"alert alert-info\"> <b>INFO</b>\n",
                 "\n",
                 "Catalogs in `xscen` are built upon Datastores in `intake_esm`. For more information on basic usage, such as the `search()` function, [please consult their documentation](https://intake-esm.readthedocs.io/en/stable/).\n",
@@ -57,15 +57,15 @@
                 "\n",
                 "If an official catalog already exists, it should be opened using `xs.DataCatalog` by pointing it to the JSON file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f25ee70d",
+            "id": "1",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from pathlib import Path\n",
                 "\n",
@@ -77,75 +77,75 @@
                 "\n",
                 "DC = DataCatalog(f\"{Path().absolute()}/samples/pangeo-cmip6.json\")\n",
                 "DC"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "47411b46",
+            "id": "2",
             "metadata": {},
             "source": [
                 "The content of the catalog can be accessed by a call to `df`, which will return a `pandas.DataFrame`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3b3840b5",
+            "id": "3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Access the catalog\n",
                 "DC.df[0:3]"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c28d8c93",
+            "id": "4",
             "metadata": {},
             "source": [
                 "The `unique` function allows listing unique elements for either all the catalog or a subset of columns. It can be called in a few various ways, listed below:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3d04a455",
+            "id": "5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# List all unique elements in the catalog, returns a pandas.Series\n",
                 "DC.unique()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "28f67f2d",
+            "id": "6",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# List all unique elements in a subset of columns, returns a pandas.Series\n",
                 "DC.unique([\"variable\", \"frequency\"])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4ef86a5e",
+            "id": "7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# List all unique elements in a single columns, returns a list\n",
                 "DC.unique(\"id\")[0:5]"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5c5c42f5",
+            "id": "8",
             "metadata": {},
             "source": [
                 "### Basic .search() commands\n",
                 "\n",
                 "The `search` function comes from `intake-esm` and allows searching for specific elements in the catalog's columns. It accepts both wildcards and regular expressions (except for *variable*, which must be exact due to being in *tuples*).\n",
                 "\n",
                 "While regex isn't great at inverse matching (\"does not contain\"), it is possible. Here are a few useful commands:\n",
@@ -164,91 +164,91 @@
                 "\n",
                 "This website can be used to test regex commands: https://regex101.com/"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "67815ad2",
+            "id": "9",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Regex: Find all entries that start with \"ssp\"\n",
                 "print(DC.search(experiment=\"^ssp\").unique(\"experiment\"))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4b7b426f",
+            "id": "10",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Regex: Exclude all entries that start with \"ssp\"\n",
                 "print(DC.search(experiment=\"^(?!ssp).*$\").unique(\"experiment\"))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b45af639",
+            "id": "11",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Regex: Find all experiments except the exact string \"ssp126\"\n",
                 "print(DC.search(experiment=\"^(?!ssp126$).*$\").unique(\"experiment\"))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9aa5aa22",
+            "id": "12",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Wildcard: Find all entries that start with NorESM2\n",
                 "print(DC.search(source=\"NorESM2.*\").unique(\"source\"))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5d8b7995",
+            "id": "13",
             "metadata": {},
             "source": [
                 "Notice that the search function returns everything available that matches some of the criteria."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "29bd4010",
+            "id": "14",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# r1i1p1f1 sftlf is not available\n",
                 "DC.search(\n",
                 "    source=\"NorESM2-MM\",\n",
                 "    experiment=\"historical\",\n",
                 "    member=[\"r1i1p1f1\", \"r2i1p1f1\"],\n",
                 "    variable=[\"sftlf\", \"pr\"],\n",
                 ").df"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8abaa553",
+            "id": "15",
             "metadata": {},
             "source": [
                 "You can restrict your search to only keep entries that matches all the criteria across a list of columns."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "253d4868",
+            "id": "16",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Only returns variables that have all members, source and experiment asked for. In this case, pr, but not sftlf.\n",
                 "DC.search(\n",
                 "    source=\"NorESM2-MM\",\n",
                 "    experiment=\"historical\",\n",
@@ -256,35 +256,35 @@
                 "    variable=[\"sftlf\", \"pr\"],\n",
                 "    require_all_on=[\"variable\"],\n",
                 ").df"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7f27214c-2524-4fb7-9b95-4a384ed13a53",
+            "id": "17",
             "metadata": {},
             "source": [
                 "It is also possible to search for files that intersect a specific time period."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ecda16b2-2d87-495d-b1e1-c2894b83fb1d",
+            "id": "18",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "DC.search(periods=[[\"2016\", \"2017\"]]).unique([\"date_start\", \"date_end\"])"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "aa903092",
+            "id": "19",
             "metadata": {},
             "source": [
                 "### Advanced search: xs.search_data_catalogs\n",
                 "\n",
                 "`search` has multiple notable limitations for more advanced searches:\n",
                 "\n",
                 "- It can't match specific criteria together, such as finding a dataset that would have both 3h precipitation and daily temperature.\n",
@@ -312,15 +312,15 @@
                 "\n",
                 "Let's start by searching for CMIP6 data that has subdaily precipitation, daily minimum temperature and the land fraction data. The main difference compared to searching for reference datasets is that in most cases, `match_hist_and_fut` will be required to match *historical* simulations to their future counterparts. This works for both CMIP5 and CMIP6 nomenclatures."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "97d91cce",
+            "id": "20",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import xscen as xs\n",
                 "\n",
@@ -335,46 +335,46 @@
                 ")\n",
                 "\n",
                 "cat_sim"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "82535e6c",
+            "id": "21",
             "metadata": {},
             "source": [
                 "If required, at this stage, a dataset can be looked at in more details. If we examine the results (look at the 'date_start' and 'date_end' columns), we'll see that it successfully found historical simulations in the *CMIP* activity and renamed both their *activity* and *experiment* to match the future simulations."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a6e5bd7e",
+            "id": "22",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "cat_sim[\"ScenarioMIP_NOAA-GFDL_GFDL-CM4_ssp585_r1i1p1f1_gr1\"].df"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "85ee34fe",
+            "id": "23",
             "metadata": {},
             "source": [
                 "#### Example 2: Restricting results\n",
                 "\n",
                 "The two previous search results were the same simulation, but on 2 different grids (`gr1` and `gr2`). If desired, `restrict_resolution` can be called to choose the finest or coarsest grid."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1958d406",
+            "id": "24",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "variables_and_freqs = {\"tasmin\": \"D\", \"pr\": \"3h\", \"sftlf\": \"fx\"}\n",
                 "other_search_criteria = {\"institution\": [\"NOAA-GFDL\"], \"experiment\": [\"ssp585\"]}\n",
@@ -388,24 +388,24 @@
                 ")\n",
                 "\n",
                 "cat_sim"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "fcd847c0-0ea8-46ad-bc28-9b73edd627bc",
+            "id": "25",
             "metadata": {},
             "source": [
                 "Similarly, if we search for historical NorESM2-MM data, we'll find that it has 3 members. If desired, `restrict_members` can be called to choose a maximum number of realization per model."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6c5ce0fc-2f25-4b55-bf65-5f140f07e331",
+            "id": "26",
             "metadata": {},
             "outputs": [],
             "source": [
                 "variables_and_freqs = {\"tasmin\": \"D\"}\n",
                 "other_search_criteria = {\"source\": [\"NorESM2-MM\"], \"experiment\": [\"historical\"]}\n",
                 "\n",
                 "cat_sim = xs.search_data_catalogs(\n",
@@ -416,24 +416,24 @@
                 ")\n",
                 "\n",
                 "cat_sim"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4fd28f58-5ab7-4d65-8906-2197592c8c94",
+            "id": "27",
             "metadata": {},
             "source": [
                 "Finally, `restrict_warming_level` can be used to be sure that the results either exist in `xscen`'s warming level database (if a boolean), or reach a given warming level."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3300b1d7-e37b-4aa4-991e-99609bb1adea",
+            "id": "28",
             "metadata": {},
             "outputs": [],
             "source": [
                 "variables_and_freqs = {\"tasmin\": \"D\"}\n",
                 "\n",
                 "cat_sim = xs.search_data_catalogs(\n",
                 "    data_catalogs=[f\"{Path().absolute()}/samples/pangeo-cmip6.json\"],\n",
@@ -445,26 +445,26 @@
                 ")\n",
                 "\n",
                 "cat_sim"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6bddc58d",
+            "id": "29",
             "metadata": {},
             "source": [
                 "#### Example 3: Search for data that can be computed from what's available\n",
                 "\n",
                 "`allow_resampling` and `allow_conversion` are powerful search tools to find data that doesn't explicitely exist in the catalog, but that can easily be computed."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9e30951b",
+            "id": "30",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "cat_sim_adv = xs.search_data_catalogs(\n",
                 "    data_catalogs=[f\"{Path().absolute()}/samples/pangeo-cmip6.json\"],\n",
@@ -475,44 +475,44 @@
                 "    allow_conversion=True,\n",
                 ")\n",
                 "cat_sim_adv"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b33b2ad7",
+            "id": "31",
             "metadata": {},
             "source": [
                 "If we examine the SSP5-8.5 results, we'll see that while it failed to find *evspsblpot*, it successfully understood that *tasmin* and *tasmax* can be used to compute it. It also understood that daily *tasmin* and *tasmax* is a valid search result for `{tas: YS}`, since it can be computed first, then aggregated to a yearly frequency."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "29b2d3c5",
+            "id": "32",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "cat_sim_adv[\"ScenarioMIP_NCC_NorESM2-MM_ssp585_r1i1p1f1_gn\"].unique()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "962a3c22-58f4-49c4-94ff-78d9c10bcc85",
+            "id": "33",
             "metadata": {},
             "source": [
                 "It's also possible to search for multiple frequencies at the same time by using a list of xrfreq."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7f79d33d-4687-416a-91e6-d4f37ea5efef",
+            "id": "34",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "cat_sim_adv_multifreq = xs.search_data_catalogs(\n",
                 "    data_catalogs=[f\"{Path().absolute()}/samples/pangeo-cmip6.json\"],\n",
@@ -531,15 +531,15 @@
                 "        \"ScenarioMIP_NCC_NorESM2-MM_ssp585_r1i1p1f1_gn\"\n",
                 "    ]._requested_variable_freqs\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "22b7350a",
+            "id": "35",
             "metadata": {},
             "source": [
                 "#### Derived variables\n",
                 "\n",
                 "The `allow_conversion` argument is built upon `xclim`'s virtual indicators module and `intake-esm`'s [DerivedVariableRegistry](https://ncar.github.io/esds/posts/2021/intake-esm-derived-variables/) in a way that should be seamless to the user. It works by using the methods defined in `xscen/xclim_modules/conversions.yml` to add a registry of *derived* variables that exist virtually through computation methods.\n",
                 "\n",
                 "In the example above, we can see that the search failed to find *evspsblpot* within *NorESM2-MM*, but understood that *tasmin* and *tasmax* could be used to estimate it using `xclim`'s `potential_evapotranspiration`.\n",
@@ -555,57 +555,57 @@
                 "`_requested_variables` should NOT be modified under any circumstance, as it is likely to make `to_dataset_dict()` fail. To add some transparency on which variables have been **requested** and which are the **dependent** ones, `xscen` has added `_requested_variables_true` and `_dependent_variables`. This is very likely to be changed in the future.\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9ee75ffb",
+            "id": "36",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "cat_sim_adv[\"ScenarioMIP_NCC_NorESM2-MM_ssp585_r1i1p1f1_gn\"].derivedcat"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c235a0f7",
+            "id": "37",
             "metadata": {},
             "outputs": [],
             "source": [
                 "print(cat_sim_adv[\"ScenarioMIP_NCC_NorESM2-MM_ssp585_r1i1p1f1_gn\"]._requested_variables)\n",
                 "print(\n",
                 "    f\"Requested: {cat_sim_adv['ScenarioMIP_NCC_NorESM2-MM_ssp585_r1i1p1f1_gn']._requested_variables_true}\"\n",
                 ")\n",
                 "print(\n",
                 "    f\"Dependent: {cat_sim_adv['ScenarioMIP_NCC_NorESM2-MM_ssp585_r1i1p1f1_gn']._dependent_variables}\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "aec5c3fc",
+            "id": "38",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-info\"> <b>INFO</b>\n",
                 "  \n",
                 "`allow_conversion`  currently fails if:\n",
                 "<ul>\n",
                 "<li>The requested DerivedVariable also requires a DerivedVariable itself.</li>\n",
                 "<li>The dependent variables exist at different frequencies (e.g. 'pr @1hr' & 'tas @3hr')</li>\n",
                 "</ul>\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4d80ca03",
+            "id": "39",
             "metadata": {},
             "source": [
                 "## Creating a New Catalog from a Directory\n",
                 "\n",
                 "### Initialisation\n",
                 "\n",
                 "The `create` argument of `ProjectCatalog` can be called to create an empty *ProjectCatalog* and a new set of JSON and CSV files.\n",
@@ -621,15 +621,15 @@
                 "\n",
                 "Other attributes and behaviours of the project definition can be modified in a similar way."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a00a0e85",
+            "id": "40",
             "metadata": {},
             "outputs": [],
             "source": [
                 "project = {\n",
                 "    \"title\": \"tutorial-catalog\",\n",
                 "    \"description\": \"Catalog for the tutorial NetCDFs.\",\n",
                 "}\n",
@@ -641,25 +641,25 @@
                 "    overwrite=True,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "830e119e",
+            "id": "41",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# The metadata is stored in PC.esmcat\n",
                 "PC.esmcat"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9513fc05",
+            "id": "42",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "### Appending new data to a ProjectCatalog\n",
                 "\n",
                 "At this stage, the CSV is still empty. There are two main ways to populate a catalog with data:\n",
@@ -686,15 +686,15 @@
                 "\n",
                 "The following example will search through the samples folder and infer information from the folder names. The filename is ignored, except its extension. The variable name and time bounds are read from the file itself."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "837b89c6",
+            "id": "43",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from xscen.catutils import parse_directory\n",
                 "\n",
                 "df = parse_directory(\n",
                 "    directories=[f\"{Path().absolute()}/samples/tutorial/\"],\n",
@@ -709,15 +709,15 @@
                 "    read_from_file=[\"variable\", \"date_start\", \"date_end\"],\n",
                 ")\n",
                 "df"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bd3b9414",
+            "id": "44",
             "metadata": {},
             "source": [
                 "#### Unique Dataset ID\n",
                 "\n",
                 "In addition to the parse itself, `parse_directory` will create a unique Dataset ID that can be used to easily determine one simulation from another. This can be edited with the `id_columns` argument of `parse_directory`, but by default, IDs are based on CMIP6's ID structure with additions related to regional models and bias adjustment:\n",
                 "\n",
                 "- `{bias_adjust_project} _ {mip_era} _ {activity} _ {driving_model} _ {institution} _ {source} _ {experiment} _ {member} _ {domain}`\n",
@@ -729,46 +729,46 @@
                 "When constructing IDs, empty columns will be skipped.\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "933fa4d2",
+            "id": "45",
             "metadata": {},
             "outputs": [],
             "source": [
                 "df.iloc[0][\"id\"]"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f7d4e420",
+            "id": "46",
             "metadata": {},
             "source": [
                 "#### Appending data using ProjectCatalog.update()\n",
                 "\n",
                 "At this stage, `df` is a `pandas.DataFrame`. `ProjectCatalog.update` is used to append this data to the CSV file and save the results on disk."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e8954662",
+            "id": "47",
             "metadata": {},
             "outputs": [],
             "source": [
                 "PC.update(df)\n",
                 "\n",
                 "PC"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "26c87a7a",
+            "id": "48",
             "metadata": {},
             "source": [
                 "#### More on patterns and advanced features\n",
                 "\n",
                 "The `patterns` argument acts as a reverse format string.\n",
                 "\n",
                 "- The \"\\_\" format specifier (like in `{field:_}` allows matching a name containing underscores for this field. The path separators (/, \\\\) are still excluded. Any format specifier supported by [`parse` are usable](https://github.com/r1chardj0n3s/parse).\n",
@@ -776,15 +776,15 @@
                 "- The `DATES` special field will match single dates or date bounds (see below).\n",
                 "- `{?:_}` is useful in filenames as a \"wildcard\" matching. For exammple: `{?:_}_{DATES}.nc` will read in the last \"element\" of the filename into `date_start` and `date_end`, ignoring all previous parts."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6a40a6ff",
+            "id": "49",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Create fake files for the example:\n",
                 "root = Path(\".\").absolute() / \"_data\" / \"parser_examples\"\n",
                 "root.mkdir(exist_ok=True)\n",
                 "\n",
@@ -802,117 +802,117 @@
                 "    (root / path).parent.mkdir(exist_ok=True, parents=True)\n",
                 "    with (root / path).open(\"w\") as f:\n",
                 "        f.write(\"example\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "27d51ee5",
+            "id": "50",
             "metadata": {},
             "source": [
                 "##### Example 1 - wrong\n",
                 "The `variable` field does not allow underscores, so  the first and last files are not parsed correctly.\n",
                 "\n",
                 "Notice how the `DATES` field was parsed into `date_start` and `date_end`. It also matched with `fx`, returning `NaT` for both fields, as expected."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ece5f91f",
+            "id": "51",
             "metadata": {},
             "outputs": [],
             "source": [
                 "patt = \"{institution}/{source}/{frequency}/{variable}/{?var}_{DATES}.nc\"\n",
                 "parse_directory(directories=[root], patterns=[patt])"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9394cd49",
+            "id": "52",
             "metadata": {},
             "source": [
                 "##### Example 2 - wrong again\n",
                 "We fixed the variable field by allowing underscores. We also modified the filename pattern to match any string, including underscores, except for the last element.\n",
                 "\n",
                 "Notice how the \"1950\" part of `tg_mean` has been converted to `date_start='1950-01-01'` and `date_end='1950-12-31'`.\n",
                 "\n",
                 "The `source` field does not allow underscores, so \"ERA5_v2\" is not parsed correctly. However, what we would want is rather to assign \"v2\" to the version field."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2c73298d",
+            "id": "53",
             "metadata": {},
             "outputs": [],
             "source": [
                 "patt = \"{institution}/{source}/{frequency}/{variable:_}/{?:_}_{DATES}.nc\"\n",
                 "parse_directory(directories=[root], patterns=[patt])"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2ca21395",
+            "id": "54",
             "metadata": {},
             "source": [
                 "##### Example 3 - Correct!\n",
                 "We added a second pattern that includes the `version` field."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d2de72a7",
+            "id": "55",
             "metadata": {},
             "outputs": [],
             "source": [
                 "patts = [\n",
                 "    \"{institution}/{source}_{version}/{frequency}/{variable:_}/{?:_}_{DATES}.nc\",\n",
                 "    \"{institution}/{source}/{frequency}/{variable:_}/{?:_}_{DATES}.nc\",\n",
                 "]\n",
                 "parse_directory(directories=[root], patterns=patts)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6a0fe5e7",
+            "id": "56",
             "metadata": {},
             "source": [
                 "##### Example 4 - Filter on folder names\n",
                 "We can filter the results to include only some folders with the `dirglob` argument."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "503d7709",
+            "id": "57",
             "metadata": {},
             "outputs": [],
             "source": [
                 "parse_directory(directories=[root], patterns=patts, dirglob=\"*/CanESM*\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7fa5110e",
+            "id": "58",
             "metadata": {},
             "source": [
                 "##### Example 5 - Modifying metadata\n",
                 "We use the `cvs` (Controlled VocabularieS) argument here to replace some terms found in the paths by others we prefer.\n",
                 "\n",
                 "Two replacement types are used :\n",
                 " - simple : in the `source` column, all values of \"CanESM-2\" are replaced by \"CanESM2\"\n",
                 " - complex : in the `institution` column, if the value \"MIROC\" is seen, it triggers the setting of \"global\" in this row's `domain` column, overriding whatever was already present in this field."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d905dbcf",
+            "id": "59",
             "metadata": {},
             "outputs": [],
             "source": [
                 "parse_directory(\n",
                 "    directories=[root],\n",
                 "    patterns=patts,\n",
                 "    cvs={\n",
@@ -920,25 +920,25 @@
                 "        \"institution\": {\"MIROC\": {\"domain\": \"global\"}},\n",
                 "    },\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7fd3e489",
+            "id": "60",
             "metadata": {},
             "source": [
                 "##### Example 6 : Even more complex field processing\n",
                 "In the preceding example, we used the `cvs` argument to replace values by others, or to trigger replacements based on values of other columns. The exact value must be matched and map to exact values. Another alternative to transform the parsed fields is to feed a function to the path parsing step. This is done by declaring a new \"type\" to the parser. In the following example, we'll implement a very useless transformation that reverses the letters of the institution."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "039f912f",
+            "id": "61",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from xscen.catutils import register_parse_type\n",
                 "\n",
                 "\n",
                 "@register_parse_type(\"rev\")\n",
@@ -951,113 +951,113 @@
                 "    \"{institution:rev}/{source}/{frequency}/{variable:_}/{?:_}_{DATES}.nc\",\n",
                 "]\n",
                 "parse_directory(directories=[root], patterns=patts_mod)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "431a735c",
+            "id": "62",
             "metadata": {},
             "source": [
                 "### Restructuring catalogued files on disk\n",
                 "\n",
                 "The opposite operation to `parse_directory` is also handled by `xscen.catutils`. In this section, we show how to create a Path from a xscen-extraced dataset or from a catalog entry.\n",
                 "\n",
                 "#### Simple : template string and attributes\n",
                 "Given a dataset that was opened by `xs.extract_dataset` or `DataCatalog.to_dataset()`, we can easily construct a path from the xscen-added attributes."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1eb19f5b",
+            "id": "63",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Open\n",
                 "ds = PC.search(variable=\"tas\", experiment=\"ssp585\").to_dataset()\n",
                 "\n",
                 "path_template = \"{institution}/{source}/{experiment}_{frequency}.nc\"\n",
                 "\n",
                 "print(path_template.format(**xs.utils.get_cat_attrs(ds)))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1b6ccd4e",
+            "id": "64",
             "metadata": {},
             "source": [
                 "While this method is simple, it can't handle neither the list-like `variable` field nor the `date_start` and `date_end` datetime fields.\n",
                 "\n",
                 "#### Complete : build_path\n",
                 "The [`build_path`](../xscen.rst#xscen.catutils.build_path) function has a more complex interface to be used in more complex workflows.\n",
                 "\n",
                 "The default parameters has a pretty good folder structure that depends on the columns `type`  (usually one of simulation, reconstruction or station-obs) and `processing_level` (often raw, biasadjusted or something else)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6b10e67b",
+            "id": "65",
             "metadata": {},
             "outputs": [],
             "source": [
                 "xs.catutils.build_path(ds)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "02d82612",
+            "id": "66",
             "metadata": {},
             "source": [
                 "The folder schema can be passed explictly, as a dictionary with two entries:\n",
                 "- \"folders\" : a list of fields to build the folder hierarchy.\n",
                 "- \"filename\" : a list of fields to build the filename.\n",
                 "\n",
                 "In both cases, a special \"DATES\" field can be given. It will be translated to the most efficient way to write the temporal bounds of the dataset."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "76bc0f37",
+            "id": "67",
             "metadata": {},
             "outputs": [],
             "source": [
                 "custom_schema = {\n",
                 "    \"folders\": [\"type\", \"institution\", \"source\", \"experiment\"],\n",
                 "    \"filename\": [\"variable\", \"DATES\"],\n",
                 "}\n",
                 "xs.catutils.build_path(ds, schemas=custom_schema)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "78f8d562",
+            "id": "68",
             "metadata": {},
             "source": [
                 "The function has more options:\n",
                 "\n",
                 "- A \"root\" folder can be specified\n",
                 "- Other fields can be passed to override those in the data or fill for missing ones."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c3758eda",
+            "id": "69",
             "metadata": {},
             "outputs": [],
             "source": [
                 "xs.catutils.build_path(ds, root=Path(\"/tmp\"), domain=\"REG\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "705a6135",
+            "id": "70",
             "metadata": {},
             "source": [
                 "Above, we called the function with a dataset. In this case, the \"facets\" are extracted from various sources, with this priority (highest at the top):\n",
                 "\n",
                 "1. Facets passed explicitly to `build_path` as keyword arguments\n",
                 "2. Attributes prefixed with \"cat:\"\n",
                 "3. Other Attributes\n",
@@ -1065,52 +1065,52 @@
                 "\n",
                 "But the function can also take a single dataframe row:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d65c8a07",
+            "id": "71",
             "metadata": {},
             "outputs": [],
             "source": [
                 "xs.catutils.build_path(PC.search(variable=\"tas\", experiment=\"ssp585\").df.iloc[0])"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bd529fd2",
+            "id": "72",
             "metadata": {},
             "source": [
                 "Or a full DataFrame/Catalog. In this case, the return value is a DataFrame, copy form the catalog, with a \"new_path\" column added."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5ad9f477",
+            "id": "73",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# We show only three columns of the output catalog\n",
                 "xs.catutils.build_path(PC.search(variable=\"tas\"))[[\"id\", \"path\", \"new_path\"]]"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "20e4678a",
+            "id": "74",
             "metadata": {},
             "source": [
                 "This can be used in a workflow that renames or copies the files to their new name, usually using `shutil`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3296422d",
+            "id": "75",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import shutil as sh\n",
                 "\n",
                 "# Create the destination folder\n",
                 "root = Path(\".\").absolute() / \"_data\" / \"path_builder_examples\"\n",
@@ -1129,15 +1129,15 @@
                 "PC.df[\"path\"] = newdf[\"new_path\"]\n",
                 "PC.update()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c7acfa82-e2e7-42ce-b24e-ab5d4acc6c57",
+            "id": "76",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "@webio": {
```

### Comparing `xscen-0.8.3/docs/notebooks/2_getting_started.ipynb` & `xscen-0.9.0/docs/notebooks/2_getting_started.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.983367935547875%*

 * *Differences: {"'cells'": "{1: {'id': '1'}, 2: {'id': '2', 'source': {insert: [(1, '\\n'), (2, '# A temporary "*

 * *            "bug fix waiting for xclim 0.49\\n'), (3, 'import xclim as xc\\n'), (6, '\\n'), (7, "*

 * *            "'xc.set_options(sdba_encode_cf=False)\\n')]}}, 3: {'id': '3'}, 4: {'id': '4'}, 5: "*

 * *            "{'id': '5'}, 6: {'id': '6'}, 7: {'id': '7'}, 8: {'id': '8'}, 9: {'id': '9'}, 10: "*

 * *            "{'id': '10'}, 11: {'id': '11'}, 12: {'id': '12'}, 13: {'id': '13'}, 14: {'id': '14'}, "*

 * *            "15: {'id' […]*

```diff
@@ -1,12 +1,31 @@
 {
     "cells": [
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "0",
+            "metadata": {
+                "nbsphinx": "hidden"
+            },
+            "outputs": [],
+            "source": [
+                "# Remove flox spam\n",
+                "\n",
+                "import logging\n",
+                "\n",
+                "# Get the logger for the 'flox' package\n",
+                "logger = logging.getLogger(\"flox\")\n",
+                "# Set the logging level to WARNING\n",
+                "logger.setLevel(logging.WARNING)"
+            ]
+        },
+        {
             "cell_type": "markdown",
-            "id": "4f220a85",
+            "id": "1",
             "metadata": {},
             "source": [
                 "# Getting Started\n",
                 "\n",
                 "This Notebook will go through all major steps of creating a climate scenario using `xscen`. These steps are:\n",
                 "\n",
                 "- `search_data_catalogs` to find a subset of datasets that match a given project's requirements.\n",
@@ -24,24 +43,29 @@
                 "\n",
                 "Typically, the first step should be to create a new *ProjectCatalog* to store the files that will be created during the process. More details on basic usage are provided in the Catalogs Notebook."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "892473e9",
+            "id": "2",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from pathlib import Path\n",
                 "\n",
+                "# A temporary bug fix waiting for xclim 0.49\n",
+                "import xclim as xc\n",
+                "\n",
                 "import xscen as xs\n",
                 "\n",
+                "xc.set_options(sdba_encode_cf=False)\n",
+                "\n",
                 "# Folder where to put the data\n",
                 "output_folder = Path().absolute() / \"_data\"\n",
                 "output_folder.mkdir(exist_ok=True)\n",
                 "\n",
                 "project = {\n",
                 "    \"title\": \"example-gettingstarted\",\n",
                 "    \"description\": \"This is an example catalog for xscen's documentation.\",\n",
@@ -53,15 +77,15 @@
                 "    project=project,\n",
                 "    overwrite=True,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4c35d860",
+            "id": "3",
             "metadata": {},
             "source": [
                 "### Searching a subset of datasets within *DataCatalogs*\n",
                 "\n",
                 "<div class=\"alert alert-info\"> <b>INFO</b>\n",
                 "\n",
                 "At this stage, the search criteria should be for variables that will be **bias corrected**, not necessarily the variables required for the final product. For example, if `sfcWindfromdir` is the final product, then `uas` and `vas` should be searched for since these are the variables that will be bias corrected.\n",
@@ -75,15 +99,15 @@
                 "\n",
                 "For the purpose of this tutorial, temperatures and the land fraction from NorESM2-MM will be used:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "eb36f6c9",
+            "id": "4",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "variables_and_freqs = {\"tas\": \"D\", \"sftlf\": \"fx\"}\n",
                 "other_search_criteria = {\n",
@@ -101,35 +125,35 @@
                 ")\n",
                 "\n",
                 "cat_sim"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "65f7dfcc",
+            "id": "5",
             "metadata": {},
             "source": [
                 "The result of `search_data_catalog` is a dictionary with one entry per unique ID. Note that a unique ID can be associated to multiple *intake datasets*, as is the case here, because `intake-esm` groups catalog lines per *id - domain - processing_level - xrfeq*."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9d15968c",
+            "id": "6",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "cat_sim[\"CMIP6_ScenarioMIP_NCC_NorESM2-MM_ssp245_r1i1p1f1_example-region\"].df"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7f7b97b1",
+            "id": "7",
             "metadata": {},
             "source": [
                 "## Extracting data\n",
                 "\n",
                 "<div class=\"alert alert-warning\"> <b>WARNING</b>\n",
                 "\n",
                 "It is heavily recommended to stop and analyse the results of `search_data_catalogs` before proceeding to the extraction function.\n",
@@ -155,15 +179,15 @@
                 "- [shape](https://clisops.readthedocs.io/en/latest/api.html#clisops.core.subset.subset_shape)\n",
                 "- *sel* is simply a call to xarray"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d273c24f",
+            "id": "8",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "region = {\n",
                 "    \"name\": \"example-region\",\n",
@@ -172,15 +196,15 @@
                 "    \"lon_bnds\": [-75, -74],\n",
                 "    \"lat_bnds\": [45, 46],\n",
                 "}"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "890cb41f",
+            "id": "9",
             "metadata": {},
             "source": [
                 "### Preparing arguments for *xarray*\n",
                 "\n",
                 "`xscen` makes use of `intake_esm`'s [to_dataset_dict()](https://intake-esm.readthedocs.io/en/stable/reference/api.html?highlight=to_dataset_dict) for the extraction process, which will automatically compute missing variables as required. Also, this function manages Catalogs, IDs, and both NetCDF and Zarr files seamlessly. When the catalog is made of a single dataset, `to_dataset()` can be used instead to directly obtain an *xr.Dataset* instead of a dictionary.\n",
                 "\n",
                 "There are a few key differences compared to using *xarray* directly, one of which being that it uses `xr.open_dataset`, even when multiple files are involved, with a subsequent call to `xr.combine_by_coords`. Kwargs are therefore separated in two:\n",
@@ -191,30 +215,30 @@
                 "\n",
                 "More information on possible kwargs can be obtained here: [xarray.open_dataset](https://xarray.pydata.org/en/stable/generated/xarray.open_dataset.html) & [xarray.combine_by_coords](https://xarray.pydata.org/en/stable/generated/xarray.combine_by_coords.html)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b781fcbf",
+            "id": "10",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Kwargs for xr.open_dataset\n",
                 "xr_open_kwargs = {\"drop_variables\": [\"height\", \"time_bnds\"], \"engine\": \"h5netcdf\"}\n",
                 "\n",
                 "# Kwargs for xr.combine_by_coords\n",
                 "xr_combine_kwargs = {\"data_vars\": \"minimal\"}"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2c62018f",
+            "id": "11",
             "metadata": {},
             "source": [
                 "### Extraction function\n",
                 "\n",
                 "Extraction is done on each dataset by calling `xs.extract_dataset()`. Since the output could have multiple frequencies, the function returns a python dictionary with keys following the output frequency.\n",
                 "\n",
                 "- `catalog` is the *DataCatalog* to extract.\n",
@@ -230,15 +254,15 @@
                 "`extract_dataset` currently only accepts a single unique ID at a time.\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ab465a36",
+            "id": "12",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Example with a single simulation\n",
                 "ds_dict = xs.extract_dataset(\n",
@@ -251,15 +275,15 @@
                 ")\n",
                 "\n",
                 "ds_dict"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c5247913",
+            "id": "13",
             "metadata": {},
             "source": [
                 "### Saving files to disk\n",
                 "\n",
                 "`extract_dataset` does not actually *save* anything to disk. It simply opens and prepares the files as per requested, using lazy computing. The result is a python dictionary containing the results, separated per *xrfreq*.\n",
                 "\n",
                 "`xscen` has two functions for the purpose of saving data: `save_to_netcdf` and `save_to_zarr`. If possible for a given project, it is strongly recommended to use Zarr files since these are often orders of magnitude faster to read and create compared to NetCDF. They do have a few quirks, however:\n",
@@ -279,15 +303,15 @@
                 "\n",
                 "This loop means that upon completing a step in the creation of a climate scenario, `ProjectCatalog.update_from_ds()` can be called to update the catalog.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dd283230",
+            "id": "14",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "for ds in ds_dict.values():\n",
                 "    filename = str(\n",
@@ -301,40 +325,40 @@
                 "    pcat.update_from_ds(ds=ds, path=filename, info_dict={\"format\": \"zarr\"})\n",
                 "\n",
                 "pcat.df"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d980e512",
+            "id": "15",
             "metadata": {},
             "source": [
                 "### Simplifying the call to extract_dataset() with search_data_catalogs()\n",
                 "\n",
                 "When a catalog was produced using `search_data_catalogs`, `xscen` will automatically save the requested periods and frequencies, in addition to *DerivedVariables*. This means that these items do not need to be included during the call to `extract_dataset` and make it possible to extract datasets that have different requirements (such as reference datasets and future simulations)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "90f1ab0a",
+            "id": "16",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "cat_sim[\n",
                 "    \"CMIP6_ScenarioMIP_NCC_NorESM2-MM_ssp245_r1i1p1f1_example-region\"\n",
                 "]._requested_periods"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d29f08c1",
+            "id": "17",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "print(\n",
                 "    cat_sim[\n",
@@ -346,24 +370,24 @@
                 "        \"CMIP6_ScenarioMIP_NCC_NorESM2-MM_ssp245_r1i1p1f1_example-region\"\n",
                 "    ]._requested_variable_freqs\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8c140dbb",
+            "id": "18",
             "metadata": {},
             "source": [
                 "Since `cat_sim` contains multiple datasets, extracting the data should be done by looping on `.items()` or `.values()`. Also, since 'CMIP6_ScenarioMIP_NCC_NorESM2-MM_ssp126_r1i1p1f1_example-region' was extracted in the previous step, `pcat.exists_in_cat` can be used to skip re-extracting."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bf5900f3",
+            "id": "19",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "for key, dc in cat_sim.items():\n",
                 "    if not pcat.exists_in_cat(id=key, processing_level=\"extracted\"):\n",
@@ -385,15 +409,15 @@
                 "            # Strongly suggested to update the project catalog AFTER you save to disk, in case it crashes during the process\n",
                 "            pcat.update_from_ds(ds=ds, path=filename, info_dict={\"format\": \"zarr\"})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "113b9cfa-d237-43d2-9c4e-9ecd5969372e",
+            "id": "20",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "outputs": [],
             "source": [
                 "# This is a hidden cell. Since the sample files are very small, we'll create fake data covering a longer time period and highjack the previously saved files.\n",
                 "\n",
@@ -471,15 +495,15 @@
                 "filename = filename.replace(Path(filename).stem, ds_ref.attrs[\"cat:id\"])\n",
                 "xs.save_to_zarr(ds_ref, filename, rechunk=chunks, mode=\"o\")\n",
                 "pcat.update_from_ds(ds=ds_ref, path=filename, info_dict={\"format\": \"zarr\"})"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9b2040b2",
+            "id": "21",
             "metadata": {},
             "source": [
                 "## Regridding data\n",
                 "\n",
                 "<div class=\"alert alert-info\"> <b>NOTE</b>\n",
                 "\n",
                 "Regridding in `xscen` is built upon `xESMF`. For more information on basic usage and available regridding methods, [please consult their documentation](https://xesmf.readthedocs.io/en/latest/). Their [masking and extrapolation tutorial](https://xesmf.readthedocs.io/en/latest/notebooks/Masking.html) is of particular interest.\n",
@@ -493,15 +517,15 @@
                 "\n",
                 "`xscen` currently does not explicitely support any function to create a destination grid. If required, however, `xESMF` itself has utilities that can easily create custom regular grids, such as `xesmf.util.cf_grid_2d`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "745e751a",
+            "id": "22",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import xesmf\n",
                 "\n",
@@ -514,15 +538,15 @@
                 "# xscen will use the domain to re-assign attributes, so it is important to set it up for custom grids like this\n",
                 "ds_grid.attrs[\"cat:domain\"] = \"finer-grid\"\n",
                 "ds_grid"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d0809950",
+            "id": "23",
             "metadata": {},
             "source": [
                 "### Masking grid cells\n",
                 "\n",
                 "Masks can be used on both the original grid and the destination grid to ignore certain grid cells during the regridding process. These masks follow the `ESMF` convention, meaning that the mask is a variable within the Dataset, named *mask* and comprised of 0 and 1.\n",
                 "\n",
                 "`xs.create_mask` will create an adequate DataArray, following the instructions given by *mask_args*. In the case of variables that have a time component, the first timestep will be chosen.\n",
@@ -533,15 +557,15 @@
                 "        - 'where_threshold'  (optional)\n",
                 "        - 'mask_nans': bool"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1c9ad4ac",
+            "id": "24",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Will mask all pixels that do not match these requirements (at least 25% land)\n",
                 "mask_args = {\n",
@@ -561,15 +585,15 @@
                 "# Masking function\n",
                 "ds_example[\"mask\"] = xs.create_mask(ds_example, mask_args=mask_args)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "081ba5f1",
+            "id": "25",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import matplotlib.patches as patches\n",
                 "import matplotlib.pyplot as plt\n",
@@ -583,15 +607,15 @@
                 "plt.subplot(122)\n",
                 "ds_example.mask.plot.imshow()\n",
                 "plt.title(\"mask\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4a311378",
+            "id": "26",
             "metadata": {},
             "source": [
                 "### Preparing arguments for xESMF.Regridder\n",
                 "\n",
                 "<div class=\"alert alert-info\">  <b>NOTE</b>\n",
                 "\n",
                 "xESMF's API appears to be broken on their ReadTheDocs. For a list of available arguments and options in `Regridder()`, please consult their [Github page](https://github.com/pangeo-data/xESMF/blob/master/xesmf/frontend.py) directly.\n",
@@ -637,41 +661,41 @@
                 "Some utilities that exist in `xESMF` have not yet been explicitely added to `xscen`. If *conservative* regridding is desired, for instance, some additional scripts might be required on the User's side to create the lon/lat boundaries\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a1176ecd",
+            "id": "27",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "regridder_kwargs = {\"extrap_method\": \"inverse_dist\"}"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ceaf40d1",
+            "id": "28",
             "metadata": {},
             "source": [
                 "### Regridding function\n",
                 "\n",
                 "Regridding for a Dataset is done through `xs.regrid_dataset`, which manages calls to `xESMF.Regridder` and makes sure that the output is CF-compliant.\n",
                 "\n",
                 "- `weights_location` provides a path where to save the regridding weights (NetCDF file). This file (alongside `reuse_weights=True`) is used by `xESMF` to reuse the transformation weights between datasets that are deemed to have the same grid and vastly improve the speed of the function.\n",
                 "- `intermediate_grids` can be called to perform the regridding process in multiple steps. This is recommended when the jump in resolution is very high between the original and destination grid (e.g. from 3\u00b0 to 0.08\u00b0).\n",
                 "- `ds_grid` & `regridder_kwargs` are described above."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "461ba262",
+            "id": "29",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# to_dataset_dict() is called to cast the search results as xr.Dataset objects\n",
                 "# frequency=\"^(?!fx$).*$\" is used to exclude fixed fields from the results\n",
@@ -712,15 +736,15 @@
                 "    xs.save_to_zarr(ds=ds_regrid, filename=filename, rechunk=chunks, mode=\"o\")\n",
                 "    pcat.update_from_ds(ds_regrid, path=filename, format=\"zarr\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8413e56a",
+            "id": "30",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import matplotlib.patches as patches\n",
                 "\n",
@@ -750,15 +774,15 @@
                 "ds_regrid.tas.isel(time=0).plot.imshow(vmin=vmin, vmax=vmax)\n",
                 "plt.title(\"tas: regridded with mask + extrapolation\")\n",
                 "plt.tight_layout()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e0c332fa",
+            "id": "31",
             "metadata": {},
             "source": [
                 "## Bias adjusting data\n",
                 "\n",
                 "<div class=\"alert alert-info\"> <b>NOTE</b>\n",
                 "\n",
                 "Bias adjustment in `xscen` is built upon `xclim.sdba`. For more information on basic usage and available methods, [please consult their documentation](https://xclim.readthedocs.io/en/stable/sdba.html).\n",
@@ -770,28 +794,28 @@
                 "\n",
                 "These arguments can be sent by using `xclim_train_kwargs` and `xclim_adjust_kwargs` during the call to `xs.train` and `xs.adjust` respectively."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "90dde88c",
+            "id": "32",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "xclim_train_args = {\"kind\": \"+\", \"nquantiles\": 50}\n",
                 "\n",
                 "xclim_adjust_args = {\"detrend\": 3, \"interp\": \"linear\", \"extrapolation\": \"constant\"}"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3401bbd1",
+            "id": "33",
             "metadata": {},
             "source": [
                 "### Bias adjustment function\n",
                 "\n",
                 "Bias adjustment is done through `xs.train` and `xs.adjust`. They are kept separate to account for cases where a voluminous dataset would require saving after the training step.\n",
                 "\n",
                 "The arguments to *train()* are:\n",
@@ -818,15 +842,15 @@
                 "These functions currently do not support multiple variables due to the fact that train and adjust arguments might vary. The function must be called separately for every variable.\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d8f8dc7e",
+            "id": "34",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ds_dict = pcat.search(processing_level=\"regridded\").to_dataset_dict()\n",
                 "\n",
@@ -865,15 +889,15 @@
                 "        xs.save_to_zarr(ds=ds_adj, filename=filename, rechunk=chunks, mode=\"o\")\n",
                 "        pcat.update_from_ds(ds_adj, path=filename, format=\"zarr\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6c7eee07",
+            "id": "35",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ds = pcat.search(\n",
                 "    processing_level=\"regridded\",\n",
@@ -926,15 +950,15 @@
                 ").transpose(\"lat\", ...).plot.imshow(vmin=-1, vmax=1, cmap=\"RdBu_r\")\n",
                 "plt.title(\"Bias (\u00b0C)\")\n",
                 "plt.tight_layout()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "65cd14ef",
+            "id": "36",
             "metadata": {},
             "source": [
                 "## Computing indicators\n",
                 "\n",
                 "<div class=\"alert alert-info\"> <b>NOTE</b>\n",
                 "\n",
                 "`xscen` relies heavily on `xclim`'s YAML support for calculating indicators. For more information on how to build the YAML file, consult [this Notebook](https://xclim.readthedocs.io/en/latest/notebooks/extendxclim.html?highlight=yaml#YAML-file).\n",
@@ -964,15 +988,15 @@
                 "    base: tg_min\n",
                 "```\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f060f23e",
+            "id": "37",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ds_dict = pcat.search(processing_level=\"biasadjusted\").to_dataset_dict()\n",
                 "\n",
@@ -994,26 +1018,26 @@
                 "    # Strongly suggested to update the project catalog AFTER you save to disk, in case it crashes during the process\n",
                 "    pcat.update_from_ds(ds=ds_ind, path=filename, format=\"zarr\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f9f8d1e9",
+            "id": "38",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "display(ds_ind)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "576bdad3",
+            "id": "39",
             "metadata": {},
             "source": [
                 "## Spatio-temporal aggregation\n",
                 "\n",
                 "### Climatological operations\n",
                 "\n",
                 "`xs.climatological_op` is used to perform *n*-year operations over `ds.time.dt.year`. \n",
@@ -1034,15 +1058,15 @@
                 "\n",
                 "In the following example, we will use `op='mean'`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fb23ba64",
+            "id": "40",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ds_dict = pcat.search(processing_level=\"indicators\").to_dataset_dict()\n",
                 "\n",
@@ -1065,26 +1089,26 @@
                 "    xs.save_to_zarr(ds=ds_mean, filename=filename, mode=\"o\")\n",
                 "    pcat.update_from_ds(ds_mean, path=filename, format=\"zarr\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ef7b336f",
+            "id": "41",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "display(ds_mean)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "205ead0d",
+            "id": "42",
             "metadata": {},
             "source": [
                 "#### Horizon coordinate and time dimension\n",
                 "\n",
                 "Even if no `stride` is called, `xs.climatological_op` will substantially change the nature of the `time` dimension, because it now represents an aggregation over time. While no standards exist on how to reflect that in a dataset, the following was chosen for `xscen`:\n",
                 "\n",
                 "- `time` corresponds to the first timestep of each temporal average.\n",
@@ -1094,28 +1118,28 @@
                 "\n",
                 "Alternatively, setting the `horizons_as_dim` argument to *True* will rearrange the dataset with a new dimension `horizon` and a dimension named according to the temporal aggregation when it is `month` or `season`, but omitting the singleton dimension `year`. The time stamps are conserved in the `time` coordinate as an array with those new dimensions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7c6aaeaa",
+            "id": "43",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "print(f\"time: {ds_mean.time.values}\")\n",
                 "print(f\"horizon: {ds_mean.horizon.values}\")\n",
                 "print(f\"cat:xrfreq attribute: {ds_mean.attrs['cat:xrfreq']}\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "de27bb4b",
+            "id": "44",
             "metadata": {},
             "source": [
                 "### Computing deltas\n",
                 "\n",
                 "`xs.compute_deltas` is pretty self-explanatory. However, note that this function relies on the `horizon` coordinate described above and, thus, is intended to be performed following some kind of temporal aggregation.\n",
                 "\n",
                 "It has the following arguments:\n",
@@ -1123,15 +1147,15 @@
                 "- `reference_horizon` indicates which horizon to use as reference.\n",
                 "- `kind` is either \"+\", \"/\", or \"%\" for absolute, relative, or percentage deltas respectively. This argument can also be a dictionary, with the keys corresponding to data variables."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a6971329",
+            "id": "45",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ds_dict = pcat.search(processing_level=\"30yr-climatology\").to_dataset_dict()\n",
                 "\n",
@@ -1152,27 +1176,27 @@
                 "    xs.save_to_zarr(ds=ds_delta, filename=filename, rechunk=chunks, mode=\"o\")\n",
                 "    pcat.update_from_ds(ds_delta, path=filename, format=\"zarr\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "698e241a",
+            "id": "46",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "print(f\"Deltas over {ds_delta.horizon.values}\")\n",
                 "display(ds_delta.tg_min_delta_1981_2010.isel(lon=0, lat=0).values)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "30f52b96",
+            "id": "47",
             "metadata": {},
             "source": [
                 "### Spatial mean\n",
                 "\n",
                 "`xs.spatial_mean` is used to compute the spatial average over a given region, using various methods. The argument `call_clisops` can also be used to subset the domain prior to the averaging.\n",
                 "\n",
                 "- `method: cos-lat` will perform an average operation over the spatial dimensions, accounting for changes in grid cell area along the 'lat' coordinate.\n",
@@ -1188,15 +1212,15 @@
                 "   - `region` is used to send a bbox or shapefile to the `SpatialAverager`. This argument is a dictionary that follows the same requirements as the one for `xs.extract` described previously.\n",
                 "   - `simplify_tolerance` is a float that can be used to change the precision (in degree) of a shapefile before sending it to `SpatialAverager`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "17168e53",
+            "id": "48",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ds_dict = pcat.search(processing_level=\"deltas\", domain=\"finer-grid\").to_dataset_dict()\n",
                 "\n",
@@ -1217,27 +1241,27 @@
                 "    xs.save_to_zarr(ds=ds_savg, filename=filename, rechunk=chunks, mode=\"o\")\n",
                 "    pcat.update_from_ds(ds_savg, path=filename, format=\"zarr\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f9bf486a",
+            "id": "49",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Aggregated deltas over the study area\n",
                 "display(ds_savg)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1ee6701a",
+            "id": "50",
             "metadata": {},
             "source": [
                 "## Ensemble statistics\n",
                 "\n",
                 "### Weights\n",
                 "\n",
                 "Typically, if an ensemble is inhomogeneous (uneven number of realizations per model, mix of GCMs and RCMs, etc.), the first step should be to call `xs.generate_weights` to create an adequate guess of what the weights should be between the various datasets. Do note, however, that this function does not replace an explicit assessment of the performance or independence of the simulations, and the results provided should be taken with a grain of salt.\n",
@@ -1255,15 +1279,15 @@
                 "`generate_weights` was built with `xscen` in mind, and thus relies on the `cat:` attributes automatically generated by `intake-esm` when data is loaded from a catalog. In the case of data generated elsewhere, the required and recommended attributes should minimally be added to the dataset before using this function.\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fa8e6d0f-5148-4bad-a2ba-ada5035df35c",
+            "id": "51",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# We don't have many simulations in this example to perform ensemble statistics, but we'll use the two SSP2-4.5 realizations\n",
                 "datasets = pcat.search(\n",
@@ -1272,15 +1296,15 @@
                 "\n",
                 "weights = xs.generate_weights(datasets, independence_level=\"model\")\n",
                 "display(weights)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "862160db-a5b8-4e54-b60c-33c7a54f3969",
+            "id": "52",
             "metadata": {},
             "source": [
                 "### Ensemble stats\n",
                 "\n",
                 "`xs.ensemble_stats` creates an ensemble out of many datasets and computes statistics on that ensemble (min, max, mean, percentiles, etc.) using the `xclim.ensembles` module. The inputs can be given in the form of a list or a dictionary of xr.Dataset or of paths.\n",
                 "\n",
                 "The arguments are as follows:\n",
@@ -1290,15 +1314,15 @@
                 "- `common_attrs_only`: `xclim.ensembles.create_ensemble` copies the attributes from the first dataset, but this might not be representative of the new ensemble. If `common_attrs_only` is True, it only keeps the global attributes that are the same for all datasets and generates a new ID.\n",
                 "- `create_kwargs`: If given a set of paths, `xclim.ensembles.create_ensemble` will ignore the chunking on disk and open the datasets with only a chunking along the new `realization` dimension. Thus, for large datasets, this should be used to explicitely specify chunks."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1c2d2d54",
+            "id": "53",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ens_stats = xs.ensemble_stats(\n",
                 "    datasets=datasets,\n",
@@ -1313,26 +1337,26 @@
                 "xs.save_to_zarr(ens_stats, filename=path, mode=\"o\")\n",
                 "pcat.update_from_ds(ds=ens_stats, path=path, format=\"zarr\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b53bb1b4",
+            "id": "54",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "display(ens_stats)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9780fd81",
+            "id": "55",
             "metadata": {},
             "source": [
                 "## Clean up\n",
                 "\n",
                 "At any time, such as after bias adjustment, `xs.clean_up` can be called to perform a number of small modifications to the datasets. That function can:\n",
                 "\n",
                 " - convert the variables to non-CF units using `xs.utils.change_units`\n",
@@ -1342,40 +1366,40 @@
                 " - change the prefix of the catalog attrs (by default: `cat:`)\n",
                 "\n",
                 "in that order.\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d599c1a1",
+            "id": "56",
             "metadata": {},
             "source": [
                 "### Calendars\n",
                 "\n",
                 "During the bias adjustment step, it is frequent to convert the calendar to 'noleap'. However, once that step has been processed, we might want to put back all the February 29th (or other missing data in the case of '360_day' calendar). This can be done using the `convert_calendar_kwargs` argument of `xs.clean_up`, which passes a dictionary to `xclim.core.calendar.convert_calendar`.\n",
                 "\n",
                 "Usually, we want to linearly interpolate the missing temperatures, but put 0 mm/day for missing precipitation. If our dataset has many variables, the `missing` argument (for `convert_calendar`) can be set for each variable with `missing_by_var`. If `missing_by_var` is given 'interpolate', the missing data will be filled with NaNs, then linearly interpolated over time.\n",
                 "\n",
                 "Eg. `{'tasmax':'interpolate', 'pr':[0]}`\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "465ca630",
+            "id": "57",
             "metadata": {},
             "outputs": [],
             "source": [
                 "convert_calendar_kwargs = {\"target\": \"standard\"}\n",
                 "missing_by_var = {\"tas\": \"interpolate\"}"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "344d2ff0",
+            "id": "58",
             "metadata": {},
             "source": [
                 "### Attributes\n",
                 "\n",
                 "We might want to add, remove or modify the attributes.\n",
                 "\n",
                 "It is possible to write a list of attributes to remove with `attrs_to_remove`, or a list of attributes to keep and remove everything else with `remove_all_attrs_except`. Both take the shape of a dictionnary where the keys are the variables (and 'global' for global attrs) and the values are the list.\n",
@@ -1389,15 +1413,15 @@
                 "\n",
                 "It is also possible to modify the catalogue prefix 'cat:' by a new string with `change_attr_prefix`. Don't use this if this is not the last step of your workflow.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bcda251f",
+            "id": "59",
             "metadata": {},
             "outputs": [],
             "source": [
                 "attrs_to_remove = {\n",
                 "    \"tas\": [\"name*\"]\n",
                 "}  # remove tas attrs that contain the substring 'name'\n",
                 "remove_all_attrs_except = {\n",
@@ -1408,15 +1432,15 @@
                 "}  # add a new tas attribute named 'notes' with value 'some crucial information'\n",
                 "change_attr_prefix = \"dataset:\"  # change /cat to dataset:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b7c6a2e2",
+            "id": "60",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ds = pcat.search(\n",
                 "    processing_level=\"biasadjusted\", variable=\"tas\", experiment=\"ssp245\", member=\"r1.*\"\n",
                 ").to_dataset()\n",
                 "\n",
@@ -1431,15 +1455,15 @@
                 "    change_attr_prefix=change_attr_prefix,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "91502867",
+            "id": "61",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from xclim.core.calendar import get_calendar\n",
                 "\n",
                 "# Inspect calendars and the interpolated values\n",
                 "print(\"Initial calendar: \", get_calendar(ds.time))\n",
@@ -1472,13 +1496,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.12"
+            "version": "3.12.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `xscen-0.8.3/docs/notebooks/3_diagnostics.ipynb` & `xscen-0.9.0/docs/notebooks/3_diagnostics.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9802489177489178%*

 * *Differences: {"'cells'": "{1: {'id': '1'}, 2: {'id': '2'}, 3: {'id': '3'}, 4: {'id': '4'}, 5: {'id': '5'}, 6: "*

 * *            "{'id': '6'}, 7: {'id': '7'}, 8: {'id': '8'}, 9: {'id': '9'}, 10: {'id': '10'}, 11: "*

 * *            "{'id': '11'}, 12: {'id': '12'}, 13: {'id': '13'}, 14: {'id': '14'}, 15: {'id': '15'}, "*

 * *            "16: {'id': '16'}, 17: {'id': '17'}, 18: {'id': '18'}, 19: {'id': '19'}, 20: {'id': "*

 * *            "'20'}, 21: {'id': '21'}, insert: [(0, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_co […]*

```diff
@@ -1,13 +1,32 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b2e9213c",
+            "id": "0",
+            "metadata": {
+                "nbsphinx": "hidden"
+            },
+            "outputs": [],
+            "source": [
+                "# Remove flox spam\n",
+                "\n",
+                "import logging\n",
+                "\n",
+                "# Get the logger for the 'flox' package\n",
+                "logger = logging.getLogger(\"flox\")\n",
+                "# Set the logging level to WARNING\n",
+                "logger.setLevel(logging.WARNING)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "1",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from pathlib import Path\n",
                 "\n",
@@ -31,42 +50,42 @@
                 "    project=project,\n",
                 "    overwrite=True,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ad709809",
+            "id": "2",
             "metadata": {},
             "source": [
                 "# Diagnostics\n",
                 "\n",
                 "It can be useful to perform a various diagnostic tests in order to check that the data that was produced is as expected. Diagnostics can also help us assess bias adjustment methods.\n",
                 "\n",
                 "Make sure you run GettingStarted.ipynb before this one, the GettingStarted outputs will be used a inputs in this notebook."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5022726c",
+            "id": "3",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Load catalog from the GettingStarted notebook\n",
                 "gettingStarted_cat = xs.ProjectCatalog(\n",
                 "    str(output_folder / \"example-gettingstarted.json\")\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "309dda71-bb05-4960-a882-1e62648c15a3",
+            "id": "4",
             "metadata": {},
             "source": [
                 "## Health checks\n",
                 "\n",
                 "<div class=\"alert alert-info\"> <b>NOTE</b>\n",
                 "\n",
                 "For more information on the available `cfchecks`, `missing`, and `data_flags` methods, [please consult the xclim documentation](https://xclim.readthedocs.io/en/stable/checks.html).\n",
@@ -89,15 +108,15 @@
                 "\n",
                 "Use the argument `raise_on` to list to list which test should raise an error if it fails. Use [\"all\"] to raise on all checks."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "50b76511-571f-4472-81c6-3c4e0872b4d8",
+            "id": "5",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# load input\n",
                 "# 'CMIP6_ScenarioMIP_NCC_NorESM2-MM_ssp245_r2i1p1f1_example-region' will be used for this example\n",
@@ -106,15 +125,15 @@
                 "    processing_level=\"regridded\",\n",
                 ").to_dataset()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "84bb901a-3806-40a5-9214-f98f1b52c515",
+            "id": "6",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# The checks that we want to perform. Note that all checks are optional.\n",
                 "structure = {\"coords\": [\"lat\", \"lon\", \"time\"]}\n",
@@ -127,15 +146,15 @@
                 "missing = {\"missing_any\": {\"freq\": \"D\"}}\n",
                 "flags = {\"tas\": {\"temperature_extremely_low\": {}}}"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ddb4a2ad-fc69-47c2-9f44-97f7ebaab7f2",
+            "id": "7",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "xs.diagnostics.health_checks(\n",
                 "    ds,\n",
@@ -149,15 +168,15 @@
                 "    missing=missing,\n",
                 "    flags=flags,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "655d0351",
+            "id": "8",
             "metadata": {},
             "source": [
                 "## Properties and measures\n",
                 "\n",
                 "This framework for the diagnostic tests was inspired by the [VALUE project](http://www.value-cost.eu/).\n",
                 "Statistical Properties is the xclim term for 'indices' in the VALUE project.\n",
                 "\n",
@@ -166,15 +185,15 @@
                 "- `xclim.sbda.properties` are statistical properties of a climate dataset. They allow for a better understanding of the climate by collapsing the time dimension. A few examples: mean, variance, mean spell length, annual cycle, etc.\n",
                 "\n",
                 "- `xclim.sbda.measures` assess the difference between two datasets of properties. A few examples: bias, ratio, circular bias, etc."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "be09b145",
+            "id": "9",
             "metadata": {},
             "source": [
                 "Let's start by calculating the properties on the reference dataset.\n",
                 "You have to provide the path to a YAML file `properties` describing the properties you want to compute.\n",
                 "You can also specify a period to select and a unit conversion to apply before computing the properties.\n",
                 "\n",
                 "This example will use a YAML file structured like this:\n",
@@ -211,35 +230,35 @@
                 "    measure: xclim.sdba.measures.BIAS\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dc1131b2",
+            "id": "10",
             "metadata": {},
             "outputs": [],
             "source": [
                 "properties = \"samples/properties.yml\"\n",
                 "period = [1981, 2010]\n",
                 "change_units_arg = {\"tas\": \"degC\"}"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "863e8722",
+            "id": "11",
             "metadata": {},
             "source": [
                 "The properties can be given an argument `group` ('time', 'time.season' or 'time.month'). For 'time', the time collapsing will be performed over the whole period. For 'time.season'/'time.month', the time collapsing will be performed over each season/month. See `quantile_98_tas` as an example for season."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fae03cbe",
+            "id": "12",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# load input\n",
                 "dref = gettingStarted_cat.search(source=\"ERA5-Land\").to_dataset()\n",
                 "\n",
                 "# calculate properties and measures\n",
@@ -259,25 +278,25 @@
                 "xs.save_to_zarr(ds=prop_ref, filename=filename, mode=\"o\")\n",
                 "pcat.update_from_ds(ds=prop_ref, path=filename, format=\"zarr\")\n",
                 "prop_ref"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "94df9616",
+            "id": "13",
             "metadata": {},
             "source": [
                 "To compute a measure as well as a property, add the `dref_for_measure` argument with the reference properties calculated above. This will mesure the difference between the reference properties and the scenario properties.\n",
                 "A default measure is associated with each properties, but it is possible to define a new one in the YAML (see `mean-tas` for example where the default (bias) was changed for ratio.)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d78534b5",
+            "id": "14",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# load input\n",
                 "dscen = gettingStarted_cat.search(\n",
                 "    source=\"NorESM2-MM\",\n",
                 "    experiment=\"ssp245\",\n",
@@ -309,15 +328,15 @@
                 "    xs.save_to_zarr(ds=ds, filename=filename, mode=\"o\")\n",
                 "    pcat.update_from_ds(ds=ds, path=filename, format=\"zarr\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "520da8a4",
+            "id": "15",
             "metadata": {},
             "outputs": [],
             "source": [
                 "var = \"mean-tas\"\n",
                 "\n",
                 "# plot\n",
                 "fig, axs = plt.subplots(1, 3, figsize=(15, 5))\n",
@@ -328,15 +347,15 @@
                 "axs[1].set_title(\"Scenario\")\n",
                 "axs[2].set_title(\"Bias between Reference and Scenario\")\n",
                 "fig.tight_layout()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9cec0236",
+            "id": "16",
             "metadata": {},
             "source": [
                 "If you have different methods of bias adjustement, you might want to compare them and see for each property which method performs best (bias close to 0, ratio close to 1) with a `measures_heatmap`.\n",
                 "\n",
                 "Below is an example comparing properties of a simulation (no bias adjustment) and a scenario (with quantile mapping bias adjustment). Both the simulation and the scenario use the same reference for the measures. \n",
                 "\n",
                 "Note that it is possible to add many rows to `measures_heatmap`.\n",
@@ -346,15 +365,15 @@
                 "The bias correction performed in the Getting Started tutorial was adjusted for speed rather than performance, using only a few quantiles. The performance results below are thus quite poor, but that was expected.\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2522cf60",
+            "id": "17",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# repeat the step above for the simulation (no bias adjustment)\n",
                 "dsim = gettingStarted_cat.search(\n",
                 "    source=\"NorESM2-MM\",\n",
                 "    experiment=\"ssp245\",\n",
@@ -380,28 +399,28 @@
                 "    xs.save_to_zarr(ds=ds, filename=filename, mode=\"o\")\n",
                 "    pcat.update_from_ds(ds=ds, path=filename, format=\"zarr\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f20a5915",
+            "id": "18",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# load the measures for both kinds of data (sim and scen)\n",
                 "meas_datasets = pcat.search(\n",
                 "    processing_level=[\"diag-measures-sim\", \"diag-measures-scen\"]\n",
                 ").to_dataset_dict()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "498ccf9d",
+            "id": "19",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from matplotlib import colors\n",
                 "\n",
                 "# calculate the heatmap\n",
                 "hm = xs.diagnostics.measures_heatmap(meas_datasets=meas_datasets)\n",
@@ -420,24 +439,24 @@
                 "cbar.ax.set_xticklabels([\"best\", \"worst\"])\n",
                 "plt.title(\"Normalised mean measure of properties\")\n",
                 "fig_hmap.tight_layout()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "aac2f2a2",
+            "id": "20",
             "metadata": {},
             "source": [
                 "`measure_improved` is another way to compare two datasets. It returns the fraction of the grid points that performed better in the second dataset than in the first dataset. It is useful to see which of properties are best corrected for by the bias adjustement method."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ba7ed6ba",
+            "id": "21",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# change the order of meas_dataset to have sim first, because we want to see how scen improved compared to sim.\n",
                 "ordered_keys = [\n",
                 "    \"CMIP6_ScenarioMIP_NCC_NorESM2-MM_ssp245_r1i1p1f1_example-region.finer-grid.diag-measures-sim.fx\",\n",
                 "    \"CMIP6_ScenarioMIP_NCC_NorESM2-MM_ssp245_r1i1p1f1_example-region.finer-grid.diag-measures-scen.fx\",\n",
@@ -480,13 +499,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.12"
+            "version": "3.12.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `xscen-0.8.3/docs/notebooks/4_ensembles.ipynb` & `xscen-0.9.0/docs/notebooks/4_ensembles.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.973495115995116%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(14, '    ds = xs.climatological_op(\\n'), (15, '        "*

 * *            'ds,\\n\'), (16, \'        op="mean",\\n\'), (17, \'        window=30,\\n\'), (18, '*

 * *            "'        periods=[[1981, 2010], [2021, 2050]],\\n'), (19, '        "*

 * *            'horizons_as_dim=True,\\n\'), (20, \'    ).drop_vars("time")\\n\'), (21, \'    '*

 * *            'datasets[d] = xs.compute_deltas(ds, reference_horizon="1981-2010")\')], delete: [17, '*

 * *            "16, 15, 14]}}, 4: {'source': { […]*

```diff
@@ -1,10 +1,28 @@
 {
     "cells": [
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "nbsphinx": "hidden"
+            },
+            "outputs": [],
+            "source": [
+                "# Remove flox spam\n",
+                "\n",
+                "import logging\n",
+                "\n",
+                "# Get the logger for the 'flox' package\n",
+                "logger = logging.getLogger(\"flox\")\n",
+                "# Set the logging level to WARNING\n",
+                "logger.setLevel(logging.WARNING)"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Ensembles"
             ]
         },
         {
@@ -32,88 +50,61 @@
                 "    \"CCSM4-r1\": \"EnsembleStats/BCCAQv2+ANUSPLIN300_CCSM4_historical+rcp45_r1i1p1_1950-2100_tg_mean_YS.nc\",\n",
                 "    \"CCSM4-r2\": \"EnsembleStats/BCCAQv2+ANUSPLIN300_CCSM4_historical+rcp45_r2i1p1_1950-2100_tg_mean_YS.nc\",\n",
                 "    \"CNRM-CM5\": \"EnsembleStats/BCCAQv2+ANUSPLIN300_CNRM-CM5_historical+rcp45_r1i1p1_1970-2050_tg_mean_YS.nc\",\n",
                 "}\n",
                 "\n",
                 "for d in datasets:\n",
                 "    ds = open_dataset(datasets[d]).isel(lon=slice(0, 4), lat=slice(0, 4))\n",
-                "    ds = xs.climatological_mean(ds, window=30, periods=[[1981, 2010], [2021, 2050]])\n",
-                "    datasets[d] = xs.compute_deltas(ds, reference_horizon=\"1981-2010\")\n",
-                "    datasets[d].attrs[\"cat:id\"] = d  # Required by build_reduction_data\n",
-                "    datasets[d].attrs[\"cat:xrfreq\"] = \"AS-JAN\""
+                "    ds = xs.climatological_op(\n",
+                "        ds,\n",
+                "        op=\"mean\",\n",
+                "        window=30,\n",
+                "        periods=[[1981, 2010], [2021, 2050]],\n",
+                "        horizons_as_dim=True,\n",
+                "    ).drop_vars(\"time\")\n",
+                "    datasets[d] = xs.compute_deltas(ds, reference_horizon=\"1981-2010\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Preparing the data\n",
                 "\n",
-                "Ensemble reduction is built upon climate indicators that are relevant to represent the ensemble's variability for a given application. In this case, we'll use the mean temperature delta between 2021-2050 and 1981-2010.\n",
+                "Ensemble reduction is built upon climate indicators that are relevant to represent the ensemble's variability for a given application. In this case, we'll use the mean temperature delta between 2021-2050 and 1981-2010, but monthly or seasonal indicators could also be required. The `horizons_as_dim` argument in `climatological_op` can help combine indicators of multiple frequencies into a single dataset. Alternatively, `xscen.utils.unstack_dates` can also accomplish the same thing if the climatological operations have already been computed.\n",
                 "\n",
-                "However, the functions implemented in `xclim.ensembles._reduce` require a very specific 2-D DataArray of dimensions \"realization\" and \"criteria\". That means that all the variables need to be combined and renamed, and that all dimensions need to be stacked together.\n",
+                "The functions implemented in `xclim.ensembles._reduce` require a very specific 2-D DataArray of dimensions \"realization\" and \"criteria\". The first solution is to first create an ensemble using `xclim.ensembles.create_ensemble`, then pass the result to `xclim.ensembles.make_criteria`. Alternatively, the datasets can be passed directly to `xscen.ensembles.reduce_ensemble` and the necessary preliminary steps will be accomplished automatically.\n",
                 "\n",
-                "`xs.build_reduction_data` can be used to prepare the data for ensemble reduction. Its arguments are:\n",
+                "In this example, the number of criteria will corresponds to: `indicators x horizons x longitude x latitude`, but criteria that are purely NaN across all realizations will be removed.\n",
                 "\n",
-                "- `datasets` (dict, list)\n",
-                "- `xrfreqs` are the unique frequencies of the indicators.\n",
-                "- `horizons` is used to instruct on which horizon(s) to build the data from.\n",
+                "Note that `xs.spatial_mean` could have been used prior to calling that function to remove the spatial dimensions.\n",
                 "\n",
-                "Because a simulation could have multiple datasets (in the case of multiple frequencies), an attempt will be made to decipher the ID and frequency from the metadata."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "data = xs.build_reduction_data(\n",
-                "    datasets=datasets,\n",
-                "    xrfreqs=[\"AS-JAN\"],\n",
-                "    horizons=[\"2021-2050\"],\n",
-                ")\n",
-                "\n",
-                "data"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "The number of criteria corresponds to: `indicators x horizons x longitude x latitude`, but criteria that are purely NaN across all realizations are removed.\n",
-                "\n",
-                "Note that `xs.spatial_mean` could have been used prior to calling that function to remove the spatial dimensions."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
                 "### Selecting a reduced ensemble\n",
                 "\n",
                 "<div class=\"alert alert-info\"> <b>NOTE</b>\n",
                 "    \n",
                 "Ensemble reduction in `xscen` is built upon `xclim.ensembles`. For more information on basic usage and available methods, [please consult their documentation](https://xclim.readthedocs.io/en/stable/notebooks/ensembles-advanced.html).\n",
                 "</div>\n",
                 "\n",
                 "Ensemble reduction through `xscen.reduce_ensemble` consists in a simple call to `xclim`. The arguments are:\n",
-                "- `data`, which is the 2D DataArray that is created by using `xs.build_reduction_data`.\n",
+                "- `data`, which is the aforementioned 2D DataArray, or the list/dict of datasets required to build it.\n",
                 "- `method` is either `kkz` or `kmeans`. See the link above for further details on each technique.\n",
-                "- `kwargs` is a dictionary of arguments to send to the method chosen."
+                "- `horizons` is used to instruct on which horizon(s) to build the data from, if data needs to be constructed.\n",
+                "- `create_kwargs`, the arguments to pass to `xclim.ensembles.create_ensemble` if data needs to be constructed.\n",
+                "- `kwargs` is a dictionary of arguments to send to the clustering method chosen."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "selected, clusters, fig_data = xs.reduce_ensemble(\n",
-                "    data=data, method=\"kmeans\", kwargs={\"method\": {\"n_clusters\": 3}}\n",
+                "    data=datasets, method=\"kmeans\", horizons=[\"2021-2050\"], max_clusters=3\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -266,13 +257,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.5"
+            "version": "3.12.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `xscen-0.8.3/docs/notebooks/5_warminglevels.ipynb` & `xscen-0.9.0/docs/notebooks/5_warminglevels.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.978016774891775%*

 * *Differences: {"'cells'": "{1: {'id': '1'}, 2: {'id': '2'}, 3: {'id': '3'}, 4: {'id': '4'}, 5: {'id': '5'}, 6: "*

 * *            "{'id': '6'}, 7: {'id': '7'}, 8: {'id': '8'}, 9: {'id': '9'}, 10: {'id': '10'}, 11: "*

 * *            "{'id': '11'}, 12: {'id': '12'}, 13: {'id': '13'}, 14: {'id': '14'}, 15: {'id': '15'}, "*

 * *            "16: {'id': '16'}, 17: {'id': '17'}, 18: {'id': '18'}, 19: {'id': '19'}, 20: {'id': "*

 * *            "'20'}, 21: {'id': '21'}, insert: [(0, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_co […]*

```diff
@@ -1,25 +1,44 @@
 {
     "cells": [
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "0",
+            "metadata": {
+                "nbsphinx": "hidden"
+            },
+            "outputs": [],
+            "source": [
+                "# Remove flox spam\n",
+                "\n",
+                "import logging\n",
+                "\n",
+                "# Get the logger for the 'flox' package\n",
+                "logger = logging.getLogger(\"flox\")\n",
+                "# Set the logging level to WARNING\n",
+                "logger.setLevel(logging.WARNING)"
+            ]
+        },
+        {
             "cell_type": "markdown",
-            "id": "3e311475",
+            "id": "1",
             "metadata": {},
             "source": [
                 "# Warming levels\n",
                 "\n",
                 "This Notebook explores the options provided in `xscen` to analyze climate simulations through the scope of global warming levels, instead of temporal horizons.\n",
                 "\n",
                 "First, we just need to prepare some data. We'll use NorESM2-MM as our example dataset."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "eec162f0",
+            "id": "2",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Basic imports\n",
                 "from pathlib import Path\n",
@@ -97,15 +116,15 @@
                 "    chunks = xs.io.estimate_chunks(ds, dims=[\"time\"], target_mb=50)\n",
                 "    xs.save_to_zarr(ds, filename, rechunk=chunks, mode=\"o\")\n",
                 "    pcat.update_from_ds(ds=ds, path=filename, info_dict={\"format\": \"zarr\"})"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0d2e4fa8-554a-4647-99c1-5dafad5f278b",
+            "id": "3",
             "metadata": {},
             "source": [
                 "## Find warming levels with only the model name\n",
                 "\n",
                 "If all that you want to know is the year or the period during which a climate model reaches a given warming level, then ``xs.get_warming_level`` is the function to use since you can simply give it a string or a list of strings and receive that information.\n",
                 "\n",
                 "The usual arguments of ``xs.get_warming_level`` are:\n",
@@ -124,15 +143,15 @@
                 "\n",
                 "If `realization` is a list of the accepted types, or a DataArray or a DataFrame, the function returns a sequence of the same size (and with the same index, if relevant). It can happen that a requested model's name was not found exactly in the database, but that arguments allowed for a relaxed search (`ignore_member = True` or regex in  `realization`). In that case, the _selected_ model doesn't have the same name as the requested one and this information is only shown in the log, unless one passes `output='selected'` to receive a dictionary instead where the keys are the _selected_ models in the database."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fa38e4c5-b693-42ea-bf9e-08862742c729",
+            "id": "4",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Multiple entries, returns a list of the same length\n",
                 "print(\n",
@@ -161,15 +180,15 @@
                 ")\n",
                 "# +10\u00b0C is never reached, returns None\n",
                 "print(xs.get_warming_level(\"CMIP6_CanESM5_ssp585_r1i1p1f1\", wl=10, window=20))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "26ddd760",
+            "id": "5",
             "metadata": {},
             "source": [
                 "## Find and extract data by warming levels\n",
                 "\n",
                 "If you instead need to subset and analyze data, then two options are currently provided in `xscen`: `subset_warming_level` and `produce_horizon`. \n",
                 "- Use `subset_warming_level` when you want to cut a dataset for a period corresponding to a given warming level, but leave its frequency untouched.\n",
                 "- Use `produce_horizon` when you need to: subset a time period, compute indicators, and compute the climatological mean for one or multiple horizons.\n",
@@ -192,15 +211,15 @@
                 "    \n",
                 "If the source, experiment, (member), and warming level are not found in the database. The function returns None."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8f4a5b3e",
+            "id": "6",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ds = pcat.search(\n",
                 "    processing_level=\"extracted\",\n",
@@ -215,30 +234,30 @@
                 "    wl=2,\n",
                 "    window=20,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "60f63d4d-38b3-48a1-af88-7170af99c9ed",
+            "id": "7",
             "metadata": {},
             "source": [
                 "#### Vectorized subsetting\n",
                 "\n",
                 "The function can also vectorize the subsetting over multiple warming levels or over a properly constructed \"realization\" dimension. In that case, the original time axis can't be preserved. It is replaced by a fake one starting in 1000. However, as this process is a bit complex, the current xscen version only supports this if the data is annual. As the time axis doesn't carry any information, a `warminglevel_bounds` coordinate is added with the time bounds of the subsetting. If a warming level was not reached, a NaN slice is inserted in the output dataset.\n",
                 "\n",
                 "This option is to be used when \"scalar\" subsetting is not enough, but you want to do things differently than `produce_horizons`.\n",
                 "\n",
                 "Here, we'll open all experiments into a single ensemble dataset where the `realization` dimension is constructed exactly as `get_warming_level` expects it to be. We'll also average the daily data to an annual scale."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e394f0d6-3cb2-4e77-a221-fc1c1bd07475",
+            "id": "8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ds = pcat.search(\n",
                 "    processing_level=\"extracted\",\n",
                 "    member=\"r1.*\",\n",
                 "    frequency=\"day\",\n",
@@ -249,24 +268,24 @@
                 "ds = ds.resample(time=\"YS\").mean()\n",
                 "ds"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "74320396-09e8-40ea-80ee-56ec7ad567c1",
+            "id": "9",
             "metadata": {},
             "outputs": [],
             "source": [
                 "xs.subset_warming_level(ds, wl=[1.5, 2, 3], wl_dim=True, to_level=\"warming-level\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c02b599e",
+            "id": "10",
             "metadata": {},
             "source": [
                 "### Method #2: Producing horizons\n",
                 "\n",
                 "If what you need is to compute indicators and their climatological mean, ``xs.aggregate.produce_horizon`` is a more convenient function to work with than `subset_warming_level`. Since the years are meaningless for warming levels, and are even detrimental to making ensemble statistics, the function formats the output as to remove the 'time' and 'year' information from the dataset, while the seasons/months are unstacked to different coordinates. Hence, the single dataset outputed can contain indicators of different frequencies, as well as multiple warming levels or temporal horizons.\n",
                 "\n",
                 "The arguments of ``xs.aggregate.produce_horizon`` are:\n",
@@ -278,15 +297,15 @@
                 "\n",
                 "If both periods and warminglevels are None, the full time series will be used. If a dataset does not contain a given period or warming level, then that specific period will be skipped."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f5f8c25d",
+            "id": "11",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "dict_input = pcat.search(processing_level=\"extracted\", xrfreq=\"D\").to_dataset_dict(\n",
                 "    xarray_open_kwargs={\"decode_timedelta\": False}\n",
@@ -310,37 +329,37 @@
                 "    xs.save_to_zarr(ds_hor, filename, mode=\"o\")\n",
                 "    pcat.update_from_ds(ds=ds_hor, path=filename, info_dict={\"format\": \"zarr\"})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "130a2168",
+            "id": "12",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "display(ds_hor)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "163f9816",
+            "id": "13",
             "metadata": {},
             "source": [
                 "## Deltas and spatial aggregation\n",
                 "\n",
                 "This step is done as in the [Getting Started](2_getting_started.ipynb#Computing-deltas) Notebook. Here we will spatially aggregate the data, but the datasets could also be regridded to a common grid."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f31c4d08",
+            "id": "14",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "dict_wl = pcat.search(processing_level=\"horizons\").to_dataset_dict(\n",
                 "    xarray_open_kwargs={\"decode_timedelta\": False}\n",
@@ -372,75 +391,75 @@
                 "    xs.save_to_zarr(ds_agg, filename, mode=\"o\")\n",
                 "    pcat.update_from_ds(ds=ds_agg, path=filename, info_dict={\"format\": \"zarr\"})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7f96ae9b",
+            "id": "15",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "display(ds_agg)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d0e70707",
+            "id": "16",
             "metadata": {},
             "source": [
                 "## Ensemble statistics\n",
                 "\n",
                 "Even more than with time-based horizons, the first step of ensemble statistics should be to generate the weights. Indeed, if a model has 3 experiments reaching a given warming level, we want it to have the same weight as a model with only 2 experiments reaching that warming level. The argument `skipna=False` should be passed to `xs.generate_weights` to properly assess which simulations reaches which warming level. If the `horizon` dimension differs between datasets (as is the case here), they are reindexed and given a weight of 0.\n",
                 "\n",
                 "When working with warming levels, how to assess experiments is more open-ended. The IPCC Atlas splits the statistics and climate change signals by SSPs, even when they are being analyzed through warming levels, but experiments could also be considered as 'members' of a given model and used to bolster the number of realizations."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "50a1152f-b1c3-4b70-baee-94366fb51453",
+            "id": "17",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "datasets = pcat.search(processing_level=\"deltas-agg\").to_dataset_dict()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dd9b6a71-0ee8-4c3e-9962-d18e4b19a1fa",
+            "id": "18",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# All realisations of NorESM2-MM are given the same weight for the first horizon, while it correctly recognizes that +1.5\u00b0C and +2\u00b0C weren't reached for the SSP126.\n",
                 "weights = xs.ensembles.generate_weights(\n",
                 "    datasets=datasets, independence_level=\"model\", skipna=False\n",
                 ")\n",
                 "display(weights)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b640fa35-d68d-4dbd-83cd-f1a1b3aa974c",
+            "id": "19",
             "metadata": {},
             "source": [
                 "Next, the weights and the datasets can be passed to `xs.ensemble_stats` to calculate the ensemble statistics."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "76c8130d",
+            "id": "20",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ds_ens = xs.ensemble_stats(\n",
                 "    datasets=datasets,\n",
@@ -460,15 +479,15 @@
                 "xs.save_to_zarr(ds_ens, filename, mode=\"o\")\n",
                 "pcat.update_from_ds(ds=ds_ens, path=filename, info_dict={\"format\": \"zarr\"})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1f0d8fa0",
+            "id": "21",
             "metadata": {},
             "outputs": [],
             "source": [
                 "display(ds_ens)"
             ]
         }
     ],
@@ -479,13 +498,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.12"
+            "version": "3.12.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `xscen-0.8.3/docs/notebooks/6_config.ipynb` & `xscen-0.9.0/docs/notebooks/6_config.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.982659556878307%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2'}, 3: {'id': '3'}, 4: {'id': '4'}, 5: "*

 * *            "{'id': '5'}, 6: {'id': '6'}, 7: {'id': '7'}, 8: {'id': '8'}, 9: {'id': '9'}, 10: "*

 * *            "{'id': '10'}, 11: {'id': '11'}, 12: {'id': '12'}, 13: {'id': '13'}, 14: {'id': '14'}, "*

 * *            "15: {'id': '15'}, 16: {'id': '16'}, 17: {'id': '17', 'source': {insert: [(4, 'time = "*

 * *            'pd.date_range("1951-01-01", "2100-01-01", freq="YS-JAN")\\n\')], delete: [4]}}, 18: '*

 * *            "{'id […]*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "3c366641",
+            "id": "0",
             "metadata": {},
             "source": [
                 "# YAML usage\n",
                 "\n",
                 "<div class=\"alert alert-info\"> <b>NOTE</b> \n",
                 "    \n",
                 "This tutorial will mostly remain xscen-specific and, thus, will not go into more advanced YAML functionalities such as anchors. More information on that can be consulted [here](https://support.atlassian.com/bitbucket-cloud/docs/yaml-anchors/), while [this template](https://github.com/Ouranosinc/xscen/blob/main/templates/1-basic_workflow_with_config/config1.yml) makes ample use of them.\n",
@@ -17,52 +17,52 @@
                 "\n",
                 "An `xscen` function supports YAML parametrisation if it is preceded by the `parse_config` wrapper in the code. Currently supported functions are:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7e6662ca",
+            "id": "1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from xscen.config import get_configurable\n",
                 "\n",
                 "list(get_configurable().keys())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1fdc6de2-2b19-4452-823e-158f690e9ff3",
+            "id": "2",
             "metadata": {},
             "source": [
                 "## Loading an existing YAML config file\n",
                 "\n",
                 "YAML files are read using `xscen.load_config`. Any number of files can be called, which will be merged together into a single python dictionary accessed through `xscen.CONFIG`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9bd25e3b-07a7-48d1-8fc3-755641f835eb",
+            "id": "3",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from pathlib import Path\n",
                 "\n",
                 "import xscen as xs\n",
                 "from xscen import CONFIG"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f2d9b141-1768-4783-aec1-8016a1201ff8",
+            "id": "4",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Load configuration\n",
                 "xs.load_config(\n",
@@ -77,26 +77,26 @@
                 "\n",
                 "# Display the dictionary keys\n",
                 "print(CONFIG.keys())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "77d673f4-9659-4aa4-935a-32020385d4ee",
+            "id": "5",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "`xscen.CONFIG` behaves similarly to a python dictionary, but has a custom `__getitem__` that returns a `deepcopy` of the requested item. As such, it is unmutable and thus, reliable and robust."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e1f292ec-d9f3-433a-9ec2-3cea84faf8dd",
+            "id": "6",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# A normal python dictionary is mutable, but a CONFIG dictionary is not.\n",
                 "pydict = dict(CONFIG[\"project\"])\n",
@@ -115,66 +115,66 @@
                 "    \", \",\n",
                 "    pydict3[\"id\"],\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e837a13d",
+            "id": "7",
             "metadata": {},
             "source": [
                 "If one really want to modify the `CONFIG` dictionary from within the workflow itself, its `set` method must be used."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f18dd390",
+            "id": "8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "CONFIG.set(\"project.id\", \"modified id\")\n",
                 "print(CONFIG[\"project\"][\"id\"])"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a565f3a1-530e-45f1-96af-e6a80fe23ca8",
+            "id": "9",
             "metadata": {},
             "source": [
                 "## Building a YAML config file\n",
                 "### Generic arguments\n",
                 "\n",
                 "Since `CONFIG` is a python dictionary, anything can be written in it if it is deemed useful for the execution of the script. A good practice, such as seen in [this template's config1.yml](https://github.com/Ouranosinc/xscen/tree/main/templates/1-basic_workflow_with_config/config1.yml), is for example to use the YAML file to provide a list of tasks to be accomplished, give the general description of the project, or provide a dask configuration:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "75bf160f-c256-4893-b147-90a864832731",
+            "id": "10",
             "metadata": {},
             "outputs": [],
             "source": [
                 "print(CONFIG[\"tasks\"])\n",
                 "print(CONFIG[\"project\"])\n",
                 "print(CONFIG[\"regrid\"][\"dask\"])"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8c4a85bc-7a8a-40b6-af6c-45d0b5b9b289",
+            "id": "11",
             "metadata": {},
             "source": [
                 "These are not linked to any function and will not automatically be called upon by `xscen`, but can be referred to during the execution of the script. Below is an example where `tasks` is used to instruct on which tasks to accomplish and which to skip. Many such example can be seen throughout [the provided templates](https://github.com/Ouranosinc/xscen/tree/main/templates)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ae19691c-e7d8-4747-bca1-acb5b042b4cf",
+            "id": "12",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "if \"extract\" in CONFIG[\"tasks\"]:\n",
                 "    print(\"This will start the extraction process.\")\n",
@@ -183,15 +183,15 @@
                 "    print(\n",
                 "        \"This would start creating figures, but it will be skipped since it is not in the list of tasks.\"\n",
                 "    )"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c8d0d86f-12f7-483a-8a85-3102e4faf8bc",
+            "id": "13",
             "metadata": {},
             "source": [
                 "### Function-specific parameters\n",
                 "\n",
                 "In addition to generic arguments, a major convenience of YAML files is that parameters can be automatically fed to functions if they are wrapped by `@parse_config` (see above for the list of currently supported functions). The exact following format has to be used:\n",
                 "\n",
                 "```\n",
@@ -226,73 +226,73 @@
                 "          \"ERA5-Land\"\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a59bcf70-9371-4fa4-ad1e-bd4f98dd9d12",
+            "id": "14",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Note that the YAML used here is more complex and separates tasks between 'reconstruction' and 'simulation', which would break the automatic passing of arguments.\n",
                 "print(\n",
                 "    CONFIG[\"extract\"][\"reconstruction\"][\"search_data_catalogs\"][\"variables_and_freqs\"]\n",
                 ")  # Dictionary\n",
                 "print(CONFIG[\"extract\"][\"reconstruction\"][\"search_data_catalogs\"][\"periods\"])  # List"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "85b36803-29b8-4993-add3-3c69e4e4a750",
+            "id": "15",
             "metadata": {},
             "source": [
                 "Let's test that it is working, using `climatological_op`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "71287ea3-a7b6-41b6-91f4-e36644d463cc",
+            "id": "16",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# We should obtain 30-year means separated in 10-year intervals.\n",
                 "CONFIG[\"aggregate\"][\"climatological_op\"]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "13e7468e-c6f6-4ae8-b204-76b3b4c49000",
+            "id": "17",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "import xarray as xr\n",
                 "\n",
                 "# Create a dummy dataset\n",
-                "time = pd.date_range(\"1951-01-01\", \"2100-01-01\", freq=\"AS-JAN\")\n",
+                "time = pd.date_range(\"1951-01-01\", \"2100-01-01\", freq=\"YS-JAN\")\n",
                 "da = xr.DataArray([0] * len(time), coords={\"time\": time})\n",
                 "da.name = \"test\"\n",
                 "ds = da.to_dataset()\n",
                 "\n",
                 "# Call climatological_op using no argument other than what's in CONFIG\n",
                 "print(xs.climatological_op(ds))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a19640b8-987d-4272-81f3-b25c9ba42bf2",
+            "id": "18",
             "metadata": {},
             "source": [
                 "### Managing paths\n",
                 "\n",
                 "As a final note, it should be said that YAML files are a good way to privately provide paths to a script without having to explicitely write them in the code. [An example is provided here](https://github.com/Ouranosinc/xscen/blob/main/templates/1-basic_workflow_with_config/paths1_example.yml). As stated earlier, `xs.load_config` will merge together the provided YAML files into a single dictionary, meaning that the separation will be seamless once the script is running.\n",
                 "\n",
                 "As an added protection, if the script is to be hosted on Github, `paths.yml` (or whatever it is being called) can then be added to the `.gitignore`.\n",
@@ -300,36 +300,36 @@
                 "### Configuration of external packages\n",
                 "As explained in the `load_config` [documentation](https://xscen.readthedocs.io/en/latest/api.html#special-sections), a few top-level sections can be used to configure packages external to xscen. For example, everything under the `logging` section will be sent to `logging.config.dictConfig(...)`, allowing the [full configuration](https://docs.python.org/3/library/logging.config.html#configuration-dictionary-schema) of python's built-in logging mechanism. The current config does exactly that by configuring a logger for `xscen` that logs to the console, with a sensibility set to the INFO level and a specified record formating :"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "cb086495",
+            "id": "19",
             "metadata": {},
             "outputs": [],
             "source": [
                 "CONFIG[\"logging\"]"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "70e64452",
+            "id": "20",
             "metadata": {},
             "source": [
                 "## Passing configuration through the command line\n",
                 "In order to have a more flexible configuration, it can be interesting to modify it using the command line. This way, the workflow can be started with different values without having to edit and save the YAML file each time. Alternatively, the command line arguments can also be used to determine which configuration file to use, so that the same workflow can be launched with different configurations without needing to duplicate the code. The [second template workflow](https://github.com/Ouranosinc/xscen/blob/main/templates/2-indicators_only/workflow2.py) uses this method.\n",
                 "\n",
                 "The idea is simply to create an `ArgumentParser` with python's built-in [argparse](https://docs.python.org/3/library/argparse.html) :"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "870c6205",
+            "id": "21",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from argparse import ArgumentParser\n",
                 "\n",
                 "parser = ArgumentParser(description=\"An example CLI arguments parser.\")\n",
                 "parser.add_argument(\"-c\", \"--conf\", action=\"append\")\n",
@@ -343,24 +343,24 @@
                 "\n",
                 "args = parser.parse_args(example_args.split())\n",
                 "print(args.conf)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "62b5fbda",
+            "id": "22",
             "metadata": {},
             "source": [
                 "And then we can simply pass this list to `load_config`, which accepts file paths and \"key=value\" pairs."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "70e2a027",
+            "id": "23",
             "metadata": {},
             "outputs": [],
             "source": [
                 "xs.load_config(*args.conf)\n",
                 "\n",
                 "print(CONFIG[\"project\"][\"title\"])\n",
                 "print(CONFIG[\"project\"][\"id\"])"
@@ -374,13 +374,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.12.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `xscen-0.8.3/docs/notebooks/global_tas_average_obs.ipynb` & `xscen-0.9.0/scripts/global_tas_average_obs.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9879807692307693%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2'}, 3: {'id': '3'}, 4: {'id': '4'}, 5: "*

 * *            "{'id': '5'}, 6: {'id': '6'}, 7: {'id': '7'}, 8: {'id': '8'}, 9: {'id': '9'}, 10: "*

 * *            "{'id': '10'}, 11: {'id': '11'}, 12: {'id': '12'}, 13: {'id': '13'}, 14: {'id': '14'}, "*

 * *            "15: {'id': '15'}, 16: {'id': '16'}, 17: {'id': '17'}, 18: {'id': '18'}, 19: {'id': "*

 * *            "'19'}, 20: {'id': '20'}, 21: {'id': '21'}, 22: {'id': '22'}, 23: {'id': '23'}, 24: "*

 * *            "{'id':  […]*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "00cbb3eb-4e4b-460b-8f5e-5cb72759f437",
+            "id": "0",
             "metadata": {},
             "source": [
                 "# Compute global temperature average for observational datasets\n",
                 "\n",
                 "This notebook follows the guidelines of the _State of the Global Climate 2021_([link]) report to compute observational timeseries of the global annual temperature average (land+ocean) to be used in warming level computations. The same datasets are used, except ERA5 for which I didn't have the data at hand when writing this.\n",
                 "\n",
                 "When possible, data is downloaded directly here.\n",
@@ -17,15 +17,15 @@
                 "\n",
                 "## Preparation"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "01cb5af8-6c27-4223-9699-fef62a08e23e",
+            "id": "1",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import re\n",
@@ -46,15 +46,15 @@
                 "\n",
                 "dask.config.set(num_workers=12)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4ff377ea-7ad6-4c57-a485-73871f61a5f3",
+            "id": "2",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# WMO's reference period\n",
                 "ref_period = [1981, 2010]\n",
@@ -85,29 +85,29 @@
                 "\n",
                 "# The output, a list of DataArrays with a year dim and a \"source\" singleton dim\n",
                 "temps = []"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "90fb65b3-1f30-4983-8564-4f3ce0d46678",
+            "id": "3",
             "metadata": {},
             "source": [
                 "### Berkeley Earth\n",
                 "Rohde, R. A.; Hausfather, Z. The Berkeley Earth Land/Ocean Temperature Record. Earth System Science Data 2020, 12, 3469\u20133479. https://doi.org/10.5194/essd-12-3469-2020.\n",
                 "\n",
                 "The annual summary of the Global Monthly Averages from 1850 to preset is available online as text file. It comes as an anomaly relative to the 1951-1980 average, which is given directly in the header of the text file. We have the choice of using temperature above or below sea ice for the ocean component. I didn't anything in the WMO recommendation about this, so we will use the temperature above.\n",
                 "\n",
                 "For this dataset, we will make two versions. One version will use the 0.69\u00b0C delta to compute absolute anomalies from 1850-1900, as done in the WMO report. The other will simply use the 1850-1900 values directly, as they are available for this dataset."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3650631b-db67-4b65-9586-7a18d1f50d57",
+            "id": "4",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Get data\n",
                 "with open(\"Berkeley_data.txt\", \"wb\") as f:\n",
@@ -142,15 +142,15 @@
                 "temps.append(daAbs.expand_dims(source=[\"Berkeley-Raw\"]))\n",
                 "temps.append(daWMO.expand_dims(source=[\"Berkeley\"]))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0f939173-be37-41ca-937c-2126863cd907",
+            "id": "5",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# A figure to look at it\n",
                 "fig, ax = plt.subplots(figsize=(10, 3))\n",
@@ -162,27 +162,27 @@
                 "ax.set_xlabel(\"years\")\n",
                 "ax.set_ylabel(\"[\u00b0C]\")\n",
                 "ax.legend()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ecf5d136-8bad-484e-ab0d-9aa3fa9c23e7",
+            "id": "6",
             "metadata": {},
             "source": [
                 "### GISTEMP v4\n",
                 "GISTEMP Team, 2023: GISS Surface Temperature Analysis (GISTEMP), version 4. NASA Goddard Institute for Space Studies. Dataset accessed 2023-12-06 at https://data.giss.nasa.gov/gistemp/.\n",
                 "\n",
                 "This dataset comes in a CSV of anomalies relative to 1951-1980.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f13eabec-2a00-4cee-b195-88c054698dfa",
+            "id": "7",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "df = pd.read_csv(\n",
                 "    \"https://data.giss.nasa.gov/gistemp/tabledata_v4/GLB.Ts+dSST.csv\",\n",
@@ -196,27 +196,27 @@
                 "daWMO = clean(da)\n",
                 "\n",
                 "temps.append(daWMO.expand_dims(source=[\"GISTEMPv4\"]))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8baeca9c-caec-4f81-9f99-233694acabb3",
+            "id": "8",
             "metadata": {},
             "source": [
                 "### HadCRUT5\n",
                 "Morice, C.P., J.J. Kennedy, N.A. Rayner, J.P. Winn, E. Hogan, R.E. Killick, R.J.H. Dunn, T.J. Osborn, P.D. Jones and I.R. Simpson (in press) An updated assessment of near-surface temperature change from 1850: the HadCRUT5 dataset. Journal of Geophysical Research (Atmospheres) doi:10.1029/2019JD032361 (supporting information). \n",
                 "\n",
                 "The CSV is an anomaly relative to 1961-1990."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5dcf304e-d43a-4c7b-b0f1-8b4203cb2cf8",
+            "id": "9",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "df = pd.read_csv(\n",
                 "    \"https://www.metoffice.gov.uk/hadobs/hadcrut5/data/HadCRUT.5.0.2.0/analysis/diagnostics/HadCRUT.5.0.2.0.analysis.summary_series.global.annual.csv\",\n",
@@ -234,27 +234,27 @@
                 "daWMO = clean(da)\n",
                 "\n",
                 "temps.append(daWMO.expand_dims(source=[\"HadCRUT5\"]))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "eaa12a90-722c-4a0a-bd21-6db3c1afe73c",
+            "id": "10",
             "metadata": {},
             "source": [
                 "### NOAAGlobalTemp v5\n",
                 "R. S. Vose, B. Huang, X. Yin, D. Arndt, D. R. Easterling, J. H. Lawrimore, M. J. Menne, A. Sanchez-Lugo, and H. M. Zhang (2022): NOAA Global Surface Temperature Dataset (NOAAGlobalTemp), Version 5.1 [indicate subset used]. NOAA National Centers for Environmental Information. doi.org/10.25921/2tj4-0e21\n",
                 "\n",
                 "Available as a text file as an anomaly relative to 1971-2000. The files are updated each month with only the last month kept available."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "86e77060-1b95-4a75-b1bf-230955b172fd",
+            "id": "11",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "df = pd.read_table(\n",
                 "    f\"https://www.ncei.noaa.gov/data/noaa-global-surface-temperature/v5.1/access/timeseries/aravg.ann.land_ocean.90S.90N.v5.1.0.202311.asc\",\n",
@@ -269,63 +269,63 @@
                 "daWMO = clean(da)\n",
                 "\n",
                 "temps.append(daWMO.expand_dims(source=[\"NOAAGlobalTempv5\"]))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "97a33f82-96e1-4f02-a74e-c7963255669e",
+            "id": "12",
             "metadata": {},
             "source": [
                 "### ERA5\n",
                 "Hersbach, H.; Bell, B.; Berrisford, P. et al. The ERA5 global reanalysis. Quarterly Journal of the Royal Meteorological Society 2020, 146 (730), 1999\u20132049. https://doi.org/10.1002/qj.3803.\n",
                 "\n",
                 "TODO"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "953de14e-68a8-40cc-9f24-98b40f32645c",
+            "id": "13",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# cat = xs.DataCatalog('/tank/scenario/catalogues/reconstruction.json')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b7ce5ea7-c3c7-4ed1-91a1-4b880c939aca",
+            "id": "14",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# cat.search(source='ERA5', variable='tas', xrfreq='MS').unique()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "cba799a0-62e6-4795-b086-708ea6556504",
+            "id": "15",
             "metadata": {},
             "source": [
                 "### JRA-55\n",
                 "Ebita, A. et al., 2011, The Japanese 55-year Reanalysis \"JRA-55\": an interim report, SOLA, 7, 149-152.\n",
                 "Kobayashi, S. et al., 2015; The JRA-55 Reanalysis: General Specifications and Basic Characteristics, to be published on JMSJ.\n",
                 "\n",
                 "Here the data is a gridded 6-hourly global dataset, so we need to resample yearly and average spatially."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "59084477-1ff6-4744-9146-0acd9172d746",
+            "id": "16",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ds = xr.open_mfdataset(\n",
                 "    \"/tank/scenario/netcdf/jra/jra55/analysis/tas/*.nc\",\n",
@@ -342,37 +342,37 @@
                 "with ProgressBar():\n",
                 "    daWMO = clean(da).load()\n",
                 "temps.append(daWMO.expand_dims(source=[\"JRA-55\"]))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c5011372-f958-4175-be0b-af9bebea8daf",
+            "id": "17",
             "metadata": {},
             "source": [
                 "## Combine all"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c77b9525-6fd1-4776-9243-0116adb297f8",
+            "id": "18",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ds = xr.concat(temps, \"source\")\n",
                 "ds"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "45030be4-2de6-40a4-bad9-af07b40037d6",
+            "id": "19",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# A figure to look at it\n",
                 "fig, ax = plt.subplots(figsize=(10, 3))\n",
@@ -381,28 +381,28 @@
                 "ax.set_xlabel(\"years\")\n",
                 "ax.set_ylabel(\"[\u00b0C]\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9d88113e-cc50-40bb-a9e9-088b9e0488eb",
+            "id": "20",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "db = xr.open_dataset(\"xscen/data/IPCC_annual_global_tas.nc\", engine=\"h5netcdf\")\n",
                 "db"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f24681dd-f883-46ad-af2d-6d80f0aa8c5c",
+            "id": "21",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ds2 = (\n",
                 "    ds.assign_coords(year=pd.to_datetime(ds.year, format=\"%Y\"))\n",
@@ -424,15 +424,15 @@
                 ")\n",
                 "ds2"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c055f123-1374-4151-8fa8-795dbad3c41b",
+            "id": "22",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "db2 = xr.concat([db, ds2], \"simulation\")\n",
                 "db2.attrs[\"description\"] = (\n",
@@ -440,39 +440,39 @@
                 "    + \" Observational datasets were also added following the WMO guidelines.\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a144b9e9-052b-45d4-88ef-8aa36d057dda",
+            "id": "23",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "db2.to_netcdf(\"xscen/data/IPCC_annual_global_tas_withObs.nc\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fcc7c566-79e3-4044-95a4-ae9e99acd9fa",
+            "id": "24",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "db2.tas.plot(hue=\"simulation\", add_legend=False)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f257e3ef-5669-487f-b40f-43f72f27004a",
+            "id": "25",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "language_info": {
```

### Comparing `xscen-0.8.3/docs/notebooks/samples/pangeo-cmip6.csv` & `xscen-0.9.0/docs/notebooks/samples/pangeo-cmip6.csv`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/docs/notebooks/samples/pangeo-cmip6.json` & `xscen-0.9.0/docs/notebooks/samples/pangeo-cmip6.json`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/docs/notebooks/samples/properties.yml` & `xscen-0.9.0/docs/notebooks/samples/properties.yml`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/pyproject.toml` & `xscen-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   "matplotlib",
   "netCDF4",
   "numcodecs",
   "numpy",
   "pandas >=2.2",
   "parse",
   # Used when opening catalogs.
-  "pyarrow",
+  "pyarrow>=10.0.1",
   "pyyaml",
   "rechunker",
   "scipy",
   "shapely >=2.0",
   "sparse",
   "toolz",
   "xarray >=2023.11.0",
@@ -67,17 +67,17 @@
   "zarr"
 ]
 
 [project.optional-dependencies]
 dev = [
   # Dev tools and testing
   "pip >=23.3.0",
-  "black ==24.2.0",
+  "black ==24.4.2",
   "blackdoc ==0.3.9",
-  "bump-my-version >=0.17.1",
+  "bump-my-version >=0.18.3",
   "coverage >=6.2.2,<8.0.0",
   "coveralls >=3.3.1",
   "flake8-alphabetize >=0.0.21",
   "flake8-rst-docstrings >=0.3.0",
   "flake8 >=6.1.0",
   "isort ==5.13.2",
   "pooch",
@@ -123,15 +123,15 @@
   "py39",
   "py310",
   "py311",
   "py312"
 ]
 
 [tool.bumpversion]
-current_version = "0.8.3"
+current_version = "0.9.0"
 commit = true
 commit_args = "--no-verify"
 tag = false
 tag_name = "v{new_version}"
 allow_dirty = false
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\-(?P<release>[a-z]+)(\\.(?P<build>\\d+)))?"
 serialize = [
@@ -158,15 +158,15 @@
   "dev",
   "release"
 ]
 
 [tool.coverage.run]
 relative_files = true
 include = ["xscen/*"]
-omit = ["docs/notebooks/*.ipynb", "tests/*.py"]
+omit = ["docs/notebooks/*.ipynb", "tests/*.py", "xscen/reduce.py"] # FIXME: Remove xscen/reduce.py when it's fully deleted.
 
 [tool.isort]
 append_only = true
 known_first_party = "xscen"
 profile = "black"
 py_version = 39
 
@@ -189,60 +189,62 @@
   "--verbose"
 ]
 filterwarnings = ["ignore::UserWarning"]
 testpaths = "tests"
 markers = ["requires_netcdf: marks tests that require netcdf files to run"]
 
 [tool.ruff]
-src = [""]
+src = ["xscen"]
 line-length = 150
 target-version = "py39"
 exclude = [
   ".eggs",
   ".git",
   "build",
   "docs"
 ]
+
+[tool.ruff.format]
+line-ending = "auto"
+
+[tool.ruff.lint]
 ignore = [
   "D205",
   "D400",
   "D401"
 ]
 select = [
   "C9",
   "D",
   "E",
   "F",
   "W"
 ]
 
-[tool.ruff.flake8-bandit]
+[tool.ruff.lint.flake8-bandit]
 check-typed-exception = true
 
-[tool.ruff.format]
-line-ending = "auto"
-
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["xscen"]
 case-sensitive = true
 detect-same-package = false
 lines-after-imports = 1
 no-lines-before = ["future", "standard-library"]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 15
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "xscen/**/__init__.py" = ["F401", "F403"]
 "tests/**/*.py" = ["D100", "D101", "D102", "D103"]
 
-[tool.ruff.pycodestyle]
+[tool.ruff.lint.pycodestyle]
 max-doc-length = 180
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.setuptools]
 license-files = ["LICENSE"]
 include-package-data = true
 
 [tool.setuptools.dynamic]
```

### Comparing `xscen-0.8.3/setup.py` & `xscen-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/tests/conftest.py` & `xscen-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/tests/test_aggregate.py` & `xscen-0.9.0/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/tests/test_catalog.py` & `xscen-0.9.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/tests/test_catutils.py` & `xscen-0.9.0/tests/test_catutils.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/tests/test_diagnostics.py` & `xscen-0.9.0/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/tests/test_ensembles.py` & `xscen-0.9.0/tests/test_ensembles.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import xarray as xr
 import xclim as xc
 
 try:
     import xesmf as xe
 except ImportError:
     xe = None
+from xclim.testing import open_dataset
 from xclim.testing.helpers import test_timeseries as timeseries
 
 import xscen as xs
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -114,29 +115,14 @@
         )
         np.testing.assert_array_almost_equal(
             out.tg_mean.sel(percentiles=90),
             [1.81, 2.81, 3.81, 4.81] if weights is None else [1.87, 2.87, 3.87, 4.87],
             decimal=2,
         )
 
-    # FIXME: This function is deprecated, so this test should be removed eventually.
-    @pytest.mark.parametrize("p_vals", [True, False])
-    def test_change_significance(self, p_vals):
-        ens = self.make_ensemble(10)
-        with pytest.warns(
-            FutureWarning,
-            match="Function change_significance is deprecated as of xclim 0.47",
-        ):
-            out = xs.ensemble_stats(
-                ens,
-                statistics={"change_significance": {"test": None, "p_vals": p_vals}},
-            )
-
-        assert len(out.data_vars) == 3 if p_vals else 2
-
     @pytest.mark.parametrize("fractions", ["only", "both", "nested", "missing"])
     def test_robustness_input(self, fractions):
         ens = self.make_ensemble(10)
 
         weights = None
         if fractions == "only":
             statistics = {
@@ -176,15 +162,19 @@
                 match="'robustness_categories' requires 'robustness_fractions'",
             ):
                 xs.ensemble_stats(ens, statistics=statistics)
             return
 
         out = xs.ensemble_stats(ens, statistics=statistics, weights=weights)
 
-        assert len(out.data_vars) == {"only": 5, "both": 6, "nested": 1}[fractions]
+        # Output length should be 1 if nested, >=5 otherwise
+        if fractions == "nested":
+            assert len(out.data_vars) == 1
+        else:
+            assert len(out.data_vars) >= 5
         if fractions in ["only", "both"]:
             np.testing.assert_array_equal(out.tg_mean_changed, [0, 0.4, 1, 1])
             np.testing.assert_array_equal(out.tg_mean_agree, [1, 1, 1, 1])
         if fractions in ["both", "nested"]:
             np.testing.assert_array_equal(
                 out.tg_mean_robustness_categories,
                 {"both": [99, 99, 1, 1], "nested": [99, 1, 1, 1]}[fractions],
@@ -1111,7 +1101,61 @@
             ValueError,
         ):
             ds = xs.ensembles.build_partition_data(
                 datasets=datasets,
                 subset_kw=dict(name="mtl", method="gridpoint", lat=[45.0], lon=[-74]),
                 indicators_kw=dict(indicators=[xc.atmos.tg_mean, xc.indicators.cf.tg]),
             )
+
+
+class TestReduceEnsemble:
+    def test_with_criteria(self):
+        ds = open_dataset("EnsembleReduce/TestEnsReduceCriteria.nc")
+        selected, clusters, fig_data = xs.reduce_ensemble(
+            ds["data"], method="kmeans", max_clusters=3
+        )
+        assert selected.shape == (3,)
+        np.testing.assert_array_equal(selected, [4, 7, 23])
+        assert len(clusters) == 3
+        assert fig_data is not None
+
+    @pytest.mark.parametrize("horizon", ["1981-2010", "2021-2050"])
+    def test_without_criteria(self, horizon):
+        datasets = {
+            "ACCESS": "EnsembleStats/BCCAQv2+ANUSPLIN300_ACCESS1-0_historical+rcp45_r1i1p1_1950-2100_tg_mean_YS.nc",
+            "BNU-ESM": "EnsembleStats/BCCAQv2+ANUSPLIN300_BNU-ESM_historical+rcp45_r1i1p1_1950-2100_tg_mean_YS.nc",
+            "CCSM4-r1": "EnsembleStats/BCCAQv2+ANUSPLIN300_CCSM4_historical+rcp45_r1i1p1_1950-2100_tg_mean_YS.nc",
+            "CCSM4-r2": "EnsembleStats/BCCAQv2+ANUSPLIN300_CCSM4_historical+rcp45_r2i1p1_1950-2100_tg_mean_YS.nc",
+            "CNRM-CM5": "EnsembleStats/BCCAQv2+ANUSPLIN300_CNRM-CM5_historical+rcp45_r1i1p1_1970-2050_tg_mean_YS.nc",
+        }
+        for d in datasets:
+            ds = open_dataset(datasets[d]).isel(lon=slice(0, 4), lat=slice(0, 4))
+            ds = xs.climatological_op(
+                ds,
+                op="mean",
+                window=30,
+                periods=[["1981", "2010"], ["2021", "2050"]],
+                horizons_as_dim=True,
+            ).drop_vars("time")
+            datasets[d] = xs.compute_deltas(ds, reference_horizon="1981-2010")
+
+        selected, clusters, fig_data = xs.reduce_ensemble(
+            datasets, method="kkz", horizons=[horizon], num_select=4
+        )
+        assert selected.shape == (4,)
+        answer = (
+            ["ACCESS", "BNU-ESM", "CNRM-CM5", "CCSM4-r1"]
+            if horizon == "2021-2050"
+            else ["ACCESS", "BNU-ESM", "CCSM4-r1", "CCSM4-r2"]
+        )
+        np.testing.assert_array_equal(selected, answer)
+        assert clusters == {}
+        assert fig_data == {}
+
+    def test_errors(self):
+        ds = open_dataset("EnsembleReduce/TestEnsReduceCriteria.nc")
+        with pytest.raises(
+            ValueError, match="Data must have a 'horizon' dimension to be subsetted."
+        ):
+            xs.reduce_ensemble(
+                ds["data"], method="kmeans", horizons=["1981-2010"], max_clusters=3
+            )
```

### Comparing `xscen-0.8.3/tests/test_extract.py` & `xscen-0.9.0/tests/test_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -401,15 +401,15 @@
 
 
 class TestSubsetWarmingLevel:
     ds = timeseries(
         np.tile(np.arange(1, 2), 50),
         variable="tas",
         start="2000-01-01",
-        freq="AS-JAN",
+        freq="YS-JAN",
         as_dataset=True,
     ).assign_attrs(
         {
             "cat:mip_era": "CMIP6",
             "cat:source": "CanESM5",
             "cat:experiment": "ssp585",
             "cat:member": "r1i1p1f1",
@@ -436,50 +436,59 @@
 
         np.testing.assert_array_equal(ds_sub.time.dt.year[0], 2009)
         np.testing.assert_array_equal(ds_sub.time.dt.year[-1], 2033)
         np.testing.assert_array_equal(ds_sub.warminglevel[0], "+1Cvs1981-2010")
         assert ds_sub.warminglevel.attrs["baseline"] == "1981-2010"
         assert ds_sub.attrs["cat:processing_level"] == "tests"
 
-    def test_outofrange(self):
-        assert xs.subset_warming_level(self.ds, wl=5) is None
-
-    def test_none(self):
-        assert xs.subset_warming_level(self.ds, wl=20) is None
+    @pytest.mark.parametrize("wl", [3.5, 5, 20, [2, 3.5, 5, 20], [3.5, 5, 20]])
+    def test_outofrange(self, wl):
+        # 3.5 is only partially covered by ds, 5 is out of range but within the csv, 20 is fully out of range
+        if not isinstance(wl, list):
+            assert xs.subset_warming_level(self.ds, wl=wl) is None
+        else:
+            ds = xs.subset_warming_level(self.ds, wl=wl)
+            assert ds.warminglevel.size == len(wl)
+            if len(wl) == 3:
+                np.testing.assert_array_equal(ds.tas.isnull().all(), [True])
+            else:
+                np.testing.assert_array_equal(
+                    ds.tas.isnull().all(dim="time"), [False, True, True, True]
+                )
 
     def test_multireals(self):
         ds = self.ds.expand_dims(
             realization=[
                 "CMIP6_CanESM5_ssp126_r1i1p1f1",
                 "CMIP6_CanESM5_ssp245_r1i1p1f1",
                 "fake_faux_falsch_falso",
             ]
         )
         ds_sub = xs.subset_warming_level(
             ds,
-            wl=1,
+            wl=1.5,
             to_level="tests",
         )
         np.testing.assert_array_equal(ds_sub.time.dt.year, np.arange(1000, 1020))
         np.testing.assert_array_equal(
-            ds_sub.warminglevel_bounds[:2].dt.year, [[[1990, 2009]], [[1990, 2009]]]
+            ds_sub.warminglevel_bounds[:2].dt.year, [[[2004, 2023]], [[2004, 2023]]]
         )
         assert ds_sub.warminglevel_bounds[2].isnull().all()
 
     def test_multilevels(self):
         ds_sub = xs.subset_warming_level(
             self.ds,
             wl=[1, 2, 3, 20],
             to_level="tests",
         )
         np.testing.assert_array_equal(
             ds_sub.warminglevel,
             ["+1Cvs1850-1900", "+2Cvs1850-1900", "+3Cvs1850-1900", "+20Cvs1850-1900"],
         )
-        np.testing.assert_array_equal(ds_sub.tas.isnull().sum("time"), [10, 0, 1, 20])
+        np.testing.assert_array_equal(ds_sub.tas.isnull().sum("time"), [20, 0, 20, 20])
 
 
 class TestResample:
     @pytest.mark.parametrize(
         "infrq,meth,outfrq,exp",
         [
             ["MS", "mean", "QS-DEC", [0.47457627, 3, 6.01086957, 9, 11.96666667]],
```

### Comparing `xscen-0.8.3/tests/test_indicators.py` & `xscen-0.9.0/tests/test_indicators.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/tests/test_io.py` & `xscen-0.9.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/tests/test_regrid.py` & `xscen-0.9.0/tests/test_regrid.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/tests/test_scripting.py` & `xscen-0.9.0/tests/test_scripting.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/tests/test_utils.py` & `xscen-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/xscen/__init__.py` & `xscen-0.9.0/xscen/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,73 +10,66 @@
     catutils,
     config,
     diagnostics,
     ensembles,
     extract,
     indicators,
     io,
-    reduce,
     regrid,
     scripting,
     spatial,
     testing,
     utils,
 )
 
 # Import top-level functions
 from .aggregate import *
 from .biasadjust import *
-from .catalog import DataCatalog, ProjectCatalog  # noqa
+from .catalog import DataCatalog, ProjectCatalog
 from .catutils import build_path, parse_directory
-from .config import CONFIG, load_config  # noqa
+from .config import CONFIG, load_config
 from .diagnostics import properties_and_measures
 from .ensembles import *
-from .extract import (  # noqa
+from .extract import (
     extract_dataset,
     get_warming_level,
     search_data_catalogs,
     subset_warming_level,
 )
-from .indicators import compute_indicators  # noqa
-from .io import save_to_netcdf, save_to_table, save_to_zarr  # noqa
-from .reduce import build_reduction_data, reduce_ensemble
+from .indicators import compute_indicators
+from .io import save_to_netcdf, save_to_table, save_to_zarr
 from .regrid import *
 from .scripting import (
     TimeoutException,
     measure_time,
     move_and_delete,
     save_and_update,
     send_mail,
     send_mail_on_exit,
     timeout,
 )
 from .utils import clean_up
 
 __author__ = """Gabriel Rondeau-Genesse"""
 __email__ = "rondeau-genesse.gabriel@ouranos.ca"
-__version__ = "0.8.3"
+__version__ = "0.9.0"
 
 
 def warning_on_one_line(
     message: str, category: Warning, filename: str, lineno: int, file=None, line=None
-):  # noqa: D103
+):
     """Monkeypatch Reformat warning so that `warnings.warn` doesn't mention itself."""
     return f"{filename}:{lineno}: {category.__name__}: {message}\n"
 
 
 warnings.formatwarning = warning_on_one_line
 
 # FIXME: This is a temporary fix for the FutureWarning spam from intake-esm.
 # Print FutureWarnings from intake-esm only once
 warnings.filterwarnings(
     "ignore",
     category=FutureWarning,
     module="intake_esm",
     message="The default of observed=False is deprecated and will be changed to True in a future version of pandas. "
-    "Pass observed=False to retain current behavior or observed=True to adopt the future default and silence this warning.",
-)
-warnings.filterwarnings(
-    "ignore",
-    category=FutureWarning,
-    module="intake_esm",
-    message="DataFrame.applymap has been deprecated. Use DataFrame.map instead.",
+    "Pass observed=False to retain current behavior or observed=True to adopt the future default "
+    "and silence this warning.",
 )
```

### Comparing `xscen-0.8.3/xscen/aggregate.py` & `xscen-0.9.0/xscen/aggregate.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/xscen/biasadjust.py` & `xscen-0.9.0/xscen/biasadjust.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from copy import deepcopy
 from typing import Optional, Union
 
 import xarray as xr
 import xclim as xc
 from xclim import sdba
 from xclim.core.calendar import convert_calendar, get_calendar
-from xclim.sdba import construct_moving_yearly_window, unpack_moving_yearly_window
 
 from .catutils import parse_from_ds
 from .config import parse_config
 from .utils import minimum_calendar, standardize_periods
 
 logger = logging.getLogger(__name__)
+xc.set_options(sdba_encode_cf=True, sdba_extra_output=False)
 
 
 __all__ = [
     "adjust",
     "train",
 ]
 
@@ -47,14 +47,15 @@
             )
         )
 
     if preproc:
         scen.attrs[
             "bias_adjustment"
         ] += ", ref and hist were prepared with " + " and ".join(preproc)
+    return scen
 
 
 @parse_config
 def train(
     dref: xr.Dataset,
     dhist: xr.Dataset,
     var: Union[str, list[str]],
@@ -118,15 +119,18 @@
         raise ValueError(
             "biasadjust currently does not support entries with multiple variables."
         )
     else:
         ref = dref[var[0]]
         hist = dhist[var[0]]
 
-    group = group or {"group": "time.dayofyear", "window": 31}
+    # we want to put default if group is None, but not if group is False
+    if group is None:
+        group = {"group": "time.dayofyear", "window": 31}
+
     xclim_train_args = xclim_train_args or {}
     if method == "DetrendedQuantileMapping":
         xclim_train_args.setdefault("nquantiles", 15)
 
     # cut out the right period
     period = standardize_periods(period, multiple=False)
     hist = hist.sel(time=slice(period[0], period[1]))
@@ -192,15 +196,14 @@
     dsim: xr.Dataset,
     periods: Union[list[str], list[list[str]]],
     *,
     xclim_adjust_args: Optional[dict] = None,
     to_level: str = "biasadjusted",
     bias_adjust_institution: Optional[str] = None,
     bias_adjust_project: Optional[str] = None,
-    moving_yearly_window: Optional[dict] = None,
     align_on: Optional[str] = "year",
 ) -> xr.Dataset:
     """
     Adjust a simulation.
 
     Parameters
     ----------
@@ -215,45 +218,30 @@
     to_level : str
       The processing level to assign to the output.
       Defaults to 'biasadjusted'
     bias_adjust_institution : str, optional
       The institution to assign to the output.
     bias_adjust_project : str, optional
       The project to assign to the output.
-    moving_yearly_window: dict, optional
-      Arguments to pass to `xclim.sdba.construct_moving_yearly_window`.
-      If not None, `construct_moving_yearly_window` will be called on dsim (and scen in xclim_adjust_args if it exists)
-      before adjusting and `unpack_moving_yearly_window` will be called on the output after the adjustment.
-      `construct_moving_yearly_window` stacks windows of the dataArray in a new 'movingwin' dimension.
-      `unpack_moving_yearly_window` unpacks it to a normal time series.
     align_on: str, optional
       `align_on` argument for the fonction `xclim.core.calendar.convert_calendar`.
 
     Returns
     -------
     xr.Dataset
       dscen, the bias-adjusted timeseries.
 
     See Also
     --------
     xclim.sdba.adjustment.DetrendedQuantileMapping, xclim.sdba.adjustment.ExtremeValues
 
     """
-    # TODO: To be adequately fixed later
-
     xclim_adjust_args = deepcopy(xclim_adjust_args)
     xclim_adjust_args = xclim_adjust_args or {}
 
-    if moving_yearly_window:
-        dsim = construct_moving_yearly_window(dsim, **moving_yearly_window)
-        if "scen" in xclim_adjust_args:
-            xclim_adjust_args["scen"] = construct_moving_yearly_window(
-                xclim_adjust_args["scen"], **moving_yearly_window
-            )
-
     # evaluate the dict that was stored as a string
     if not isinstance(dtrain.attrs["train_params"], dict):
         dtrain.attrs["train_params"] = eval(dtrain.attrs["train_params"])
 
     var = dtrain.attrs["train_params"]["var"]
     if len(var) != 1:
         raise ValueError(
@@ -265,46 +253,40 @@
 
     # get right calendar
     simcal = get_calendar(sim)
     mincal = minimum_calendar(simcal, dtrain.attrs["train_params"]["maximal_calendar"])
     if simcal != mincal:
         sim = convert_calendar(sim, mincal, align_on=align_on)
 
+    # adjust
+    ADJ = sdba.adjustment.TrainAdjust.from_dataset(dtrain)
+
+    if ("detrend" in xclim_adjust_args) and (
+        isinstance(xclim_adjust_args["detrend"], dict)
+    ):
+        name, kwargs = list(xclim_adjust_args["detrend"].items())[0]
+        kwargs = kwargs or {}
+        kwargs.setdefault("group", ADJ.group)
+        kwargs.setdefault("kind", ADJ.kind)
+        xclim_adjust_args["detrend"] = getattr(sdba.detrending, name)(**kwargs)
+
     # do the adjustment for all the simulation_period lists
     periods = standardize_periods(periods)
     slices = []
     for period in periods:
         sim_sel = sim.sel(time=slice(period[0], period[1]))
 
-        # adjust
-        ADJ = sdba.adjustment.TrainAdjust.from_dataset(dtrain)
-
-        if ("detrend" in xclim_adjust_args) and (
-            isinstance(xclim_adjust_args["detrend"], dict)
-        ):
-            name, kwargs = list(xclim_adjust_args["detrend"].items())[0]
-            kwargs = kwargs or {}
-            kwargs.setdefault("group", ADJ.group)
-            kwargs.setdefault("kind", ADJ.kind)
-            xclim_adjust_args["detrend"] = getattr(sdba.detrending, name)(**kwargs)
-
-        with xc.set_options(sdba_encode_cf=True, sdba_extra_output=False):
-            out = ADJ.adjust(sim_sel, **xclim_adjust_args)
-            slices.extend([out])
+        out = ADJ.adjust(sim_sel, **xclim_adjust_args)
+        slices.extend([out])
     # put all the adjusted period back together
     dscen = xr.concat(slices, dim="time")
 
-    _add_preprocessing_attr(dscen, dtrain.attrs["train_params"])
+    dscen = _add_preprocessing_attr(dscen, dtrain.attrs["train_params"])
     dscen = xr.Dataset(data_vars={var: dscen}, attrs=dsim.attrs)
-    # TODO: History, attrs, etc. (TODO kept from previous version of `biasadjust`)
-    # TODO: Check for variables to add (grid_mapping, etc.) (TODO kept from previous version of `biasadjust`)
     dscen.attrs["cat:processing_level"] = to_level
     dscen.attrs["cat:variable"] = parse_from_ds(dscen, ["variable"])["variable"]
     if bias_adjust_institution is not None:
         dscen.attrs["cat:bias_adjust_institution"] = bias_adjust_institution
     if bias_adjust_project is not None:
         dscen.attrs["cat:bias_adjust_project"] = bias_adjust_project
 
-    if moving_yearly_window:
-        dscen = unpack_moving_yearly_window(dscen)
-
     return dscen
```

### Comparing `xscen-0.8.3/xscen/catalog.py` & `xscen-0.9.0/xscen/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 import intake_esm
 import pandas as pd
 import tlz
 import xarray as xr
 from intake_esm.cat import ESMCatalogModel
 
 from .config import CONFIG, args_as_str, recursive_update
-from .utils import (  # noqa
-    CV,
+from .utils import (
+    _xarray_defaults,
     date_parser,
     ensure_correct_time,
     ensure_new_xrfreq,
     standardize_periods,
 )
 
 logger = logging.getLogger(__name__)
@@ -38,14 +38,15 @@
 __all__ = [
     "COLUMNS",
     "DataCatalog",
     "ID_COLUMNS",
     "ProjectCatalog",
     "concat_data_catalogs",
     "generate_id",
+    "subset_file_coverage",
     "unstack_id",
 ]
 
 
 # As much as possible, these catalog columns and entries should align with:
 # https://github.com/WCRP-CMIP/CMIP6_CVs and https://github.com/ES-DOC/pyessv-archive
 # See docs/columns.rst for a description of each entry.
@@ -525,14 +526,17 @@
                 axis=1,
             )
 
         if (N := len(cat.keys())) != 1:
             raise ValueError(
                 f"Expected exactly one dataset, received {N} instead : {cat.keys()}"
             )
+
+        kwargs = _xarray_defaults(**kwargs)
+
         ds = cat.to_dask(**kwargs)
         return ds
 
 
 class ProjectCatalog(DataCatalog):
     """A DataCatalog with additional 'write' functionalities that can update and upload itself.
```

### Comparing `xscen-0.8.3/xscen/catutils.py` & `xscen-0.9.0/xscen/catutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,22 +26,15 @@
 import zarr
 from intake_esm import esm_datastore
 from pandas import isna
 
 from .catalog import COLUMNS, DataCatalog, generate_id
 from .config import parse_config
 from .io import get_engine
-from .utils import (  # noqa
-    CV,
-    date_parser,
-    ensure_correct_time,
-    ensure_new_xrfreq,
-    get_cat_attrs,
-    standardize_periods,
-)
+from .utils import CV, date_parser, ensure_new_xrfreq, get_cat_attrs
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = ["build_path", "parse_directory", "parse_from_ds", "register_parse_type"]
 # ## File finding and path parsing ## #
 
@@ -430,15 +423,15 @@
     for col, val in fromfile.items():
         for i in grp.index:  # If val is an iterable we can't use loc.
             out.at[i, col] = val
     return out
 
 
 @parse_config
-def parse_directory(  # noqa:C901
+def parse_directory(  # noqa: C901
     directories: list[Union[str, os.PathLike]],
     patterns: list[str],
     *,
     id_columns: Optional[list[str]] = None,
     read_from_file: Union[
         bool,
         Sequence[str],
@@ -637,19 +630,21 @@
 
     # Fix potential legacy xrfreq
     if "xrfreq" in df.columns:
         df["xrfreq"] = df["xrfreq"].apply(ensure_new_xrfreq)
 
     # translate xrfreq into frequencies and vice-versa
     if {"xrfreq", "frequency"}.issubset(df.columns):
-        df["xrfreq"].fillna(
-            df["frequency"].apply(CV.frequency_to_xrfreq, default=pd.NA), inplace=True
+        df.fillna(
+            {"xrfreq": df["frequency"].apply(CV.frequency_to_xrfreq, default=pd.NA)},
+            inplace=True,
         )
-        df["frequency"].fillna(
-            df["xrfreq"].apply(CV.xrfreq_to_frequency, default=pd.NA), inplace=True
+        df.fillna(
+            {"frequency": df["xrfreq"].apply(CV.xrfreq_to_frequency, default=pd.NA)},
+            inplace=True,
         )
 
     # Parse dates
     # If we don't do the to_numpy(na_value=np.datetime64('')).astype('<M8[ms]') trick,
     # the dtype will be "object" if any of the dates are out-of-bounds.
     # `na_values=np.datetime64('')` is needed because pandas' NaT does not translate to numpy's NaT, but to float.
     if "date_start" in df.columns:
@@ -760,15 +755,15 @@
     attrs = {}
 
     for name in names:
         if name == "variable":
             attrs["variable"] = tuple(sorted(variables))
         elif name in ("frequency", "xrfreq") and time is not None and time.size > 3:
             # round to the minute to catch floating point imprecision
-            freq = xr.infer_freq(time.round("T"))
+            freq = xr.infer_freq(time.round("min"))
             if freq:
                 if "xrfreq" in names:
                     attrs["xrfreq"] = freq
                 if "frequency" in names:
                     attrs["frequency"] = CV.xrfreq_to_frequency(freq)
             else:
                 warnings.warn(
```

### Comparing `xscen-0.8.3/xscen/config.py` & `xscen-0.9.0/xscen/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,17 @@
         if isinstance(arg, Path):
             new_args.append(str(arg))
         else:
             new_args.append(arg)
     return tuple(new_args)
 
 
-def load_config(*elements, reset: bool = False, verbose: bool = False):
+def load_config(
+    *elements, reset: bool = False, encoding: str = None, verbose: bool = False
+):
     """Load configuration from given files or key=value pairs.
 
     Once all elements are loaded, special sections are dispatched to their module, but only if
     the section was changed by the loaded elements. These special sections are:
 
     * `locales` : The locales to use when writing metadata in xscen, xclim and figanos. This section must be a list of 2-char strings.
     * `logging` : Everything passed to :py:func:`logging.config.dictConfig`.
@@ -147,14 +149,16 @@
     elements : str
         Files or values to add into the config.
         If a directory is passed, all `.yml` files of this directory are added, in alphabetical order.
         If a "key=value" string, "key" is a dotted name and value will be evaluated if possible.
         "key=value" pairs are set last, after all files are being processed.
     reset: bool
         If True, the current config is erased before loading files.
+    encoding: str, optional
+        The encoding to use when reading files.
     verbose: bool
         if True, each element triggers a INFO log line.
 
     Example
     -------
     .. code-block:: python
 
@@ -180,15 +184,15 @@
             if file.is_dir():
                 # Get all yml files, sort by name
                 configfiles = sorted(file.glob("*.yml"), key=lambda p: p.name)
             else:
                 configfiles = [file]
 
             for configfile in configfiles:
-                with configfile.open() as f:
+                with configfile.open(encoding=encoding) as f:
                     recursive_update(CONFIG, yaml.safe_load(f))
                     if verbose:
                         logger.info(f"Updated the config with {configfile}.")
 
     for module, old in zip(EXTERNAL_MODULES, old_external):
         if old != CONFIG.get(module, {}):
             _setup_external(module, CONFIG.get(module, {}))
```

### Comparing `xscen-0.8.3/xscen/data/IPCC_annual_global_tas.nc` & `xscen-0.9.0/xscen/data/IPCC_annual_global_tas.nc`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/xscen/data/file_schema.yml` & `xscen-0.9.0/xscen/data/file_schema.yml`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/xscen/data/fr/LC_MESSAGES/xscen.mo` & `xscen-0.9.0/xscen/data/fr/LC_MESSAGES/xscen.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Pascal Bourgault <bourgault.pascal@ouranos.ca>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Content"
 msgstr "Contenu"
 
 msgid "Description"
 msgstr "Description"
```

### Comparing `xscen-0.8.3/xscen/data/fr/LC_MESSAGES/xscen.po` & `xscen-0.9.0/xscen/data/fr/LC_MESSAGES/xscen.po`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/xscen/diagnostics.py` & `xscen-0.9.0/xscen/diagnostics.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,19 +258,24 @@
             if isinstance(missing, str):
                 missing = {missing: {}}
             elif isinstance(missing, list):
                 missing = {m: {} for m in missing}
             for method, kwargs in missing.items():
                 kwargs.setdefault("freq", "YS")
                 for v in ds.data_vars:
-                    ms = getattr(xc.core.missing, method)(ds[v], **kwargs)
-                    if ms.any():
-                        _error(
-                            f"The variable '{v}' has missing values according to the '{method}' method.",
-                            "missing",
+                    if "time" in ds[v].dims:
+                        ms = getattr(xc.core.missing, method)(ds[v], **kwargs)
+                        if ms.any():
+                            _error(
+                                f"The variable '{v}' has missing values according to the '{method}' method.",
+                                "missing",
+                            )
+                    else:
+                        logger.info(
+                            f"Variable '{v}' has no time dimension. The missing data check will be skipped.",
                         )
 
     if flags is not None:
         if return_flags:
             out = xr.Dataset()
         for v in flags:
             dsflags = xc.core.dataflags.data_flags(
```

### Comparing `xscen-0.8.3/xscen/ensembles.py` & `xscen-0.9.0/xscen/ensembles.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "build_partition_data",
     "ensemble_stats",
     "generate_weights",
+    "reduce_ensemble",
 ]
 
 
 @parse_config
 def ensemble_stats(  # noqa: C901
     datasets: Union[
         dict,
@@ -760,7 +761,80 @@
     rename_dict.setdefault("source", "model")
     rename_dict.setdefault("experiment", "scenario")
     rename_dict.setdefault("bias_adjust_project", "downscaling")
     rename_dict = {k: v for k, v in rename_dict.items() if k in ens.dims}
     ens = ens.rename(rename_dict)
 
     return ens
+
+
+@parse_config
+def reduce_ensemble(
+    data: Union[xr.DataArray, dict, list, xr.Dataset],
+    method: str,
+    *,
+    horizons: Optional[list[str]] = None,
+    create_kwargs: Optional[dict] = None,
+    **kwargs,
+):
+    r"""Reduce an ensemble of simulations using clustering algorithms from xclim.ensembles.
+
+    Parameters
+    ----------
+    data : xr.DataArray
+        Selection criteria data : 2-D xr.DataArray with dimensions 'realization' and 'criteria'.
+        These are the values used for clustering. Realizations represent the individual original
+        ensemble members and criteria the variables/indicators used in the grouping algorithm.
+        This data can be generated using py:func:`xclim.ensembles.make_criteria`.
+        Alternatively, either a xr.Dataset, a list of xr.Dataset or a dictionary of xr.Dataset can be passed,
+        in which case the data will be built using py:func:`xclim.ensembles.create_ensemble` and py:func:`xclim.ensembles.make_criteria`.
+    method : str
+      ['kkz', 'kmeans']. Clustering method.
+    horizons : list of str, optional
+        Subset of horizons on which to create the data. Only used if `data` needs to be built.
+    create_kwargs : dict, optional
+        Arguments to pass to py:func:`xclim.ensembles.create_ensemble` if `data` is not an xr.DataArray.
+    \*\*kwargs : dict
+        Arguments to send to either py:func:`xclim.ensembles.kkz_reduce_ensemble` or py:func:`xclim.ensembles.kmeans_reduce_ensemble`.
+
+    Returns
+    -------
+    selected : xr.DataArray
+        DataArray of dimension 'realization' with the selected simulations.
+    clusters : dict
+        If using kmeans clustering, realizations grouped by cluster.
+    fig_data : dict
+        If using kmeans clustering, data necessary to call py:func:`xclim.ensembles.plot_rsqprofile`.
+
+    Notes
+    -----
+    If building `data` to be constructed by this function, the datasets should already have a climatology computed on them, such that the data
+    has no temporal dimension aside from the "horizon" coordinate (which is optional and might be used to subset the data).
+    If the indicators are a mix of yearly, seasonal, and monthly, they should be stacked on the same time/horizon axis and put in the same dataset.
+    You can use py:func:`xscen.utils.unstack_dates` on seasonal or monthly indicators to this end.
+    """
+    if isinstance(data, (list, dict)):
+        data = ensembles.create_ensemble(datasets=data, **(create_kwargs or {}))
+    if horizons:
+        if "horizon" not in data.dims:
+            raise ValueError("Data must have a 'horizon' dimension to be subsetted.")
+        data = data.sel(horizon=horizons)
+    if "criteria" not in data.dims:
+        data = ensembles.make_criteria(data)
+
+    selected = getattr(ensembles, f"{method}_reduce_ensemble")(data=data, **kwargs)
+
+    clusters = {}
+    fig_data = {}
+    if method == "kmeans":
+        fig_data = selected[2]
+        clusters_tmp = selected[1]
+        selected = selected[0]
+        realization = np.arange(len(clusters_tmp))
+
+        clusters = {
+            g: data.realization.isel(realization=realization[clusters_tmp == g])
+            for g in np.unique(clusters_tmp)
+        }
+    selected = data.realization.isel(realization=selected)
+
+    return selected, clusters, fig_data
```

### Comparing `xscen-0.8.3/xscen/extract.py` & `xscen-0.9.0/xscen/extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,26 @@
 import numpy as np
 import pandas as pd
 import xarray as xr
 import xclim as xc
 from intake_esm.derived import DerivedVariableRegistry
 from xclim.core.calendar import compare_offsets
 
-from .catalog import DataCatalog  # noqa
-from .catalog import ID_COLUMNS, concat_data_catalogs, generate_id, subset_file_coverage
+from .catalog import (
+    ID_COLUMNS,
+    DataCatalog,
+    concat_data_catalogs,
+    generate_id,
+    subset_file_coverage,
+)
 from .catutils import parse_from_ds
 from .config import parse_config
 from .indicators import load_xclim_module, registry_from_module
 from .spatial import subset
-from .utils import CV
+from .utils import CV, _xarray_defaults
 from .utils import ensure_correct_time as _ensure_correct_time
 from .utils import get_cat_attrs, natural_sort, standardize_periods, xrfreq_to_timedelta
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = [
@@ -36,54 +41,14 @@
     "get_warming_level",
     "resample",
     "search_data_catalogs",
     "subset_warming_level",
 ]
 
 
-def clisops_subset(ds: xr.Dataset, region: dict) -> xr.Dataset:
-    """Customize a call to clisops.subset() that allows for an automatic buffer around the region.
-
-    Parameters
-    ----------
-    ds : xr.Dataset
-        Dataset to be subsetted
-    region : dict
-        Description of the region and the subsetting method (required fields listed in the Notes)
-
-    Notes
-    -----
-    'region' fields:
-        method: str
-            ['gridpoint', 'bbox', shape']
-        <method>: dict
-            Arguments specific to the method used.
-        buffer: float, optional
-            Multiplier to apply to the model resolution.
-
-    Returns
-    -------
-    xr.Dataset
-        Subsetted Dataset.
-
-    See Also
-    --------
-    clisops.core.subset.subset_gridpoint, clisops.core.subset.subset_bbox, clisops.core.subset.subset_shape
-    """
-    warnings.warn(
-        "clisops_subset is deprecated and will not be available in future versions. "
-        "Use xscen.spatial.subset instead.",
-        category=FutureWarning,
-    )
-
-    ds_subset = subset(ds, region=region)
-
-    return ds_subset
-
-
 @parse_config
 def extract_dataset(  # noqa: C901
     catalog: DataCatalog,
     *,
     variables_and_freqs: Optional[dict] = None,
     periods: Optional[Union[list[str], list[list[str]]]] = None,
     region: Optional[dict] = None,
@@ -192,29 +157,28 @@
         # Make everything a list
         variables_and_freqs = {
             k: [v] if not isinstance(v, list) else v
             for k, v in variables_and_freqs.items()
         }
 
     # Default arguments to send xarray
-    xr_open_kwargs = xr_open_kwargs or {}
-    xr_combine_kwargs = xr_combine_kwargs or {}
-    xr_combine_kwargs.setdefault("data_vars", "minimal")
+    xr_kwargs = _xarray_defaults(
+        xr_open_kwargs=xr_open_kwargs or {}, xr_combine_kwargs=xr_combine_kwargs or {}
+    )
 
     # Open the catalog
     ds_dict = catalog.to_dataset_dict(
-        xarray_open_kwargs=xr_open_kwargs,
-        xarray_combine_by_coords_kwargs=xr_combine_kwargs,
         preprocess=preprocess,
         # Only print a progress bar when it is minimally useful
         progressbar=(len(catalog.keys()) > 1),
+        **xr_kwargs,
     )
 
     out_dict = {}
-    for xrfreq in pd.unique([x for y in variables_and_freqs.values() for x in y]):
+    for xrfreq in np.unique([x for y in variables_and_freqs.values() for x in y]):
         ds = xr.Dataset()
         attrs = {}
         # iterate on the datasets, in reverse timedelta order
         for key, ds_ts in sorted(
             ds_dict.items(),
             key=lambda kv: pd.Timedelta(
                 CV.xrfreq_to_timedelta(catalog[kv[0]].df.xrfreq.iloc[0], default="NAN")
@@ -317,27 +281,14 @@
             slices = []
             for period in periods_extract:
                 slices.extend([ds.sel({"time": slice(period[0], period[1])})])
             ds = xr.concat(slices, dim="time", **xr_combine_kwargs)
 
         # subset to the region
         if region is not None:
-            if (region["method"] in region) and (
-                isinstance(region[region["method"]], dict)
-            ):
-                warnings.warn(
-                    "You seem to be using a deprecated version of region. Please use the new formatting.",
-                    category=FutureWarning,
-                )
-                region = deepcopy(region)
-                if "buffer" in region:
-                    region["tile_buffer"] = region.pop("buffer")
-                _kwargs = region.pop(region["method"])
-                region.update(_kwargs)
-
             ds = subset(ds, **region)
 
         # add relevant attrs
         ds.attrs["cat:processing_level"] = to_level
         if "cat:variable" not in ds.attrs:
             ds.attrs["cat:variable"] = parse_from_ds(ds, ["variable"])["variable"]
 
@@ -858,15 +809,16 @@
 
                         # For each dataset (id * xrfreq * processing_level * domain * variable),
                         # make sure that file availability covers the requested time periods
                         if periods is not None and len(varcat) > 0:
                             valid_tp = []
                             for var, group in varcat.df.groupby(
                                 varcat.esmcat.aggregation_control.groupby_attrs
-                                + ["variable"]
+                                + ["variable"],
+                                observed=True,
                             ):
                                 valid_tp.append(
                                     subset_file_coverage(
                                         group, periods, **coverage_kwargs
                                     )
                                 )  # If valid, this returns the subset of files that cover the time period
                             varcat.esmcat._df = pd.concat(valid_tp)
@@ -974,15 +926,15 @@
         If True, the output will be a list following the format ['start_yr', 'end_yr']
         If False, the output will be a string representing the middle of the period.
 
     Returns
     -------
     dict, list or str
         If `realization` is not a sequence, the output will follow the format indicated by `return_horizon`.
-        If `realization` is a sequence, the output will be a list or dictionary depending on `output`,
+        If `realization` is a sequence, the output will be of the same type,
         with values following the format indicated by `return_horizon`.
     """
     tas_src = tas_src or Path(__file__).parent / "data" / "IPCC_annual_global_tas.nc"
     tas_baseline_period = standardize_periods(
         tas_baseline_period or ["1850", "1900"], multiple=False
     )
 
@@ -1098,15 +1050,15 @@
 
     out = list(map(_get_warming_level, info_models))
     if isinstance(realization, pd.DataFrame):
         return pd.Series(out, index=realization.index)
     if isinstance(realization, xr.DataArray):
         if return_horizon:
             return xr.DataArray(
-                out, dims=(realization.dims[0], "bounds"), coords=realization.coords
+                out, dims=(realization.dims[0], "wl_bounds"), coords=realization.coords
             )
         return xr.DataArray(out, dims=(realization.dims[0],), coords=realization.coords)
 
     if len(out) == 1:
         return out[0]
     return out
 
@@ -1118,14 +1070,15 @@
     to_level: str = "warminglevel-{wl}vs{period0}-{period1}",
     wl_dim: Union[str, bool] = "+{wl}Cvs{period0}-{period1}",
     **kwargs,
 ) -> Optional[xr.Dataset]:
     r"""
     Subsets the input dataset with only the window of time over which the requested level of global warming
     is first reached, using the IPCC Atlas method.
+    A warming level is considered reached only if the full `window` years are available in the dataset.
 
     Parameters
     ----------
     ds : xr.Dataset
        Input dataset.
        The dataset should include attributes to help recognize it and find its
        warming levels - 'cat:mip_era', 'cat:experiment', 'cat:member', and either
@@ -1226,54 +1179,66 @@
     date_cls = xc.core.calendar.datetime_classes[ds.time.dt.calendar]
     if "realization" in ds.dims:
         # Vectorized subset
         bounds = get_warming_level(ds.realization, wl, return_horizon=True, **kwargs)
         reals = []
         for real in bounds.realization.values:
             start, end = bounds.sel(realization=real).values
-            if start is not None:
-                data = ds.sel(realization=[real], time=slice(start, end))
+            data = ds.sel(realization=[real], time=slice(start, end))
+            wl_not_reached = (
+                (start is None)
+                or (data.time.size == 0)
+                or ((data.time.dt.year[-1] - data.time.dt.year[0] + 1) != window)
+            )
+            if not wl_not_reached:
                 bnds_crd = [
                     date_cls(int(start), 1, 1),
                     date_cls(int(end) + 1, 1, 1) - datetime.timedelta(seconds=1),
                 ]
             else:
+                # In the case of not reaching the WL, data might be too short
+                # We create it again with the proper length
                 data = (
                     ds.sel(realization=[real]).isel(time=slice(0, fake_time.size))
-                    * np.NaN
+                    * np.nan
                 )
-                bnds_crd = [np.NaN, np.NaN]
+                bnds_crd = [np.nan, np.nan]
             reals.append(
                 data.expand_dims(warminglevel=wl_crd).assign_coords(
                     time=fake_time[: data.time.size],
                     warminglevel_bounds=(
-                        ("realization", "warminglevel", "bounds"),
+                        ("realization", "warminglevel", "wl_bounds"),
                         [[bnds_crd]],
                     ),
                 )
             )
         ds_wl = xr.concat(reals, "realization")
     else:
         # Scalar subset, single level
         start_yr, end_yr = get_warming_level(ds, wl=wl, return_horizon=True, **kwargs)
         # cut the window selected above and expand dims with wl_crd
         ds_wl = ds.sel(time=slice(start_yr, end_yr))
+        wl_not_reached = (
+            (start_yr is None)
+            or (ds_wl.time.size == 0)
+            or ((ds_wl.time.dt.year[-1] - ds_wl.time.dt.year[0] + 1) != window)
+        )
         if fake_time is None:
-            # WL not reached or completely outside ds time
-            if start_yr is None or ds_wl.time.size == 0:
+            # WL not reached, not in ds, or not fully contained in ds.time
+            if wl_not_reached:
                 return None
             ds_wl = ds_wl.expand_dims(warminglevel=wl_crd)
         else:
-            # WL not reached or not completely inside ds time
-            if start_yr is None or ds_wl.time.size == 0:
+            # WL not reached, not in ds, or not fully contained in ds.time
+            if wl_not_reached:
                 ds_wl = ds.isel(time=slice(0, fake_time.size)) * np.NaN
-                wlbnds = (("warminglevel", "bounds"), [[np.NaN, np.NaN]])
+                wlbnds = (("warminglevel", "wl_bounds"), [[np.NaN, np.NaN]])
             else:
                 wlbnds = (
-                    ("warminglevel", "bounds"),
+                    ("warminglevel", "wl_bounds"),
                     [
                         [
                             date_cls(int(start_yr), 1, 1),
                             date_cls(int(end_yr) + 1, 1, 1)
                             - datetime.timedelta(seconds=1),
                         ]
                     ],
```

### Comparing `xscen-0.8.3/xscen/indicators.py` & `xscen-0.9.0/xscen/indicators.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from xscen.config import parse_config
 
 from .catutils import parse_from_ds
 from .utils import CV, standardize_periods
 
 logger = logging.getLogger(__name__)
 
-__all__ = ["compute_indicators", "load_xclim_module"]
+__all__ = ["compute_indicators", "load_xclim_module", "registry_from_module"]
 
 
 def load_xclim_module(
     filename: Union[str, os.PathLike], reload: bool = False
 ) -> ModuleType:
     """Return the xclim module described by the yaml file (or group of yaml, jsons and py).
 
@@ -130,15 +130,15 @@
         logger.info(f"Computing {N} indicators.")
 
     def _infer_freq_from_meta(ind):
         return (
             ind.injected_parameters["freq"]
             if "freq" in ind.injected_parameters
             else (
-                ind.parameters["freq"]["default"]
+                ind.parameters["freq"].default
                 if "freq" in ind.parameters
                 else ind.src_freq
             )
         )
 
     periods = standardize_periods(periods)
```

### Comparing `xscen-0.8.3/xscen/io.py` & `xscen-0.9.0/xscen/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,14 +397,16 @@
     netcdf_kwargs = netcdf_kwargs or {}
     netcdf_kwargs.setdefault("engine", "h5netcdf")
     netcdf_kwargs.setdefault("format", "NETCDF4")
 
     for var in list(ds.data_vars.keys()):
         if keepbits := _get_keepbits(bitround, var, ds[var].dtype):
             ds = ds.assign({var: round_bits(ds[var], keepbits)})
+        # Remove original_shape from encoding, since it can cause issues with some engines.
+        ds[var].encoding.pop("original_shape", None)
 
     _coerce_attrs(ds.attrs)
     for var in ds.variables.values():
         _coerce_attrs(var.attrs)
 
     return ds.to_netcdf(filename, compute=compute, **netcdf_kwargs)
 
@@ -515,14 +517,16 @@
         if _skip(var):
             logger.info(f"Skipping {var} in {path}.")
             ds = ds.drop_vars(var)
             if encoding:
                 encoding.pop(var)
         if keepbits := _get_keepbits(bitround, var, ds[var].dtype):
             ds = ds.assign({var: round_bits(ds[var], keepbits)})
+        # Remove original_shape from encoding, since it can cause issues with some engines.
+        ds[var].encoding.pop("original_shape", None)
 
     if len(ds.data_vars) == 0:
         return None
 
     _coerce_attrs(ds.attrs)
     for var in ds.variables.values():
         _coerce_attrs(var.attrs)
@@ -900,16 +904,20 @@
             rechunk_dims[ds.cf.axes["X"][0]] = rechunk_dims.pop("X")
         if "Y" in rechunk_dims and "Y" not in ds.dims:
             rechunk_dims[ds.cf.axes["Y"][0]] = rechunk_dims.pop("Y")
 
         ds[rechunk_var] = ds[rechunk_var].chunk(
             {d: chnks for d, chnks in rechunk_dims.items() if d in ds[rechunk_var].dims}
         )
-        ds[rechunk_var].encoding.pop("chunksizes", None)
+        ds[rechunk_var].encoding["chunksizes"] = tuple(
+            rechunk_dims[d] if d in rechunk_dims else ds[d].shape[0]
+            for d in ds[rechunk_var].dims
+        )
         ds[rechunk_var].encoding.pop("chunks", None)
+        ds[rechunk_var].encoding.pop("preferred_chunks", None)
 
     return ds
 
 
 @parse_config
 def rechunk(
     path_in: Union[os.PathLike, str, xr.Dataset],
```

### Comparing `xscen-0.8.3/xscen/reduce.py` & `xscen-0.9.0/xscen/reduce.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 """Functions to reduce an ensemble of simulations."""
 
-import logging
+import warnings
 from typing import Optional, Union
 
 import numpy as np
 import xarray as xr
 import xclim.ensembles as xce
 
 from .config import parse_config
 
-logger = logging.getLogger(__name__)
-
-__all__ = ["build_reduction_data", "reduce_ensemble"]
-
 
 @parse_config
 def build_reduction_data(
     datasets: Union[dict, list[xr.Dataset]],
     *,
     xrfreqs: Optional[list[str]] = None,
     horizons: Optional[list[str]] = None,
@@ -36,14 +32,21 @@
         Subset of horizons on which to create the data.
 
     Returns
     -------
     xr.DataArray
         2D DataArray of dimensions "realization" and "criteria", to be used as input for ensemble reduction.
     """
+    warnings.warn(
+        "This function will be dropped in a future version, as it is now redundant with xclim.ensembles.make_criteria."
+        "Either use xclim.ensembles.make_criteria directly (preceded by xclim.ensembles.create_ensemble if needed) or "
+        "use xscen's reduce_ensemble function to build the criteria and reduce the ensemble in one step.",
+        FutureWarning,
+    )
+
     # Use metadata to identify the simulation attributes
     info = {}
     keys = datasets.keys() if isinstance(datasets, dict) else range(len(datasets))
     for key in keys:
         info[key] = {}
         info[key]["id"] = datasets[key].attrs.get("cat:id", None) or key
         info[key]["xrfreq"] = datasets[key].attrs.get("cat:xrfreq") or xr.infer_freq(
@@ -76,55 +79,69 @@
     # Attributes
     criteria.attrs = {"long_name": "criteria for ensemble selection"}
 
     return criteria
 
 
 @parse_config
-def reduce_ensemble(data: xr.DataArray, method: str, kwargs: dict):
-    """Reduce an ensemble of simulations using clustering algorithms from xclim.ensembles.
+def reduce_ensemble(
+    data: Union[xr.DataArray, dict, list, xr.Dataset],
+    method: str,
+    *,
+    horizons: Optional[list[str]] = None,
+    create_kwargs: Optional[dict] = None,
+    **kwargs,
+):
+    r"""Reduce an ensemble of simulations using clustering algorithms from xclim.ensembles.
 
     Parameters
     ----------
     data : xr.DataArray
         Selection criteria data : 2-D xr.DataArray with dimensions 'realization' and 'criteria'.
         These are the values used for clustering. Realizations represent the individual original
         ensemble members and criteria the variables/indicators used in the grouping algorithm.
-        This data can be generated using build_reduction_data().
+        This data can be generated using py:func:`xclim.ensembles.make_criteria`.
+        Alternatively, either a xr.Dataset, a list of xr.Dataset or a dictionary of xr.Dataset can be passed,
+        in which case the data will be built using py:func:`xclim.ensembles.create_ensemble` and py:func:`xclim.ensembles.make_criteria`.
     method : str
       ['kkz', 'kmeans']. Clustering method.
-    kwargs : dict
-        Arguments to send to either xclim.ensembles.kkz_reduce_ensemble or xclim.ensembles.kmeans_reduce_ensemble
+    horizons : list of str, optional
+        Subset of horizons on which to create the data. Only used if `data` needs to be built.
+    create_kwargs : dict, optional
+        Arguments to pass to py:func:`xclim.ensembles.create_ensemble` if `data` is not an xr.DataArray.
+    \*\*kwargs : dict
+        Arguments to send to either py:func:`xclim.ensembles.kkz_reduce_ensemble` or py:func:`xclim.ensembles.kmeans_reduce_ensemble`.
 
     Returns
     -------
     selected : xr.DataArray
         DataArray of dimension 'realization' with the selected simulations.
     clusters : dict
         If using kmeans clustering, realizations grouped by cluster.
     fig_data : dict
-        If using kmeans clustering, data necessary to call xclim.ensembles.plot_rsqprofile()
-    """
-    selected = getattr(xce, f"{method}_reduce_ensemble")(data=data, **kwargs)
+        If using kmeans clustering, data necessary to call py:func:`xclim.ensembles.plot_rsqprofile`.
 
-    clusters = {}
-    fig_data = {}
-    if method == "kmeans":
-        fig_data = selected[2]
-        clusters_tmp = selected[1]
-        selected = selected[0]
-        realization = np.arange(len(clusters_tmp))
-
-        clusters = {
-            g: data.realization.isel(realization=realization[clusters_tmp == g])
-            for g in np.unique(clusters_tmp)
-        }
-    selected = data.realization.isel(realization=selected)
-
-    return selected, clusters, fig_data
+    Notes
+    -----
+    If building `data` to be constructed by this function, the datasets should already have a climatology computed on them, such that the data
+    has no temporal dimension aside from the "horizon" coordinate (which is optional and might be used to subset the data).
+    If the indicators are a mix of yearly, seasonal, and monthly, they should be stacked on the same time/horizon axis and put in the same dataset.
+    You can use py:func:`xscen.utils.unstack_dates` on seasonal or monthly indicators to this end.
+    """
+    warnings.warn(
+        "This function has been moved to xscen.ensembles.reduce_ensemble. This version will be dropped in a future release.",
+        FutureWarning,
+    )
+    return reduce_ensemble(
+        data=data,
+        method=method,
+        horizons=horizons,
+        create_kwargs=create_kwargs,
+        **kwargs,
+    )
 
 
 def _concat_criteria(criteria: Optional[xr.DataArray], ens: xr.Dataset):
     """Combine all variables and dimensions excepting 'realization'."""
     if criteria is None:
         i = 0
     else:
```

### Comparing `xscen-0.8.3/xscen/regrid.py` & `xscen-0.9.0/xscen/regrid.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/xscen/scripting.py` & `xscen-0.9.0/xscen/scripting.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/xscen/testing.py` & `xscen-0.9.0/xscen/testing.py`

 * *Files identical despite different names*

### Comparing `xscen-0.8.3/xscen/utils.py` & `xscen-0.9.0/xscen/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,29 +29,33 @@
 from xclim.testing.utils import show_versions as _show_versions
 
 from .config import parse_config
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
+    "CV",
     "add_attr",
     "change_units",
     "clean_up",
     "date_parser",
+    "ensure_correct_time",
+    "ensure_new_xrfreq",
     "get_cat_attrs",
     "maybe_unstack",
     "minimum_calendar",
     "natural_sort",
     "publish_release_notes",
     "stack_drop_nans",
     "standardize_periods",
     "translate_time_chunk",
     "unstack_dates",
     "unstack_fill_nan",
     "update_attr",
+    "xrfreq_to_timedelta",
 ]
 
 TRANSLATOR = defaultdict(lambda: lambda s: s)
 """Dictionary of translating objects.
 
 Each key is a two letter locale code and values are functions that return the translated message as compiled in the gettext catalogs.
 If a language is not defined or a message not translated, the function will return the raw message.
@@ -164,15 +168,15 @@
     """Return a datetime from a string.
 
     Parameters
     ----------
     date : str, cftime.datetime, pd.Timestamp, datetime.datetime, pd.Period
         Date to be converted
     end_of_period : bool or str
-        If 'Y' or 'M', the returned date will be the end of the year or month that contains the received date.
+        If 'YE' or 'ME', the returned date will be the end of the year or month that contains the received date.
         If True, the period is inferred from the date's precision, but `date` must be a string, otherwise nothing is done.
     out_dtype : str
         Choices are 'datetime', 'period' or 'str'
     strtime_format : str
         If out_dtype=='str', this sets the strftime format
     freq : str
         If out_dtype=='period', this sets the frequency of the period.
@@ -237,20 +241,20 @@
         date = pd.Timestamp(date.strftime("%Y-%m-%dT%H:%M:%S"))
 
     if not isinstance(date, pd.Timestamp):
         date = pd.Timestamp(date)
 
     if isinstance(end_of_period, str) or (end_of_period is True and fmt):
         quasiday = (pd.Timedelta(1, "d") - pd.Timedelta(1, "s")).as_unit(date.unit)
-        if end_of_period == "Y" or "m" not in fmt:
+        if end_of_period in ["Y", "YE"] or "m" not in fmt:
             date = (
-                pd.tseries.frequencies.to_offset("A-DEC").rollforward(date) + quasiday
+                pd.tseries.frequencies.to_offset("YE-DEC").rollforward(date) + quasiday
             )
-        elif end_of_period == "M" or "d" not in fmt:
-            date = pd.tseries.frequencies.to_offset("M").rollforward(date) + quasiday
+        elif end_of_period in ["M", "ME"] or "d" not in fmt:
+            date = pd.tseries.frequencies.to_offset("ME").rollforward(date) + quasiday
         # TODO: Implement subdaily ?
 
     if out_dtype == "str":
         return date.strftime(strtime_format)
     elif out_dtype == "period":
         return date.to_period(freq)
     else:
@@ -710,14 +714,17 @@
                 elif time_in_ds - time_in_out == -1:
                     # ds is a rate
                     ds[v] = units.rate2amount(ds[v], out_units=variables_and_units[v])
                 else:
                     raise NotImplementedError(
                         f"No known transformation between {ds[v].units} and {variables_and_units[v]} (temporal dimensionality mismatch)."
                     )
+            elif (v in ds) and (ds[v].units != variables_and_units[v]):
+                # update unit name if physical units are equal but not their name (ex. degC vs °C)
+                ds[v] = ds[v].assign_attrs(units=variables_and_units[v])
 
     return ds
 
 
 def clean_up(  # noqa: C901
     ds: xr.Dataset,
     *,
@@ -1074,15 +1081,15 @@
 
     if base not in "YAQM":
         raise ValueError(
             f"Only monthly frequencies or coarser are supported. Got: {freq}."
         )
 
     # Fast track for annual
-    if base == "A":
+    if base in "YA":
         if seasons:
             seaname = seasons[first.month]
         elif anchor == "JAN":
             seaname = "annual"
         else:
             seaname = f"annual-{anchor}"
         dso = ds.expand_dims({new_dim: [seaname]})
@@ -1391,7 +1398,21 @@
         freq = freq.replace("S", "s")
     elif isinstance(freq_as_offset, cfoff.Millisecond):
         freq = freq.replace("L", "ms")
     elif isinstance(freq_as_offset, cfoff.Microsecond):
         freq = freq.replace("U", "us")
 
     return freq
+
+
+def _xarray_defaults(**kwargs):
+    """Translate from xscen's extract names to intake-esm names and put better defaults."""
+    if "xr_open_kwargs" in kwargs:
+        kwargs["xarray_open_kwargs"] = kwargs.pop("xr_open_kwargs")
+    if "xr_combine_kwargs" in kwargs:
+        kwargs["xarray_combine_by_coords_kwargs"] = kwargs.pop("xr_combine_kwargs")
+
+    kwargs.setdefault("xarray_open_kwargs", {}).setdefault("chunks", {})
+    kwargs.setdefault("xarray_combine_by_coords_kwargs", {}).setdefault(
+        "data_vars", "minimal"
+    )
+    return kwargs
```

### Comparing `xscen-0.8.3/xscen/xclim_modules/conversions.py` & `xscen-0.9.0/xscen/xclim_modules/conversions.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,15 +20,15 @@
       Liquid precipitation flux.
 
     Returns
     -------
     xr.DataArray, [same as prsn]
       Surface precipitation flux (all phases)
     """
-    prlp = convert_units_to(prlp, prsn)
+    prlp = convert_units_to(prlp, prsn, context="hydro")
     pr = prsn + prlp
     pr.attrs["units"] = prsn.attrs["units"]
     return pr
 
 
 @declare_units(dtr="[temperature]", tasmax="[temperature]")
 def tasmin_from_dtr(dtr: xr.DataArray, tasmax: xr.DataArray) -> xr.DataArray:
@@ -44,17 +44,20 @@
       Daily maximal temperature.
 
     Returns
     -------
     xr.DataArray, [same as tasmax]
       Daily minimum temperature
     """
-    dtr = convert_units_to(dtr, tasmax)
+    out_units = tasmax.units
+    # To prevent strange behaviors that could arise from changing DTR units, we change the units of tasmax to match DTR
+    tasmax = convert_units_to(tasmax, dtr)
     tasmin = tasmax - dtr
-    tasmin.attrs["units"] = tasmax.units
+    tasmin.attrs["units"] = dtr.units
+    tasmin = convert_units_to(tasmin, out_units)
     return tasmin
 
 
 @declare_units(dtr="[temperature]", tasmin="[temperature]")
 def tasmax_from_dtr(dtr: xr.DataArray, tasmin: xr.DataArray) -> xr.DataArray:
     """Tasmax computed from DTR and tasmin.
 
@@ -68,22 +71,25 @@
       Daily minimal temperature.
 
     Returns
     -------
     xr.DataArray, [same as tasmin]
       Daily maximum temperature
     """
-    dtr = convert_units_to(dtr, tasmin)
+    out_units = tasmin.attrs["units"]
+    # To prevent strange behaviors that could arise from changing DTR units, we change the units of tasmin to match DTR
+    tasmin = convert_units_to(tasmin, dtr)
     tasmax = tasmin + dtr
-    tasmax.attrs["units"] = tasmin.units
+    tasmax.attrs["units"] = dtr.attrs["units"]
+    tasmax = convert_units_to(tasmax, out_units)
     return tasmax
 
 
 @declare_units(tasmin="[temperature]", tasmax="[temperature]")
-def dtr(tasmin: xr.DataArray, tasmax: xr.DataArray) -> xr.DataArray:
+def dtr_from_minmax(tasmin: xr.DataArray, tasmax: xr.DataArray) -> xr.DataArray:
     """DTR computed from tasmin and tasmax.
 
     Dtr as tasmin subtracted from tasmax.
 
     Parameters
     ----------
     tasmin: xr.DataArray
```

### Comparing `xscen-0.8.3/xscen/xclim_modules/conversions.yml` & `xscen-0.9.0/xscen/xclim_modules/conversions.yml`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         kind: 0
       tasmax:
         kind: 0
     cf_attrs:
       - var_name: evspsblpot
   dtr:
     src_freq: D
-    compute: dtr
+    compute: dtr_from_minmax
     cf_attrs:
       units: K
       description: Daily temperature range.
       cell_methods: "time: range within days"
       var_name: dtr
   tasmin_from_dtr:
     src_freq: D
```

### Comparing `xscen-0.8.3/xscen.egg-info/PKG-INFO` & `xscen-0.9.0/xscen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xscen
-Version: 0.8.3
+Version: 0.9.0
 Summary: A climate change scenario-building analysis framework, built with xclim/xarray.
 Author-email: Gabriel Rondeau-Genesse <rondeau-genesse.gabriel@ouranos.ca>
 Project-URL: About Ouranos, https://www.ouranos.ca/en/
 Project-URL: Changelog, https://xscen.readthedocs.io/en/stable/changes.html
 Project-URL: Homepage, https://xscen.readthedocs.io/
 Project-URL: Issue tracker, https://github.com/Ouranosinc/xscen/issues
 Project-URL: Source, https://github.com/Ouranosinc/xscen
@@ -41,29 +41,29 @@
 Requires-Dist: intake-esm>=2023.07.07; python_version >= "3.10"
 Requires-Dist: matplotlib
 Requires-Dist: netCDF4
 Requires-Dist: numcodecs
 Requires-Dist: numpy
 Requires-Dist: pandas>=2.2
 Requires-Dist: parse
-Requires-Dist: pyarrow
+Requires-Dist: pyarrow>=10.0.1
 Requires-Dist: pyyaml
 Requires-Dist: rechunker
 Requires-Dist: scipy
 Requires-Dist: shapely>=2.0
 Requires-Dist: sparse
 Requires-Dist: toolz
 Requires-Dist: xarray>=2023.11.0
 Requires-Dist: xclim>=0.48.2
 Requires-Dist: zarr
 Provides-Extra: dev
 Requires-Dist: pip>=23.3.0; extra == "dev"
-Requires-Dist: black==24.2.0; extra == "dev"
+Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: blackdoc==0.3.9; extra == "dev"
-Requires-Dist: bump-my-version>=0.17.1; extra == "dev"
+Requires-Dist: bump-my-version>=0.18.3; extra == "dev"
 Requires-Dist: coverage<8.0.0,>=6.2.2; extra == "dev"
 Requires-Dist: coveralls>=3.3.1; extra == "dev"
 Requires-Dist: flake8-alphabetize>=0.0.21; extra == "dev"
 Requires-Dist: flake8-rst-docstrings>=0.3.0; extra == "dev"
 Requires-Dist: flake8>=6.1.0; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
 Requires-Dist: pooch; extra == "dev"
```

### Comparing `xscen-0.8.3/xscen.egg-info/SOURCES.txt` & `xscen-0.9.0/xscen.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -30,32 +30,35 @@
 docs/_static/_images/xscen-logo.png
 docs/notebooks/1_catalog.ipynb
 docs/notebooks/2_getting_started.ipynb
 docs/notebooks/3_diagnostics.ipynb
 docs/notebooks/4_ensembles.ipynb
 docs/notebooks/5_warminglevels.ipynb
 docs/notebooks/6_config.ipynb
-docs/notebooks/global_tas_average_obs.ipynb
 docs/notebooks/index.rst
 docs/notebooks/samples/indicators.yml
 docs/notebooks/samples/pangeo-cmip6.csv
 docs/notebooks/samples/pangeo-cmip6.json
 docs/notebooks/samples/properties.yml
+scripts/global_tas_average_obs.ipynb
 tests/conftest.py
 tests/test_aggregate.py
+tests/test_biasadjust.py
 tests/test_catalog.py
 tests/test_catutils.py
 tests/test_diagnostics.py
 tests/test_ensembles.py
 tests/test_extract.py
 tests/test_indicators.py
 tests/test_io.py
 tests/test_regrid.py
 tests/test_scripting.py
+tests/test_spatial.py
 tests/test_utils.py
+tests/test_xclimmod_conversions.py
 xscen/__init__.py
 xscen/aggregate.py
 xscen/biasadjust.py
 xscen/catalog.py
 xscen/catutils.py
 xscen/config.py
 xscen/diagnostics.py
```

### Comparing `xscen-0.8.3/xscen.egg-info/requires.txt` & `xscen-0.9.0/xscen.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 h5py
 matplotlib
 netCDF4
 numcodecs
 numpy
 pandas>=2.2
 parse
-pyarrow
+pyarrow>=10.0.1
 pyyaml
 rechunker
 scipy
 shapely>=2.0
 sparse
 toolz
 xarray>=2023.11.0
@@ -30,17 +30,17 @@
 intake-esm<v2024.2.6,>=2023.07.07
 
 [:python_version >= "3.10"]
 intake-esm>=2023.07.07
 
 [dev]
 pip>=23.3.0
-black==24.2.0
+black==24.4.2
 blackdoc==0.3.9
-bump-my-version>=0.17.1
+bump-my-version>=0.18.3
 coverage<8.0.0,>=6.2.2
 coveralls>=3.3.1
 flake8-alphabetize>=0.0.21
 flake8-rst-docstrings>=0.3.0
 flake8>=6.1.0
 isort==5.13.2
 pooch
```

