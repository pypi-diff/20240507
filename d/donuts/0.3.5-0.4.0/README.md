# Comparing `tmp/donuts-0.3.5.tar.gz` & `tmp/donuts-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/donuts-0.3.5.tar", last modified: Thu Jan  6 20:14:29 2022, max compression
+gzip compressed data, was "donuts-0.4.0.tar", last modified: Tue May  7 16:35:53 2024, max compression
```

## Comparing `donuts-0.3.5.tar` & `donuts-0.4.0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/
--rw-r--r--   0 jmcc       (501) staff       (20)     6372 2022-01-06 20:14:29.000000 donuts-0.3.5/PKG-INFO
--rw-r--r--   0 jmcc       (501) staff       (20)     4651 2021-08-13 15:02:43.000000 donuts-0.3.5/README.rst
--rw-r--r--   0 jmcc       (501) staff       (20)    36433 2021-08-12 17:23:13.000000 donuts-0.3.5/ah_bootstrap.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/
--rw-r--r--   0 jmcc       (501) staff       (20)    16528 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/CHANGES.rst
--rw-r--r--   0 jmcc       (501) staff       (20)     1491 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/LICENSE.rst
--rw-r--r--   0 jmcc       (501) staff       (20)     2587 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/README.rst
--rw-r--r--   0 jmcc       (501) staff       (20)    35044 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/ah_bootstrap.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/
--rw-r--r--   0 jmcc       (501) staff       (20)     1836 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/__init__.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/commands/
--rw-r--r--   0 jmcc       (501) staff       (20)        0 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/commands/__init__.py
--rw-r--r--   0 jmcc       (501) staff       (20)     2940 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/commands/_dummy.py
--rw-r--r--   0 jmcc       (501) staff       (20)    19700 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/commands/build_ext.py
--rw-r--r--   0 jmcc       (501) staff       (20)     1454 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/commands/build_py.py
--rw-r--r--   0 jmcc       (501) staff       (20)    10431 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/commands/build_sphinx.py
--rw-r--r--   0 jmcc       (501) staff       (20)      486 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/commands/install.py
--rw-r--r--   0 jmcc       (501) staff       (20)      512 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/commands/install_lib.py
--rw-r--r--   0 jmcc       (501) staff       (20)      120 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/commands/setup_package.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/commands/src/
--rw-r--r--   0 jmcc       (501) staff       (20)     3033 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/commands/src/compiler.c
--rw-r--r--   0 jmcc       (501) staff       (20)     1283 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/commands/test.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/compat/
--rw-r--r--   0 jmcc       (501) staff       (20)      368 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/compat/__init__.py
--rw-r--r--   0 jmcc       (501) staff       (20)     7922 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/distutils_helpers.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/
--rw-r--r--   0 jmcc       (501) staff       (20)      589 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/__init__.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/automodapi/
--rw-r--r--   0 jmcc       (501) staff       (20)       20 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/automodapi/__init__.py
--rw-r--r--   0 jmcc       (501) staff       (20)     5316 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/automodapi/autodoc_enhancements.py
--rw-r--r--   0 jmcc       (501) staff       (20)    15785 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/automodapi/automodapi.py
--rw-r--r--   0 jmcc       (501) staff       (20)    26026 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/automodapi/automodsumm.py
--rw-r--r--   0 jmcc       (501) staff       (20)     3711 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/automodapi/smart_resolver.py
--rw-r--r--   0 jmcc       (501) staff       (20)     7140 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/automodapi/utils.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/numpydoc/
--rw-r--r--   0 jmcc       (501) staff       (20)      117 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/numpydoc/__init__.py
--rw-r--r--   0 jmcc       (501) staff       (20)    18769 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape.py
--rw-r--r--   0 jmcc       (501) staff       (20)    10822 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape_sphinx.py
--rw-r--r--   0 jmcc       (501) staff       (20)     9563 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/numpydoc/numpydoc.py
--rw-r--r--   0 jmcc       (501) staff       (20)      189 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/extern/setup_package.py
--rw-r--r--   0 jmcc       (501) staff       (20)     6464 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/git_helpers.py
--rw-r--r--   0 jmcc       (501) staff       (20)     3115 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/openmp_helpers.py
--rw-r--r--   0 jmcc       (501) staff       (20)    27801 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/setup_helpers.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/
--rw-r--r--   0 jmcc       (501) staff       (20)      437 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/__init__.py
--rw-r--r--   0 jmcc       (501) staff       (20)    11919 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/conf.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/ext/
--rw-r--r--   0 jmcc       (501) staff       (20)       66 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/ext/__init__.py
--rw-r--r--   0 jmcc       (501) staff       (20)     2915 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py
--rw-r--r--   0 jmcc       (501) staff       (20)     1953 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py
--rw-r--r--   0 jmcc       (501) staff       (20)     5940 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/ext/tests/
--rw-r--r--   0 jmcc       (501) staff       (20)        0 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/ext/tests/__init__.py
--rw-r--r--   0 jmcc       (501) staff       (20)      760 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/ext/tocdepthfix.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/local/
--rw-r--r--   0 jmcc       (501) staff       (20)      562 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.inv
--rw-r--r--   0 jmcc       (501) staff       (20)     1638 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.txt
--rw-r--r--   0 jmcc       (501) staff       (20)      658 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv
--rw-r--r--   0 jmcc       (501) staff       (20)     2820 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt
--rw-r--r--   0 jmcc       (501) staff       (20)      292 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/setup_package.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/
--rw-r--r--   0 jmcc       (501) staff       (20)       73 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/globaltoc.html
--rw-r--r--   0 jmcc       (501) staff       (20)     3433 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html
--rw-r--r--   0 jmcc       (501) staff       (20)       34 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/localtoc.html
--rw-r--r--   0 jmcc       (501) staff       (20)      272 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/searchbox.html
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/
--rw-r--r--   0 jmcc       (501) staff       (20)     5201 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg
--rw-r--r--   0 jmcc       (501) staff       (20)     1725 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png
--rw-r--r--   0 jmcc       (501) staff       (20)    32988 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico
--rw-r--r--   0 jmcc       (501) staff       (20)     4634 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg
--rw-r--r--   0 jmcc       (501) staff       (20)     1884 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png
--rw-r--r--   0 jmcc       (501) staff       (20)    12067 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css
--rw-r--r--   0 jmcc       (501) staff       (20)     2769 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js
--rw-r--r--   0 jmcc       (501) staff       (20)     4971 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js
--rw-r--r--   0 jmcc       (501) staff       (20)      192 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/theme.conf
--rw-r--r--   0 jmcc       (501) staff       (20)      515 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/test_helpers.py
--rw-r--r--   0 jmcc       (501) staff       (20)    27125 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/utils.py
--rw-r--r--   0 jmcc       (501) staff       (20)     6974 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/version.py
--rw-r--r--   0 jmcc       (501) staff       (20)     9755 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/astropy_helpers/version_helpers.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/astropy_helpers.egg-info/
--rw-r--r--   0 jmcc       (501) staff       (20)     2980 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers.egg-info/PKG-INFO
--rw-r--r--   0 jmcc       (501) staff       (20)     3546 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 jmcc       (501) staff       (20)        1 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 jmcc       (501) staff       (20)        1 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers.egg-info/not-zip-safe
--rw-r--r--   0 jmcc       (501) staff       (20)       16 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/astropy_helpers.egg-info/top_level.txt
--rw-r--r--   0 jmcc       (501) staff       (20)    12537 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/ez_setup.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/astropy_helpers/licenses/
--rw-r--r--   0 jmcc       (501) staff       (20)     1644 2017-10-23 16:20:57.000000 donuts-0.3.5/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst
--rw-r--r--   0 jmcc       (501) staff       (20)     2505 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst
--rw-r--r--   0 jmcc       (501) staff       (20)     5959 2016-07-05 10:09:37.000000 donuts-0.3.5/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/docs/
--rw-r--r--   0 jmcc       (501) staff       (20)     4724 2016-06-03 09:55:32.000000 donuts-0.3.5/docs/Makefile
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/docs/_templates/
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/docs/_templates/autosummary/
--rw-r--r--   0 jmcc       (501) staff       (20)      250 2016-06-03 09:55:32.000000 donuts-0.3.5/docs/_templates/autosummary/base.rst
--rw-r--r--   0 jmcc       (501) staff       (20)      251 2016-06-03 09:55:32.000000 donuts-0.3.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0 jmcc       (501) staff       (20)      252 2016-06-03 09:55:32.000000 donuts-0.3.5/docs/_templates/autosummary/module.rst
--rw-r--r--   0 jmcc       (501) staff       (20)     6535 2021-08-12 17:23:20.000000 donuts-0.3.5/docs/conf.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/docs/donuts/
--rw-r--r--   0 jmcc       (501) staff       (20)     1455 2016-07-05 10:08:05.000000 donuts-0.3.5/docs/donuts/advanced.rst
--rw-r--r--   0 jmcc       (501) staff       (20)      105 2016-06-03 09:55:32.000000 donuts-0.3.5/docs/donuts/api.rst
--rw-r--r--   0 jmcc       (501) staff       (20)      906 2021-08-12 17:23:32.000000 donuts-0.3.5/docs/donuts/install.rst
--rw-r--r--   0 jmcc       (501) staff       (20)     5375 2016-07-05 10:08:05.000000 donuts-0.3.5/docs/donuts/user_guide.rst
--rw-r--r--   0 jmcc       (501) staff       (20)     4304 2016-07-05 10:08:05.000000 donuts-0.3.5/docs/index.rst
--rw-r--r--   0 jmcc       (501) staff       (20)     4513 2016-06-03 09:55:32.000000 donuts-0.3.5/docs/make.bat
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/donuts/
--rw-r--r--   0 jmcc       (501) staff       (20)      524 2016-06-03 09:55:32.000000 donuts-0.3.5/donuts/__init__.py
--rw-r--r--   0 jmcc       (501) staff       (20)     5273 2016-06-03 09:55:32.000000 donuts-0.3.5/donuts/_astropy_init.py
--rw-r--r--   0 jmcc       (501) staff       (20)     1435 2016-06-03 09:55:32.000000 donuts-0.3.5/donuts/conftest.py
--rw-r--r--   0 jmcc       (501) staff       (20)    10309 2022-01-06 20:11:45.000000 donuts-0.3.5/donuts/donuts.py
--rw-r--r--   0 jmcc       (501) staff       (20)    17629 2022-01-06 19:57:37.000000 donuts-0.3.5/donuts/image.py
-drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2022-01-06 20:14:29.000000 donuts-0.3.5/donuts/tests/
--rw-r--r--   0 jmcc       (501) staff       (20)      121 2016-06-03 09:55:32.000000 donuts-0.3.5/donuts/tests/__init__.py
--rw-r--r--   0 jmcc       (501) staff       (20)      768 2016-06-03 09:55:32.000000 donuts-0.3.5/donuts/tests/coveragerc
--rw-r--r--   0 jmcc       (501) staff       (20)      450 2017-10-23 15:43:31.000000 donuts-0.3.5/donuts/tests/helpers.py
--rw-r--r--   0 jmcc       (501) staff       (20)       96 2016-06-03 09:55:32.000000 donuts-0.3.5/donuts/tests/setup_package.py
--rw-r--r--   0 jmcc       (501) staff       (20)     1848 2019-05-31 10:51:01.000000 donuts-0.3.5/donuts/tests/synthetic_data.py
--rw-r--r--   0 jmcc       (501) staff       (20)      505 2016-06-03 09:55:32.000000 donuts-0.3.5/donuts/tests/test_choosing_image_class.py
--rw-r--r--   0 jmcc       (501) staff       (20)     4115 2019-05-31 10:58:22.000000 donuts-0.3.5/donuts/tests/test_donuts_with_synthetic_data.py
--rw-r--r--   0 jmcc       (501) staff       (20)     9699 2016-06-03 09:55:32.000000 donuts-0.3.5/donuts/tests/test_image.py
--rw-r--r--   0 jmcc       (501) staff       (20)     2600 2016-06-03 09:55:32.000000 donuts-0.3.5/donuts/tests/test_integration.py
--rw-r--r--   0 jmcc       (501) staff       (20)     1396 2016-06-03 09:55:32.000000 donuts-0.3.5/donuts/tests/test_integration2.py
--rw-r--r--   0 jmcc       (501) staff       (20)      258 2016-06-03 09:55:32.000000 donuts-0.3.5/donuts/tests/test_read_image.py
--rw-r--r--   0 jmcc       (501) staff       (20)     1243 2016-06-03 09:55:32.000000 donuts-0.3.5/donuts/tests/test_summary.py
--rw-r--r--   0 jmcc       (501) staff       (20)     2850 2016-06-03 09:55:32.000000 donuts-0.3.5/donuts/tests/test_synthetic_data.py
--rw-r--r--   0 jmcc       (501) staff       (20)     7300 2022-01-06 20:14:29.000000 donuts-0.3.5/donuts/version.py
--rw-r--r--   0 jmcc       (501) staff       (20)      289 2022-01-06 20:14:11.000000 donuts-0.3.5/donuts_version.py
--rw-r--r--   0 jmcc       (501) staff       (20)    11477 2016-06-03 09:55:32.000000 donuts-0.3.5/ez_setup.py
--rw-r--r--   0 jmcc       (501) staff       (20)      605 2019-05-31 09:50:01.000000 donuts-0.3.5/setup.cfg
--rwxr--r--   0 jmcc       (501) staff       (20)     4626 2017-10-23 18:09:03.000000 donuts-0.3.5/setup.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.467176 donuts-0.4.0/
+-rw-r--r--   0 jmcc       (501) staff       (20)     5457 2024-05-07 16:35:53.467070 donuts-0.4.0/PKG-INFO
+-rw-r--r--   0 jmcc       (501) staff       (20)     4651 2024-05-07 09:20:32.124674 donuts-0.4.0/README.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)    36433 2024-05-07 09:20:32.125187 donuts-0.4.0/ah_bootstrap.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.438168 donuts-0.4.0/astropy_helpers/
+-rw-r--r--   0 jmcc       (501) staff       (20)    16528 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/CHANGES.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)     1491 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/LICENSE.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)     2587 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/README.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)    35044 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/ah_bootstrap.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.446147 donuts-0.4.0/astropy_helpers/astropy_helpers/
+-rw-r--r--   0 jmcc       (501) staff       (20)     1836 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/__init__.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.450732 donuts-0.4.0/astropy_helpers/astropy_helpers/commands/
+-rw-r--r--   0 jmcc       (501) staff       (20)        0 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/commands/__init__.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     2940 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/commands/_dummy.py
+-rw-r--r--   0 jmcc       (501) staff       (20)    19700 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/commands/build_ext.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     1454 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/commands/build_py.py
+-rw-r--r--   0 jmcc       (501) staff       (20)    10431 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/commands/build_sphinx.py
+-rw-r--r--   0 jmcc       (501) staff       (20)      486 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/commands/install.py
+-rw-r--r--   0 jmcc       (501) staff       (20)      512 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/commands/install_lib.py
+-rw-r--r--   0 jmcc       (501) staff       (20)      120 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/commands/setup_package.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.450943 donuts-0.4.0/astropy_helpers/astropy_helpers/commands/src/
+-rw-r--r--   0 jmcc       (501) staff       (20)     3033 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/commands/src/compiler.c
+-rw-r--r--   0 jmcc       (501) staff       (20)     1283 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/commands/test.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.451169 donuts-0.4.0/astropy_helpers/astropy_helpers/compat/
+-rw-r--r--   0 jmcc       (501) staff       (20)      368 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/compat/__init__.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     7922 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/distutils_helpers.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.451608 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/
+-rw-r--r--   0 jmcc       (501) staff       (20)      589 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/__init__.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.452914 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/automodapi/
+-rw-r--r--   0 jmcc       (501) staff       (20)       20 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/automodapi/__init__.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     5316 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/automodapi/autodoc_enhancements.py
+-rw-r--r--   0 jmcc       (501) staff       (20)    15785 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/automodapi/automodapi.py
+-rw-r--r--   0 jmcc       (501) staff       (20)    26026 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/automodapi/automodsumm.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     3711 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/automodapi/smart_resolver.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     7140 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/automodapi/utils.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.453773 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/numpydoc/
+-rw-r--r--   0 jmcc       (501) staff       (20)      117 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/numpydoc/__init__.py
+-rw-r--r--   0 jmcc       (501) staff       (20)    18769 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape.py
+-rw-r--r--   0 jmcc       (501) staff       (20)    10822 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape_sphinx.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     9563 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/numpydoc/numpydoc.py
+-rw-r--r--   0 jmcc       (501) staff       (20)      189 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/extern/setup_package.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     6464 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/git_helpers.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     3115 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/openmp_helpers.py
+-rw-r--r--   0 jmcc       (501) staff       (20)    27801 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/setup_helpers.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.454409 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/
+-rw-r--r--   0 jmcc       (501) staff       (20)      437 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/__init__.py
+-rw-r--r--   0 jmcc       (501) staff       (20)    11919 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/conf.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.455503 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/ext/
+-rw-r--r--   0 jmcc       (501) staff       (20)       66 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/ext/__init__.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     2915 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     1953 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     5940 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.455731 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/ext/tests/
+-rw-r--r--   0 jmcc       (501) staff       (20)        0 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/ext/tests/__init__.py
+-rw-r--r--   0 jmcc       (501) staff       (20)      760 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/ext/tocdepthfix.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.456589 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/local/
+-rw-r--r--   0 jmcc       (501) staff       (20)      562 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.inv
+-rw-r--r--   0 jmcc       (501) staff       (20)     1638 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.txt
+-rw-r--r--   0 jmcc       (501) staff       (20)      658 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv
+-rw-r--r--   0 jmcc       (501) staff       (20)     2820 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt
+-rw-r--r--   0 jmcc       (501) staff       (20)      292 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/setup_package.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.435176 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.457708 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/
+-rw-r--r--   0 jmcc       (501) staff       (20)       73 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/globaltoc.html
+-rw-r--r--   0 jmcc       (501) staff       (20)     3433 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html
+-rw-r--r--   0 jmcc       (501) staff       (20)       34 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/localtoc.html
+-rw-r--r--   0 jmcc       (501) staff       (20)      272 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/searchbox.html
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.459571 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/
+-rw-r--r--   0 jmcc       (501) staff       (20)     5201 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg
+-rw-r--r--   0 jmcc       (501) staff       (20)     1725 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png
+-rw-r--r--   0 jmcc       (501) staff       (20)    32988 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico
+-rw-r--r--   0 jmcc       (501) staff       (20)     4634 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg
+-rw-r--r--   0 jmcc       (501) staff       (20)     1884 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png
+-rw-r--r--   0 jmcc       (501) staff       (20)    12067 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css
+-rw-r--r--   0 jmcc       (501) staff       (20)     2769 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js
+-rw-r--r--   0 jmcc       (501) staff       (20)     4971 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js
+-rw-r--r--   0 jmcc       (501) staff       (20)      192 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/theme.conf
+-rw-r--r--   0 jmcc       (501) staff       (20)      515 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/test_helpers.py
+-rw-r--r--   0 jmcc       (501) staff       (20)    27125 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/utils.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     6974 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/version.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     9755 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/astropy_helpers/version_helpers.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.448781 donuts-0.4.0/astropy_helpers/astropy_helpers.egg-info/
+-rw-r--r--   0 jmcc       (501) staff       (20)     2980 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 jmcc       (501) staff       (20)     3546 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 jmcc       (501) staff       (20)        1 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 jmcc       (501) staff       (20)        1 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers.egg-info/not-zip-safe
+-rw-r--r--   0 jmcc       (501) staff       (20)       16 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/astropy_helpers.egg-info/top_level.txt
+-rw-r--r--   0 jmcc       (501) staff       (20)    12537 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/ez_setup.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.460304 donuts-0.4.0/astropy_helpers/licenses/
+-rw-r--r--   0 jmcc       (501) staff       (20)     1644 2017-10-23 16:20:57.000000 donuts-0.4.0/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)     2505 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)     5959 2016-07-05 10:09:37.000000 donuts-0.4.0/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.461249 donuts-0.4.0/docs/
+-rw-r--r--   0 jmcc       (501) staff       (20)     4724 2016-06-03 09:55:32.000000 donuts-0.4.0/docs/Makefile
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.435520 donuts-0.4.0/docs/_templates/
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.461897 donuts-0.4.0/docs/_templates/autosummary/
+-rw-r--r--   0 jmcc       (501) staff       (20)      250 2016-06-03 09:55:32.000000 donuts-0.4.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)      251 2016-06-03 09:55:32.000000 donuts-0.4.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)      252 2016-06-03 09:55:32.000000 donuts-0.4.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)     6535 2024-05-07 09:20:32.125561 donuts-0.4.0/docs/conf.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.462745 donuts-0.4.0/docs/donuts/
+-rw-r--r--   0 jmcc       (501) staff       (20)     1455 2016-07-05 10:08:05.000000 donuts-0.4.0/docs/donuts/advanced.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)      105 2016-06-03 09:55:32.000000 donuts-0.4.0/docs/donuts/api.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)      906 2024-05-07 09:20:32.125809 donuts-0.4.0/docs/donuts/install.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)     5375 2016-07-05 10:08:05.000000 donuts-0.4.0/docs/donuts/user_guide.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)     4304 2016-07-05 10:08:05.000000 donuts-0.4.0/docs/index.rst
+-rw-r--r--   0 jmcc       (501) staff       (20)     4513 2016-06-03 09:55:32.000000 donuts-0.4.0/docs/make.bat
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.464014 donuts-0.4.0/donuts/
+-rw-r--r--   0 jmcc       (501) staff       (20)      524 2016-06-03 09:55:32.000000 donuts-0.4.0/donuts/__init__.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     5273 2016-06-03 09:55:32.000000 donuts-0.4.0/donuts/_astropy_init.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     1435 2016-06-03 09:55:32.000000 donuts-0.4.0/donuts/conftest.py
+-rw-r--r--   0 jmcc       (501) staff       (20)    10309 2024-05-07 09:20:32.126089 donuts-0.4.0/donuts/donuts.py
+-rw-r--r--   0 jmcc       (501) staff       (20)    17597 2024-05-07 16:33:12.438776 donuts-0.4.0/donuts/image.py
+drwxr-xr-x   0 jmcc       (501) staff       (20)        0 2024-05-07 16:35:53.466718 donuts-0.4.0/donuts/tests/
+-rw-r--r--   0 jmcc       (501) staff       (20)      121 2016-06-03 09:55:32.000000 donuts-0.4.0/donuts/tests/__init__.py
+-rw-r--r--   0 jmcc       (501) staff       (20)      768 2016-06-03 09:55:32.000000 donuts-0.4.0/donuts/tests/coveragerc
+-rw-r--r--   0 jmcc       (501) staff       (20)      450 2024-05-07 09:20:32.126722 donuts-0.4.0/donuts/tests/helpers.py
+-rw-r--r--   0 jmcc       (501) staff       (20)       96 2016-06-03 09:55:32.000000 donuts-0.4.0/donuts/tests/setup_package.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     1848 2024-05-07 09:20:32.126968 donuts-0.4.0/donuts/tests/synthetic_data.py
+-rw-r--r--   0 jmcc       (501) staff       (20)      505 2016-06-03 09:55:32.000000 donuts-0.4.0/donuts/tests/test_choosing_image_class.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     4115 2024-05-07 09:20:32.127209 donuts-0.4.0/donuts/tests/test_donuts_with_synthetic_data.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     9699 2016-06-03 09:55:32.000000 donuts-0.4.0/donuts/tests/test_image.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     2600 2016-06-03 09:55:32.000000 donuts-0.4.0/donuts/tests/test_integration.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     1396 2016-06-03 09:55:32.000000 donuts-0.4.0/donuts/tests/test_integration2.py
+-rw-r--r--   0 jmcc       (501) staff       (20)      258 2016-06-03 09:55:32.000000 donuts-0.4.0/donuts/tests/test_read_image.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     1243 2016-06-03 09:55:32.000000 donuts-0.4.0/donuts/tests/test_summary.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     2850 2016-06-03 09:55:32.000000 donuts-0.4.0/donuts/tests/test_synthetic_data.py
+-rw-r--r--   0 jmcc       (501) staff       (20)     7300 2024-05-07 16:35:53.303399 donuts-0.4.0/donuts/version.py
+-rw-r--r--   0 jmcc       (501) staff       (20)      289 2024-05-07 16:33:50.128328 donuts-0.4.0/donuts_version.py
+-rw-r--r--   0 jmcc       (501) staff       (20)    11477 2016-06-03 09:55:32.000000 donuts-0.4.0/ez_setup.py
+-rw-r--r--   0 jmcc       (501) staff       (20)      605 2024-05-07 09:20:32.156008 donuts-0.4.0/setup.cfg
+-rwxr-xr-x   0 jmcc       (501) staff       (20)     4506 2024-05-07 16:33:12.439887 donuts-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `donuts-0.3.5/PKG-INFO` & `donuts-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,132 +1,133 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: donuts
-Version: 0.3.5
+Version: 0.4.0
 Summary: Align astronomical images
 Home-page: https://github.com/jmccormac01/Donuts
 Author: James McCormac, Simon Walker
 Author-email: jmccormac001@gmail.com
 License: MIT
-Description: =======
-        Donuts
-        =======
-        
-        .. image:: https://img.shields.io/pypi/v/donuts.svg?text=version
-            :target: https://pypi.python.org/pypi/donuts
-            :alt: Latest Pypi Release
-        .. image:: https://img.shields.io/pypi/pyversions/donuts.svg
-            :target: https://pypi.python.org/pypi/donuts
-        .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
-            :target: http://www.astropy.org/
-            :alt: Powered by astropy
-        .. image:: https://travis-ci.org/jmccormac01/Donuts.svg?branch=master
-            :target: https://travis-ci.org/jmccormac01/Donuts
-            :alt: Travis Build Status
-        .. image:: https://ci.appveyor.com/api/projects/status/gs02nr4o4n2vdu22?svg=true
-            :target: https://ci.appveyor.com/project/JamesMcCormac/Donuts
-            :alt: Appveyor Build Status
-        .. image:: https://landscape.io/github/jmccormac01/Donuts/master/landscape.svg?style=flat
-            :target: https://landscape.io/github/jmccormac01/Donuts/master
-            :alt: Code Health
-        .. image:: https://coveralls.io/repos/github/jmccormac01/Donuts/badge.svg?branch=master 
-            :target: https://coveralls.io/github/jmccormac01/Donuts?branch=master
-            :alt: Test Coverage
-        .. image:: https://readthedocs.org/projects/donuts/badge/?version=latest
-            :target: http://donuts.readthedocs.io/en/latest/
-            :alt: Latest Documentation Status
-        .. image:: https://badges.gitter.im/jmccormac01/Donuts.svg?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
-            :target: https://gitter.im/jmccormac01/Donuts
-            :alt: Gitter Chat
-        
-        A science frame autoguiding and image alignment algorithm with sub-pixel
-        precision, capable of guiding on defocused stars.
-        
-        
-        Project documentation: https://donuts.readthedocs.io/en/latest/
-        
-        See the changelog_ for latest changes.
-        
-        Motivation
-        ----------
-        
-        We operate or have access to several telescopes (NGTS, NITES, Warwick
-        1m, 1.5m San Pedro Martir) that require precise autoguiding. Sometimes
-        we need to defocus a telescope but we would still like to autoguide. 
-        Donuts was designed to allow this. The algorithm had to be
-        simple, fast and accurate. It has been shown to perform well as an 
-        autoguiding algorithm for equatorial telescopes (no field rotation).
-        
-        The process of aligning apertures for photometry is essentially the same. 
-        Rather than correcting the telescope pointing, the apertures
-        must track the drift of the stars. Donuts can therefore be used to track
-        the stellar positions for CCD photometry also.
-        
-        By default Donuts measures frame-to-frame translational offsets (X
-        and Y) using all the stars in the image. The algorithm could be adjusted 
-        in the to select a specific region of interest (for extremely wide or
-        distorted fields).
-        
-        The algorithm has its limitations. It currently does not deal with
-        rotation or very large drifts - where the field moves by approx. half a FOV
-        or more. Our paper describing the details can be found here:
-        
-        http://adsabs.harvard.edu/abs/2013PASP..125..548M
-        
-        Example
-        -------
-        
-        Below is a sample of 10 nights autoguiding residuals from NGTS while using 
-        Donuts. The upper plot shows the frame-to-frame error, while the bottom 
-        shows the drift which would have occured if not for Donuts. Aligning 
-        photometry apertures is essentially the same process and similar performance
-        is expected under that scenario. We routinely achieve an autoguiding RMS of 
-        1/20 pixels with NGTS. 
-        
-        .. image:: AgResiduals_802_March2016.png
-        
-        Contributors
-        ------------
-        
-        `James McCormac <https://github.com/jmccormac01>`_,
-        `Simon Walker <https://github.com/mindriot101>`_.
-        
-        
-        License
-        -------
-        
-        MIT License
-        
-        Copyright (c) 2021 James McCormac & Simon Walker
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-        .. _changelog: https://github.com/jmccormac01/Donuts/blob/devel/CHANGELOG.md
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Dist: astropy
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-image
+
+=======
+Donuts
+=======
+
+.. image:: https://img.shields.io/pypi/v/donuts.svg?text=version
+    :target: https://pypi.python.org/pypi/donuts
+    :alt: Latest Pypi Release
+.. image:: https://img.shields.io/pypi/pyversions/donuts.svg
+    :target: https://pypi.python.org/pypi/donuts
+.. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
+    :target: http://www.astropy.org/
+    :alt: Powered by astropy
+.. image:: https://travis-ci.org/jmccormac01/Donuts.svg?branch=master
+    :target: https://travis-ci.org/jmccormac01/Donuts
+    :alt: Travis Build Status
+.. image:: https://ci.appveyor.com/api/projects/status/gs02nr4o4n2vdu22?svg=true
+    :target: https://ci.appveyor.com/project/JamesMcCormac/Donuts
+    :alt: Appveyor Build Status
+.. image:: https://landscape.io/github/jmccormac01/Donuts/master/landscape.svg?style=flat
+    :target: https://landscape.io/github/jmccormac01/Donuts/master
+    :alt: Code Health
+.. image:: https://coveralls.io/repos/github/jmccormac01/Donuts/badge.svg?branch=master 
+    :target: https://coveralls.io/github/jmccormac01/Donuts?branch=master
+    :alt: Test Coverage
+.. image:: https://readthedocs.org/projects/donuts/badge/?version=latest
+    :target: http://donuts.readthedocs.io/en/latest/
+    :alt: Latest Documentation Status
+.. image:: https://badges.gitter.im/jmccormac01/Donuts.svg?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
+    :target: https://gitter.im/jmccormac01/Donuts
+    :alt: Gitter Chat
+
+A science frame autoguiding and image alignment algorithm with sub-pixel
+precision, capable of guiding on defocused stars.
+
+
+Project documentation: https://donuts.readthedocs.io/en/latest/
+
+See the changelog_ for latest changes.
+
+Motivation
+----------
+
+We operate or have access to several telescopes (NGTS, NITES, Warwick
+1m, 1.5m San Pedro Martir) that require precise autoguiding. Sometimes
+we need to defocus a telescope but we would still like to autoguide. 
+Donuts was designed to allow this. The algorithm had to be
+simple, fast and accurate. It has been shown to perform well as an 
+autoguiding algorithm for equatorial telescopes (no field rotation).
+
+The process of aligning apertures for photometry is essentially the same. 
+Rather than correcting the telescope pointing, the apertures
+must track the drift of the stars. Donuts can therefore be used to track
+the stellar positions for CCD photometry also.
+
+By default Donuts measures frame-to-frame translational offsets (X
+and Y) using all the stars in the image. The algorithm could be adjusted 
+in the to select a specific region of interest (for extremely wide or
+distorted fields).
+
+The algorithm has its limitations. It currently does not deal with
+rotation or very large drifts - where the field moves by approx. half a FOV
+or more. Our paper describing the details can be found here:
+
+http://adsabs.harvard.edu/abs/2013PASP..125..548M
+
+Example
+-------
+
+Below is a sample of 10 nights autoguiding residuals from NGTS while using 
+Donuts. The upper plot shows the frame-to-frame error, while the bottom 
+shows the drift which would have occured if not for Donuts. Aligning 
+photometry apertures is essentially the same process and similar performance
+is expected under that scenario. We routinely achieve an autoguiding RMS of 
+1/20 pixels with NGTS. 
+
+.. image:: AgResiduals_802_March2016.png
+
+Contributors
+------------
+
+`James McCormac <https://github.com/jmccormac01>`_,
+`Simon Walker <https://github.com/mindriot101>`_.
+
+
+License
+-------
+
+MIT License
+
+Copyright (c) 2021 James McCormac & Simon Walker
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+.. _changelog: https://github.com/jmccormac01/Donuts/blob/devel/CHANGELOG.md
```

### Comparing `donuts-0.3.5/README.rst` & `donuts-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/ah_bootstrap.py` & `donuts-0.4.0/ah_bootstrap.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/CHANGES.rst` & `donuts-0.4.0/astropy_helpers/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/LICENSE.rst` & `donuts-0.4.0/astropy_helpers/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/README.rst` & `donuts-0.4.0/astropy_helpers/README.rst`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/ah_bootstrap.py` & `donuts-0.4.0/astropy_helpers/ah_bootstrap.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/__init__.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/commands/_dummy.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/commands/_dummy.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/commands/build_ext.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/commands/build_ext.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/commands/build_py.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/commands/build_py.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/commands/build_sphinx.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/commands/build_sphinx.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/commands/install_lib.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/commands/install_lib.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/commands/src/compiler.c` & `donuts-0.4.0/astropy_helpers/astropy_helpers/commands/src/compiler.c`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/commands/test.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/commands/test.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/distutils_helpers.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/distutils_helpers.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/extern/__init__.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/extern/automodapi/autodoc_enhancements.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/extern/automodapi/autodoc_enhancements.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/extern/automodapi/automodapi.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/extern/automodapi/automodapi.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/extern/automodapi/automodsumm.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/extern/automodapi/automodsumm.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/extern/automodapi/smart_resolver.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/extern/automodapi/smart_resolver.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/extern/automodapi/utils.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/extern/automodapi/utils.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape_sphinx.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape_sphinx.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/extern/numpydoc/numpydoc.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/extern/numpydoc/numpydoc.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/git_helpers.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/git_helpers.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/openmp_helpers.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/openmp_helpers.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/setup_helpers.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/conf.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/ext/tocdepthfix.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/ext/tocdepthfix.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.inv` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.inv`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.txt` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.txt`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js` & `donuts-0.4.0/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/test_helpers.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/test_helpers.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/utils.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/version.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/version.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers/version_helpers.py` & `donuts-0.4.0/astropy_helpers/astropy_helpers/version_helpers.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers.egg-info/PKG-INFO` & `donuts-0.4.0/astropy_helpers/astropy_helpers.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt` & `donuts-0.4.0/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/ez_setup.py` & `donuts-0.4.0/astropy_helpers/ez_setup.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst` & `donuts-0.4.0/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst` & `donuts-0.4.0/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst` & `donuts-0.4.0/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/docs/Makefile` & `donuts-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/docs/conf.py` & `donuts-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/docs/donuts/advanced.rst` & `donuts-0.4.0/docs/donuts/advanced.rst`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/docs/donuts/install.rst` & `donuts-0.4.0/docs/donuts/install.rst`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/docs/donuts/user_guide.rst` & `donuts-0.4.0/docs/donuts/user_guide.rst`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/docs/index.rst` & `donuts-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/docs/make.bat` & `donuts-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/donuts/__init__.py` & `donuts-0.4.0/donuts/__init__.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/donuts/_astropy_init.py` & `donuts-0.4.0/donuts/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/donuts/conftest.py` & `donuts-0.4.0/donuts/conftest.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/donuts/donuts.py` & `donuts-0.4.0/donuts/donuts.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/donuts/image.py` & `donuts-0.4.0/donuts/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 import warnings
 import numpy as np
 from astropy import units as u
-from scipy import (
-    conjugate,
-    polyfit,
-)
 from scipy.fftpack import fft, ifft
 from skimage.transform import resize
 
 # pylint: disable=invalid-name
 
 class Image(object):
     '''Low level class which handles the image transformations and cross
@@ -416,48 +412,48 @@
         '''
         tst = np.empty(3)
         if z_pos[0][0] <= len(phi_ref_check_m) / 2 and z_pos[0][0] != 0:
             lra = [z_pos[0][0] - 1, z_pos[0][0], z_pos[0][0] + 1]
             tst[0] = phi_ref_check_m[lra[0]].real
             tst[1] = phi_ref_check_m[lra[1]].real
             tst[2] = phi_ref_check_m[lra[2]].real
-            coeffs = polyfit(lra, tst, 2)
+            coeffs = np.polyfit(lra, tst, 2)
             solution = -(-coeffs[1] / (2 * coeffs[0]))
         elif z_pos[0][0] > len(phi_ref_check_m) / 2 and z_pos[0][0] != len(phi_ref_check_m) - 1:
             lra = [z_pos[0][0] - 1, z_pos[0][0], z_pos[0][0] + 1]
             tst[0] = phi_ref_check_m[lra[0]].real
             tst[1] = phi_ref_check_m[lra[1]].real
             tst[2] = phi_ref_check_m[lra[2]].real
-            coeffs = polyfit(lra, tst, 2)
+            coeffs = np.polyfit(lra, tst, 2)
             solution = len(phi_ref_check_m) + (coeffs[1] / (2 * coeffs[0]))
         elif z_pos[0][0] == len(phi_ref_check_m) - 1:
             lra = [-1, 0, 1]
             tst[0] = phi_ref_check_m[-2].real
             tst[1] = phi_ref_check_m[-1].real
             tst[2] = phi_ref_check_m[0].real
-            coeffs = polyfit(lra, tst, 2)
+            coeffs = np.polyfit(lra, tst, 2)
             solution = 1 + (coeffs[1] / (2 * coeffs[0]))
         else:  # if z_pos[0][0] == 0:
             lra = [1, 0, -1]
             tst[0] = phi_ref_check_m[-1].real
             tst[1] = phi_ref_check_m[0].real
             tst[2] = phi_ref_check_m[1].real
-            coeffs = polyfit(lra, tst, 2)
+            coeffs = np.polyfit(lra, tst, 2)
             solution = -coeffs[1] / (2 * coeffs[0])
         return solution * u.pixel
 
     def _cross_correlate(self, reference_image):
         # FFT of the projection spectra
         f_ref_xproj = fft(reference_image.proj_x)
         f_ref_yproj = fft(reference_image.proj_y)
         f_check_xproj = fft(self.proj_x)
         f_check_yproj = fft(self.proj_y)
         # cross correlate in and look for the maximium correlation
-        f_ref_xproj_conj = conjugate(f_ref_xproj)
-        f_ref_yproj_conj = conjugate(f_ref_yproj)
+        f_ref_xproj_conj = np.conjugate(f_ref_xproj)
+        f_ref_yproj_conj = np.conjugate(f_ref_yproj)
         complex_sum_x = f_ref_xproj_conj * f_check_xproj
         complex_sum_y = f_ref_yproj_conj * f_check_yproj
         phi_ref_check_m_x = ifft(complex_sum_x)
         phi_ref_check_m_y = ifft(complex_sum_y)
         z_x = max(phi_ref_check_m_x)
         z_pos_x = np.where(phi_ref_check_m_x == z_x)
         z_y = max(phi_ref_check_m_y)
```

### Comparing `donuts-0.3.5/donuts/tests/coveragerc` & `donuts-0.4.0/donuts/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/donuts/tests/synthetic_data.py` & `donuts-0.4.0/donuts/tests/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/donuts/tests/test_donuts_with_synthetic_data.py` & `donuts-0.4.0/donuts/tests/test_donuts_with_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/donuts/tests/test_image.py` & `donuts-0.4.0/donuts/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/donuts/tests/test_integration.py` & `donuts-0.4.0/donuts/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/donuts/tests/test_integration2.py` & `donuts-0.4.0/donuts/tests/test_integration2.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/donuts/tests/test_summary.py` & `donuts-0.4.0/donuts/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/donuts/tests/test_synthetic_data.py` & `donuts-0.4.0/donuts/tests/test_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/donuts/version.py` & `donuts-0.4.0/donuts/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Autogenerated by Astropy-affiliated package donuts's setup.py on 2022-01-06 20:14:29
+# Autogenerated by Astropy-affiliated package donuts's setup.py on 2024-05-07 16:35:53
 from __future__ import unicode_literals
 import datetime
 
 
 import locale
 import os
 import subprocess
@@ -182,16 +182,16 @@
             break
 
         current_dir = os.path.dirname(current_dir)
 
     return None
 
 _packagename = "donuts"
-_last_generated_version = "0.3.5"
-_last_githash = "ba1dbb8f6f721e52008611a87bdc1b8900b5bd66"
+_last_generated_version = "0.4.0"
+_last_githash = "df49d7805c45265ad15e44b462badfffedbaf03b"
 
 # Determine where the source code for this module
 # lives.  If __file__ is not a filesystem path then
 # it is assumed not to live in a git repo at all.
 if _get_repo_path(__file__, levels=len(_packagename.split('.'))):
     version = update_git_devstr(_last_generated_version, path=__file__)
     githash = get_git_devstr(sha=True, show_warning=False,
@@ -200,19 +200,19 @@
     # The file does not appear to live in a git repo so don't bother
     # invoking git
     version = _last_generated_version
     githash = _last_githash
 
 
 major = 0
-minor = 3
-bugfix = 5
+minor = 4
+bugfix = 0
 
 release = True
-timestamp = datetime.datetime(2022, 1, 6, 20, 14, 29)
+timestamp = datetime.datetime(2024, 5, 7, 16, 35, 53)
 debug = False
 
 try:
     from ._compiler import compiler
 except ImportError:
     compiler = "unknown"
```

### Comparing `donuts-0.3.5/ez_setup.py` & `donuts-0.4.0/ez_setup.py`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/setup.cfg` & `donuts-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `donuts-0.3.5/setup.py` & `donuts-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,21 +108,18 @@
       long_description=LONG_DESCRIPTION,
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: MIT License',
           'Operating System :: OS Independent',
           'Programming Language :: Python',
-          'Programming Language :: Python :: 2',
-          'Programming Language :: Python :: 2.7',
           'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.3',
-          'Programming Language :: Python :: 3.4',
-          'Programming Language :: Python :: 3.5',
+          'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
           'Topic :: Scientific/Engineering :: Astronomy',
       ],        
       cmdclass=cmdclassd,
       zip_safe=False,
-      use_2to3=True,
       entry_points=entry_points,
       **package_info
 )
```

