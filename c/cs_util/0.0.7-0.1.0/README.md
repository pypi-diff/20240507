# Comparing `tmp/cs_util-0.0.7.tar.gz` & `tmp/cs_util-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mkilbing/astro/repositories/github/cs_util/dist/.tmp-poly4njj/cs_util-0.0.7.tar", last modified: Wed Jan 24 16:50:34 2024, max compression
+gzip compressed data, was "cs_util-0.1.0.tar", max compression
```

## Comparing `cs_util-0.0.7.tar` & `cs_util-0.1.0.tar`

### file list

```diff
@@ -1,69 +1,21 @@
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2024-01-24 16:50:34.455788 cs_util-0.0.7/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       73 2022-09-28 15:28:14.000000 cs_util-0.0.7/.coveragerc
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2024-01-24 16:50:34.396788 cs_util-0.0.7/.github/
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2024-01-24 16:50:34.412788 cs_util-0.0.7/.github/workflows/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2195 2022-09-28 15:31:29.000000 cs_util-0.0.7/.github/workflows/cd-build.yml
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2945 2022-09-28 15:31:29.000000 cs_util-0.0.7/.github/workflows/ci-build.yml
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2237 2022-10-19 08:52:59.000000 cs_util-0.0.7/.gitignore
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       41 2022-09-28 15:28:14.000000 cs_util-0.0.7/.pylintrc
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      245 2022-09-28 15:28:14.000000 cs_util-0.0.7/.pyup.yml
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     3219 2022-09-28 15:28:14.000000 cs_util-0.0.7/CODE_OF_CONDUCT.md
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      115 2022-09-28 15:28:14.000000 cs_util-0.0.7/CONTRIBUTING.md
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1073 2022-09-28 15:31:29.000000 cs_util-0.0.7/LICENCE.txt
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      113 2022-09-28 15:28:14.000000 cs_util-0.0.7/MANIFEST.in
--rw-r--r--   0 mkilbing  (1016) mkilbing  (1016)     4082 2024-01-24 16:50:34.455788 cs_util-0.0.7/PKG-INFO
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2467 2023-09-14 09:44:57.000000 cs_util-0.0.7/README.md
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2024-01-24 16:50:34.420788 cs_util-0.0.7/cs_util/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      869 2024-01-24 15:58:53.000000 cs_util-0.0.7/cs_util/__init__.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1379 2023-09-14 09:45:17.000000 cs_util-0.0.7/cs_util/calc.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     3176 2023-09-14 09:45:17.000000 cs_util-0.0.7/cs_util/canfar.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     5530 2023-09-14 09:45:17.000000 cs_util-0.0.7/cs_util/cat.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2306 2023-09-14 09:45:17.000000 cs_util-0.0.7/cs_util/cfis.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     7671 2023-09-14 09:45:17.000000 cs_util-0.0.7/cs_util/cosmo.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1504 2023-09-14 09:44:57.000000 cs_util-0.0.7/cs_util/logging.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     7984 2024-01-24 15:15:52.000000 cs_util-0.0.7/cs_util/plots.py
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2024-01-24 16:50:34.432788 cs_util-0.0.7/cs_util/tests/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       61 2023-06-21 12:32:56.000000 cs_util-0.0.7/cs_util/tests/__init__.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1522 2023-09-14 09:45:17.000000 cs_util-0.0.7/cs_util/tests/test_calc.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1032 2023-09-14 09:44:57.000000 cs_util-0.0.7/cs_util/tests/test_canfar.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2647 2023-09-14 09:45:17.000000 cs_util-0.0.7/cs_util/tests/test_cat.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     3731 2023-09-14 09:45:17.000000 cs_util-0.0.7/cs_util/tests/test_cfis.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     8337 2023-09-14 09:45:17.000000 cs_util-0.0.7/cs_util/tests/test_cosmo.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     3189 2023-09-14 09:45:17.000000 cs_util-0.0.7/cs_util/tests/test_logging.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2314 2023-09-14 09:44:57.000000 cs_util-0.0.7/cs_util/tests/test_plots.py
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2024-01-24 16:50:34.452788 cs_util-0.0.7/cs_util.egg-info/
--rw-r--r--   0 mkilbing  (1016) mkilbing  (1016)     4082 2024-01-24 16:50:34.000000 cs_util-0.0.7/cs_util.egg-info/PKG-INFO
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1263 2024-01-24 16:50:34.000000 cs_util-0.0.7/cs_util.egg-info/SOURCES.txt
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)        1 2024-01-24 16:50:34.000000 cs_util-0.0.7/cs_util.egg-info/dependency_links.txt
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      210 2024-01-24 16:50:34.000000 cs_util-0.0.7/cs_util.egg-info/requires.txt
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)        8 2024-01-24 16:50:34.000000 cs_util-0.0.7/cs_util.egg-info/top_level.txt
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       70 2022-10-16 16:28:42.000000 cs_util-0.0.7/develop.txt
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2024-01-24 16:50:34.433788 cs_util-0.0.7/docs/
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2024-01-24 16:50:34.436788 cs_util-0.0.7/docs/_script_templates/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      174 2022-09-28 15:28:14.000000 cs_util-0.0.7/docs/_script_templates/module.rst_t
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1070 2022-09-28 15:28:14.000000 cs_util-0.0.7/docs/_script_templates/package.rst_t
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      128 2022-09-28 15:28:14.000000 cs_util-0.0.7/docs/_script_templates/toc.rst_t
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2024-01-24 16:50:34.439788 cs_util-0.0.7/docs/_templates/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      174 2022-09-28 15:28:14.000000 cs_util-0.0.7/docs/_templates/module.rst_t
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1060 2022-09-28 15:28:14.000000 cs_util-0.0.7/docs/_templates/package.rst_t
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      128 2022-09-28 15:28:14.000000 cs_util-0.0.7/docs/_templates/toc.rst_t
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      138 2022-09-28 15:28:14.000000 cs_util-0.0.7/docs/requirements.txt
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2024-01-24 16:50:34.449788 cs_util-0.0.7/docs/source/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      119 2022-09-28 15:28:14.000000 cs_util-0.0.7/docs/source/about.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      318 2022-09-28 15:28:14.000000 cs_util-0.0.7/docs/source/citing.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     7060 2023-09-14 09:44:57.000000 cs_util-0.0.7/docs/source/conf.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      422 2022-09-28 15:31:29.000000 cs_util-0.0.7/docs/source/contributing.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      811 2022-09-28 15:28:14.000000 cs_util-0.0.7/docs/source/index.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      680 2022-09-28 15:31:29.000000 cs_util-0.0.7/docs/source/installation.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      120 2022-09-28 15:28:14.000000 cs_util-0.0.7/docs/source/my_ref.bib
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      262 2022-09-28 15:31:29.000000 cs_util-0.0.7/docs/source/quickstart.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2743 2023-06-21 12:32:56.000000 cs_util-0.0.7/docs/source/refs.bib
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      395 2022-10-16 16:56:43.000000 cs_util-0.0.7/docs/source/toc.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       67 2022-09-28 15:28:14.000000 cs_util-0.0.7/docs/source/z_ref.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      117 2022-10-16 17:46:09.000000 cs_util-0.0.7/environment.yml
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1763 2024-01-24 15:49:37.000000 cs_util-0.0.7/pyproject.toml
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       51 2023-09-14 09:45:17.000000 cs_util-0.0.7/requirements.txt
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2024-01-24 16:50:34.451788 cs_util-0.0.7/scripts/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      628 2022-09-28 15:28:14.000000 cs_util-0.0.7/scripts/__init__.py
--rwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)     2359 2023-09-14 09:44:57.000000 cs_util-0.0.7/scripts/example_script.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       38 2024-01-24 16:50:34.456788 cs_util-0.0.7/setup.cfg
+-rw-r--r--   0        0        0     2467 2023-08-24 16:31:13.459486 cs_util-0.1.0/README.md
+-rw-r--r--   0        0        0      869 2024-05-07 12:41:15.421287 cs_util-0.1.0/cs_util/__init__.py
+-rw-r--r--   0        0        0     5636 2024-05-07 12:41:15.421287 cs_util-0.1.0/cs_util/args.py
+-rw-r--r--   0        0        0     1379 2023-08-24 16:31:15.915513 cs_util-0.1.0/cs_util/calc.py
+-rw-r--r--   0        0        0     3176 2023-08-24 16:31:13.459486 cs_util-0.1.0/cs_util/canfar.py
+-rw-r--r--   0        0        0     5530 2024-04-30 09:33:53.574745 cs_util-0.1.0/cs_util/cat.py
+-rw-r--r--   0        0        0     2305 2024-05-07 12:41:15.421287 cs_util-0.1.0/cs_util/cfis.py
+-rw-r--r--   0        0        0     7671 2024-04-30 09:33:53.574745 cs_util-0.1.0/cs_util/cosmo.py
+-rw-r--r--   0        0        0     1503 2024-05-07 12:41:15.421287 cs_util-0.1.0/cs_util/logging.py
+-rw-r--r--   0        0        0     8102 2024-05-07 12:41:15.421287 cs_util-0.1.0/cs_util/plots.py
+-rw-r--r--   0        0        0       61 2023-08-24 15:45:50.967664 cs_util-0.1.0/cs_util/tests/__init__.py
+-rw-r--r--   0        0        0     4071 2024-05-07 12:41:15.421287 cs_util-0.1.0/cs_util/tests/test_args.py
+-rw-r--r--   0        0        0     1522 2023-08-24 16:31:13.459486 cs_util-0.1.0/cs_util/tests/test_calc.py
+-rw-r--r--   0        0        0     1032 2023-08-24 16:31:13.463486 cs_util-0.1.0/cs_util/tests/test_canfar.py
+-rw-r--r--   0        0        0     2647 2023-08-24 16:31:13.463486 cs_util-0.1.0/cs_util/tests/test_cat.py
+-rw-r--r--   0        0        0     3731 2023-08-24 16:31:13.463486 cs_util-0.1.0/cs_util/tests/test_cfis.py
+-rw-r--r--   0        0        0     8332 2024-05-07 12:41:15.421287 cs_util-0.1.0/cs_util/tests/test_cosmo.py
+-rw-r--r--   0        0        0     3189 2023-08-24 16:31:15.915513 cs_util-0.1.0/cs_util/tests/test_logging.py
+-rw-r--r--   0        0        0     2314 2023-08-24 16:31:13.463486 cs_util-0.1.0/cs_util/tests/test_plots.py
+-rw-r--r--   0        0        0      836 2024-05-07 15:46:08.837407 cs_util-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 cs_util-0.1.0/PKG-INFO
```

### Comparing `cs_util-0.0.7/PKG-INFO` & `cs_util-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,27 @@
 Metadata-Version: 2.1
 Name: cs_util
-Version: 0.0.7
-Author: The CosmoStat Lab
-Maintainer-email: Martin Kilbinger <martin.kilbinger@cea.fr>
-Project-URL: Source, https://github.com/CosmoStat/cs_util
-Project-URL: Documentation, https://github.com/CosmoStat/cs_util
-Project-URL: Tracker, https://github.com/CosmoStat/cs_util/issues
-Keywords: CosmoStat,cosmology,weak gravitational lensing
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: OSI Approved :: MIT License
+Version: 0.1.0
+Summary: Utility library for CosmoStat
+Author: Martin Kilbinger
+Author-email: martin.kilbinger@cea.fr
+Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: astropy (==5.2)
+Requires-Dist: camb (==1.5.4)
+Requires-Dist: datetime (>=5.5,<6.0)
+Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
+Requires-Dist: swig (>=4.2.1,<5.0.0)
+Requires-Dist: vos (>=3.6.1,<4.0.0)
 Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-Requires-Dist: astropy>=4.0
-Requires-Dist: datetime>=4.7
-Requires-Dist: matplotlib>=3.3
-Requires-Dist: numpy>=1.21
-Requires-Dist: vos>=3.3
-Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
-Requires-Dist: jinja2==3.0; extra == "lint"
-Provides-Extra: release
-Requires-Dist: build; extra == "release"
-Requires-Dist: twine; extra == "release"
-Requires-Dist: sdist; extra == "release"
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-black; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
-Requires-Dist: pytest-pydocstyle; extra == "test"
-Provides-Extra: dev
-Requires-Dist: cs_util[lint,release,test]; extra == "dev"
 
 # cs_util package
 
 Utility library for CosmoStat
 
 | Usage | Development | Release |
 | ----- | ----------- | ------- |
@@ -67,7 +46,8 @@
 - Galaxy catalogue handling
 - Weak-lensing related cosmological quantities (e.g. surface mass density)
 - VOS (Virtual Observatory Software)
 - Command line logging
 - Plotting
 - Basic statistic calculations
 - UNIONS/CFIS weak-lensing survey handling
+
```

#### html2text {}

```diff
@@ -1,53 +1,40 @@
-Metadata-Version: 2.1 Name: cs_util Version: 0.0.7 Author: The CosmoStat Lab
-Maintainer-email: Martin Kilbinger
-cea.fr> Project-URL: Source, https://github.com/CosmoStat/cs_util Project-URL:
-Documentation, https://github.com/CosmoStat/cs_util Project-URL: Tracker,
-https://github.com/CosmoStat/cs_util/issues Keywords: CosmoStat,cosmology,weak
-gravitational lensing Classifier: Development Status :: 1 - Planning
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: POSIX :: Linux Classifier: Operating System ::
-MacOS Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENCE.txt Requires-
-Dist: astropy>=4.0 Requires-Dist: datetime>=4.7 Requires-Dist: matplotlib>=3.3
-Requires-Dist: numpy>=1.21 Requires-Dist: vos>=3.3 Provides-Extra: lint
-Requires-Dist: black; extra == "lint" Requires-Dist: jinja2==3.0; extra ==
-"lint" Provides-Extra: release Requires-Dist: build; extra == "release"
-Requires-Dist: twine; extra == "release" Requires-Dist: sdist; extra ==
-"release" Provides-Extra: test Requires-Dist: pytest; extra == "test" Requires-
-Dist: pytest-black; extra == "test" Requires-Dist: pytest-cov; extra == "test"
-Requires-Dist: pytest-pydocstyle; extra == "test" Provides-Extra: dev Requires-
-Dist: cs_util[lint,release,test]; extra == "dev" # cs_util package Utility
-library for CosmoStat | Usage | Development | Release | | ----- | ----------- |
-------- | | [![docs](https://img.shields.io/badge/docs-Sphinx-blue)](https://
-martinkilbinger.github.io/cs_util/) | [![build](https://github.com/
-martinkilbinger/cs_util/workflows/CI/badge.svg)](https://github.com/
-martinkilbinger/cs_util/actions?query=workflow%3ACI) | [![release](https://
-img.shields.io/github/v/release/martinkilbinger/cs_util)](https://github.com/
-martinkilbinger/cs_util/releases/latest) | | [![license](https://
-img.shields.io/github/license/martinkilbinger/cs_util)](https://github.com/
-martinkilbinger/cs_util/blob/master/LICENCE.txt) | [![deploy](https://
-github.com/martinkilbinger/cs_util/workflows/CD/badge.svg)](https://github.com/
-martinkilbinger/cs_util/actions?query=workflow%3ACD) | [![pypi](https://
-img.shields.io/pypi/v/cs_util)](https://pypi.org/project/cs_util/) | | [!
-[wemake-python-styleguide](https://img.shields.io/badge/style-wemake-
-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide) | [!
-[codecov](https://codecov.io/gh/martinkilbinger/cs_util/branch/master/graph/
-badge.svg?token=XHJIQXV7AX)](https://codecov.io/gh/martinkilbinger/cs_util) |
-[![python](https://img.shields.io/pypi/pyversions/cs_util)](https://
-www.python.org/downloads/source/) | | [![contribute](https://img.shields.io/
-badge/contribute-read-lightgrey)](https://github.com/martinkilbinger/cs_util/
-blob/master/CONTRIBUTING.md) | [![CodeFactor](https://www.codefactor.io/
-repository/github/martinkilbinger/cs_util/badge)](https://www.codefactor.io/
-repository/github/martinkilbinger/cs_util) | | | [![coc](https://
-img.shields.io/badge/conduct-read-lightgrey)](https://github.com/
-martinkilbinger/cs_util/blob/master/CODE_OF_CONDUCT.md) | [![Updates](https://
-pyup.io/repos/github/martinkilbinger/cs_util/shield.svg)](https://pyup.io/
-repos/github/martinkilbinger/cs_util/) | | --- > Author: _M_a_r_t_i_n_ _K_i_l_b_i_n_g_e_r >
-Email: _m_a_r_t_i_n_._k_i_l_b_i_n_g_e_r_@_c_e_a_._f_r > Year: 2022 --- ## Contents ### Library -
-Galaxy catalogue handling - Weak-lensing related cosmological quantities (e.g.
-surface mass density) - VOS (Virtual Observatory Software) - Command line
-logging - Plotting - Basic statistic calculations - UNIONS/CFIS weak-lensing
-survey handling
+Metadata-Version: 2.1 Name: cs_util Version: 0.1.0 Summary: Utility library for
+CosmoStat Author: Martin Kilbinger Author-email: martin.kilbinger@cea.fr
+Requires-Python: >=3.9,<3.12 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: astropy (==5.2) Requires-Dist: camb (==1.5.4) Requires-Dist:
+datetime (>=5.5,<6.0) Requires-Dist: matplotlib (>=3.8.4,<4.0.0) Requires-Dist:
+numpy (>=1.26.4,<2.0.0) Requires-Dist: scipy (>=1.13.0,<2.0.0) Requires-Dist:
+swig (>=4.2.1,<5.0.0) Requires-Dist: vos (>=3.6.1,<4.0.0) Description-Content-
+Type: text/markdown # cs_util package Utility library for CosmoStat | Usage |
+Development | Release | | ----- | ----------- | ------- | | [![docs](https://
+img.shields.io/badge/docs-Sphinx-blue)](https://martinkilbinger.github.io/
+cs_util/) | [![build](https://github.com/martinkilbinger/cs_util/workflows/CI/
+badge.svg)](https://github.com/martinkilbinger/cs_util/
+actions?query=workflow%3ACI) | [![release](https://img.shields.io/github/v/
+release/martinkilbinger/cs_util)](https://github.com/martinkilbinger/cs_util/
+releases/latest) | | [![license](https://img.shields.io/github/license/
+martinkilbinger/cs_util)](https://github.com/martinkilbinger/cs_util/blob/
+master/LICENCE.txt) | [![deploy](https://github.com/martinkilbinger/cs_util/
+workflows/CD/badge.svg)](https://github.com/martinkilbinger/cs_util/
+actions?query=workflow%3ACD) | [![pypi](https://img.shields.io/pypi/v/cs_util)]
+(https://pypi.org/project/cs_util/) | | [![wemake-python-styleguide](https://
+img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-
+services/wemake-python-styleguide) | [![codecov](https://codecov.io/gh/
+martinkilbinger/cs_util/branch/master/graph/badge.svg?token=XHJIQXV7AX)](https:
+//codecov.io/gh/martinkilbinger/cs_util) | [![python](https://img.shields.io/
+pypi/pyversions/cs_util)](https://www.python.org/downloads/source/) | | [!
+[contribute](https://img.shields.io/badge/contribute-read-lightgrey)](https://
+github.com/martinkilbinger/cs_util/blob/master/CONTRIBUTING.md) | [!
+[CodeFactor](https://www.codefactor.io/repository/github/martinkilbinger/
+cs_util/badge)](https://www.codefactor.io/repository/github/martinkilbinger/
+cs_util) | | | [![coc](https://img.shields.io/badge/conduct-read-lightgrey)]
+(https://github.com/martinkilbinger/cs_util/blob/master/CODE_OF_CONDUCT.md) |
+[![Updates](https://pyup.io/repos/github/martinkilbinger/cs_util/shield.svg)]
+(https://pyup.io/repos/github/martinkilbinger/cs_util/) | | --- > Author:
+_M_a_r_t_i_n_ _K_i_l_b_i_n_g_e_r > Email: _m_a_r_t_i_n_._k_i_l_b_i_n_g_e_r_@_c_e_a_._f_r > Year: 2022 --- ## Contents
+### Library - Galaxy catalogue handling - Weak-lensing related cosmological
+quantities (e.g. surface mass density) - VOS (Virtual Observatory Software) -
+Command line logging - Plotting - Basic statistic calculations - UNIONS/CFIS
+weak-lensing survey handling
```

### Comparing `cs_util-0.0.7/README.md` & `cs_util-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.7/cs_util/__init__.py` & `cs_util-0.1.0/cs_util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     supressed in this module to allow the defintion of a package
     ``__version__``, which is standard for most Python packages.
 
 """
 
 from warnings import warn
 
-__version__ = "0.0.7"
+__version__ = "0.1.0"
```

### Comparing `cs_util-0.0.7/cs_util/calc.py` & `cs_util-0.1.0/cs_util/calc.py`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.7/cs_util/canfar.py` & `cs_util-0.1.0/cs_util/canfar.py`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.7/cs_util/cat.py` & `cs_util-0.1.0/cs_util/cat.py`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.7/cs_util/cfis.py` & `cs_util-0.1.0/cs_util/cfis.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 :Description: This script contains CFIS-specific methods.
 
 :Author: Martin Kilbinger <martin.kilbinger@cea.fr>
 
 """
 
-
 import re
 import numpy as np
 from astropy import units
 from astropy import coordinates as coords
 
 
 class Cfis(object):
```

### Comparing `cs_util-0.0.7/cs_util/cosmo.py` & `cs_util-0.1.0/cs_util/cosmo.py`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.7/cs_util/logging.py` & `cs_util-0.1.0/cs_util/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 :Description: This script contains utility methods for job execution and
 progress logging.
 
 :Author: Martin Kilbinger <martin.kilblinger@cea.fr>
 
 """
 
-
 import os
 import sys
 
 
 def log_command(argv, name=None, close_no_return=True):
     """Log Command.
```

### Comparing `cs_util-0.0.7/cs_util/plots.py` & `cs_util-0.1.0/cs_util/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 :Description: This file contains methods for plotting.
 
 :Author: Martin Kilbinger <martin.kilbinger@cea.fr>
 
 """
 
-
 import matplotlib.pylab as plt
 import numpy as np
 
 
 def figure(figsize=(30, 30)):
     """Figure.
 
@@ -49,15 +48,16 @@
     """
     plt.savefig(fname, facecolor="w", bbox_inches="tight")
     if close_fig:
         plt.close()
 
 
 def dx(idx, nx=3, fx=1.025, log=True):
-    """Dx Plot.
+    """Dx.
+
     Return small shift useful to diplace points along the the x-axis
     for a more readable plot.
 
     Parameters
     ----------
     idx : int
         dataset index
@@ -70,14 +70,15 @@
 
     """
     if log:
         return fx ** (idx - (nx - 1) / 2)
     else:
         return fx * (idx - (nx - 1) / 2)
 
+
 def plot_histograms(
     xs,
     labels,
     title,
     x_label,
     y_label,
     x_range,
@@ -201,15 +202,15 @@
     colors=None,
     linestyles=None,
     eb_linestyles=None,
     linewidths=None,
     markers=None,
     xlim=None,
     ylim=None,
-    shift_x=True,
+    shift_x=False,
     close_fig=True,
 ):
     """Plot Data 1D.
 
     Plot one-dimensional data points with errorbars.
 
     Parameters
@@ -257,23 +258,26 @@
     if linestyles is None:
         linestyles = ["-"] * len(x)
     if eb_linestyles is None:
         eb_linestyles = ["-"] * len(x)
     if linewidths is None:
         linewidths = [2] * len(x)
     if markers is None:
-        markers = ['o'] * len(x)
+        markers = ["o"] * len(x)
 
     if create_figure:
         figure(figsize=(10, 10))
 
     for idx in range(len(x)):
         this_x = x[idx]
         if shift_x:
-            this_x *= dx(idx, len(x), log=xlog)
+            if xlog:
+                this_x *= dx(idx, len(x), log=xlog)
+            else:
+                raise ValueError("shift_x without log not implemented yet")
         if np.isnan(yerr[idx]).all():
             eb = plt.plot(
                 this_x,
                 y[idx],
                 label=labels[idx],
                 color=colors[idx],
                 linestyle=linestyles[idx],
@@ -288,15 +292,15 @@
                 linestyle=linestyles[idx],
                 marker=markers[idx],
                 markerfacecolor="none",
                 capsize=4,
             )
             eb[-1][0].set_linestyle(eb_linestyles[idx])
 
-    plt.axhline(color="k", linestyle="dashed", linewidth=linewidths[0]/2)
+    plt.axhline(color="k", linestyle="dashed", linewidth=linewidths[0] / 2)
 
     if xlog:
         plt.xscale("log")
         plt.xticks(
             [0.1, 0.2, 0.5, 1, 2, 5, 10, 20, 50, 100, 200, 500],
             labels=[
                 "0.1",
```

### Comparing `cs_util-0.0.7/cs_util/tests/test_calc.py` & `cs_util-0.1.0/cs_util/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.7/cs_util/tests/test_canfar.py` & `cs_util-0.1.0/cs_util/tests/test_canfar.py`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.7/cs_util/tests/test_cat.py` & `cs_util-0.1.0/cs_util/tests/test_cat.py`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.7/cs_util/tests/test_cfis.py` & `cs_util-0.1.0/cs_util/tests/test_cfis.py`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.7/cs_util/tests/test_cosmo.py` & `cs_util-0.1.0/cs_util/tests/test_cosmo.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     def setUp(self):
         """Set test parameter values."""
         self._z_source = 0.8
         self._z_lens = 0.5
         self._z_source_arr = [0.4, 0.6, 0.8, 0.9]
         self._nz_source_arr = [0.5, 0.6, 2.2, 1.6]
-        self._cosmo = ccl.core.CosmologyVanillaLCDM()
+        self._cosmo = ccl.CosmologyVanillaLCDM()
         self._sigma_crit_value = 3920.1478
         # Value verified with package dsigma as 3919.700
 
         self._sigma_crit_value_eff = 3917.2681
         self._sigma_crit_value_eff_m1 = 0.0002267
 
         self._sigma_crit_unit = units.Msun / units.pc**2
@@ -83,15 +83,15 @@
             self._z_source,
             self._cosmo,
         )
         # Test return value
         npt.assert_almost_equal(
             sigma_crit.value,
             self._sigma_crit_value,
-            decimal=4,
+            decimal=3,
         )
         # Test return unit
         npt.assert_equal(sigma_crit.unit, self._sigma_crit_unit)
 
         # Test with lens behind source
         sigma_crit = cosmo.sigma_crit(
             self._z_lens, self._z_lens / 2, self._cosmo
@@ -144,15 +144,15 @@
             self._nz_source_arr,
             self._cosmo,
         )
         # Test return value
         npt.assert_almost_equal(
             sigma_crit_eff.value,
             self._sigma_crit_value_eff,
-            decimal=4,
+            decimal=3,
         )
 
         # Test return unit
         npt.assert_equal(sigma_crit_eff.unit, self._sigma_crit_unit)
 
         # Test exception
         self.assertRaises(
```

### Comparing `cs_util-0.0.7/cs_util/tests/test_logging.py` & `cs_util-0.1.0/cs_util/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.7/cs_util/tests/test_plots.py` & `cs_util-0.1.0/cs_util/tests/test_plots.py`

 * *Files identical despite different names*

