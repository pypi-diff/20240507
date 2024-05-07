# Comparing `tmp/pydata_sphinx_theme-0.9.0.tar.gz` & `tmp/pydata_sphinx_theme-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydata_sphinx_theme-0.9.0.tar", last modified: Wed Jun  8 15:24:09 2022, max compression
+gzip compressed data, was "pydata_sphinx_theme-0.9.0rc1.tar", last modified: Fri May 27 19:54:27 2022, max compression
```

## Comparing `pydata_sphinx_theme-0.9.0.tar` & `pydata_sphinx_theme-0.9.0rc1.tar`

### file list

```diff
@@ -1,234 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:24:08.862220 pydata_sphinx_theme-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)    50617 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/_static/demo-expandable-navigation.gif
--rw-r--r--   0 runner    (1001) docker     (121)     2762 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2762 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)    75503 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/_static/pull-request-preview-link.png
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/_static/pydata-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/_static/switcher.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/_templates/custom-template.html
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/_templates/navbar-version.html
--rw-r--r--   0 runner    (1001) docker     (121)     5080 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/contribute/
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/contribute/index.md
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/contribute/manual.md
--rw-r--r--   0 runner    (1001) docker     (121)     6201 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/contribute/setup.md
--rw-r--r--   0 runner    (1001) docker     (121)    12258 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/contribute/topics.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/
--rw-r--r--   0 runner    (1001) docker     (121)     3596 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/demo/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)    36161 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/demo/example_pandas.rst
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/demo/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.109276 pydata_sphinx_theme-0.9.0/docs/demo/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/demo/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/demo/kitchen-sink/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10125 2022-06-08 15:23:54.105276 pydata_sphinx_theme-0.9.0/docs/demo/kitchen-sink/lists-and-tables.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14388 2022-06-08 15:23:54.109276 pydata_sphinx_theme-0.9.0/docs/demo/kitchen-sink/paragraph-markup.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2592 2022-06-08 15:23:54.109276 pydata_sphinx_theme-0.9.0/docs/demo/kitchen-sink/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-06-08 15:23:54.109276 pydata_sphinx_theme-0.9.0/docs/demo/mult_headers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-06-08 15:23:54.109276 pydata_sphinx_theme-0.9.0/docs/demo/no-sidebar.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/static/
--rw-r--r--   0 runner    (1001) docker     (121)   670068 2022-06-08 15:23:54.109276 pydata_sphinx_theme-0.9.0/docs/demo/static/Sphinx-and-the-Pyramids-of-Ghiza-by-Facchinelli.png
--rw-r--r--   0 runner    (1001) docker     (121)    15921 2022-06-08 15:23:54.109276 pydata_sphinx_theme-0.9.0/docs/demo/static/logo-wordmark-light.svg
--rw-r--r--   0 runner    (1001) docker     (121)   140497 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/static/screen_desktop.png
--rw-r--r--   0 runner    (1001) docker     (121)    85705 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/static/screen_mobile.png
--rw-r--r--   0 runner    (1001) docker     (121)     6614 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/static/yi_jing_01_chien.jpg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subpage1.rst
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subpage2.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage1.rst
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage10.rst
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage11.rst
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage12.rst
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage13.rst
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage14.rst
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage15.rst
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage16.rst
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage17.rst
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage18.rst
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage19.rst
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage2.rst
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage20.rst
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage3.rst
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage4.rst
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage5.rst
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage6.rst
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage7.rst
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage8.rst
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage9.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/test_py_module/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/test_py_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/test_py_module/test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/demo/theme-elements.md
--rw-r--r--   0 runner    (1001) docker     (121)     2624 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/scripts/a11y-roadmap.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3565 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/scripts/a11y.py
--rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (121)     4648 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/user_guide/accessibility.rst
--rw-r--r--   0 runner    (1001) docker     (121)    30268 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/user_guide/configuring.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11994 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/user_guide/customizing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/user_guide/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4757 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/docs/user_guide/sections.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4452 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/github_deploy_key_pandas_dev_pandas_sphinx_theme.enc
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/package.json
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (121)    26232 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     5499 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/scripts/index.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/abstracts/
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/abstracts/_mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (121)     2870 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/base/_base.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/_icon-links.scss
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/_search.scss
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/_switcher-theme.scss
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/_switcher-version.scss
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/_toc-inpage.scss
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/_versionmodified.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/header/
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/header/_header-logo.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (121)     4651 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/content/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/content/_api.scss
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/content/_footnotes.scss
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/content/_hacks.scss
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/content/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/content/_quotes.scss
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/content/_spans.scss
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-06-08 15:23:54.113276 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/content/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/content/_toctree.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/extensions/_bootstrap.scss
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/extensions/_ethical-ads.scss
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/extensions/_pydata.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1731 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/extensions/_sphinx_design.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/extensions/_sphinx_panels.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/index.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/pages/
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/pages/_search.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/sections/_article.scss
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/sections/_container.scss
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/sections/_footer-article.scss
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (121)     2057 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/sections/_header.scss
--rw-r--r--   0 runner    (1001) docker     (121)     3600 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/sections/_sidebar-primary.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/sections/_sidebar-secondary.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (121)     3863 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/variables/_color.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/variables/_versionmodified.scss
--rw-r--r--   0 runner    (1001) docker     (121)     2061 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/bootstrap_html_translator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/edit-this-page.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/footer-article/
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/footer-article/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/icon-links.html
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/navbar-icon-links.html
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/navbar-logo.html
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/navbar-nav.html
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/page-toc.html
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/sidebar-ethical-ads.html
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/sidebar-nav-bs.html
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/theme-switcher.html
--rw-r--r--   0 runner    (1001) docker     (121)     3777 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/version-switcher.html
--rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/announcement.html
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/article.html
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/footer-article.html
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/header.html
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/sidebar-primary.html
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/sidebar-secondary.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/static/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/static/styles/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/static/styles/theme.css
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/base/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/base/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/base/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/base/emptylogo.png
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/base/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/base/page1.rst
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/base/page2.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/base/section1/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/base/section1/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/base/section1/page1.rst
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/base/switcher.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/_templates_sidebar_level2/
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/_templates_sidebar_level2/sidebar-nav-bs.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/_templates_single_sidebar/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/_templates_single_sidebar/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/_templates_single_sidebar/sidebar-nav-bs.html
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/section1/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/section1/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/section1/page2.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/section1/subsection1/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/section1/subsection1/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/section1/subsection1/page1.rst
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/section1/subsection1/page2.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/section2/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/section2/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/sidebars/section2/page1.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/test_included_toc/
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/test_included_toc/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/test_included_toc/included-page.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/test_included_toc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/test_included_toc/toc-extension.include.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/test_navbar_no_in_page_headers/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/test_navbar_no_in_page_headers/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/test_navbar_no_in_page_headers/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/test_navbar_no_in_page_headers/page1.rst
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/sites/test_navbar_no_in_page_headers/page2.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/test_build/
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/test_build/navbar_icon_links.html
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/test_build/navbar_ix.html
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/test_build/navbar_switcher.html
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/test_build/navbar_theme.html
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/test_build/sidebar_ix.html
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/test_build/sidebar_subpage.html
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/test_build/test_navbar_no_in_page_headers.html
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/test_build/test_sidebars_captions.html
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/test_build/test_sidebars_level2.html
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/test_build/test_sidebars_nested_page.html
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/test_build/test_sidebars_single.html
--rw-r--r--   0 runner    (1001) docker     (121)    19539 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-06-08 15:23:54.117277 pydata_sphinx_theme-0.9.0/webpack.config.js
--rw-r--r--   0        0        0     4390 1970-01-01 00:00:00.000000 pydata_sphinx_theme-0.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:27.146633 pydata_sphinx_theme-0.9.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (121)    50617 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/docs/_static/demo-expandable-navigation.gif
+-rw-r--r--   0 runner    (1001) docker     (121)      733 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/docs/_static/pandas-square.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     2624 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/docs/_static/pandas.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    75503 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/docs/_static/pull-request-preview-link.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/docs/_static/switcher.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/docs/_templates/custom-template.html
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/docs/_templates/navbar-version.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5783 2022-05-27 19:54:10.750499 pydata_sphinx_theme-0.9.0rc1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/contribute/
+-rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/contribute/index.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/contribute/manual.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6201 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/contribute/setup.md
+-rw-r--r--   0 runner    (1001) docker     (121)    10425 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/contribute/topics.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/
+-rw-r--r--   0 runner    (1001) docker     (121)     3596 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/demo/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    36161 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/demo/example_pandas.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/demo/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/demo/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/demo/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/demo/kitchen-sink/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10125 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/demo/kitchen-sink/lists-and-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    14388 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/demo/kitchen-sink/paragraph-markup.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2592 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/demo/kitchen-sink/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/demo/mult_headers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/demo/no-sidebar.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/static/
+-rw-r--r--   0 runner    (1001) docker     (121)   670068 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/demo/static/Sphinx-and-the-Pyramids-of-Ghiza-by-Facchinelli.png
+-rw-r--r--   0 runner    (1001) docker     (121)    15921 2022-05-27 19:54:10.754499 pydata_sphinx_theme-0.9.0rc1/docs/demo/static/logo-wordmark-light.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   140497 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/static/screen_desktop.png
+-rw-r--r--   0 runner    (1001) docker     (121)    85705 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/static/screen_mobile.png
+-rw-r--r--   0 runner    (1001) docker     (121)     6614 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/static/yi_jing_01_chien.jpg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/
+-rw-r--r--   0 runner    (1001) docker     (121)      245 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subpage2.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage10.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage11.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage12.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage13.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage14.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage15.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage16.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage17.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage18.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage19.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage2.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage20.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage3.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage4.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage5.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage6.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage7.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage8.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage9.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/test_py_module/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/test_py_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/test_py_module/test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/demo/theme-elements.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2047 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/scripts/a11y-roadmap.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3565 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/scripts/a11y.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (121)     4648 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/user_guide/accessibility.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    28103 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/user_guide/configuring.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11176 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/user_guide/customizing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/user_guide/install.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4757 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/docs/user_guide/sections.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4452 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/github_deploy_key_pandas_dev_pandas_sphinx_theme.enc
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/package.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (121)    25054 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/scripts/index.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/abstracts/_mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/base/_base.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     3718 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/base/_color.scss
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/_icon-links.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/_search.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/_switcher-theme.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/_switcher-version.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/_toc-inpage.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/_versionmodified.scss
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/header/
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/header/_header-logo.scss
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (121)     4651 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/content/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/content/_api.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/content/_footnotes.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/content/_hacks.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/content/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/content/_quotes.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/content/_spans.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/content/_tables.scss
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/extensions/_bootstrap.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/extensions/_ethical-ads.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/extensions/_pydata.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     1731 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/extensions/_sphinx_design.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/extensions/_sphinx_panels.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/index.scss
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/pages/
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/pages/_search.scss
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/sections/_article.scss
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/sections/_footer-article.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/sections/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     3692 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/sections/_sidebar-primary.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/sections/_sidebar-secondary.scss
+-rw-r--r--   0 runner    (1001) docker     (121)     2061 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/bootstrap_html_translator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/edit-this-page.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/footer-article/
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/footer-article/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/icon-links.html
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/navbar-icon-links.html
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/navbar-logo.html
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/navbar-nav.html
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-05-27 19:54:10.758499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/page-toc.html
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/sidebar-ethical-ads.html
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/theme-switcher.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3789 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/version-switcher.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/announcement.html
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/article.html
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/footer-article.html
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/header.html
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/sidebar-primary.html
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/sidebar-secondary.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/static/styles/
+-rw-r--r--   0 runner    (1001) docker     (121)     2949 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/static/styles/theme.css
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/base/
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/base/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      684 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/base/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/base/emptylogo.png
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/base/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/base/page1.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/base/page2.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/base/section1/
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/base/section1/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/base/section1/page1.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/base/switcher.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/_templates_sidebar_level2/
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/_templates_sidebar_level2/sidebar-nav-bs.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/_templates_single_sidebar/
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/_templates_single_sidebar/layout.html
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/_templates_single_sidebar/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/section1/
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/section1/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/section1/page2.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/section1/subsection1/
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/section1/subsection1/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/section1/subsection1/page1.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/section1/subsection1/page2.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/section2/
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/section2/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/sidebars/section2/page1.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/test_included_toc/
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/test_included_toc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/test_included_toc/included-page.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/test_included_toc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/test_included_toc/toc-extension.include.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/test_navbar_no_in_page_headers/
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/test_navbar_no_in_page_headers/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/test_navbar_no_in_page_headers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/test_navbar_no_in_page_headers/page1.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/sites/test_navbar_no_in_page_headers/page2.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/test_build/
+-rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/test_build/navbar_icon_links.html
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/test_build/navbar_ix.html
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/test_build/navbar_switcher.html
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/test_build/navbar_theme.html
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/test_build/sidebar_ix.html
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/test_build/sidebar_subpage.html
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/test_build/test_navbar_no_in_page_headers.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/test_build/test_sidebars_captions.html
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/test_build/test_sidebars_level2.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/test_build/test_sidebars_nested_page.html
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/test_build/test_sidebars_single.html
+-rw-r--r--   0 runner    (1001) docker     (121)    18772 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-05-27 19:54:10.762499 pydata_sphinx_theme-0.9.0rc1/webpack.config.js
+-rw-r--r--   0        0        0     4393 1970-01-01 00:00:00.000000 pydata_sphinx_theme-0.9.0rc1/PKG-INFO
```

### Comparing `pydata_sphinx_theme-0.9.0/LICENSE` & `pydata_sphinx_theme-0.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/README.md` & `pydata_sphinx_theme-0.9.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/_static/demo-expandable-navigation.gif` & `pydata_sphinx_theme-0.9.0rc1/docs/_static/demo-expandable-navigation.gif`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/_static/pull-request-preview-link.png` & `pydata_sphinx_theme-0.9.0rc1/docs/_static/pull-request-preview-link.png`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/_static/switcher.json` & `pydata_sphinx_theme-0.9.0rc1/docs/_static/switcher.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.925925925925926%*

 * *Differences: {'1': "{'name': '0.9.0rc1 (prerelease)'}",*

 * * '2': "{'name': '0.8.1 (stable)', 'version': 'stable', 'url': "*

 * *      "'https://pydata-sphinx-theme.readthedocs.io/en/stable/'}"}*

```diff
@@ -1,22 +1,22 @@
 [
     {
         "name": "dev",
         "url": "https://pydata-sphinx-theme.readthedocs.io/en/latest/",
         "version": "latest"
     },
     {
-        "name": "0.9.0 (stable)",
+        "name": "0.9.0rc1 (prerelease)",
         "url": "https://pydata-sphinx-theme.readthedocs.io/en/stable/",
         "version": "stable"
     },
     {
-        "name": "0.8.1",
-        "url": "https://pydata-sphinx-theme.readthedocs.io/en/v0.8.1/",
-        "version": "v0.8.1"
+        "name": "0.8.1 (stable)",
+        "url": "https://pydata-sphinx-theme.readthedocs.io/en/stable/",
+        "version": "stable"
     },
     {
         "name": "0.8.0",
         "url": "https://pydata-sphinx-theme.readthedocs.io/en/v0.8.0/",
         "version": "v0.8.0"
     },
     {
```

### Comparing `pydata_sphinx_theme-0.9.0/docs/conf.py` & `pydata_sphinx_theme-0.9.0rc1/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,40 @@
+# Configuration file for the Sphinx documentation builder.
+#
+# This file only contains a selection of the most common options. For a full
+# list see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
 # -- Path setup --------------------------------------------------------------
+
+# If extensions (or modules to document with autodoc) are in another directory,
+# add these directories to sys.path here. If the directory is relative to the
+# documentation root, use os.path.abspath to make it absolute, like shown here.
+#
 import os
 
+# import sys
+# sys.path.insert(0, os.path.abspath('.'))
+
+
 # -- Project information -----------------------------------------------------
 
-project = "PyData Theme"
+project = "PyData Sphinx Theme"
 copyright = "2019, PyData Community"
 author = "PyData Community"
 
 import pydata_sphinx_theme
 
 
 # -- General configuration ---------------------------------------------------
 
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
+# ones.
+
 extensions = [
     "jupyter_sphinx",
     "myst_parser",
     "numpydoc",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinxext.rediraffe",
@@ -55,16 +74,15 @@
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "pydata_sphinx_theme"
-html_logo = "_static/logo.svg"
-html_favicon = "_static/logo.svg"
+# html_logo = "_static/pandas.svg"  # For testing
 
 # Define the json_url for our version switcher.
 json_url = "https://pydata-sphinx-theme.readthedocs.io/en/latest/_static/switcher.json"
 
 # Define the version we use for matching in the version switcher.
 version_match = os.environ.get("READTHEDOCS_VERSION")
 # If READTHEDOCS_VERSION doesn't exist, we're not on RTD
@@ -82,42 +100,39 @@
 
 html_theme_options = {
     "external_links": [
         {
             "url": "https://github.com/pydata/pydata-sphinx-theme/releases",
             "name": "Changelog",
         },
+        {"url": "https://pandas.pydata.org/pandas-docs/stable/", "name": "Pandas Docs"},
     ],
     "github_url": "https://github.com/pydata/pydata-sphinx-theme",
-    "twitter_url": "https://twitter.com/PyData",
+    "twitter_url": "https://twitter.com/pandas_dev",
     "icon_links": [
         {
             "name": "PyPI",
             "url": "https://pypi.org/project/pydata-sphinx-theme",
             "icon": "fas fa-box",
         },
         {
-            "name": "PyData",
-            "url": "https://pydata.org",
-            "icon": "_static/pydata-logo.png",
+            "name": "Pandas",
+            "url": "https://pandas.pydata.org",
+            "icon": "_static/pandas-square.svg",
             "type": "local",
         },
     ],
-    "logo": {
-        "text": "PyData Theme",
-        "image_dark": "logo-dark.svg",
-    },
     "use_edit_page_button": True,
     "show_toc_level": 1,
     # "show_nav_level": 2,
     # "search_bar_position": "navbar",  # TODO: Deprecated - remove in future version
     # "navbar_align": "left",  # [left, content, right] For testing that the navbar items align properly
-    "navbar_start": ["navbar-logo", "version-switcher"],
+    # "navbar_start": ["navbar-logo", "navbar-version"],
     # "navbar_center": ["navbar-nav", "navbar-version"],  # Just for testing
-    "navbar_end": ["theme-switcher", "navbar-icon-links"],
+    "navbar_end": ["theme-switcher", "version-switcher", "navbar-icon-links"],
     # "left_sidebar_end": ["custom-template.html", "sidebar-ethical-ads.html"],
     # "footer_items": ["copyright", "sphinx-version", ""]
     "switcher": {
         "json_url": json_url,
         "version_match": version_match,
     },
 }
```

### Comparing `pydata_sphinx_theme-0.9.0/docs/contribute/index.md` & `pydata_sphinx_theme-0.9.0rc1/docs/contribute/index.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 ---
-myst:
-  html_meta:
-    "description lang=en": "How to become a contributor to the pydata-sphinx-theme."
+html_meta:
+  "description lang=en": "How to become a contributor to the pydata-sphinx-theme."
 ---
 
 # Contribute
 
 These pages contain information about how you can get up-and-running with a development version of this theme, and how you can contribute to the project.
 
 ## Workflow for contributing changes
```

### Comparing `pydata_sphinx_theme-0.9.0/docs/contribute/manual.md` & `pydata_sphinx_theme-0.9.0rc1/docs/contribute/manual.md`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/contribute/setup.md` & `pydata_sphinx_theme-0.9.0rc1/docs/contribute/setup.md`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/contribute/topics.md` & `pydata_sphinx_theme-0.9.0rc1/docs/contribute/topics.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Contribution guides
+# Topic guides and how-tos
 
 These sections cover common operations and topics that are relevant to developing this theme.
 
 ## Make a release
 
 This theme uses GitHub tags and releases to automatically push new releases to
 PyPI. For information on this process, see [the release checklist](https://github.com/pydata/pydata-sphinx-theme/wiki/Release-checklist#release-instructions).
@@ -208,45 +208,23 @@
 ```
 
 The output of the last command includes:
 
 - a short summary of the current state of the accessibility rules we are trying to maintain
 - local paths to JSON and HTML reports which contain all of the issues found
 
-## Supporting new Python versions
+## Update support for new Sphinx versions
 
-For releases of Python, we aim to follow this approach[^1]:
+This theme does not pin the upper version of Sphinx that it supports, but there may be changes that need to happen when Sphinx releases a new version.
+As a general rule, we try to support new major Sphinx versions within 6 months of its release.
 
-> For a new major/minor release of this theme, we support any minor Python versions released in the last 3.5 years (42 months), as defined in [the EOL schedule for Python](https://endoflife.date/python)[^2].
+Here's a list of things to check when Sphinx releases a new version:
 
-We define "support" as testing against each of these versions, so that users can be assured they will not trigger any bugs.
-
-For example, if we made a minor release tomorrow, we'd [look at the EOL schedule for Python](https://endoflife.date/python) and support all of the versions that fall within a 3.5 year window.
-
-[^1]: Our support for Python versions is inspired by [NEP 029](https://numpy.org/neps/nep-0029-deprecation_policy.html).
-[^2]: These policies are goals, but not promises. We are a volunteer-led community with limited time. Consider these sections to be our intention, but we recognize that we may not always be able to meet these criteria if we do not have capacity to do so. We welcome contributions from others to help us more sustainably meet these goals!
-
-## Supporting new Sphinx versions
-
-For supporting versions of Sphinx, we aim to follow this approach:
-
-> We support the latest released version of Sphinx that is **older than 6 months**.
-> We unofficially support earlier released versions of Sphinx, but may increase the lower-bound in our dependency pin without warning if needed[^2].
-
-When a new pre-release of Sphinx is released, we should follow these steps:
-
-- Ensure that our tests are passing. We run our tests with any **pre-releases** of Sphinx, so we can test major errors quickly and make the necessary changes.
-- [Look at the Sphinx Changelog](https://www.sphinx-doc.org/en/master/changes.html) and make sure there are no changes that might break things that aren't captured by our tests.
-- [Look at the deprecated API changes](https://www.sphinx-doc.org/en/master/extdev/deprecated.html) and make sure there are no changes that might break things that aren't captured by our tests.
-- [Look at the docutils changelog](https://docutils.sourceforge.io/RELEASE-NOTES.html) in case there's a new docutils version supported that breaks something.
-
-```{note}
-This theme does not pin the upper version of Sphinx that it supports.
-If a Sphinx release causes major breaking changes for our users, and we do not have the capacity to update our code and release a fix, we may temporarily pin the upper bound of Sphinx we support until this is fixed.
-```
+- [Look at the Sphinx Changelog](https://www.sphinx-doc.org/en/master/changes.html) and make sure there are no obvious breaking changes.
+- [Look at the deprecated API changes](https://www.sphinx-doc.org/en/master/extdev/deprecated.html) and make sure there are no obvious breaking changes.
 
 ## Update our kitchen sink documents
 
 The [kitchen sink reference](../demo/kitchen-sink/index.rst) is for demonstrating as much syntax and style for Sphinx builds as possible.
 It is copied directly from the [`sphinx-themes.org` documentation](https://sphinx-themes.org/) so that we use standardized reference docs compared with other communities.
 The source files for these pages are stored [in the `sphinx-themes.org` repository](https://github.com/sphinx-themes/sphinx-themes.org/raw/master/sample-docs/kitchen-sink/).
```

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/api.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/api.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/example_pandas.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/example_pandas.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/index.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/index.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/kitchen-sink/lists-and-tables.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/kitchen-sink/lists-and-tables.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/kitchen-sink/paragraph-markup.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/kitchen-sink/paragraph-markup.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/kitchen-sink/web-components.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/kitchen-sink/web-components.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/mult_headers.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/mult_headers.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/static/Sphinx-and-the-Pyramids-of-Ghiza-by-Facchinelli.png` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/static/Sphinx-and-the-Pyramids-of-Ghiza-by-Facchinelli.png`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/static/logo-wordmark-light.svg` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/static/logo-wordmark-light.svg`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/static/screen_desktop.png` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/static/screen_desktop.png`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/static/screen_mobile.png` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/static/screen_mobile.png`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/static/yi_jing_01_chien.jpg` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/static/yi_jing_01_chien.jpg`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subpage1.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subpage1.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subpage2.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subpage2.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage1.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage1.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage10.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage10.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage11.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage11.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage12.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage12.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage13.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage13.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage14.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage14.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage15.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage15.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage16.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage16.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage17.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage17.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage18.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage18.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage19.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage19.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage2.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage2.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage20.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage20.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage3.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage3.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage4.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage4.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage5.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage5.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage6.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage6.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage7.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage7.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage8.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage8.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/subpages/subsubpages/subsubpage9.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/subpages/subsubpages/subsubpage9.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/test_py_module/test.py` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/test_py_module/test.py`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/demo/theme-elements.md` & `pydata_sphinx_theme-0.9.0rc1/docs/demo/theme-elements.md`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/index.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -31,25 +31,14 @@
 - Pandas: https://pandas.pydata.org/docs/
 - SciPy: https://scipy.github.io/devdocs/
 - JupyterHub and Binder: https://docs.mybinder.org/, http://z2jh.jupyter.org/en/latest/, https://repo2docker.readthedocs.io/en/latest/, https://jupyterhub-team-compass.readthedocs.io/en/latest/
 - Jupyter Book beta version uses an extension of this theme: https://beta.jupyterbook.org
 - Fairlearn: https://fairlearn.org/main/about/
 - PyVista: https://docs.pyvista.org
 
-Aknowledgment and inspirations
-==============================
-
-To build this theme we drew inspiration from other great projects on the web that we would like to acknowledge here:
-
-- GitBook / Metaflow: https://docs.metaflow.org/introduction/what-is-metaflow
-- Furo: https://pradyunsg.me/furo/quickstart (and we also draw a lot of implementation / code from this)
-- Docker: https://docs.docker.com/engine/docker-overview/
-- PyTorch: https://pytorch.org/docs/stable/notes/autograd.html
-
-Thanks to `@drammock <https://github.com/drammock>`_ for initial design of the theme logo.
 
 .. toctree::
    :caption: Theme Documentation
    :maxdepth: 2
 
    user_guide/index
    contribute/index
```

### Comparing `pydata_sphinx_theme-0.9.0/docs/scripts/a11y-roadmap.txt` & `pydata_sphinx_theme-0.9.0rc1/docs/scripts/a11y-roadmap.txt`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/scripts/a11y.py` & `pydata_sphinx_theme-0.9.0rc1/docs/scripts/a11y.py`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/serve.py` & `pydata_sphinx_theme-0.9.0rc1/docs/serve.py`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/user_guide/accessibility.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/user_guide/accessibility.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/user_guide/configuring.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/user_guide/configuring.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,119 +5,58 @@
 *************
 
 There are a number of options for configuring your site's look and feel.
 All configuration options are passed with the ``html_theme_options`` variable
 in your ``conf.py`` file. This is a dictionary with ``key: val`` pairs that
 you can configure in various ways. This page describes the options available to you.
 
-Configure project logo and title
-================================
-
-By default the theme will use the value of ``project`` on the left side of the header navbar.
-This can be replaced by a Logo image, and optionally a custom ``html_title`` as well.
-
-Single logo for light and dark mode
------------------------------------
+Configure project logo
+======================
 
-Put an image in a folder that is in `html_static_path`, and use the following configuration:
+To add a logo that's placed at the left of your nav bar, put a logo file under your
+doc path's _static folder, and use the following configuration:
 
 .. code:: python
 
-   html_static_path = ["_static"]
    html_logo = "_static/logo.png"
 
-Different logos for light and dark mode
----------------------------------------
-
-You may specify use a different version of your logo image for "light" and "dark" modes.
-This is useful if your logo image is not adapted to a dark mode (light background, not enough contrast, etc...).
-
-To do so, put the 2 image files in a folder that is in ``html_static_path`` and configure the relative path to each image with ``logo.image_light`` and ``logo.image_dark`` in ``html_theme_options``, like so:
-
-.. code-block:: python
-
-   html_static_path = ["_static"]
-   html_theme_options = {
-      "logo": {
-         "image_light": "logo-light.png",
-         "image_dark": "logo-dark.png",
-      }
-   }
-
-.. note::
-
-   ``image_light`` and ``image_dark`` will override the ``html_logo`` setting. If you only specify one of them, but not the other, then the un-specified setting will re-use ``html_logo``.
-
-Customize logo link
--------------------
-
 The logo links to ``root_doc`` (usually the first page of your documentation) by default.
 If you'd like it to link to another page or use an external link instead, use the following configuration:
 
-.. code-block:: python
-
-   html_theme_options = {
-       "logo": {
-           "link": "<other page or external link>",
-       }
-   }
-
-Add a logo title
-----------------
-
-To add a title in the brand section of your documentation, define a value for ``html_theme_options.logo["text"]``
-This will appear just after your logo image if it is set.
-
-.. code-block:: python
+.. code:: python
 
    html_theme_options = {
-       "logo": {
-           "text": "My awesome documentation",
-       }
+       "logo_link": "<other page or external link>"
    }
 
-.. note:: The ``html_title`` field will work as well if no logo images are specified.
-
 
 .. _icon-links:
 
-Configure default mode
-======================
+Configure default theme
+=======================
 
 The theme mode can be changed by the user. By default landing on the documentation will switch the mode to ``auto``. You can specified this value to be one of ``auto``, ``dark``, ``light``.
 
 .. code-block:: python
 
    html_context = {
-      # ...
-      "default_mode": "light"
+      ...
+      "default_mode": "auto"
    }
 
 For more information, see :ref:`manage-themes`.
 
-.. tip::
-
-   To completely remove the theme management, configure ``default_mode`` to the value you want in your documentation (``light`` or ``dark``) and then remove the theme-switcher from the ``navbar_end`` section of the header navbar configuration:
-
-   .. code-block:: python
-
-      html_theme_options {
-          # ...
-          # Note we have omitted `theme-switcher` below
-          "navbar_end": ["navbar-icon-links"]
-      }
-
 Configure pygment theme
 =======================
 
 As the Sphinx theme supports multiple modes, the code highlighting colors can be modified for each one of them by modifying the `pygment_light_style`and `pygment_style_style`. You can check available Pygments colors on this `page <https://help.farbox.com/pygments.html>`__.
 
 .. code-block:: python
 
-   html_theme_options = {
+   html_context = {
       ...
       "pygment_light_style": "tango",
       "pygment_dark_style": "native"
    }
 
 .. danger::
 
@@ -638,15 +577,15 @@
 of the locations in ``html_theme_options`` (e.g., ``navbar_end``,
 ``footer_items``, etc). For example:
 
 .. code:: python
 
    html_theme_options = {
       ...,
-      "navbar_start": ["navbar-logo", "version-switcher"]
+      "navbar_end": ["version-switcher"]
    }
 
 
 Alternatively, you could override one of the other templates to include the
 version switcher in a sidebar. For example, you could define
 ``_templates/sidebar-nav-bs.html`` as:
 
@@ -692,22 +631,22 @@
       background-color: green;
    }
 
 In addition, the parent button of the dropdown list contains similar metadata
 about the **current version**. This could be used to style the entire dropdown
 a certain color based on the active version.
 
-For example, if you wanted to style the dropdown button to use the theme's secondary color (PyData orange by default) if it was a ``dev``
+For example, if you wanted to style the dropdown button orange if it was a ``dev``
 version, you could use the following CSS selector:
 
 .. code-block:: scss
 
    // If the active version has the name "dev", style it orange
    #version_switcher_button[data-active-version-name*="dev"] {
-      background-color: var(--pst-color-secondary);
+      background-color: rgb(255 138 62);
    }
 
 .. seealso::
 
    See the `MDN documentation on dataset properties <https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/dataset>`_
    for more information on using and styling with these properties.
```

### Comparing `pydata_sphinx_theme-0.9.0/docs/user_guide/customizing.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/user_guide/customizing.rst`

 * *Files 7% similar despite different names*

```diff
@@ -167,37 +167,20 @@
    `SASS variables <https://sass-lang.com/documentation/variables>`_.
    The theme is defined with CSS variables, not SASS variables! Refer to the previous section if
    you desire a different behavior between the light and dark theme.
 
 For a complete list of the theme variables that you may override, see the
 `theme variables defaults CSS file <pydata-css-variables_>`_:
 
-.. literalinclude:: ../../src/pydata_sphinx_theme/assets/styles/variables/_layout.scss
-  :language: scss
-
-.. literalinclude:: ../../src/pydata_sphinx_theme/assets/styles/variables/_fonts.scss
-  :language: scss
-
-.. literalinclude:: ../../src/pydata_sphinx_theme/assets/styles/variables/_icons.scss
-  :language: scss
-
-.. literalinclude:: ../../src/pydata_sphinx_theme/assets/styles/variables/_admonitions.scss
-  :language: scss
-
-.. literalinclude:: ../../src/pydata_sphinx_theme/assets/styles/variables/_versionmodified.scss
-  :language: scss
+.. literalinclude:: ../../src/pydata_sphinx_theme/theme/pydata_sphinx_theme/static/styles/theme.css
+  :language: CSS
 
 Color variables
 ---------------
 
-There are two special color variables for primary and secondary theme colors (``--pst-color-primary`` and ``--pst-color-secondary``, respectively).
-These are meant to complement one another visually across the theme, if you modify these, choose colors that look good when paired with one another.
-
-There are also several other color variables that control color for admonitions, links, menu items, etc.
-
 Each color variable has two values, one corresponding to the "light" and one for the "dark" theme.
 These are used throughout many of the theme elements to define text color, background color, etc.
 
 You can control the colors used for these variables for each theme by
 :ref:`adding a custom CSS stylesheet <custom-css>` and adding a structure like so:
 
 .. code-block:: css
@@ -209,33 +192,33 @@
     html[data-theme="dark"] {
         --pst-color-primary: white;
     }
 
 For a complete list of the theme colors that you may override, see the
 `color variables defaults CSS file <pydata-css-colors_>`_:
 
-.. literalinclude:: ../../src/pydata_sphinx_theme/assets/styles/variables/_color.scss
+.. literalinclude:: ../../src/pydata_sphinx_theme/assets/styles/base/_color.scss
   :language: scss
 
 Change footer display
 =====================
 
 Each footer element is wrapped in a ``<div>`` with a ``footer-item`` class, allowing you to style the structure of these items with custom CSS.
 
 For example, by default the footer items are displayed as blocks that stack vertically.
 To change this behavior so that they stack **horizontally**, add a rule like the following in your custom ``.css`` file.
 
 .. code-block:: css
 
-   /* Make each footer item in-line so they stack horizontally instead of vertically */
+   // Make each footer item in-line so they stack horizontally instead of vertically
    .footer-item {
      display: inline-block;
    }
 
-   /* Add a separating border line for all but the last item */
+   // Add a separating border line for all but the last item
    .footer-item:not(:last-child) {
      border-right: 1px solid var(--pst-color-text-base);
      margin-right: .5em;
      padding-right: .5em;
    }
 
 Replacing/Removing Fonts
@@ -256,15 +239,15 @@
 
 The default body and header fonts can be changed as follows:
 
 - Using :ref:`custom-css`, you can specify which fonts to use for body, header
   and monospace text. For example, the following can be added to a custom
   css file:
 
-  .. code-block:: css
+  .. code-block:: none
 
       :root {
           --pst-font-family-base: Verdana, var(--pst-font-family-base-system);
           --pst-font-family-heading: Cambria, Georgia, Times, var(--pst-font-family-base-system);
           --pst-font-family-monospace: Courier, var(--pst-font-family-monospace-system);
       }
 
@@ -292,14 +275,14 @@
       {% endblock %}
 
     To reduce the `Flash of Unstyled Content`, you may wish to explore various options for
     `preloading content <https://developer.mozilla.org/en-US/docs/Web/HTML/Preloading_content>`__,
     specifically the binary font files. This ensure the files will be loaded
     before waiting for the CSS to be parsed, but should be used with care.
 
-.. _pydata-css-variables: https://github.com/pydata/pydata-sphinx-theme/blob/main/src/pydata_sphinx_theme/assets/styles/variables/
-.. _pydata-css-colors: https://github.com/pydata/pydata-sphinx-theme/blob/main/src/pydata_sphinx_theme/assets/styles/variables/_color.scss
+.. _pydata-css-variables: https://github.com/pydata/pydata-sphinx-theme/blob/main/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/static/styles/theme.css
+.. _pydata-css-colors: https://github.com/pydata/pydata-sphinx-theme/blob/main/src/pydata_sphinx_theme/assets/styles/base/_color.scss
 .. _css-variable-help: https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties
 
 .. meta::
     :description lang=en:
         Advanced customization of pydata-sphinx-theme's HTML and CSS.
```

### Comparing `pydata_sphinx_theme-0.9.0/docs/user_guide/index.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/user_guide/install.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/user_guide/install.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/docs/user_guide/sections.rst` & `pydata_sphinx_theme-0.9.0rc1/docs/user_guide/sections.rst`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/github_deploy_key_pandas_dev_pandas_sphinx_theme.enc` & `pydata_sphinx_theme-0.9.0rc1/github_deploy_key_pandas_dev_pandas_sphinx_theme.enc`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/noxfile.py` & `pydata_sphinx_theme-0.9.0rc1/noxfile.py`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/package.json` & `pydata_sphinx_theme-0.9.0rc1/package.json`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/pyproject.toml` & `pydata_sphinx_theme-0.9.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/__init__.py` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 from sphinx.errors import ExtensionError
 from sphinx.util import logging
 from pygments.formatters import HtmlFormatter
 from pygments.styles import get_all_styles
 
 from .bootstrap_html_translator import BootstrapHTML5Translator
 
-__version__ = "0.9.0"
+__version__ = "0.9.0rc1"
 
 logger = logging.getLogger(__name__)
 
 
 def update_config(app, env):
-    theme_options = env.config.html_theme_options
+    theme_options = app.config["html_theme_options"]
 
-    # DEPRECATE >= v0.10
+    # DEPRECATE after v0.9
     if theme_options.get("search_bar_position") == "navbar":
         logger.warn(
             (
                 "Deprecated config `search_bar_position` used."
                 "Use `search-field.html` in `navbar_end` template list instead."
             )
         )
@@ -80,42 +80,14 @@
             """
 
         # Link the JS files
         app.add_js_file(gid_js_path, loading_method="async")
         app.add_js_file(None, body=gid_script)
 
 
-def prepare_html_config(app, pagename, templatename, context, doctree):
-    """Prepare some configuration values for the HTML build.
-
-    For some reason updating the html_theme_options in an earlier Sphinx
-    event doesn't seem to update the values in context, so we manually update
-    it here with our config.
-    """
-    # Prepare the logo config dictionary
-    theme_logo = context.get("theme_logo")
-    if not theme_logo:
-        # In case theme_logo is an empty string
-        theme_logo = {}
-    if not isinstance(theme_logo, dict):
-        raise ValueError(f"Incorrect logo config type: {type(theme_logo)}")
-
-    # DEPRECATE: >= 0.11
-    if context.get("theme_logo_link"):
-        logger.warn(
-            (
-                "DEPRECATION: Config `logo_link` will be deprecated in v0.11. "
-                "Use the `logo.link` configuration dictionary instead."
-            )
-        )
-        theme_logo = context.get("theme_logo_link")
-
-    context["theme_logo"] = theme_logo
-
-
 def update_templates(app, pagename, templatename, context, doctree):
     """Update template names and assets for page build."""
     # Allow for more flexibility in template names
     template_sections = [
         "theme_navbar_start",
         "theme_navbar_center",
         "theme_navbar_end",
@@ -406,17 +378,15 @@
         kwargs["includehidden"] = True
     if "maxdepth" not in kwargs or not kwargs["maxdepth"]:
         kwargs["maxdepth"] = 0
     else:
         kwargs["maxdepth"] = int(kwargs["maxdepth"])
     kwargs["collapse"] = collapse
 
-    # FIX: Can just use "findall" once docutils 0.18+ is required
-    meth = "findall" if hasattr(doctree, "findall") else "traverse"
-    for toctreenode in getattr(doctree, meth)(addnodes.toctree):
+    for toctreenode in doctree.traverse(addnodes.toctree):
         toctree = self.resolve(docname, builder, toctreenode, prune=True, **kwargs)
         if toctree:
             toctrees.append(toctree)
     if not toctrees:
         return None
     result = toctrees[0]
     for toctree in toctrees[1:]:
@@ -688,14 +658,13 @@
     app.set_translator("readthedocs", BootstrapHTML5Translator, override=True)
     app.set_translator("readthedocsdirhtml", BootstrapHTML5Translator, override=True)
 
     app.connect("env-updated", update_config)
     app.connect("html-page-context", setup_edit_url)
     app.connect("html-page-context", add_toctree_functions)
     app.connect("html-page-context", update_templates)
-    app.connect("html-page-context", prepare_html_config)
     app.connect("build-finished", _overwrite_pygments_css)
 
     # Include component templates
     app.config.templates_path.append(str(theme_path / "components"))
 
     return {"parallel_read_safe": True, "parallel_write_safe": True}
```

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/scripts/index.js` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/scripts/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -81,17 +81,15 @@
 function addModeListener() {
     // the theme was set a first time using the initial mini-script
     // running setMode will ensure the use of the dark mode if auto is selected
     setTheme(document.documentElement.dataset.mode);
 
     // Attach event handlers for toggling themes colors
     const btn = document.getElementById("theme-switch");
-    if (btn != null) {
-        btn.addEventListener("click", cycleMode);
-    }
+    btn.addEventListener("click", cycleMode);
 }
 
 /*******************************************************************************
  * TOC interactivity
  */
 
 function addTOCInteractivity() {
```

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/abstracts/_mixins.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/abstracts/_mixins.scss`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/base/_base.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/base/_base.scss`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 html {
   font-size: var(--pst-font-size-base);
   scroll-padding-top: calc(var(--pst-header-height) + 12px);
 }
 
 body {
   padding-top: var(--pst-header-height);
+
   background-color: var(--pst-color-background);
   font-family: var(--pst-font-family-base);
   font-weight: 400;
   line-height: 1.65;
   color: var(--pst-color-text-base);
-  min-height: 100vh;
-  display: flex;
-  flex-direction: column;
 
   @include scrollbar-style();
   @include scrollbar-on-hover();
 
   // hack to avoid the black background on some browser including Safari
   &::-webkit-scrollbar-track {
     background: var(--pst-color-background);
@@ -44,15 +42,15 @@
 
   &:hover {
     color: var(--pst-color-link-hover);
     text-decoration: underline;
   }
 
   &.headerlink {
-    color: var(--pst-color-warning);
+    color: var(--pst-color-danger);
     opacity: 0.4;
     font-size: 0.8em;
     padding: 0 4px 0 4px;
     margin-left: 0.2em;
     text-decoration: none;
     transition: all 0.2s ease-out;
     user-select: none;
```

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/_prev-next.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/_search.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/_search.scss`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/_switcher-theme.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/_switcher-theme.scss`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/components/_versionmodified.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/components/_versionmodified.scss`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/content/_admonitions.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/content/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/content/_api.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/content/_api.scss`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/content/_spans.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/content/_spans.scss`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/extensions/_ethical-ads.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/extensions/_ethical-ads.scss`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/extensions/_sphinx_design.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/extensions/_sphinx_design.scss`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/extensions/_sphinx_panels.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/extensions/_sphinx_panels.scss`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/index.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/index.scss`

 * *Files 14% similar despite different names*

```diff
@@ -14,30 +14,22 @@
   sm: 540px,
   md: 720px,
   lg: 960px,
   xl: 1200px,
 );
 @import "~bootstrap/scss/bootstrap";
 
-// re-usable SCSS functions
+// Variables and re-usable SCSS functions
 @import "abstracts/mixins";
 
-// Variables
-@import "variables/layout";
-@import "variables/fonts";
-@import "variables/icons";
-@import "variables/admonitions";
-@import "variables/versionmodified";
-@import "variables/color";
-
 // Basic styling applied throughout site
 @import "./base/base";
+@import "./base/color";
 
 // Major theme layout, skeleton, and whitespace
-@import "./sections/container";
 @import "./sections/article";
 @import "./sections/footer";
 @import "./sections/footer-article";
 @import "./sections/header";
 @import "./sections/sidebar-primary";
 @import "./sections/sidebar-secondary";
 
@@ -56,15 +48,14 @@
 @import "./content/api";
 @import "./content/footnotes";
 @import "./content/hacks";
 @import "./content/lists";
 @import "./content/quotes";
 @import "./content/spans";
 @import "./content/tables";
-@import "./content/toctree";
 
 // Content blocks from Sphinx extensions
 @import "./extensions/bootstrap";
 @import "./extensions/ethical-ads";
 @import "./extensions/pydata";
 @import "./extensions/sphinx_design";
 @import "./extensions/sphinx_panels";
```

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/sections/_header.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/sections/_header.scss`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,15 @@
   width: 100%;
   padding: 0;
 
   .container-xl {
     height: 100%;
   }
 
-  #navbar-end,
-  #navbar-center,
-  #navbar-start {
+  #navbar-end {
     display: flex;
     align-items: center;
   }
 
   // On smaller screens, add margin to the navbar start/stop
   @include media-breakpoint-down(lg) {
     #navbar-start {
```

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/sections/_sidebar-primary.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/sections/_sidebar-primary.scss`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,22 @@
   padding-top: 1em;
   overflow-y: auto;
   display: flex;
   flex-direction: column;
 
   @include media-breakpoint-up(md) {
     border-right: 1px solid var(--pst-color-border);
-    position: sticky;
-    top: var(--pst-header-height);
-    z-index: 1000;
-    max-height: calc(100vh - var(--pst-header-height));
+
+    @supports (position: -webkit-sticky) or (position: sticky) {
+      position: -webkit-sticky;
+      position: sticky;
+      top: var(--pst-header-height);
+      z-index: 1000;
+      height: calc(100vh - var(--pst-header-height));
+    }
   }
 
   @include scrollbar-style();
   @include scrollbar-on-hover();
 
   &.no-sidebar {
     border-right: 0;
@@ -82,15 +86,15 @@
       right: 0em; // aligning chevron to the right
     }
   }
 }
 
 /* Between-page links and captions */
 nav.bd-links {
-  font-size: var(--pst-sidebar-primary-font-size);
+  font-size: var(--pst-sidebar-font-size);
 
   ul {
     list-style: none;
     padding: 0 0 0 1.5rem;
   }
 
   li > a {
@@ -121,15 +125,15 @@
       font-weight: 600;
       color: var(--pst-color-primary);
     }
   }
 
   // Toctree captions
   p.caption {
-    font-size: var(--pst-sidebar-primary-caption-font-size);
+    font-size: var(--pst-sidebar-caption-font-size);
     text-transform: uppercase;
     font-weight: bold;
     position: relative;
     margin-top: 1.25em;
     margin-bottom: 0.5em;
     padding: 0 1.5rem;
     color: var(--pst-color-text-base);
```

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/sections/_sidebar-secondary.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/sections/_sidebar-secondary.scss`

 * *Files 13% similar despite different names*

```diff
@@ -23,18 +23,25 @@
     padding-left: 1rem;
   }
 }
 
 .bd-toc {
   -ms-flex-order: 2;
   order: 2;
-  max-height: calc(100vh - 5rem);
+
+  height: calc(100vh - 2rem);
   overflow-y: auto;
-  top: var(--pst-header-height);
-  position: sticky;
+
+  @supports (position: -webkit-sticky) or (position: sticky) {
+    position: -webkit-sticky;
+    position: sticky;
+    top: var(--pst-header-height);
+    height: calc(100vh - 5rem);
+    overflow-y: auto;
+  }
 
   .onthispage {
     color: var(--pst-color-text-base);
   }
 
   @include scrollbar-style();
   @include scrollbar-on-hover();
```

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/assets/styles/variables/_color.scss` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/assets/styles/base/_color.scss`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 *
 * all the variables used for light theme coloring
 */
 html[data-theme="light"] {
   /*****************************************************************************
   * main colors
   */
-  --pst-color-primary: rgb(69 157 185);
-  --pst-color-secondary: rgb(238 144 64);
+  --pst-color-primary: rgb(19, 6, 84);
   --pst-color-success: rgb(40, 167, 69);
-  --pst-color-info: var(--pst-color-primary);
-  --pst-color-warning: var(--pst-color-secondary);
+  --pst-color-info: rgb(0, 123, 255);
+  --pst-color-warning: rgb(255, 193, 7);
   --pst-color-danger: rgb(220, 53, 69);
   --pst-color-text-base: rgb(51, 51, 51);
   --pst-color-text-muted: rgb(77, 77, 77);
   --pst-color-border: rgb(201, 201, 201);
   --pst-color-shadow: rgb(216, 216, 216);
 
   /*****************************************************************************
@@ -38,16 +37,16 @@
   --pst-color-panel-background: var(--pst-color-background);
 
   /*****************************************************************************
   * layout
   */
 
   // links
-  --pst-color-link: var(--pst-color-primary);
-  --pst-color-link-hover: var(--pst-color-secondary);
+  --pst-color-link: rgb(0, 91, 129);
+  --pst-color-link-hover: rgb(227, 46, 0);
 
   // inline code
   --pst-color-inline-code: rgb(232, 62, 140);
 
   // targeted content
   --pst-color-target: rgb(251, 229, 78);
 
@@ -62,19 +61,18 @@
 *
 * all the variables used for dark theme coloring
 */
 html[data-theme="dark"] {
   /*****************************************************************************
   * main colors
   */
-  --pst-color-primary: rgb(69 157 185);
-  --pst-color-secondary: rgb(238 144 64);
+  --pst-color-primary: rgb(76, 145, 219);
   --pst-color-success: rgb(72, 135, 87);
-  --pst-color-info: var(--pst-color-primary);
-  --pst-color-warning: var(--pst-color-secondary);
+  --pst-color-info: rgb(64, 125, 191);
+  --pst-color-warning: rgb(193, 162, 69);
   --pst-color-danger: rgb(203, 70, 83);
   --pst-color-text-base: rgb(201, 209, 217);
   --pst-color-text-muted: rgb(192, 192, 192);
   --pst-color-border: rgb(192, 192, 192);
   --pst-color-shadow: var(--pst-color-background);
 
   /*****************************************************************************
@@ -98,15 +96,15 @@
 
   /*****************************************************************************
   * layout
   */
 
   // links
   --pst-color-link: var(--pst-color-primary);
-  --pst-color-link-hover: var(--pst-color-secondary);
+  --pst-color-link-hover: rgb(170, 103, 196);
 
   // inline code
   --pst-color-inline-code: rgb(221, 158, 194);
 
   // targeted content
   --pst-color-target: rgb(71, 39, 0);
```

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/bootstrap_html_translator.py` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/bootstrap_html_translator.py`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/footer-article/prev-next.html` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/footer-article/prev-next.html`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/icon-links.html` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/icon-links.html`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/version-switcher.html` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/version-switcher.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div class="dropdown" id="version_switcher">
-    <button type="button" class="btn btn-sm navbar-btn dropdown-toggle" id="version_switcher_button" data-toggle="dropdown">
+    <button type="button" class="btn btn-primary btn-sm navbar-btn dropdown-toggle" id="version_switcher_button" data-toggle="dropdown">
         {{ theme_switcher.get('version_match') }}  <!-- this text may get changed later by javascript -->
         <span class="caret"></span>
     </button>
     <div id="version_switcher_menu" class="dropdown-menu list-group-flush py-0" aria-labelledby="version_switcher_button">
     <!-- dropdown will be populated by javascript on page load -->
     </div>
 </div>
```

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/layout.html` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/header.html` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/header.html`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/sidebar-primary.html` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/sections/sidebar-primary.html`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/theme.conf` & `pydata_sphinx_theme-0.9.0rc1/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/theme.conf`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 sidebars = search-field.html, sidebar-nav-bs.html
 
 [options]
 sidebarwidth = 270
 sidebar_includehidden = True
 use_edit_page_button = False
 external_links =
+logo_link =
 bitbucket_url =
 github_url =
 gitlab_url =
 twitter_url =
 icon_links_label = Icon Links
 icon_links =
 google_analytics_id =
@@ -33,11 +34,7 @@
 navbar_end = theme-switcher.html, navbar-icon-links.html
 left_sidebar_end = sidebar-ethical-ads.html
 footer_items = copyright.html, sphinx-version.html
 page_sidebar_items = page-toc.html, edit-this-page.html
 switcher =
 pygment_light_style = tango
 pygment_dark_style = native
-logo =
-
-# DEPRECATE after 0.11
-logo_text =
```

### Comparing `pydata_sphinx_theme-0.9.0/tests/sites/base/Makefile` & `pydata_sphinx_theme-0.9.0rc1/tests/sites/base/Makefile`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/tests/sites/base/conf.py` & `pydata_sphinx_theme-0.9.0rc1/tests/sites/base/conf.py`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/tests/test_build/navbar_icon_links.html` & `pydata_sphinx_theme-0.9.0rc1/tests/test_build/navbar_icon_links.html`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/tests/test_build/navbar_ix.html` & `pydata_sphinx_theme-0.9.0rc1/tests/test_build/navbar_ix.html`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/tests/test_build/sidebar_ix.html` & `pydata_sphinx_theme-0.9.0rc1/tests/test_build/sidebar_ix.html`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/tests/test_build/sidebar_subpage.html` & `pydata_sphinx_theme-0.9.0rc1/tests/test_build/sidebar_subpage.html`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/tests/test_build/test_sidebars_captions.html` & `pydata_sphinx_theme-0.9.0rc1/tests/test_build/test_sidebars_captions.html`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/tests/test_build/test_sidebars_level2.html` & `pydata_sphinx_theme-0.9.0rc1/tests/test_build/test_sidebars_level2.html`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/tests/test_build/test_sidebars_nested_page.html` & `pydata_sphinx_theme-0.9.0rc1/tests/test_build/test_sidebars_nested_page.html`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/tests/test_build/test_sidebars_single.html` & `pydata_sphinx_theme-0.9.0rc1/tests/test_build/test_sidebars_single.html`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/tests/test_build.py` & `pydata_sphinx_theme-0.9.0rc1/tests/test_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,51 +133,32 @@
     # Navbar should have the right icons
     icon_links = sphinx_build.html_tree("index.html").select("#navbar-icon-links")[0]
     file_regression.check(
         icon_links.prettify(), basename="navbar_icon_links", extension=".html"
     )
 
 
-def test_logo_basic(sphinx_build_factory):
+def test_logo(sphinx_build_factory):
     """Test that the logo is shown by default, project title if no logo."""
     sphinx_build = sphinx_build_factory("base").build()
 
     # By default logo is shown
     index_html = sphinx_build.html_tree("index.html")
     assert index_html.select(".navbar-brand img")
-    assert "emptylogo" in str(index_html.select(".navbar-brand")[0])
     assert not index_html.select(".navbar-brand")[0].text.strip()
 
 
-def test_logo_no_image(sphinx_build_factory):
-    """Test that the text is shown if no image specified."""
+def test_logo_name(sphinx_build_factory):
+    """Test that the logo is shown by default, project title if no logo."""
     confoverrides = {"html_logo": ""}
     sphinx_build = sphinx_build_factory("base", confoverrides=confoverrides).build()
-    index_html = sphinx_build.html_tree("index.html")
-    assert "PyData Tests" in index_html.select(".navbar-brand")[0].text.strip()
-    assert "emptylogo" not in str(index_html.select(".navbar-brand")[0])
 
-
-def test_logo_two_images(sphinx_build_factory):
-    """Test that the logo image / text is correct when both dark / light given."""
-    # Test with a specified title and a dark logo
-    confoverrides = {
-        "html_theme_options": {
-            "logo": {
-                "text": "Foo Title",
-                "image_dark": "emptydarklogo.png",
-            }
-        },
-    }
-    sphinx_build = sphinx_build_factory("base", confoverrides=confoverrides).build()
+    # if no logo is specified, use project title instead
     index_html = sphinx_build.html_tree("index.html")
-    index_str = str(index_html.select(".navbar-brand")[0])
-    assert "emptylogo" in index_str
-    assert "emptydarklogo" in index_str
-    assert "Foo Title" in index_str
+    assert "PyData Tests" in index_html.select(".navbar-brand")[0].text.strip()
 
 
 def test_favicons(sphinx_build_factory):
     """Test that arbitrary favicons are included."""
     html_theme_options_favicons = {
         "favicons": [
             {
```

### Comparing `pydata_sphinx_theme-0.9.0/webpack.config.js` & `pydata_sphinx_theme-0.9.0rc1/webpack.config.js`

 * *Files identical despite different names*

### Comparing `pydata_sphinx_theme-0.9.0/PKG-INFO` & `pydata_sphinx_theme-0.9.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydata-sphinx-theme
-Version: 0.9.0
+Version: 0.9.0rc1
 Summary: Bootstrap-based Sphinx theme from the PyData community
 Maintainer-Email: Joris Van den Bossche <jorisvandenbossche@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: License :: OSI Approved :: BSD License
```

