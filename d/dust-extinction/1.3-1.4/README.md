# Comparing `tmp/dust_extinction-1.3.tar.gz` & `tmp/dust_extinction-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dust_extinction-1.3.tar", last modified: Tue Nov 28 18:15:58 2023, max compression
+gzip compressed data, was "dust_extinction-1.4.tar", last modified: Tue May  7 19:41:30 2024, max compression
```

## Comparing `dust_extinction-1.3.tar` & `dust_extinction-1.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2023-11-28 18:15:58.674654 dust_extinction-1.3/
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2023-11-28 18:15:58.660655 dust_extinction-1.3/.github/
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2023-11-28 18:15:58.661655 dust_extinction-1.3/.github/workflows/
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     4800 2023-11-28 13:31:44.000000 dust_extinction-1.3/.github/workflows/tox-tests.yml
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      720 2022-01-04 15:34:07.000000 dust_extinction-1.3/.gitignore
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)      219 2023-11-28 13:31:44.000000 dust_extinction-1.3/.readthedocs.yml
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1328 2023-11-28 18:06:15.000000 dust_extinction-1.3/CHANGES.rst
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)      367 2023-04-19 09:36:19.000000 dust_extinction-1.3/CITATION.cff
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1516 2023-11-28 17:20:24.000000 dust_extinction-1.3/LICENSE
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      305 2022-01-04 15:34:07.000000 dust_extinction-1.3/MANIFEST.in
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     5730 2023-11-28 18:15:58.674654 dust_extinction-1.3/PKG-INFO
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     5144 2023-11-28 13:31:44.000000 dust_extinction-1.3/README.rst
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2023-11-28 18:15:58.662654 dust_extinction-1.3/docs/
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4581 2022-01-04 15:34:07.000000 dust_extinction-1.3/docs/Makefile
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2023-11-28 18:15:58.660655 dust_extinction-1.3/docs/_templates/
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2023-11-28 18:15:58.663655 dust_extinction-1.3/docs/_templates/autosummary/
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      250 2022-01-04 15:34:07.000000 dust_extinction-1.3/docs/_templates/autosummary/base.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      251 2022-01-04 15:34:07.000000 dust_extinction-1.3/docs/_templates/autosummary/class.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      252 2022-01-04 15:34:07.000000 dust_extinction-1.3/docs/_templates/autosummary/module.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     7210 2022-01-04 15:34:07.000000 dust_extinction-1.3/docs/conf.py
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2023-11-28 18:15:58.663655 dust_extinction-1.3/docs/dust_extinction/
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)    11499 2023-11-28 17:49:38.000000 dust_extinction-1.3/docs/dust_extinction/choose_model.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4220 2022-01-04 15:34:07.000000 dust_extinction-1.3/docs/dust_extinction/extinction.rst
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2521 2023-04-04 15:22:25.000000 dust_extinction-1.3/docs/dust_extinction/extinguish.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4666 2022-01-04 15:34:07.000000 dust_extinction-1.3/docs/dust_extinction/fit_extinction.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      774 2022-01-04 15:34:07.000000 dust_extinction-1.3/docs/dust_extinction/install.rst
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)    18181 2023-11-28 17:49:38.000000 dust_extinction-1.3/docs/dust_extinction/model_flavors.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      330 2022-01-04 15:34:07.000000 dust_extinction-1.3/docs/dust_extinction/reference_api.rst
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     3396 2023-11-28 17:20:24.000000 dust_extinction-1.3/docs/dust_extinction/references.rst
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     6024 2023-11-28 13:31:44.000000 dust_extinction-1.3/docs/index.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4549 2022-01-04 15:34:07.000000 dust_extinction-1.3/docs/make.bat
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2023-11-28 18:15:58.665655 dust_extinction-1.3/dust_extinction/
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)      174 2023-11-28 17:49:38.000000 dust_extinction-1.3/dust_extinction/__init__.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    38499 2022-03-30 13:46:42.000000 dust_extinction-1.3/dust_extinction/averages.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4020 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/baseclasses.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1957 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/conftest.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1149 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/conversions.py
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2023-11-28 18:15:58.671655 dust_extinction-1.3/dust_extinction/data/
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4924 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/CT06_pixiedust.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     8758 2022-03-30 13:46:42.000000 dust_extinction-1.3/dust_extinction/data/D22.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1513 2022-03-30 13:46:42.000000 dust_extinction-1.3/dust_extinction/data/D22_Rv_slope.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   145064 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/EXT_C11.RES.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    90880 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/EXT_DBP90.RES.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   121046 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/EXT_J13.RES.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     3193 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/F19_tabulated.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2724 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/G21_IRS.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    16186 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/G21_IRS_fullres.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      550 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/G21_PHOT.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1868 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/GCC09_FUSE.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     7385 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/GCC09_IUE.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      181 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/GCC09_PHOT.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      246 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/README.rst
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)  3098880 2023-11-28 17:20:24.000000 dust_extinction-1.3/dust_extinction/data/astrodust+PAH_MW_RV3.1.fits
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      373 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/fritz11_galcenter.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110119 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_LMC2_10.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110125 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_LMCavg_20.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110428 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_MW_3.1_60.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    64842 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_MW_3.1_60_D03.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    64842 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_MW_4.0A_40_D03.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110130 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_MW_4.0B_40.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    64849 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_MW_5.5A_30_D03.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110130 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_MW_5.5B_30.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110116 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_SMCbar_0.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    32453 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/data/zubko2004_bare-gr-s_alam_av.dat
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)    16750 2023-11-28 17:20:24.000000 dust_extinction-1.3/dust_extinction/grain_models.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2203 2023-04-19 09:36:19.000000 dust_extinction-1.3/dust_extinction/helpers.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)    44111 2023-04-19 09:36:19.000000 dust_extinction-1.3/dust_extinction/parameter_averages.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)    25764 2023-11-28 17:49:38.000000 dust_extinction-1.3/dust_extinction/shapes.py
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2023-11-28 18:15:58.673654 dust_extinction-1.3/dust_extinction/tests/
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      108 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/tests/__init__.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1524 2023-11-28 17:49:38.000000 dust_extinction-1.3/dust_extinction/tests/helpers.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2466 2023-04-04 14:41:44.000000 dust_extinction-1.3/dust_extinction/tests/test_axavtoexv.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     5520 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/tests/test_ccm89.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     5220 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/tests/test_corvals.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1225 2022-03-04 18:58:24.000000 dust_extinction-1.3/dust_extinction/tests/test_corvals_aves.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1222 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/tests/test_corvals_grainmods.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2307 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/tests/test_fm90.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2095 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/tests/test_g16.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2971 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/tests/test_gcc09.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     3699 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/tests/test_o94.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     3860 2023-04-04 14:41:44.000000 dust_extinction-1.3/dust_extinction/tests/test_p92.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1896 2022-01-04 15:34:07.000000 dust_extinction-1.3/dust_extinction/tests/test_vcg04.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2894 2022-03-30 13:46:42.000000 dust_extinction-1.3/dust_extinction/tests/test_warnings.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)      335 2023-11-28 18:15:58.000000 dust_extinction-1.3/dust_extinction/version.py
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2023-11-28 18:15:58.673654 dust_extinction-1.3/dust_extinction.egg-info/
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     5730 2023-11-28 18:15:58.000000 dust_extinction-1.3/dust_extinction.egg-info/PKG-INFO
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2807 2023-11-28 18:15:58.000000 dust_extinction-1.3/dust_extinction.egg-info/SOURCES.txt
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)        1 2023-11-28 18:15:58.000000 dust_extinction-1.3/dust_extinction.egg-info/dependency_links.txt
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)        1 2023-04-04 15:41:14.000000 dust_extinction-1.3/dust_extinction.egg-info/not-zip-safe
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)       80 2023-11-28 18:15:58.000000 dust_extinction-1.3/dust_extinction.egg-info/requires.txt
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)       16 2023-11-28 18:15:58.000000 dust_extinction-1.3/dust_extinction.egg-info/top_level.txt
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2023-11-28 18:15:58.673654 dust_extinction-1.3/licenses/
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1483 2022-01-04 15:34:07.000000 dust_extinction-1.3/licenses/LICENSE.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      134 2022-01-04 15:34:07.000000 dust_extinction-1.3/pyproject.toml
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1773 2023-11-28 18:15:58.675655 dust_extinction-1.3/setup.cfg
--rwxrwxr-x   0 kgordon   (1000) kgordon   (1000)     1964 2022-01-04 15:34:07.000000 dust_extinction-1.3/setup.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2305 2023-11-28 13:31:44.000000 dust_extinction-1.3/tox.ini
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.328994 dust_extinction-1.4/
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.319994 dust_extinction-1.4/.github/
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.320994 dust_extinction-1.4/.github/workflows/
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     4803 2024-05-07 15:29:44.000000 dust_extinction-1.4/.github/workflows/tox-tests.yml
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      720 2022-01-04 15:34:07.000000 dust_extinction-1.4/.gitignore
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)      219 2023-11-28 13:31:44.000000 dust_extinction-1.4/.readthedocs.yml
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1356 2024-05-07 19:41:12.000000 dust_extinction-1.4/CHANGES.rst
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)      367 2023-04-19 09:36:19.000000 dust_extinction-1.4/CITATION.cff
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1517 2024-05-07 15:08:39.000000 dust_extinction-1.4/LICENSE
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      305 2022-01-04 15:34:07.000000 dust_extinction-1.4/MANIFEST.in
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     5695 2024-05-07 19:41:30.328994 dust_extinction-1.4/PKG-INFO
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     5144 2023-11-28 13:31:44.000000 dust_extinction-1.4/README.rst
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.321994 dust_extinction-1.4/docs/
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4581 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/Makefile
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.319994 dust_extinction-1.4/docs/_templates/
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.321994 dust_extinction-1.4/docs/_templates/autosummary/
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      250 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/_templates/autosummary/base.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      251 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/_templates/autosummary/class.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      252 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/_templates/autosummary/module.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     7210 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/conf.py
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.322994 dust_extinction-1.4/docs/dust_extinction/
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)    11854 2024-05-07 19:37:16.000000 dust_extinction-1.4/docs/dust_extinction/choose_model.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4220 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/dust_extinction/extinction.rst
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2521 2023-04-04 15:22:25.000000 dust_extinction-1.4/docs/dust_extinction/extinguish.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4666 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/dust_extinction/fit_extinction.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      774 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/dust_extinction/install.rst
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)    18458 2024-05-07 19:37:16.000000 dust_extinction-1.4/docs/dust_extinction/model_flavors.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      330 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/dust_extinction/reference_api.rst
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     3436 2024-05-07 19:37:16.000000 dust_extinction-1.4/docs/dust_extinction/references.rst
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     6155 2024-01-18 14:25:03.000000 dust_extinction-1.4/docs/index.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4549 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/make.bat
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.322994 dust_extinction-1.4/dust_extinction/
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)      174 2023-11-28 17:49:38.000000 dust_extinction-1.4/dust_extinction/__init__.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)    44332 2024-05-07 19:37:16.000000 dust_extinction-1.4/dust_extinction/averages.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     3954 2024-03-19 17:36:34.000000 dust_extinction-1.4/dust_extinction/baseclasses.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1961 2023-11-28 19:59:56.000000 dust_extinction-1.4/dust_extinction/conftest.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1149 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/conversions.py
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.327994 dust_extinction-1.4/dust_extinction/data/
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4924 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/CT06_pixiedust.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     8758 2022-03-30 13:46:42.000000 dust_extinction-1.4/dust_extinction/data/D22.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1513 2022-03-30 13:46:42.000000 dust_extinction-1.4/dust_extinction/data/D22_Rv_slope.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   145064 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/EXT_C11.RES.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    90880 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/EXT_DBP90.RES.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   121046 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/EXT_J13.RES.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     3193 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/F19_tabulated.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2724 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/G21_IRS.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    16186 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/G21_IRS_fullres.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      550 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/G21_PHOT.dat
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2001 2024-05-07 19:37:16.000000 dust_extinction-1.4/dust_extinction/data/G24_SMCAvg.dat
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1874 2024-05-07 19:37:16.000000 dust_extinction-1.4/dust_extinction/data/G24_SMCBumps.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1868 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/GCC09_FUSE.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     7385 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/GCC09_IUE.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      181 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/GCC09_PHOT.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      246 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/README.rst
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)  3098880 2023-11-28 17:20:24.000000 dust_extinction-1.4/dust_extinction/data/astrodust+PAH_MW_RV3.1.fits
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      373 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/fritz11_galcenter.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110119 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_LMC2_10.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110125 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_LMCavg_20.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110428 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_3.1_60.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    64842 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_3.1_60_D03.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    64842 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_4.0A_40_D03.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110130 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_4.0B_40.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    64849 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_5.5A_30_D03.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110130 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_5.5B_30.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110116 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_SMCbar_0.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    32453 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/zubko2004_bare-gr-s_alam_av.dat
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)    16750 2023-11-28 17:20:24.000000 dust_extinction-1.4/dust_extinction/grain_models.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2217 2023-11-28 19:59:56.000000 dust_extinction-1.4/dust_extinction/helpers.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)    44065 2024-03-19 17:36:34.000000 dust_extinction-1.4/dust_extinction/parameter_averages.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)    25744 2024-03-19 16:39:20.000000 dust_extinction-1.4/dust_extinction/shapes.py
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.328994 dust_extinction-1.4/dust_extinction/tests/
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      108 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/__init__.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1592 2024-05-07 19:37:16.000000 dust_extinction-1.4/dust_extinction/tests/helpers.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2466 2023-04-04 14:41:44.000000 dust_extinction-1.4/dust_extinction/tests/test_axavtoexv.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     5520 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_ccm89.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     5220 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_corvals.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1225 2022-03-04 18:58:24.000000 dust_extinction-1.4/dust_extinction/tests/test_corvals_aves.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1222 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_corvals_grainmods.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2309 2023-11-28 19:59:56.000000 dust_extinction-1.4/dust_extinction/tests/test_fm90.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2095 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_g16.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2971 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_gcc09.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     3699 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_o94.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     3860 2023-04-04 14:41:44.000000 dust_extinction-1.4/dust_extinction/tests/test_p92.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1896 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_vcg04.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2970 2024-03-19 17:36:34.000000 dust_extinction-1.4/dust_extinction/tests/test_warnings.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)      335 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction/version.py
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.328994 dust_extinction-1.4/dust_extinction.egg-info/
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     5695 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction.egg-info/PKG-INFO
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2860 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction.egg-info/SOURCES.txt
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)        1 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction.egg-info/dependency_links.txt
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)        1 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction.egg-info/not-zip-safe
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)       80 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction.egg-info/requires.txt
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)       16 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction.egg-info/top_level.txt
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      134 2022-01-04 15:34:07.000000 dust_extinction-1.4/pyproject.toml
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1773 2024-05-07 19:41:30.329994 dust_extinction-1.4/setup.cfg
+-rwxrwxr-x   0 kgordon   (1000) kgordon   (1000)     1964 2022-01-04 15:34:07.000000 dust_extinction-1.4/setup.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2306 2024-05-07 15:29:44.000000 dust_extinction-1.4/tox.ini
```

### Comparing `dust_extinction-1.3/.github/workflows/tox-tests.yml` & `dust_extinction-1.4/.github/workflows/tox-tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,23 @@
         # https://help.github.com/en/actions/reference/virtual-environments-for-github-hosted-runners
         #
         # Only run on ubuntu by default, but can add other os's to the test matrix here.
         # For example -- os: [ubuntu-latest, macos-latest, windows-latest]
         os: [ubuntu-latest, macos-latest, windows-latest]
 
         # Test python version 3.x
-        python-ver: [9, 10, 11]
+        python-ver: [10, 11, 12]
 
         # Specify which tox environments to test in this list.
         # tox-env: [cov, alldeps, devdeps, astropylts]
         tox-env: [alldeps]
     steps:
-    - uses: actions/checkout@v1
+    - uses: actions/checkout@v4
     - name: Set up python 3.${{ matrix.python-ver }} with tox environment py3${{ matrix.python-ver }}-${{ matrix.tox-env }} on ${{ matrix.os }}
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
         python-version: 3.${{ matrix.python-ver }}
     - name: Install base dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox
     - name: Test with tox
@@ -66,44 +66,44 @@
   #       tox -e py38-devdeps
 
   # LTS version test
   lts_test:
     runs-on: ubuntu-latest
     if: "!contains(github.event.head_commit.message, '[ci skip]')"
     steps:
-    - uses: actions/checkout@v1
+    - uses: actions/checkout@v4
     - name: Set up python for astropy lts test
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
-        python-version: 3.9
+        python-version: 3.11
     - name: Install base dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox
     - name: Test with tox
       run: |
-        tox -e py39-astropylts
+        tox -e py311-astropylts
 
   # Coverage test
   cov_test:
     runs-on: ubuntu-latest
     if: "!contains(github.event.head_commit.message, '[ci skip]')"
     steps:
-    - uses: actions/checkout@v1
+    - uses: actions/checkout@v4
     - name: Set up python for coverage test
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
-        python-version: 3.11
+        python-version: 3.12
     - name: Install base dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox
     - name: Test with tox
       run: |
-        tox -e py311-cov
+        tox -e py312-cov
     - name: Upload coverage to codecov
       uses: codecov/codecov-action@v1
       with:
         token: ${{ secrets.CODECOV }}
         fail_ci_if_error: true
 
 #      if: matrix.tox-env == 'cov' && matrix.python-ver == '8'
@@ -114,19 +114,19 @@
 #        fail_ci_if_error: true
 
   # Test building of docs and check the links
   doc_test:
     runs-on: ubuntu-latest
     if: "!contains(github.event.head_commit.message, '[ci skip]')"
     steps:
-    - uses: actions/checkout@v1
+    - uses: actions/checkout@v4
     - name: Set up Python to build docs with sphinx
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
-        python-version: 3.11
+        python-version: 3.12
     - name: Install base dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox
         sudo apt-get install graphviz
     - name: Build and check docs using tox
       run: |
@@ -134,19 +134,19 @@
         tox -e linkcheck
 
   # Perform codestyle check
   codestyle:
     runs-on: ubuntu-latest
     if: "!contains(github.event.head_commit.message, '[ci skip]')"
     steps:
-    - uses: actions/checkout@v1
+    - uses: actions/checkout@v4
     - name: Python codestyle check
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
-        python-version: 3.11
+        python-version: 3.12
     - name: Install base dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox
     - name: Check codestyle using tox
       run: |
         tox -e codestyle
```

### Comparing `dust_extinction-1.3/.gitignore` & `dust_extinction-1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/CHANGES.rst` & `dust_extinction-1.4/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-1.4 (unreleased)
+1.4 (2024-05-07)
 ================
 
-- no changes yet
+- Added G24 Average and Bumps average models
 
 1.3 (2023-11-28)
 ================
 
 - Added HD23 dust grain model
 - Added FM90_B3 shape model
 - updated docs
```

### Comparing `dust_extinction-1.3/LICENSE` & `dust_extinction-1.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2017-2023, Karl Gordon
+Copyright (c) 2017-2024, Karl Gordon
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
@@ -23,7 +23,8 @@
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
```

### Comparing `dust_extinction-1.3/PKG-INFO` & `dust_extinction-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: dust_extinction
-Version: 1.3
+Version: 1.4
 Summary: Interstellar Dust Extinction Models
 Home-page: http://dust-extinction.readthedocs.io/
 Author: Karl Gordon
 Author-email: kgordon@stsci.edu
 License: BSD 3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-License-File: licenses/LICENSE.rst
 Requires-Dist: astropy
 Requires-Dist: scipy
 Provides-Extra: test
 Requires-Dist: pytest-astropy; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx-astropy; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
```

### Comparing `dust_extinction-1.3/README.rst` & `dust_extinction-1.4/README.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/docs/Makefile` & `dust_extinction-1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/docs/conf.py` & `dust_extinction-1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/docs/dust_extinction/choose_model.rst` & `dust_extinction-1.4/docs/dust_extinction/choose_model.rst`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 :class:`~dust_extinction.averages.RRP89_MWGC`,
 :class:`~dust_extinction.averages.B92_MWAvg`,
 :class:`~dust_extinction.averages.I05_MWAvg`,
 :class:`~dust_extinction.averages.CT06_MWLoc`,
 :class:`~dust_extinction.averages.CT06_MWGC`,
 :class:`~dust_extinction.averages.GCC09_MWAvg`,
 :class:`~dust_extinction.averages.F11_MWGC`,
-:class:`~dust_extinction.averages.G21_MWAvg`;
+:class:`~dust_extinction.averages.G21_MWAvg`,
 :class:`~dust_extinction.averages.D22_MWAvg`;
 Note the different valid wavelength ranges), the LMC
 (:class:`~dust_extinction.averages.G03_LMCAvg`,
 :class:`~dust_extinction.averages.G03_LMC2`) and the SMC
-(:class:`~dust_extinction.averages.G03_SMCBar`).
+(:class:`~dust_extinction.averages.G03_SMCBar`,
+:class:`~dust_extinction.averages.G24_SMCAvg`,
+:class:`~dust_extinction.averages.G24_SMCBumps`).
 
 One often used alternative to these straight average models is to use one of
 the parameter dependent models with the average R(V) value.  For the Milky
 Way, the usual average used is R(V) = 3.1.  See the next section.
 
 +--------------+-------------+------------------+--------------+
 | Model        | x range     | wavelength range |       galaxy |
@@ -59,15 +61,18 @@
 +--------------+-------------+------------------+--------------+
 | G03_LMCAvg   |  0.3 - 10.0 |        0.1 - 3.3 |          LMC |
 +--------------+-------------+------------------+--------------+
 | G03_LMC2     |  0.3 - 10.0 |        0.1 - 3.3 | LMC (30 Dor) |
 +--------------+-------------+------------------+--------------+
 | G03_SMCBar   |  0.3 - 10.0 |        0.1 - 3.3 |          SMC |
 +--------------+-------------+------------------+--------------+
-
+| G24_SMCAvg   |  0.3 - 10.0 |        0.1 - 3.3 |          SMC |
++--------------+-------------+------------------+--------------+
+| G24_SMCBumps |  0.3 - 10.0 |        0.1 - 3.3 |          SMC |
++--------------+-------------+------------------+--------------+
 
 Parameter Dependent Average Curves
 ----------------------------------
 
 The models that are dependent on parameters provide average curves that account
 for overall changes in the extinction curve shapes.  For example, the average
 behavior of Milky Way extinction curves has been shown to be dependent on R(V)
```

### Comparing `dust_extinction-1.3/docs/dust_extinction/extinction.rst` & `dust_extinction-1.4/docs/dust_extinction/extinction.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/docs/dust_extinction/extinguish.rst` & `dust_extinction-1.4/docs/dust_extinction/extinguish.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/docs/dust_extinction/fit_extinction.rst` & `dust_extinction-1.4/docs/dust_extinction/fit_extinction.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/docs/dust_extinction/install.rst` & `dust_extinction-1.4/docs/dust_extinction/install.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/docs/dust_extinction/model_flavors.rst` & `dust_extinction-1.4/docs/dust_extinction/model_flavors.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 ==============
 
    These models provide averages from the literature with the ability to
    interpolate between the observed data points.
    Models are provided for the Milky Way for the optical (Bastiaansen 1992),
    ultraviolet through near-infrared
    (Gordon, Cartlege, & Clayton 2009) and near- and mid-infrared
-   (Rieke & Lebofsky 1985; Indebetouw et al. 2005; Chiar & Tielens 2006; Fritz et al. 2011)
-   and the Magellanic Clouds (Gordon et al. 2003).
+   (Rieke & Lebofsky 1985; Indebetouw et al. 2005; Chiar & Tielens 2006; Fritz et al. 2011;
+   Gordon et al. 2021; Decleir et al. 2022)
+   and the Magellanic Clouds (Gordon et al. 2003; Gordon et al. 2024).
 
    For the Milky Way for the ultraviolet through near-infrared,
    one of the R(V) dependent models with R(V) = 3.1
    (see next section) is often used for the Milky Way 'average'.
 
 .. plot::
 
@@ -27,22 +28,25 @@
    from matplotlib.ticker import ScalarFormatter
    import astropy.units as u
 
    from dust_extinction.averages import (GCC09_MWAvg,
                                          B92_MWAvg,
                                          G03_SMCBar,
                                          G03_LMCAvg,
-					                               G03_LMC2)
+					                          G03_LMC2,
+                                         G24_SMCAvg,
+                                         G24_SMCBumps)
 
    fig, ax = plt.subplots()
 
    # generate the curves and plot them
    x = np.arange(0.3,11.0,0.1)/u.micron
 
-   models = [GCC09_MWAvg, B92_MWAvg, G03_SMCBar, G03_LMCAvg, G03_LMC2]
+   models = [GCC09_MWAvg, B92_MWAvg, G03_SMCBar, G03_LMCAvg, G03_LMC2, 
+             G24_SMCAvg, G24_SMCBumps]
 
    for cmodel in models:
       ext_model = cmodel()
       indxs, = np.where(np.logical_and(
          x.value >= ext_model.x_range[0],
          x.value <= ext_model.x_range[1]))
       yvals = ext_model(x[indxs])
@@ -107,16 +111,17 @@
 ====================================================
 
    These models provide predictions of the shape of the dust extinction
    given input variable(s).
 
    The R(V) dependent models include CCM89 the original such model
    (Cardelli, Clayton, and Mathis 1989), the O94 model that updates the
-   optical portion of the CCM89 model (O'Donnell 1994), and the F99 model
-   (Fitzpatrick 1999) updated as F04 (Fitzpatrick 2004),
+   optical portion of the CCM89 model (O'Donnell 1994), the F99 model
+   (Fitzpatrick 1999) updated as F04 (Fitzpatrick 2004), and the
+   fully spectroscopic far-UV to mid-IR G23 (Gordon et al. 2023).
    These models are based on the average
    behavior of extinction in the Milky Way as a function of R(V).
    The M14 model refines the optical portion of the CCM89 model
    (Maiz Apellaniz et al. 2014), was developed for the LMC but
    has been shown valid elsewhere in the Milky Way.
 
    In addition, the (R(V), f_A) two parameter relationship from
```

### Comparing `dust_extinction-1.3/docs/dust_extinction/references.rst` & `dust_extinction-1.4/docs/dust_extinction/references.rst`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,19 @@
 
 G16: `Gordon et al. 2016, ApJ 826, 104
 <https://ui.adsabs.harvard.edu/abs/2016ApJ...826..104G>`_
 
 G21: `Gordon et al. 2021, ApJ, 916, 33
 <https://ui.adsabs.harvard.edu/abs/2021ApJ...916...33G>`_
 
-G23: `Gordon et al. 2022, ApJ, 950, 86
+G23: `Gordon et al. 2023, ApJ, 950, 86
 <https://ui.adsabs.harvard.edu/abs/2023ApJ...950...86G/abstract>`_
 
+G24: Gordon et al. 2024, ApJ, in press
+
 HD23: `Hensley & Draine 2023, ApJ, 948, 55
 <https://ui.adsabs.harvard.edu/abs/2023ApJ...948...55H/abstract>`_
 
 I05: `Indebetouw et al. 2005, ApJ, 619, 931
 <https://ui.adsabs.harvard.edu/abs/2005ApJ...619..931I>`_
 
 J13: `Jones et al. 2013, A&A, 558, 62
```

### Comparing `dust_extinction-1.3/docs/index.rst` & `dust_extinction-1.4/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 
 User Documentation
 ==================
 
 .. toctree::
    :maxdepth: 2
 
-   Extinction versus Attenuation <dust_extinction/extinction.rst>
-   Flavors of Models <dust_extinction/model_flavors.rst>
-   How to choose a model <dust_extinction/choose_model.rst>
-   Extinguish (or unextinguish) data <dust_extinction/extinguish.rst>
+   Extinction versus Attenuation (what is the difference) <dust_extinction/extinction.rst>
+   Flavors of Models (including plots of all models) <dust_extinction/model_flavors.rst>
+   How to choose a model (including listing of all models) <dust_extinction/choose_model.rst>
+   Extinguish (or unextinguish) data (how to correct/account for extinction) <dust_extinction/extinguish.rst>
    Fitting extinction curves <dust_extinction/fit_extinction.rst>
    References <dust_extinction/references.rst>
 
 Installation
 ============
 
 .. toctree::
```

### Comparing `dust_extinction-1.3/docs/make.bat` & `dust_extinction-1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/averages.py` & `dust_extinction-1.4/dust_extinction/averages.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import, print_function, division
-
 import pkg_resources
 
 import numpy as np
 from scipy.interpolate import interp1d
 from astropy.table import Table
 from astropy.modeling.models import PowerLaw1D
 
@@ -21,14 +19,16 @@
     "I05_MWAvg",
     "CT06_MWGC",
     "CT06_MWLoc",
     "GCC09_MWAvg",
     "F11_MWGC",
     "G21_MWAvg",
     "D22_MWAvg",
+    "G24_SMCAvg",
+    "G24_SMCBumps",
 ]
 
 
 class RL85_MWGC(BaseExtModel):
     r"""
     Reike & Lebofsky (1985) MW Average Extinction Curve
 
@@ -1511,7 +1511,249 @@
 
         # setup the model
         d22_fit = PowerLaw1D(alpha=1.71, amplitude=0.386, x_0=1.0)
 
         # return A(x)/A(V)
         # Note that model in D22 was done versus wavelength in microns
         return d22_fit(1.0 / x)
+
+
+class G24_SMCAvg(BaseExtModel):
+    r"""
+    Gordon et al (2024) SMC Average Extinction Curve
+
+    Parameters
+    ----------
+    None
+
+    Raises
+    ------
+    None
+
+    Notes
+    -----
+    From Gordon et al. (2024, ApJ, in press)
+
+    Example showing the average curve
+
+    .. plot::
+        :include-source:
+
+        import numpy as np
+        import matplotlib.pyplot as plt
+        import astropy.units as u
+
+        from dust_extinction.averages import G24_SMCAvg
+
+        fig, ax = plt.subplots()
+
+        # define the extinction model
+        ext_model = G24_SMCAvg()
+
+        # generate the curves and plot them
+        x = np.arange(ext_model.x_range[0], ext_model.x_range[1],0.1)/u.micron
+
+        ax.plot(x,ext_model(x),label='G24 SMC Average')
+        ax.plot(ext_model.obsdata_x, ext_model.obsdata_axav, 'ko',
+                label='obsdata')
+
+        ax.set_xlabel(r'$x$ [$\mu m^{-1}$]')
+        ax.set_ylabel(r'$A(x)/A(V)$')
+
+        ax.legend(loc='best')
+        plt.show()
+    """
+
+    x_range = [0.3, 10.0]
+
+    Rv = 3.06
+
+    def __init__(self, **kwargs):
+
+        # get the tabulated information
+        data_path = pkg_resources.resource_filename("dust_extinction", "data/")
+
+        # D22 sigma clipped average of 13 diffuse sightlines
+        a = Table.read(data_path + "G24_SMCAvg.dat", format="ascii.commented_header")
+
+        # data
+        self.obsdata_x = 1.0 / a["wave"].data
+        self.obsdata_axav = a["A(l)/A(V)"].data
+        self.obsdata_axav_unc = a["unc"].data
+
+        # accuracy of the observed data based on published table
+        self.obsdata_tolerance = (
+            0.1  # large value driven by short wavelength uncertainties
+        )
+
+        super().__init__(**kwargs)
+
+    def evaluate(self, in_x):
+        """
+        G24 SMCAvg function
+
+        Parameters
+        ----------
+        in_x: float
+           expects either x in units of wavelengths or frequency
+           or assumes wavelengths in wavenumbers [1/micron]
+
+           internally wavenumbers are used
+
+        Returns
+        -------
+        axav: np array (float)
+            A(x)/A(V) extinction curve [mag]
+
+        Raises
+        ------
+        ValueError
+           Input x values outside of defined range
+        """
+        C1 = -5.07
+        C2 = 2.30
+        C3 = 0.12
+        C4 = 0.08
+        xo = 4.59
+        gamma = 0.95
+
+        optnir_axav_x = 1.0 / np.array([2.198, 1.65, 1.25, 0.55, 0.44, 0.37])
+        optnir_axav_y = [0.075, 0.137, 0.333, 1.021, 1.345, 1.507]
+
+        # return A(x)/A(V)
+        return _curve_F99_method(
+            in_x,
+            self.Rv,
+            C1,
+            C2,
+            C3,
+            C4,
+            xo,
+            gamma,
+            optnir_axav_x,
+            optnir_axav_y,
+            self.x_range,
+            self.__class__.__name__,
+        )
+
+
+class G24_SMCBumps(BaseExtModel):
+    r"""
+    Gordon et al (2024) SMC Bumps Extinction Curve
+
+    Parameters
+    ----------
+    None
+
+    Raises
+    ------
+    None
+
+    Notes
+    -----
+    From Gordon et al. (2024, ApJ, in press)
+
+    Two data points in the FUV from the data file giving the observed average were removed
+    as they are *very* deviate from the FM90 parametrization.  This cause the automated tests
+    to fail.
+
+    Example showing the average curve
+
+    .. plot::
+        :include-source:
+
+        import numpy as np
+        import matplotlib.pyplot as plt
+        import astropy.units as u
+
+        from dust_extinction.averages import G24_SMCBumps
+
+        fig, ax = plt.subplots()
+
+        # define the extinction model
+        ext_model = G24_SMCBumps()
+
+        # generate the curves and plot them
+        x = np.arange(ext_model.x_range[0], ext_model.x_range[1],0.1)/u.micron
+
+        ax.plot(x,ext_model(x),label='G24 SMC Bumps')
+        ax.plot(ext_model.obsdata_x, ext_model.obsdata_axav, 'ko',
+                label='obsdata')
+
+        ax.set_xlabel(r'$x$ [$\mu m^{-1}$]')
+        ax.set_ylabel(r'$A(x)/A(V)$')
+
+        ax.legend(loc='best')
+        plt.show()
+    """
+
+    x_range = [0.3, 10.0]
+
+    Rv = 2.59
+
+    def __init__(self, **kwargs):
+
+        # get the tabulated information
+        data_path = pkg_resources.resource_filename("dust_extinction", "data/")
+
+        # D22 sigma clipped average of 13 diffuse sightlines
+        a = Table.read(data_path + "G24_SMCBumps.dat", format="ascii.commented_header")
+
+        # data
+        self.obsdata_x = 1.0 / a["wave"].data
+        self.obsdata_axav = a["A(l)/A(V)"].data
+        self.obsdata_axav_unc = a["unc"].data
+
+        # accuracy of the observed data based on published table
+        self.obsdata_tolerance = (
+            0.1  # large value driven by short wavelength uncertainties
+        )
+
+        super().__init__(**kwargs)
+
+    def evaluate(self, in_x):
+        """
+        G24 SMCBumps function
+
+        Parameters
+        ----------
+        in_x: float
+           expects either x in units of wavelengths or frequency
+           or assumes wavelengths in wavenumbers [1/micron]
+
+           internally wavenumbers are used
+
+        Returns
+        -------
+        axav: np array (float)
+            A(x)/A(V) extinction curve [mag]
+
+        Raises
+        ------
+        ValueError
+           Input x values outside of defined range
+        """
+        C1 = -2.87
+        C2 = 1.51
+        C3 = 2.64
+        C4 = 0.25
+        xo = 4.73
+        gamma = 1.16
+
+        optnir_axav_x = 1.0 / np.array([2.198, 1.65, 1.25, 0.55, 0.44, 0.37])
+        optnir_axav_y = [0.068, 0.174, 0.302, 1.017, 1.394, 1.675]
+
+        # return A(x)/A(V)
+        return _curve_F99_method(
+            in_x,
+            self.Rv,
+            C1,
+            C2,
+            C3,
+            C4,
+            xo,
+            gamma,
+            optnir_axav_x,
+            optnir_axav_y,
+            self.x_range,
+            self.__class__.__name__,
+        )
```

### Comparing `dust_extinction-1.3/dust_extinction/baseclasses.py` & `dust_extinction-1.4/dust_extinction/baseclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import, print_function, division
-
 import numpy as np
 
 from astropy.modeling import Model, Parameter, InputParameterError
 
 __all__ = ["BaseExtModel", "BaseExtRvModel", "BaseExtRvAfAModel"]
```

### Comparing `dust_extinction-1.3/dust_extinction/conftest.py` & `dust_extinction-1.4/dust_extinction/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,41 +4,45 @@
 # packagename.test
 
 import os
 
 from astropy.version import version as astropy_version
 
 # For Astropy 3.0 and later, we can use the standalone pytest plugin
-if astropy_version < '3.0':
+if astropy_version < "3.0":
     from astropy.tests.pytest_plugins import *  # noqa
+
     del pytest_report_header
     ASTROPY_HEADER = True
 else:
     try:
         from pytest_astropy_header.display import PYTEST_HEADER_MODULES, TESTED_VERSIONS
+
         ASTROPY_HEADER = True
     except ImportError:
         ASTROPY_HEADER = False
 
 
 def pytest_configure(config):
 
     if ASTROPY_HEADER:
 
         config.option.astropy_header = True
 
         # Customize the following lines to add/remove entries from the list of
         # packages for which version numbers are displayed when running the tests.
-        PYTEST_HEADER_MODULES.pop('Pandas', None)
-        PYTEST_HEADER_MODULES['scikit-image'] = 'skimage'
+        PYTEST_HEADER_MODULES.pop("Pandas", None)
+        PYTEST_HEADER_MODULES["scikit-image"] = "skimage"
 
         from . import __version__
+
         packagename = os.path.basename(os.path.dirname(__file__))
         TESTED_VERSIONS[packagename] = __version__
 
+
 # Uncomment the last two lines in this block to treat all DeprecationWarnings as
 # exceptions. For Astropy v2.0 or later, there are 2 additional keywords,
 # as follow (although default should work for most cases).
 # To ignore some packages that produce deprecation warnings on import
 # (in addition to 'compiler', 'scipy', 'pygments', 'ipykernel', and
 # 'setuptools'), add:
 #     modules_to_ignore_on_import=['module_1', 'module_2']
```

### Comparing `dust_extinction-1.3/dust_extinction/conversions.py` & `dust_extinction-1.4/dust_extinction/conversions.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/CT06_pixiedust.dat` & `dust_extinction-1.4/dust_extinction/data/CT06_pixiedust.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/D22.dat` & `dust_extinction-1.4/dust_extinction/data/D22.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/D22_Rv_slope.dat` & `dust_extinction-1.4/dust_extinction/data/D22_Rv_slope.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/EXT_C11.RES.dat` & `dust_extinction-1.4/dust_extinction/data/EXT_C11.RES.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/EXT_DBP90.RES.dat` & `dust_extinction-1.4/dust_extinction/data/EXT_DBP90.RES.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/EXT_J13.RES.dat` & `dust_extinction-1.4/dust_extinction/data/EXT_J13.RES.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/F19_tabulated.dat` & `dust_extinction-1.4/dust_extinction/data/F19_tabulated.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/G21_IRS.dat` & `dust_extinction-1.4/dust_extinction/data/G21_IRS.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/G21_IRS_fullres.dat` & `dust_extinction-1.4/dust_extinction/data/G21_IRS_fullres.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/G21_PHOT.dat` & `dust_extinction-1.4/dust_extinction/data/G21_PHOT.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/GCC09_FUSE.dat` & `dust_extinction-1.4/dust_extinction/data/GCC09_FUSE.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/GCC09_IUE.dat` & `dust_extinction-1.4/dust_extinction/data/GCC09_IUE.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/astrodust+PAH_MW_RV3.1.fits` & `dust_extinction-1.4/dust_extinction/data/astrodust+PAH_MW_RV3.1.fits`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_LMC2_10.dat` & `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_LMC2_10.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_LMCavg_20.dat` & `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_LMCavg_20.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_MW_3.1_60.dat` & `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_3.1_60.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_MW_3.1_60_D03.dat` & `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_3.1_60_D03.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_MW_4.0A_40_D03.dat` & `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_4.0A_40_D03.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_MW_4.0B_40.dat` & `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_4.0B_40.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_MW_5.5A_30_D03.dat` & `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_5.5A_30_D03.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_MW_5.5B_30.dat` & `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_5.5B_30.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/kext_albedo_WD_SMCbar_0.dat` & `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_SMCbar_0.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/data/zubko2004_bare-gr-s_alam_av.dat` & `dust_extinction-1.4/dust_extinction/data/zubko2004_bare-gr-s_alam_av.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/grain_models.py` & `dust_extinction-1.4/dust_extinction/grain_models.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/helpers.py` & `dust_extinction-1.4/dust_extinction/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,17 @@
     x_range: 2 floats
        allowed min/max of x
 
     outname: str
        name of curve for error message
     """
     deltacheck = 1e-6  # delta to allow for small numerical issues
-    if np.logical_or(np.any(x <= (x_range[0] - deltacheck)), np.any(x >= (x_range[1] + deltacheck))):
+    if np.logical_or(
+        np.any(x <= (x_range[0] - deltacheck)), np.any(x >= (x_range[1] + deltacheck))
+    ):
         raise ValueError(
             "Input x outside of range defined for "
             + outname
             + " ["
             + str(x_range[0])
             + " <= x <= "
             + str(x_range[1])
```

### Comparing `dust_extinction-1.3/dust_extinction/parameter_averages.py` & `dust_extinction-1.4/dust_extinction/parameter_averages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import, print_function, division
-
 import pkg_resources
 
 import numpy as np
 from scipy import interpolate
 
 import astropy.units as u
 from astropy.table import Table
@@ -1363,15 +1361,15 @@
     InputParameterError
        Input Rv values outside of defined range
 
     Notes
     -----
     From Gordon et al. (2023, ApJ, in press)
 
-    Example showing CCM89 curves for a range of R(V) values.
+    Example showing G23 curves for a range of R(V) values.
 
     .. plot::
         :include-source:
 
         import numpy as np
         import matplotlib.pyplot as plt
         import astropy.units as u
@@ -1481,17 +1479,15 @@
         # weights = (1.0 / optir_waves[1] - x[optir_overlap]) / (
         #     1.0 / optir_waves[1] - 1.0 / optir_waves[0]
         # )
         weights = _smoothstep(
             1.0 / x[optir_overlap], x_min=optir_waves[0], x_max=optir_waves[1], N=1
         )
         self.a[optir_overlap] = (1.0 - weights) * m20_model_a(x[optir_overlap])
-        self.a[optir_overlap] += weights * self.nirmir_intercept(
-            x[optir_overlap], ir_a
-        )
+        self.a[optir_overlap] += weights * self.nirmir_intercept(x[optir_overlap], ir_a)
         self.b[optir_overlap] = (1.0 - weights) * m20_model_b(x[optir_overlap])
         self.b[optir_overlap] += weights * irpow(x[optir_overlap])
 
         # Ultraviolet
         uv_a = [0.81297, 0.2775, 1.06295, 0.11303, 4.60, 0.99]
         uv_b = [-2.97868, 1.89808, 3.10334, 0.65484, 4.60, 0.99]
 
@@ -1505,17 +1501,21 @@
         # overlap between uv/optical
         # weights = (1.0 / uvopt_waves[1] - x[uvopt_overlap]) / (
         #     1.0 / uvopt_waves[1] - 1.0 / uvopt_waves[0]
         # )
         weights = _smoothstep(
             1.0 / x[uvopt_overlap], x_min=uvopt_waves[0], x_max=uvopt_waves[1], N=1
         )
-        self.a[uvopt_overlap] = (1.0 - weights) * fm90_model_a(x[uvopt_overlap] / u.micron)
+        self.a[uvopt_overlap] = (1.0 - weights) * fm90_model_a(
+            x[uvopt_overlap] / u.micron
+        )
         self.a[uvopt_overlap] += weights * m20_model_a(x[uvopt_overlap])
-        self.b[uvopt_overlap] = (1.0 - weights) * fm90_model_b(x[uvopt_overlap] / u.micron)
+        self.b[uvopt_overlap] = (1.0 - weights) * fm90_model_b(
+            x[uvopt_overlap] / u.micron
+        )
         self.b[uvopt_overlap] += weights * m20_model_b(x[uvopt_overlap])
 
         # return A(x)/A(V)
         return self.a + self.b * (1 / Rv - 1 / 3.1)
 
     @staticmethod
     def nirmir_intercept(x, params):
```

### Comparing `dust_extinction-1.3/dust_extinction/shapes.py` & `dust_extinction-1.4/dust_extinction/shapes.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,55 +270,55 @@
         # check that the wavenumbers are within the defined range
         _test_valid_x_range(x, x_range_FM90, "FM90")
 
         # linear term
         exvebv = C1 + C2 * x
 
         # bump term
-        x2 = x ** 2
-        exvebv += C3 * (x2 / ((x2 - xo ** 2) ** 2 + x2 * (gamma ** 2)))
+        x2 = x**2
+        exvebv += C3 * (x2 / ((x2 - xo**2) ** 2 + x2 * (gamma**2)))
 
         # FUV rise term
         fnuv_indxs = np.where(x >= 5.9)
         if len(fnuv_indxs) > 0:
             y = x[fnuv_indxs] - 5.9
-            exvebv[fnuv_indxs] += C4 * (0.5392 * (y ** 2) + 0.05644 * (y ** 3))
+            exvebv[fnuv_indxs] += C4 * (0.5392 * (y**2) + 0.05644 * (y**3))
 
         # return E(x-V)/E(B-V)
         return exvebv
 
     @staticmethod
     def fit_deriv(in_x, C1, C2, C3, C4, xo, gamma):
         """
         Derivatives of the FM90 function with respect to the parameters
         """
         x = in_x
 
         # useful quantitites
-        x2 = x ** 2
-        xo2 = xo ** 2
-        g2 = gamma ** 2
+        x2 = x**2
+        xo2 = xo**2
+        g2 = gamma**2
         x2mxo2_2 = (x2 - xo2) ** 2
         denom = (x2mxo2_2 - x2 * g2) ** 2
 
         # derivatives
         d_C1 = np.full((len(x)), 1.0)
         d_C2 = x
 
         d_C3 = x2 / (x2mxo2_2 + x2 * g2)
 
         d_xo = (4.0 * C2 * x2 * xo * (x2 - xo2)) / denom
 
-        d_gamma = (2.0 * C2 * (x2 ** 2) * gamma) / denom
+        d_gamma = (2.0 * C2 * (x2**2) * gamma) / denom
 
         d_C4 = np.zeros((len(x)))
         fuv_indxs = np.where(x >= 5.9)
         if len(fuv_indxs) > 0:
             y = x[fuv_indxs] - 5.9
-            d_C4[fuv_indxs] = 0.5392 * (y ** 2) + 0.05644 * (y ** 3)
+            d_C4[fuv_indxs] = 0.5392 * (y**2) + 0.05644 * (y**3)
 
         return [d_C1, d_C2, d_C3, d_C4, d_xo, d_gamma]
 
     # @property
     # def input_units(self):
     #     if self.xo.unit is None:
     #         return None
@@ -437,22 +437,22 @@
         # check that the wavenumbers are within the defined range
         _test_valid_x_range(x, x_range_FM90, "FM90_B3")
 
         # linear term
         exvebv = C1 + C2 * x
 
         # bump term
-        x2 = x ** 2
-        exvebv += (B3 * gamma ** 2) * (x2 / ((x2 - xo ** 2) ** 2 + x2 * (gamma ** 2)))
+        x2 = x**2
+        exvebv += (B3 * gamma**2) * (x2 / ((x2 - xo**2) ** 2 + x2 * (gamma**2)))
 
         # FUV rise term
         fnuv_indxs = np.where(x >= 5.9)
         if len(fnuv_indxs) > 0:
             y = x[fnuv_indxs] - 5.9
-            exvebv[fnuv_indxs] += C4 * (0.5392 * (y ** 2) + 0.05644 * (y ** 3))
+            exvebv[fnuv_indxs] += C4 * (0.5392 * (y**2) + 0.05644 * (y**3))
 
         # return E(x-V)/E(B-V)
         return exvebv
 
 
 class P92(Fittable1DModel):
     r"""
@@ -828,15 +828,17 @@
         plt.show()
 
     """
 
     # inputs = ("x",)
     # outputs = ("axav",)
 
-    scale = Parameter(description="powerlaw: amplitude", default=0.37, bounds=(0.0, 1.0))
+    scale = Parameter(
+        description="powerlaw: amplitude", default=0.37, bounds=(0.0, 1.0)
+    )
     alpha = Parameter(description="powerlaw: alpha", default=1.5, bounds=(0.5, 5.0))
     sil1_amp = Parameter(
         description="silicate 10um: amplitude", default=0.07, bounds=(0.001, 0.3)
     )
     sil1_center = Parameter(
         description="silicate 10um: center", default=9.87, bounds=(8.0, 12.0)
     )
```

### Comparing `dust_extinction-1.3/dust_extinction/tests/helpers.py` & `dust_extinction-1.4/dust_extinction/tests/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     I05_MWAvg,
     CT06_MWGC,
     CT06_MWLoc,
     GCC09_MWAvg,
     F11_MWGC,
     G21_MWAvg,
     D22_MWAvg,
+    G24_SMCAvg,
+    G24_SMCBumps,
 )
 from dust_extinction.grain_models import DBP90, WD01, D03, ZDA04, C11, J13, HD23
 
 param_ave_models_Rv = [CCM89, O94, F99, F04, VCG04, GCC09, M14, F19, D22, G23]
 param_ave_models_Rv_fA = [G16]
 param_ave_models = param_ave_models_Rv + param_ave_models_Rv_fA
 shape_models = [FM90, FM90_B3, P92, G21]
@@ -45,14 +47,16 @@
     I05_MWAvg,
     CT06_MWGC,
     CT06_MWLoc,
     GCC09_MWAvg,
     F11_MWGC,
     G21_MWAvg,
     D22_MWAvg,
+    G24_SMCAvg,
+    G24_SMCBumps,
 ]
 grain_models = [DBP90, WD01, D03, ZDA04, C11, J13, HD23]
 
 all_models = (
     param_ave_models_Rv
     + param_ave_models_Rv_fA
     + shape_models
```

### Comparing `dust_extinction-1.3/dust_extinction/tests/test_axavtoexv.py` & `dust_extinction-1.4/dust_extinction/tests/test_axavtoexv.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/tests/test_ccm89.py` & `dust_extinction-1.4/dust_extinction/tests/test_ccm89.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/tests/test_corvals.py` & `dust_extinction-1.4/dust_extinction/tests/test_corvals.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/tests/test_corvals_aves.py` & `dust_extinction-1.4/dust_extinction/tests/test_corvals_aves.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/tests/test_corvals_grainmods.py` & `dust_extinction-1.4/dust_extinction/tests/test_corvals_grainmods.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/tests/test_fm90.py` & `dust_extinction-1.4/dust_extinction/tests/test_fm90.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     # get an observed extinction curve to fit
     g03_model = G03_LMCAvg()
 
     x = g03_model.obsdata_x
     # convert to E(x-V)/E(B0V)
     y = (g03_model.obsdata_axav - 1.0) * g03_model.Rv
     # only fit the UV portion (FM90 only valid in UV)
-    gindxs, = np.where(x > 3.125)
+    (gindxs,) = np.where(x > 3.125)
 
     fm90_init = FM90()
     fit = LevMarLSQFitter()
     g03_fit = fit(fm90_init, x[gindxs], y[gindxs])
     fit_vals = [
         g03_fit.C1.value,
         g03_fit.C2.value,
```

### Comparing `dust_extinction-1.3/dust_extinction/tests/test_g16.py` & `dust_extinction-1.4/dust_extinction/tests/test_g16.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/tests/test_gcc09.py` & `dust_extinction-1.4/dust_extinction/tests/test_gcc09.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/tests/test_o94.py` & `dust_extinction-1.4/dust_extinction/tests/test_o94.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/tests/test_p92.py` & `dust_extinction-1.4/dust_extinction/tests/test_p92.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/tests/test_vcg04.py` & `dust_extinction-1.4/dust_extinction/tests/test_vcg04.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/dust_extinction/tests/test_warnings.py` & `dust_extinction-1.4/dust_extinction/tests/test_warnings.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,20 +23,21 @@
 
     with pytest.warns(
         UserWarning, match="x has no units, assuming x units are inverse microns"
     ):
         ext(x)
 
 
+@pytest.mark.skip("Testing for no warnings got more complicated/does not work")
 @pytest.mark.parametrize("model", all_models)
 def test_units_nowarning_expected(model):
     ext = model()
     x = [0.5 * (ext.x_range[0] + ext.x_range[1])] / u.micron
 
-    with pytest.warns(None) as record:
+    with pytest.warns() as record:
         ext(x)
     assert len(record) == 0
 
 
 @pytest.mark.parametrize("model", param_ave_models_Rv)
 @pytest.mark.parametrize("Rv_invalid", [-1.0, 0.0, 1.9, 6.1, 10.0])
 def test_invalid_Rv_input(model, Rv_invalid):
```

### Comparing `dust_extinction-1.3/dust_extinction.egg-info/PKG-INFO` & `dust_extinction-1.4/dust_extinction.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
-Name: dust-extinction
-Version: 1.3
+Name: dust_extinction
+Version: 1.4
 Summary: Interstellar Dust Extinction Models
 Home-page: http://dust-extinction.readthedocs.io/
 Author: Karl Gordon
 Author-email: kgordon@stsci.edu
 License: BSD 3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-License-File: licenses/LICENSE.rst
 Requires-Dist: astropy
 Requires-Dist: scipy
 Provides-Extra: test
 Requires-Dist: pytest-astropy; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx-astropy; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
```

### Comparing `dust_extinction-1.3/dust_extinction.egg-info/SOURCES.txt` & `dust_extinction-1.4/dust_extinction.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 dust_extinction/data/EXT_C11.RES.dat
 dust_extinction/data/EXT_DBP90.RES.dat
 dust_extinction/data/EXT_J13.RES.dat
 dust_extinction/data/F19_tabulated.dat
 dust_extinction/data/G21_IRS.dat
 dust_extinction/data/G21_IRS_fullres.dat
 dust_extinction/data/G21_PHOT.dat
+dust_extinction/data/G24_SMCAvg.dat
+dust_extinction/data/G24_SMCBumps.dat
 dust_extinction/data/GCC09_FUSE.dat
 dust_extinction/data/GCC09_IUE.dat
 dust_extinction/data/GCC09_PHOT.dat
 dust_extinction/data/README.rst
 dust_extinction/data/astrodust+PAH_MW_RV3.1.fits
 dust_extinction/data/fritz11_galcenter.dat
 dust_extinction/data/kext_albedo_WD_LMC2_10.dat
@@ -76,9 +78,8 @@
 dust_extinction/tests/test_corvals_grainmods.py
 dust_extinction/tests/test_fm90.py
 dust_extinction/tests/test_g16.py
 dust_extinction/tests/test_gcc09.py
 dust_extinction/tests/test_o94.py
 dust_extinction/tests/test_p92.py
 dust_extinction/tests/test_vcg04.py
-dust_extinction/tests/test_warnings.py
-licenses/LICENSE.rst
+dust_extinction/tests/test_warnings.py
```

### Comparing `dust_extinction-1.3/setup.cfg` & `dust_extinction-1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/setup.py` & `dust_extinction-1.4/setup.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.3/tox.ini` & `dust_extinction-1.4/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py{39,310,311}-test{,-alldeps}{,-cov}
+    py{310,311,312}-test{,-alldeps}{,-cov}
     build_docs
     linkcheck
     codestyle
 requires =
     setuptools >= 30.3.0
     pip >= 19.3.1
 isolated_build = true
```

