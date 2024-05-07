# Comparing `tmp/erlab-2.4.1.tar.gz` & `tmp/erlab-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.4.1.tar", last modified: Fri May  3 08:53:21 2024, max compression
+gzip compressed data, was "erlab-2.4.2.tar", last modified: Tue May  7 12:07:35 2024, max compression
```

## Comparing `erlab-2.4.1.tar` & `erlab-2.4.2.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.760013 erlab-2.4.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.716012 erlab-2.4.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.720012 erlab-2.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)     2200 2024-05-03 08:53:14.000000 erlab-2.4.1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-03 08:53:14.000000 erlab-2.4.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-03 08:53:14.000000 erlab-2.4.1/.github/ISSUE_TEMPLATE/feature-request.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.720012 erlab-2.4.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-05-03 08:53:14.000000 erlab-2.4.1/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-05-03 08:53:14.000000 erlab-2.4.1/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-03 08:53:14.000000 erlab-2.4.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)      893 2024-05-03 08:53:14.000000 erlab-2.4.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      793 2024-05-03 08:53:14.000000 erlab-2.4.1/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   123417 2024-05-03 08:53:18.000000 erlab-2.4.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-05-03 08:53:14.000000 erlab-2.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    48438 2024-05-03 08:53:21.760013 erlab-2.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-05-03 08:53:14.000000 erlab-2.4.1/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     5147 2024-05-03 08:53:14.000000 erlab-2.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.724012 erlab-2.4.1/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      726 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.724012 erlab-2.4.1/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    17977 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    15203 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      106 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      224 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     5039 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.732012 erlab-2.4.1/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   328062 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/images/flowchart_multiple.pdf
--rw-r--r--   0 root         (0) root         (0)   328737 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/images/flowchart_single.pdf
--rw-r--r--   0 root         (0) root         (0)   996803 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     3119 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.732012 erlab-2.4.1/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2604 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     3099 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.736013 erlab-2.4.1/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)    41238 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/user-guide/curve-fitting.ipynb
--rw-r--r--   0 root         (0) root         (0)     2598 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/user-guide/imagetool.rst
--rw-r--r--   0 root         (0) root         (0)     1291 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)    12039 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)    54817 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)    10710 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    27564 2024-05-03 08:53:14.000000 erlab-2.4.1/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-03 08:53:14.000000 erlab-2.4.1/environment.yml
--rw-r--r--   0 root         (0) root         (0)     5353 2024-05-03 08:53:14.000000 erlab-2.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      315 2024-05-03 08:53:14.000000 erlab-2.4.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 08:53:21.760013 erlab-2.4.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.716012 erlab-2.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.736013 erlab-2.4.1/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-03 08:53:18.000000 erlab-2.4.1/src/erlab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.740013 erlab-2.4.1/src/erlab/accessors/
--rw-r--r--   0 root         (0) root         (0)      792 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/accessors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26123 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/accessors/fit.py
--rw-r--r--   0 root         (0) root         (0)    30007 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/accessors/kspace.py
--rw-r--r--   0 root         (0) root         (0)     7071 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/accessors/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.740013 erlab-2.4.1/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      880 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5322 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.740013 erlab-2.4.1/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      168 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.740013 erlab-2.4.1/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      957 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10779 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     9594 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6905 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)    12739 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    20223 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    18221 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)    14968 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.740013 erlab-2.4.1/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     5397 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8505 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     5443 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.744013 erlab-2.4.1/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      232 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.744013 erlab-2.4.1/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      526 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14330 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    21371 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    23024 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11793 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)    19282 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.744013 erlab-2.4.1/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    20018 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.748013 erlab-2.4.1/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52053 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114641 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27909 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    57794 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    14551 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25660 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    16051 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19382 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     2749 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    55581 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.748013 erlab-2.4.1/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     2194 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.748013 erlab-2.4.1/src/erlab/io/characterization/
--rw-r--r--   0 root         (0) root         (0)      170 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/io/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3058 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/io/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1981 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/io/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)    43727 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)    12313 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/io/exampledata.py
--rw-r--r--   0 root         (0) root         (0)     6998 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.748013 erlab-2.4.1/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3811 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     8166 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7667 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     6737 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2528 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     1522 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.752013 erlab-2.4.1/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.752013 erlab-2.4.1/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     2113 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30641 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18686 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4420 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    39760 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    37467 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2739 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.756013 erlab-2.4.1/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-05-03 08:53:14.000000 erlab-2.4.1/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.756013 erlab-2.4.1/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    48438 2024-05-03 08:53:21.000000 erlab-2.4.1/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4937 2024-05-03 08:53:21.000000 erlab-2.4.1/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 08:53:21.000000 erlab-2.4.1/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-03 08:53:21.000000 erlab-2.4.1/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-03 08:53:21.000000 erlab-2.4.1/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.756013 erlab-2.4.1/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-05-03 08:53:14.000000 erlab-2.4.1/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-05-03 08:53:14.000000 erlab-2.4.1/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-03 08:53:14.000000 erlab-2.4.1/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.720012 erlab-2.4.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.756013 erlab-2.4.1/tests/accessors/
--rw-r--r--   0 root         (0) root         (0)     5785 2024-05-03 08:53:14.000000 erlab-2.4.1/tests/accessors/test_fit.py
--rw-r--r--   0 root         (0) root         (0)     4035 2024-05-03 08:53:14.000000 erlab-2.4.1/tests/accessors/test_kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.756013 erlab-2.4.1/tests/analysis/
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-03 08:53:14.000000 erlab-2.4.1/tests/analysis/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     4497 2024-05-03 08:53:14.000000 erlab-2.4.1/tests/analysis/test_fit_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4794 2024-05-03 08:53:14.000000 erlab-2.4.1/tests/analysis/test_fit_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     6035 2024-05-03 08:53:14.000000 erlab-2.4.1/tests/analysis/test_fit_models.py
--rw-r--r--   0 root         (0) root         (0)     5228 2024-05-03 08:53:14.000000 erlab-2.4.1/tests/analysis/test_image.py
--rw-r--r--   0 root         (0) root         (0)     3126 2024-05-03 08:53:14.000000 erlab-2.4.1/tests/analysis/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     1513 2024-05-03 08:53:14.000000 erlab-2.4.1/tests/analysis/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-05-03 08:53:14.000000 erlab-2.4.1/tests/analysis/test_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:53:21.756013 erlab-2.4.1/tests/io/
--rw-r--r--   0 root         (0) root         (0)     9385 2024-05-03 08:53:14.000000 erlab-2.4.1/tests/io/test_dataloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.013511 erlab-2.4.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.965511 erlab-2.4.2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.973511 erlab-2.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-05-07 12:07:26.000000 erlab-2.4.2/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-07 12:07:26.000000 erlab-2.4.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-07 12:07:26.000000 erlab-2.4.2/.github/ISSUE_TEMPLATE/feature-request.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.973511 erlab-2.4.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-05-07 12:07:26.000000 erlab-2.4.2/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-07 12:07:26.000000 erlab-2.4.2/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-07 12:07:26.000000 erlab-2.4.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      893 2024-05-07 12:07:26.000000 erlab-2.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      793 2024-05-07 12:07:26.000000 erlab-2.4.2/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   124266 2024-05-07 12:07:30.000000 erlab-2.4.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-05-07 12:07:26.000000 erlab-2.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    48438 2024-05-07 12:07:35.013511 erlab-2.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-05-07 12:07:26.000000 erlab-2.4.2/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     5147 2024-05-07 12:07:26.000000 erlab-2.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.973511 erlab-2.4.2/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      726 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.977511 erlab-2.4.2/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    17977 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    15203 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     5039 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.985511 erlab-2.4.2/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   328062 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   328737 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.985511 erlab-2.4.2/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2604 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     3099 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.989511 erlab-2.4.2/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)    41238 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/curve-fitting.ipynb
+-rw-r--r--   0 root         (0) root         (0)     2598 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/imagetool.rst
+-rw-r--r--   0 root         (0) root         (0)     1291 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)    12039 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    54817 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)    10710 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    27564 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-07 12:07:26.000000 erlab-2.4.2/environment.yml
+-rw-r--r--   0 root         (0) root         (0)     5353 2024-05-07 12:07:26.000000 erlab-2.4.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      315 2024-05-07 12:07:26.000000 erlab-2.4.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 12:07:35.013511 erlab-2.4.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.969511 erlab-2.4.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.989511 erlab-2.4.2/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-07 12:07:30.000000 erlab-2.4.2/src/erlab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.989511 erlab-2.4.2/src/erlab/accessors/
+-rw-r--r--   0 root         (0) root         (0)      792 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/accessors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26123 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/accessors/fit.py
+-rw-r--r--   0 root         (0) root         (0)    30007 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/accessors/kspace.py
+-rw-r--r--   0 root         (0) root         (0)     7071 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/accessors/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.993511 erlab-2.4.2/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      880 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.993511 erlab-2.4.2/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.993511 erlab-2.4.2/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10779 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     9594 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)    12739 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    20223 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    18221 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)    14968 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.993511 erlab-2.4.2/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     5397 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8505 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5443 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.993511 erlab-2.4.2/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      232 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.997511 erlab-2.4.2/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      526 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14330 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    21371 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    23024 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11891 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)    19282 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.997511 erlab-2.4.2/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    20018 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.997511 erlab-2.4.2/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52053 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114641 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27909 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    57841 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    14551 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25660 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    15911 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19321 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    55581 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.001511 erlab-2.4.2/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.001511 erlab-2.4.2/src/erlab/io/characterization/
+-rw-r--r--   0 root         (0) root         (0)      170 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)    43727 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    12313 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)     6998 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.001511 erlab-2.4.2/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     8166 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7667 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     6737 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.001511 erlab-2.4.2/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.005511 erlab-2.4.2/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30641 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18686 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    39760 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    37467 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.005511 erlab-2.4.2/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.009511 erlab-2.4.2/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    48438 2024-05-07 12:07:34.000000 erlab-2.4.2/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4937 2024-05-07 12:07:34.000000 erlab-2.4.2/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 12:07:34.000000 erlab-2.4.2/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-07 12:07:34.000000 erlab-2.4.2/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-07 12:07:34.000000 erlab-2.4.2/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.005511 erlab-2.4.2/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-07 12:07:26.000000 erlab-2.4.2/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-05-07 12:07:26.000000 erlab-2.4.2/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-07 12:07:26.000000 erlab-2.4.2/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.969511 erlab-2.4.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.009511 erlab-2.4.2/tests/accessors/
+-rw-r--r--   0 root         (0) root         (0)     5785 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/accessors/test_fit.py
+-rw-r--r--   0 root         (0) root         (0)     4035 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/accessors/test_kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.009511 erlab-2.4.2/tests/analysis/
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     4497 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_fit_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4794 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_fit_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     6035 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_fit_models.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)     3126 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.009511 erlab-2.4.2/tests/io/
+-rw-r--r--   0 root         (0) root         (0)     9385 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/io/test_dataloader.py
```

### Comparing `erlab-2.4.1/.github/ISSUE_TEMPLATE/bug-report.yml` & `erlab-2.4.2/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/.github/ISSUE_TEMPLATE/feature-request.yml` & `erlab-2.4.2/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/.github/workflows/pr.yml` & `erlab-2.4.2/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/.github/workflows/release.yml` & `erlab-2.4.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/.gitignore` & `erlab-2.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/.pre-commit-config.yaml` & `erlab-2.4.2/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,14 @@
       - id: check-merge-conflict
       - id: mixed-line-ending
       - id: check-ast
 
   # Lint and format with ruff
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.4.2
+    rev: v0.4.3
     hooks:
       # Run the linter.
       - id: ruff
         args: [ --fix ]
       # Run the formatter.
       - id: ruff-format
```

### Comparing `erlab-2.4.1/.readthedocs.yaml` & `erlab-2.4.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/CHANGELOG.md` & `erlab-2.4.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,31 @@
 # CHANGELOG
 
 
 
+## v2.4.2 (2024-05-07)
+
+### Fix
+
+* (**ktool**) resolve ktool initialization problem, closes #32 ([`e88a58e`](https://github.com/kmnhan/erlabpy/commit/e88a58e6aaed326af1a68aa33322d6ea9f0e800d))
+
+* (**itool**) disable flag checking for non-numpy arrays ([`da6eb1d`](https://github.com/kmnhan/erlabpy/commit/da6eb1db9e81d51b52d4b361de938bcf7ba45e68))
+
+### Unknown
+
+* Merge pull request #31 from kmnhan/pre-commit-ci-update-config ([`e3a4a9f`](https://github.com/kmnhan/erlabpy/commit/e3a4a9f6bda7a21d824ecfc0d70e2e1419898cbf))
+
+  [pre-commit.ci] pre-commit autoupdate
+
+* [pre-commit.ci] pre-commit autoupdate ([`ec62bea`](https://github.com/kmnhan/erlabpy/commit/ec62bea6af2b4074f77ef11a2ddf82b7b7a4db33))
+
+  updates:
+  - [github.com/astral-sh/ruff-pre-commit: v0.4.2 → v0.4.3](https://github.com/astral-sh/ruff-pre-commit/compare/v0.4.2...v0.4.3)
+
+
 ## v2.4.1 (2024-05-03)
 
 ### Fix
 
 * (**plotting**) fix wrong regex in `scale_units` ([`d7826d0`](https://github.com/kmnhan/erlabpy/commit/d7826d0269214dfd822a4d0293e42a9840015ce8))
 
 * fix bug in `modelfit` parameter concatenation ([`edaa556`](https://github.com/kmnhan/erlabpy/commit/edaa5566c6e3817e1d9220f7a96e8e731cf7eede))
```

### Comparing `erlab-2.4.1/LICENSE` & `erlab-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/PKG-INFO` & `erlab-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.4.1
+Version: 2.4.2
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.4.1/PythonInterface.ipf` & `erlab-2.4.2/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/README.md` & `erlab-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/Makefile` & `erlab-2.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/environment.yml` & `erlab-2.4.2/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/make.bat` & `erlab-2.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/conf.py` & `erlab-2.4.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/contributing.rst` & `erlab-2.4.2/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/getting-started.rst` & `erlab-2.4.2/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/images/flowchart_multiple.pdf` & `erlab-2.4.2/docs/source/images/flowchart_multiple.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/images/flowchart_single.pdf` & `erlab-2.4.2/docs/source/images/flowchart_single.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/images/imagetool_dark.png` & `erlab-2.4.2/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/images/imagetool_light.png` & `erlab-2.4.2/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/images/ktool_1_dark.png` & `erlab-2.4.2/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/images/ktool_1_light.png` & `erlab-2.4.2/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/images/ktool_2_dark.png` & `erlab-2.4.2/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/images/ktool_2_light.png` & `erlab-2.4.2/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/index.rst` & `erlab-2.4.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/pyplots/norms.py` & `erlab-2.4.2/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/reference.rst` & `erlab-2.4.2/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/refs.bib` & `erlab-2.4.2/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/user-guide/curve-fitting.ipynb` & `erlab-2.4.2/docs/source/user-guide/curve-fitting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/user-guide/imagetool.rst` & `erlab-2.4.2/docs/source/user-guide/imagetool.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/user-guide/index.rst` & `erlab-2.4.2/docs/source/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/user-guide/indexing.ipynb` & `erlab-2.4.2/docs/source/user-guide/indexing.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/user-guide/io.ipynb` & `erlab-2.4.2/docs/source/user-guide/io.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/user-guide/kconv.ipynb` & `erlab-2.4.2/docs/source/user-guide/kconv.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/docs/source/user-guide/plotting.ipynb` & `erlab-2.4.2/docs/source/user-guide/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/pyproject.toml` & `erlab-2.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/accessors/__init__.py` & `erlab-2.4.2/src/erlab/accessors/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/accessors/fit.py` & `erlab-2.4.2/src/erlab/accessors/fit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/accessors/kspace.py` & `erlab-2.4.2/src/erlab/accessors/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/accessors/utils.py` & `erlab-2.4.2/src/erlab/accessors/utils.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/__init__.py` & `erlab-2.4.2/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/correlation.py` & `erlab-2.4.2/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.4.2/src/erlab/analysis/fit/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.4.2/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/fit/functions/general.py` & `erlab-2.4.2/src/erlab/analysis/fit/functions/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/fit/minuit.py` & `erlab-2.4.2/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/fit/models.py` & `erlab-2.4.2/src/erlab/analysis/fit/models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/fit/spline.py` & `erlab-2.4.2/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/gold.py` & `erlab-2.4.2/src/erlab/analysis/gold.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/image.py` & `erlab-2.4.2/src/erlab/analysis/image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/interpolate.py` & `erlab-2.4.2/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/kspace.py` & `erlab-2.4.2/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/mask/__init__.py` & `erlab-2.4.2/src/erlab/analysis/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/mask/polygon.py` & `erlab-2.4.2/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/transform.py` & `erlab-2.4.2/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/analysis/utilities.py` & `erlab-2.4.2/src/erlab/analysis/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/constants.py` & `erlab-2.4.2/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/__init__.py` & `erlab-2.4.2/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/bzplot.py` & `erlab-2.4.2/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/colors.py` & `erlab-2.4.2/src/erlab/interactive/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/curvefittingtool.py` & `erlab-2.4.2/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/derivative.py` & `erlab-2.4.2/src/erlab/interactive/derivative.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,18 @@
 
 class DerivativeTool(
     *uic.loadUiType(os.path.join(os.path.dirname(__file__), "dtool.ui"))  # type: ignore[misc]
 ):
     def __init__(self, data: xr.DataArray, *, data_name: str | None = None):
         if data_name is None:
             try:
-                data_name = varname.argname("data", func=self.__init__, vars_only=False)  # type: ignore[misc]
+                data_name = cast(
+                    str,
+                    varname.argname("data", func=self.__init__, vars_only=False),  # type: ignore[misc]
+                )
             except varname.VarnameRetrievingError:
                 data_name = "data"
 
         self.data_name: str = data_name
 
         # Initialize UI
         super().__init__()
@@ -305,15 +308,15 @@
 
         copy_to_clipboard(lines)
 
 
 def dtool(data, data_name: str | None = None, *, execute: bool | None = None):
     if data_name is None:
         try:
-            data_name = varname.argname("data", func=dtool, vars_only=False)
+            data_name = varname.argname("data", func=dtool, vars_only=False)  # type: ignore[assignment]
         except varname.VarnameRetrievingError:
             data_name = "data"
 
     qapp = QtWidgets.QApplication.instance()
     if not qapp:
         qapp = QtWidgets.QApplication(sys.argv)
```

### Comparing `erlab-2.4.1/src/erlab/interactive/dtool.ui` & `erlab-2.4.2/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/fermiedge.py` & `erlab-2.4.2/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.4.2/src/erlab/interactive/imagetool/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.4.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.4.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/imagetool/controls.py` & `erlab-2.4.2/src/erlab/interactive/imagetool/controls.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/imagetool/core.py` & `erlab-2.4.2/src/erlab/interactive/imagetool/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -649,17 +649,17 @@
             n_cursors_old = 1
 
         if not isinstance(data, xr.DataArray):
             if isinstance(data, xr.Dataset):
                 data = data[next(iter(data.data_vars.keys()))]
             else:
                 data = xr.DataArray(np.asarray(data))
-
-        if not data.data.flags["WRITEABLE"]:
-            data = data.copy()
+        if hasattr(data.data, "flags"):
+            if not data.data.flags["WRITEABLE"]:
+                data = data.copy()
 
         if not rad2deg:
             self._data = data
         else:
             if np.iterable(rad2deg):
                 conv_dims = rad2deg
             else:
```

### Comparing `erlab-2.4.1/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.4.2/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.4.2/src/erlab/interactive/imagetool/slicer.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/kspace.py` & `erlab-2.4.2/src/erlab/interactive/kspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Interactive momentum conversion tool."""
 
 __all__ = ["ktool"]
 
 import os
 import sys
+from typing import cast
 
 import numpy as np
 import numpy.typing as npt
 import pyqtgraph as pg
 import varname
 import xarray as xr
-from qtpy import QtCore, QtGui, QtWidgets, uic
+from qtpy import QtGui, QtWidgets, uic
 
 import erlab.analysis
 from erlab.interactive.colors import (
     BetterColorBarItem,  # noqa: F401
     ColorMapComboBox,  # noqa: F401
     ColorMapGammaWidget,  # noqa: F401
 )
@@ -23,20 +24,14 @@
 from erlab.plotting.bz import get_bz_edge
 
 
 class KspaceToolGUI(
     *uic.loadUiType(os.path.join(os.path.dirname(__file__), "ktool.ui"))  # type: ignore[misc]
 ):
     def __init__(self):
-        # Start the QApplication if it doesn't exist
-        self.qapp = QtCore.QCoreApplication.instance()
-        if not self.qapp:
-            self.qapp = QtWidgets.QApplication(sys.argv)
-        self.qapp.setStyle("Fusion")
-
         # Initialize UI
         super().__init__()
         self.setupUi(self)
         self.setWindowTitle("Momentum Conversion")
 
         self.plotitems: tuple[pg.PlotItem, pg.PlotItem] = (pg.PlotItem(), pg.PlotItem())
         self.images: tuple[xImageItem, xImageItem] = (
@@ -122,33 +117,14 @@
                 symbol="o",
                 pen=pg.mkColor(255, 255, 255, 0),
                 symbolPen=pg.mkColor(255, 255, 255, 0),
                 symbolBrush=pg.mkColor("m"),
                 symbolSize=6,
             )
 
-    def __post_init__(self, execute=None):
-        self.show()
-        self.raise_()
-        self.activateWindow()
-
-        if execute is None:
-            execute = True
-            try:
-                shell = get_ipython().__class__.__name__  # type: ignore
-                if shell in ["ZMQInteractiveShell", "TerminalInteractiveShell"]:
-                    execute = False
-                    from IPython.lib.guisupport import start_event_loop_qt4
-
-                    start_event_loop_qt4(self.qapp)
-            except NameError:
-                pass
-        if execute:
-            self.qapp.exec()
-
 
 class KspaceTool(KspaceToolGUI):
     def __init__(self, data: xr.DataArray, *, data_name: str | None = None):
         super().__init__()
 
         self._argnames = {}
 
@@ -238,16 +214,14 @@
         for pi in self.plotitems:
             if self.data.kspace.has_beta and not self.data.kspace.has_hv:
                 pi.vb.setAspectLocked(lock=True, ratio=1)
         self.open_btn.clicked.connect(self.show_converted)
         self.copy_btn.clicked.connect(self.copy_code)
         self.update()
 
-        self.__post_init__()
-
     def calculate_resolution(self):
         for k, spin in self._resolution_spins.items():
             spin.setValue(
                 self.data.kspace.estimate_resolution(
                     k, from_numpoints=self.res_npts_check.isChecked()
                 )
             )
@@ -415,22 +389,48 @@
         return lines, vertices
 
     def closeEvent(self, event: QtGui.QCloseEvent):
         del self.data
         super().closeEvent(event)
 
 
-def ktool(data: xr.DataArray, *, data_name: str | None = None) -> KspaceTool:
+def ktool(
+    data: xr.DataArray, *, data_name: str | None = None, execute: bool | None = None
+) -> KspaceTool:
     """Interactive momentum conversion tool."""
     if data_name is None:
         try:
-            data_name = varname.argname("data", func=ktool, vars_only=False)
+            data_name = varname.argname("data", func=ktool, vars_only=False)  # type: ignore[assignment]
         except varname.VarnameRetrievingError:
             data_name = "data"
-    return KspaceTool(data, data_name=data_name)
 
+    qapp = QtWidgets.QApplication.instance()
+    if not qapp:
+        qapp = QtWidgets.QApplication(sys.argv)
+
+    cast(QtWidgets.QApplication, qapp).setStyle("Fusion")
+
+    win = KspaceTool(data, data_name=data_name)
+    win.show()
+    win.raise_()
+    win.activateWindow()
 
-if __name__ == "__main__":
-    from typing import cast
+    if execute is None:
+        execute = True
+        try:
+            shell = get_ipython().__class__.__name__  # type: ignore
+            if shell in ["ZMQInteractiveShell", "TerminalInteractiveShell"]:
+                execute = False
+                from IPython.lib.guisupport import start_event_loop_qt4
+
+                start_event_loop_qt4(qapp)
+        except NameError:
+            pass
+    if execute:
+        qapp.exec()
+
+    return win
 
+
+if __name__ == "__main__":
     dat = cast(xr.DataArray, erlab.io.load_hdf5("/Users/khan/2210_ALS_f0008.h5"))
     win = ktool(dat)
```

### Comparing `erlab-2.4.1/src/erlab/interactive/ktool.ui` & `erlab-2.4.2/src/erlab/interactive/ktool.ui`

 * *Files 2% similar despite different names*

#### Comparing `erlab-2.4.1/src/erlab/interactive/ktool.ui` & `erlab-2.4.2/src/erlab/interactive/ktool.ui`

```diff
@@ -2,16 +2,16 @@
 <ui version="4.0">
   <class>MainWindow</class>
   <widget class="QMainWindow" name="MainWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>750</width>
-        <height>300</height>
+        <width>759</width>
+        <height>667</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>MainWindow</string>
     </property>
     <widget class="QWidget" name="centralwidget">
       <layout class="QHBoxLayout" name="horizontalLayout_2">
@@ -20,18 +20,18 @@
             <property name="sizePolicy">
               <sizepolicy hsizetype="Maximum" vsizetype="Expanding">
                 <horstretch>0</horstretch>
                 <verstretch>0</verstretch>
               </sizepolicy>
             </property>
             <property name="tabPosition">
-              <enum>QTabWidget::West</enum>
+              <enum>QTabWidget::TabPosition::West</enum>
             </property>
             <property name="tabShape">
-              <enum>QTabWidget::Rounded</enum>
+              <enum>QTabWidget::TabShape::Rounded</enum>
             </property>
             <property name="currentIndex">
               <number>0</number>
             </property>
             <widget class="QWidget" name="tab">
               <attribute name="title">
                 <string>Parameters</string>
@@ -112,15 +112,15 @@
                             </property>
                           </layout>
                         </widget>
                       </item>
                       <item>
                         <widget class="QPushButton" name="res_btn">
                           <property name="toolTip">
-                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Estimate momentum resolution from the data.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                            <string>Estimate momentum resolution from the data.</string>
                           </property>
                           <property name="text">
                             <string>Estimate</string>
                           </property>
                         </widget>
                       </item>
                       <item>
@@ -170,15 +170,15 @@
                     </property>
                     <layout class="QVBoxLayout" name="verticalLayout_3">
                       <item>
                         <layout class="QFormLayout" name="bz_form">
                           <item row="0" column="0">
                             <widget class="QLabel" name="label">
                               <property name="text">
-                                <string>𝒂</string>
+                                <string>a</string>
                               </property>
                             </widget>
                           </item>
                           <item row="0" column="1">
                             <widget class="QDoubleSpinBox" name="a_spin">
                               <property name="keyboardTracking">
                                 <bool>false</bool>
@@ -196,15 +196,15 @@
                                 <double>3.540000000000000</double>
                               </property>
                             </widget>
                           </item>
                           <item row="1" column="0">
                             <widget class="QLabel" name="label_2">
                               <property name="text">
-                                <string>𝒃</string>
+                                <string>b</string>
                               </property>
                             </widget>
                           </item>
                           <item row="1" column="1">
                             <widget class="QDoubleSpinBox" name="b_spin">
                               <property name="keyboardTracking">
                                 <bool>false</bool>
@@ -251,15 +251,15 @@
                                 <string>ang</string>
                               </property>
                             </widget>
                           </item>
                           <item row="3" column="0">
                             <widget class="QLabel" name="label_13">
                               <property name="text">
-                                <string>𝒄</string>
+                                <string>c</string>
                               </property>
                             </widget>
                           </item>
                           <item row="3" column="1">
                             <widget class="QDoubleSpinBox" name="c_spin">
                               <property name="keyboardTracking">
                                 <bool>false</bool>
@@ -296,15 +296,15 @@
                                 <double>3.540000000000000</double>
                               </property>
                             </widget>
                           </item>
                           <item row="4" column="0">
                             <widget class="QLabel" name="label_14">
                               <property name="text">
-                                <string>𝒂 or 𝒃</string>
+                                <string>a or b</string>
                               </property>
                             </widget>
                           </item>
                           <item row="5" column="1">
                             <widget class="QDoubleSpinBox" name="rot_spin">
                               <property name="keyboardTracking">
                                 <bool>false</bool>
@@ -502,15 +502,15 @@
                       </item>
                     </layout>
                   </widget>
                 </item>
                 <item>
                   <spacer name="verticalSpacer">
                     <property name="orientation">
-                      <enum>Qt::Vertical</enum>
+                      <enum>Qt::Orientation::Vertical</enum>
                     </property>
                     <property name="sizeHint" stdset="0">
                       <size>
                         <width>20</width>
                         <height>40</height>
                       </size>
                     </property>
@@ -543,16 +543,16 @@
       </layout>
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
-          <width>750</width>
-          <height>21</height>
+          <width>759</width>
+          <height>24</height>
         </rect>
       </property>
     </widget>
   </widget>
   <customwidgets>
     <customwidget>
       <class>GraphicsLayoutWidget</class>
```

### Comparing `erlab-2.4.1/src/erlab/interactive/masktool.py` & `erlab-2.4.2/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/interactive/utilities.py` & `erlab-2.4.2/src/erlab/interactive/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/io/__init__.py` & `erlab-2.4.2/src/erlab/io/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/io/characterization/resistance.py` & `erlab-2.4.2/src/erlab/io/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/io/characterization/xrd.py` & `erlab-2.4.2/src/erlab/io/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/io/dataloader.py` & `erlab-2.4.2/src/erlab/io/dataloader.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/io/exampledata.py` & `erlab-2.4.2/src/erlab/io/exampledata.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/io/igor.py` & `erlab-2.4.2/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/io/plugins/__init__.py` & `erlab-2.4.2/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/io/plugins/da30.py` & `erlab-2.4.2/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/io/plugins/kriss.py` & `erlab-2.4.2/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/io/plugins/merlin.py` & `erlab-2.4.2/src/erlab/io/plugins/merlin.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/io/plugins/ssrl52.py` & `erlab-2.4.2/src/erlab/io/plugins/ssrl52.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/io/utilities.py` & `erlab-2.4.2/src/erlab/io/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/lattice.py` & `erlab-2.4.2/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/parallel.py` & `erlab-2.4.2/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.4.2/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.4.2/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.4.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.4.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.4.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.4.2/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.4.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.4.2/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.4.2/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.4.2/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/__init__.py` & `erlab-2.4.2/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/annotations.py` & `erlab-2.4.2/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/atoms.py` & `erlab-2.4.2/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/bz.py` & `erlab-2.4.2/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/colors.py` & `erlab-2.4.2/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/erplot.py` & `erlab-2.4.2/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/general.py` & `erlab-2.4.2/src/erlab/plotting/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/plot3d.py` & `erlab-2.4.2/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.4.2/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.4.2/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.4.2/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.4.2/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.4.2/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.4.2/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab.egg-info/PKG-INFO` & `erlab-2.4.2/src/erlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.4.1
+Version: 2.4.2
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.4.1/src/erlab.egg-info/SOURCES.txt` & `erlab-2.4.2/src/erlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/src/erlab.egg-info/requires.txt` & `erlab-2.4.2/src/erlab.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/templates/.macros.j2` & `erlab-2.4.2/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/tests/accessors/test_fit.py` & `erlab-2.4.2/tests/accessors/test_fit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/tests/accessors/test_kspace.py` & `erlab-2.4.2/tests/accessors/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/tests/analysis/test_fastbinning.py` & `erlab-2.4.2/tests/analysis/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/tests/analysis/test_fit_functions_dynamic.py` & `erlab-2.4.2/tests/analysis/test_fit_functions_dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/tests/analysis/test_fit_functions_general.py` & `erlab-2.4.2/tests/analysis/test_fit_functions_general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/tests/analysis/test_fit_models.py` & `erlab-2.4.2/tests/analysis/test_fit_models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/tests/analysis/test_image.py` & `erlab-2.4.2/tests/analysis/test_image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/tests/analysis/test_interpolate.py` & `erlab-2.4.2/tests/analysis/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/tests/analysis/test_kspace.py` & `erlab-2.4.2/tests/analysis/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/tests/analysis/test_utilities.py` & `erlab-2.4.2/tests/analysis/test_utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.1/tests/io/test_dataloader.py` & `erlab-2.4.2/tests/io/test_dataloader.py`

 * *Files identical despite different names*

