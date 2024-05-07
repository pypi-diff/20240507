# Comparing `tmp/plasmapy_sphinx-0.1.0a4.tar.gz` & `tmp/plasmapy_sphinx-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plasmapy_sphinx-0.1.0a4.tar", last modified: Thu Apr 25 18:04:19 2024, max compression
+gzip compressed data, was "plasmapy_sphinx-0.1.0a5.tar", last modified: Tue May  7 00:16:01 2024, max compression
```

## Comparing `plasmapy_sphinx-0.1.0a4.tar` & `plasmapy_sphinx-0.1.0a5.tar`

### file list

```diff
@@ -1,95 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.423573 plasmapy_sphinx-0.1.0a4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.407573 plasmapy_sphinx-0.1.0a4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.411573 plasmapy_sphinx-0.1.0a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/.github/workflows/mint-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-25 18:04:19.423573 plasmapy_sphinx-0.1.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.411573 plasmapy_sphinx-0.1.0a4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.411573 plasmapy_sphinx-0.1.0a4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    90022 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/_static/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/_static/with-text-light-190px.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/docs/api_static/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.autodoc.automodapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.autodoc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.automodsumm.core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.automodsumm.generate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.automodsumm.rst
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.directives.confval.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.directives.event.rst
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.directives.rst
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.ext.autodoc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.ext.automodsumm.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.ext.css.rst
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.ext.directives.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.ext.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.rst
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.theme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/common_links.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13719 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/docs/first_steps/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/first_steps/configure.rst
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/first_steps/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/autodoc/
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/autodoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30418 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/autodoc/automodapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23883 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    18359 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/confval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/ext/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/ext/autodoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/ext/automodsumm.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/ext/css.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/ext/directives.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.419573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.407573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.419573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/css/admonition_color_contrast.css
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/css/plasmapy.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.407573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.419573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/templates/automodsumm/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/templates/automodsumm/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/templates/automodsumm/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/templates/automodsumm/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.419573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-25 18:04:19.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-25 18:04:19.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:04:19.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 18:04:19.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-25 18:04:19.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 18:04:19.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.419573 plasmapy_sphinx-0.1.0a4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements/extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements/install.txt
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:04:19.423573 plasmapy_sphinx-0.1.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.864031 plasmapy_sphinx-0.1.0a5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.848031 plasmapy_sphinx-0.1.0a5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.852031 plasmapy_sphinx-0.1.0a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/.github/workflows/mint-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-07 00:16:01.864031 plasmapy_sphinx-0.1.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.852031 plasmapy_sphinx-0.1.0a5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.852031 plasmapy_sphinx-0.1.0a5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    90022 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/_static/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/_static/with-text-light-190px.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.856031 plasmapy_sphinx-0.1.0a5/docs/api_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.autodoc.automodapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.autodoc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.automodsumm.core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.automodsumm.generate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.automodsumm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.directives.confval.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.directives.event.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.directives.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.ext.autodoc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.ext.automodsumm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.ext.css.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.ext.directives.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.ext.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.theme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/api_static/plasmapy_sphinx.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/common_links.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13719 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.856031 plasmapy_sphinx-0.1.0a5/docs/first_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/first_steps/configure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/first_steps/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/docs/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.856031 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.856031 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/autodoc/
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/autodoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30418 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/autodoc/automodapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.860031 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/automodsumm/
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/automodsumm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23883 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/automodsumm/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18359 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/automodsumm/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.860031 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/directives/
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/directives/confval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/directives/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.860031 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/ext/autodoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/ext/automodsumm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/ext/css.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/ext/directives.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.860031 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.848031 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.860031 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/static/css/admonition_color_contrast.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/static/css/plasmapy.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.848031 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/static/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.860031 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/static/templates/automodsumm/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/static/templates/automodsumm/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/static/templates/automodsumm/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/static/templates/automodsumm/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.864031 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-07 00:16:01.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-07 00:16:01.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 00:16:01.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 00:16:01.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-07 00:16:01.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 00:16:01.000000 plasmapy_sphinx-0.1.0a5/plasmapy_sphinx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:16:01.864031 plasmapy_sphinx-0.1.0a5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/requirements/install.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 00:16:01.864031 plasmapy_sphinx-0.1.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-07 00:15:57.000000 plasmapy_sphinx-0.1.0a5/setup.py
```

### Comparing `plasmapy_sphinx-0.1.0a4/.github/workflows/documentation.yml` & `plasmapy_sphinx-0.1.0a5/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/.github/workflows/mint-release.yml` & `plasmapy_sphinx-0.1.0a5/.github/workflows/mint-release.yml`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/.github/workflows/publish-to-pypi.yml` & `plasmapy_sphinx-0.1.0a5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/.gitignore` & `plasmapy_sphinx-0.1.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/.pre-commit-config.yaml` & `plasmapy_sphinx-0.1.0a5/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ci:
   autofix_prs: false
   autoupdate_schedule: monthly
 
 repos:
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: check-ast
     name: validate Python code
   - id: check-merge-conflict
     name: check for git merge conflicts
     exclude: .*\.rst
   - id: check-case-conflict
@@ -20,15 +20,15 @@
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-json
   - id: check-toml
   - id: check-yaml
 
 - repo: https://github.com/python-jsonschema/check-jsonschema
-  rev: 0.28.1
+  rev: 0.28.2
   hooks:
   - id: check-github-workflows
 
 - repo: https://github.com/sirosen/texthooks
   rev: 0.6.6
   hooks:
   - id: fix-smartquotes
@@ -63,15 +63,15 @@
   - id: codespell
     name: codespell (add false positives to pyproject.toml)
     args: [--write-changes]
     additional_dependencies:
     - tomli
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.3.5
+  rev: v0.4.3
   hooks:
   - id: ruff
     name: ruff (see https://docs.astral.sh/ruff/rules)
     args: [--fix]
 
 - repo: https://github.com/asottile/blacken-docs
   rev: 1.16.0
```

### Comparing `plasmapy_sphinx-0.1.0a4/LICENSE.md` & `plasmapy_sphinx-0.1.0a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/PKG-INFO` & `plasmapy_sphinx-0.1.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plasmapy_sphinx
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Sphinx extensions for the PlasmaPy Project
 Maintainer-email: "Erik T. Everson" <eeverson@plasmapy.org>, "Nicholas A. Murphy" <namurphy@cfa.harvard.edu>
 License: # BSD 2-Clause License
         
         Copyright (c) 2021, PlasmaPy Developers.
         All rights reserved.
```

### Comparing `plasmapy_sphinx-0.1.0a4/docs/Makefile` & `plasmapy_sphinx-0.1.0a5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/docs/_static/icon.ico` & `plasmapy_sphinx-0.1.0a5/docs/_static/icon.ico`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/docs/_static/with-text-light-190px.png` & `plasmapy_sphinx-0.1.0a5/docs/_static/with-text-light-190px.png`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/docs/conf.py` & `plasmapy_sphinx-0.1.0a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/docs/index.rst` & `plasmapy_sphinx-0.1.0a5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/docs/make.bat` & `plasmapy_sphinx-0.1.0a5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/__init__.py` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/autodoc/__init__.py` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/autodoc/__init__.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/autodoc/automodapi.py` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/autodoc/automodapi.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/__init__.py` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/automodsumm/__init__.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/core.py` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/automodsumm/core.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/generate.py` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/automodsumm/generate.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/__init__.py` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/confval.py` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/directives/confval.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/event.py` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/directives/event.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/ext/css.py` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/ext/css.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/__init__.py` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/footer.html` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/footer.html`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/layout.html` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/layout.html`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/css/admonition_color_contrast.css` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/static/css/admonition_color_contrast.css`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/css/plasmapy.css` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/static/css/plasmapy.css`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/templates/automodsumm/class.rst` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/theme/static/templates/automodsumm/class.rst`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/utils.py` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx/utils.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/PKG-INFO` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plasmapy_sphinx
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Sphinx extensions for the PlasmaPy Project
 Maintainer-email: "Erik T. Everson" <eeverson@plasmapy.org>, "Nicholas A. Murphy" <namurphy@cfa.harvard.edu>
 License: # BSD 2-Clause License
         
         Copyright (c) 2021, PlasmaPy Developers.
         All rights reserved.
```

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/SOURCES.txt` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,11 +64,9 @@
 plasmapy_sphinx/theme/static/css/admonition_color_contrast.css
 plasmapy_sphinx/theme/static/css/plasmapy.css
 plasmapy_sphinx/theme/static/templates/automodsumm/base.rst
 plasmapy_sphinx/theme/static/templates/automodsumm/class.rst
 plasmapy_sphinx/theme/static/templates/automodsumm/module.rst
 requirements/build.txt
 requirements/docs.txt
-requirements/environment.yml
-requirements/extras.txt
 requirements/install.txt
 requirements/tests.txt
```

### Comparing `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/requires.txt` & `plasmapy_sphinx-0.1.0a5/plasmapy_sphinx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a4/pyproject.toml` & `plasmapy_sphinx-0.1.0a5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [build-system]
-requires = ["setuptools >= 41.2",
-            "setuptools_scm",
-            "wheel >= 0.29.0"]  # ought to mirror 'requirements/build.txt'
+requires = [  # ought to mirror 'requirements/build.txt'
+    "setuptools >= 41.2",
+    "setuptools_scm",
+    "wheel >= 0.29.0",
+]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "plasmapy_sphinx"
 maintainers = [
   {name = "Erik T. Everson", email = "eeverson@plasmapy.org"},
   {name = "Nicholas A. Murphy", email = "namurphy@cfa.harvard.edu"},
@@ -27,25 +29,25 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-dependencies = [
+dependencies = [  # ought to mirror 'requirements/install.txt'
   "docutils",
   "importlib_metadata; python_version < '3.8'",
   "jinja2 != 3.1",
   "sphinx >= 4.4",
   "sphinx-gallery",
   "sphinx_rtd_theme >= 1.0.0",
 ]
 
 [project.optional-dependencies]
-tests = [
+tests = [  # ought to mirror 'requirements/tests.txt'
   "codespell",
   "dlint",
   "flake8",
   "flake8-absolute-import",
   "flake8-implicit-str-concat",
   "flake8-mutable",
   "flake8-rst-docstrings",
@@ -55,15 +57,15 @@
   "pre-commit",
   "pydocstyle",
   "pytest >= 5.4.0",
   "pytest-regressions",
   "pytest-xdist",
   "tox",
 ]
-docs = [
+docs = [  # ought to mirror 'requirements/docs.txt'
     "numpydoc",
     "packaging",
     "pillow",
     "pygments >= 2.11.0",
     "sphinx-changelog",
     "sphinx-copybutton",
     "sphinx-hoverxref >= 1.1.1",
```

