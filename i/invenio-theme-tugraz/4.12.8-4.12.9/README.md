# Comparing `tmp/invenio-theme-tugraz-4.12.8.tar.gz` & `tmp/invenio-theme-tugraz-4.12.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-theme-tugraz-4.12.8.tar", last modified: Mon Mar 11 19:21:25 2024, max compression
+gzip compressed data, was "invenio-theme-tugraz-4.12.9.tar", last modified: Tue May  7 08:54:09 2024, max compression
```

## Comparing `invenio-theme-tugraz-4.12.8.tar` & `invenio-theme-tugraz-4.12.9.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.862125 invenio-theme-tugraz-4.12.8/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.842126 invenio-theme-tugraz-4.12.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.846125 invenio-theme-tugraz-4.12.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.846125 invenio-theme-tugraz-4.12.8/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-03-11 19:21:25.862125 invenio-theme-tugraz-4.12.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.846125 invenio-theme-tugraz-4.12.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.850125 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.842126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.842126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.842126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.850125 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.842126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.850125 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/communities.less
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/deposit.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.842126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.854125 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)    94816 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   269108 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/login.less
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/macros.less
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/record.less
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.854125 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.854125 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/extra/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/extra/orcid.png
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.858126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    18533 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/Icon_1_v2.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/TU_Austria_Logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/cyan_400x400.png
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/dark_blue_400x400.png
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/diamond.svg
--rw-r--r--   0 runner    (1001) docker     (127)   225210 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/footer.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/group-discussion.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/icon_use.png
--rw-r--r--   0 runner    (1001) docker     (127)    18643 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/inveniordm-tail.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/library-book-svgrepo-com.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/library_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/light_green_400x400.png
--rw-r--r--   0 runner    (1001) docker     (127)    23820 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/login_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    97455 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/oea.svg
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/play.svg
--rw-r--r--   0 runner    (1001) docker     (127)    38212 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/re3data.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/red_400x400.png
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/rosa_400x400.png
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/tug_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/umbrella.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.842126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.858126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/423.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.858126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/contact_us.html
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/frontpage_overview.html
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.858126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/overview.html
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/recent_uploads.html
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/tu_graz_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.858126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.842126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.858126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-03-11 19:21:25.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    22541 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.842126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.858126 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-11 19:21:25.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.850125 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-03-11 19:21:25.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-03-11 19:21:25.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 19:21:25.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-11 19:21:25.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 19:21:25.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-11 19:21:25.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 19:21:25.000000 invenio-theme-tugraz-4.12.8/invenio_theme_tugraz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-11 19:21:25.862125 invenio-theme-tugraz-4.12.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:21:25.858126 invenio-theme-tugraz-4.12.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-11 19:21:20.000000 invenio-theme-tugraz-4.12.8/tests/test_invenio_theme_tugraz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.684284 invenio-theme-tugraz-4.12.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.664284 invenio-theme-tugraz-4.12.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.668284 invenio-theme-tugraz-4.12.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.668284 invenio-theme-tugraz-4.12.9/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-07 08:54:09.684284 invenio-theme-tugraz-4.12.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.672284 invenio-theme-tugraz-4.12.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.672284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.664284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.664284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.664284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.672284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.664284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.676284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/communities.less
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/deposit.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.664284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.676284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    94816 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   269108 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/login.less
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/macros.less
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/record.less
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.676284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.676284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/extra/orcid.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.680284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    18533 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/Icon_1_v2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/TU_Austria_Logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/cyan_400x400.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/dark_blue_400x400.png
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/diamond.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   225210 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/footer.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/group-discussion.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/icon_use.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18643 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/inveniordm-tail.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/library-book-svgrepo-com.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/library_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/light_green_400x400.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23820 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/login_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    97455 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/oea.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/play.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    38212 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/re3data.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/red_400x400.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/rosa_400x400.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/tug_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/umbrella.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.664284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.684284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/423.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.684284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/contact_us.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/frontpage_overview.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.684284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/overview.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/recent_uploads.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/tu_graz_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.684284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.668284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.684284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-07 08:54:09.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    22541 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.668284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.684284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-07 08:54:09.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.672284 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-07 08:54:09.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-07 08:54:09.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:54:09.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-07 08:54:09.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:54:09.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-07 08:54:09.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 08:54:09.000000 invenio-theme-tugraz-4.12.9/invenio_theme_tugraz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-07 08:54:09.688284 invenio-theme-tugraz-4.12.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:54:09.684284 invenio-theme-tugraz-4.12.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-07 08:54:04.000000 invenio-theme-tugraz-4.12.9/tests/test_invenio_theme_tugraz.py
```

### Comparing `invenio-theme-tugraz-4.12.8/.editorconfig` & `invenio-theme-tugraz-4.12.9/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/.github/workflows/tests.yml` & `invenio-theme-tugraz-4.12.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/.tx/config` & `invenio-theme-tugraz-4.12.9/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/CHANGES.rst` & `invenio-theme-tugraz-4.12.9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     invenio-theme-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v4.12.9 (release 2024-05-07)
+
+- overview: view publications only if permission
+
+
 Version v4.12.8 (release 2024-03-11)
 
 - ui: add banner to header
 
 
 Version v4.12.7 (release 2024-02-12)
```

### Comparing `invenio-theme-tugraz-4.12.8/CONTRIBUTING.rst` & `invenio-theme-tugraz-4.12.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/LICENSE` & `invenio-theme-tugraz-4.12.9/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/MANIFEST.in` & `invenio-theme-tugraz-4.12.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/PKG-INFO` & `invenio-theme-tugraz-4.12.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tugraz
-Version: 4.12.8
+Version: 4.12.9
 Summary: "Invenio module for TUGRAZ theme."
 Home-page: https://github.com/tu-graz-library/invenio-theme-tugraz
 Author: "Graz University of Technology"
 Author-email: mojib.wali@tugraz.at
 License: MIT
 Keywords: invenio theme invenioRDM TU-Graz
 Platform: any
@@ -76,14 +76,19 @@
     invenio-theme-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v4.12.9 (release 2024-05-07)
+
+- overview: view publications only if permission
+
+
 Version v4.12.8 (release 2024-03-11)
 
 - ui: add banner to header
 
 
 Version v4.12.7 (release 2024-02-12)
```

### Comparing `invenio-theme-tugraz-4.12.8/README.rst` & `invenio-theme-tugraz-4.12.9/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/docs/Makefile` & `invenio-theme-tugraz-4.12.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/docs/conf.py` & `invenio-theme-tugraz-4.12.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/docs/index.rst` & `invenio-theme-tugraz-4.12.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/docs/make.bat` & `invenio-theme-tugraz-4.12.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/config.py` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/config.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/ext.py` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/ext.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 #
 # invenio-theme-tugraz is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """invenio module for TUGRAZ theme."""
 
+from invenio_records_marc21.ui.theme import current_identity_can_view
+
 from . import config
 from .views import index, locked
 
 
 class InvenioThemeTugraz(object):
     """invenio-theme-tugraz extension."""
 
@@ -25,14 +27,18 @@
         # add index route rule
         # https://flask.palletsprojects.com/en/1.1.x/api/#flask.Flask.add_url_rule
         app.add_url_rule("/", "index", index)
         self.init_config(app)
 
         app.register_error_handler(423, locked)
 
+        @app.context_processor
+        def inject_visibility():
+            return {"can_view_marc21": current_identity_can_view()}
+
         app.extensions["invenio-theme-tugraz"] = self
 
     def init_config(self, app):
         """Initialize configuration."""
         for k in dir(config):
             if k.startswith("INVENIO_THEME_TUGRAZ_") or k.startswith("THEME_TUGRAZ_"):
                 app.config.setdefault(k, getattr(config, k))
```

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/search.py` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/search.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/extra/orcid.png` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/extra/orcid.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/favicon.ico` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/Icon_1_v2.svg` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/Icon_1_v2.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/TU_Austria_Logo.png` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/TU_Austria_Logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/cyan_400x400.png` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/cyan_400x400.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/dark_blue_400x400.png` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/dark_blue_400x400.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/diamond.svg` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/diamond.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/footer.jpg` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/footer.jpg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/group-discussion.svg` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/group-discussion.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/icon_use.png` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/icon_use.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/inveniordm-tail.svg` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/inveniordm-tail.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/library-book-svgrepo-com.svg` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/library-book-svgrepo-com.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/library_logo.png` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/library_logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/light_green_400x400.png` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/light_green_400x400.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/login_logo.png` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/login_logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/logo.svg` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/oea.svg` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/oea.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/re3data.svg` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/re3data.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/red_400x400.png` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/red_400x400.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/rosa_400x400.png` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/rosa_400x400.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/static/images/tug_logo.png` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/static/images/tug_logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/contact_us.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/contact_us.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/frontpage_overview.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/frontpage_overview.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/overview.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/overview.html`

 * *Files 11% similar despite different names*

```diff
@@ -50,25 +50,27 @@
             <img width="400px" alt="Requests" src="{{ url_for("static", filename="images/umbrella.svg") }}">
           </a>
           <div>
             {{ _("Overview: Description of Requests") }}
           </div>
         </div>
       </div>
+      {% if can_view_marc21 %}
       <div class="column">
         <div class="ui segment" style="height: 480px">
           <h2>{{ _("Publications") }}</h2>
           <a class="ui left floated image" href="/publications/uploads">
             <img width="400px" alt="Publications" src="{{ url_for("static", filename="images/library-book-svgrepo-com.svg") }}">
           </a>
           <div>
             {{ _("Overview: Description for publications") }}
           </div>
         </div>
       </div>
+      {% endif %}
       <div class="column">
         <div class="ui segment" style="height: 480px">
           <h2>{{ _("Educational Resources") }}</h2>
           <a class="ui left floated image" href="/oer/uploads">
             <img width="400px" alt="Open Educational Resources" src="{{ url_for("static", filename="images/play.svg") }}">
           </a>
           <div>
```

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/recent_uploads.html` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/recent_uploads.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/templates/invenio_theme_tugraz/tu_graz_logo.svg` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/templates/invenio_theme_tugraz/tu_graz_logo.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: \n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "A service from TU Graz, developed in cooperation with CERN."
 msgstr "Ein Service der TU Graz, entwickelt in Kooperation mit CERN."
 
 msgid ""
 "Accept or reject uploads to your own community (e.g workshops, EU projects, "
 "institutions or entire disciplines)."
```

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/en/LC_MESSAGES/messages.mo` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/en/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: \n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Frontpage: Description for open educational resources"
 msgstr ""
 "In this area, you can upload your openly licensed educational content (OER, "
 "Open Educational Resources) and search for educational resources uploaded by "
 "others. Your uploaded content will be automatically transferred to the <a "
 "href=\"https://oerhub.at/en\" target=\"_blank\">OERhub.at</a>. To upload "
```

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/en/LC_MESSAGES/messages.po` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/translations/messages.pot` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/views.py` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/views.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz/webpack.py` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz.egg-info/PKG-INFO` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tugraz
-Version: 4.12.8
+Version: 4.12.9
 Summary: "Invenio module for TUGRAZ theme."
 Home-page: https://github.com/tu-graz-library/invenio-theme-tugraz
 Author: "Graz University of Technology"
 Author-email: mojib.wali@tugraz.at
 License: MIT
 Keywords: invenio theme invenioRDM TU-Graz
 Platform: any
@@ -76,14 +76,19 @@
     invenio-theme-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v4.12.9 (release 2024-05-07)
+
+- overview: view publications only if permission
+
+
 Version v4.12.8 (release 2024-03-11)
 
 - ui: add banner to header
 
 
 Version v4.12.7 (release 2024-02-12)
```

### Comparing `invenio-theme-tugraz-4.12.8/invenio_theme_tugraz.egg-info/SOURCES.txt` & `invenio-theme-tugraz-4.12.9/invenio_theme_tugraz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/requirements-devel.txt` & `invenio-theme-tugraz-4.12.9/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/run-tests.sh` & `invenio-theme-tugraz-4.12.9/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/setup.cfg` & `invenio-theme-tugraz-4.12.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 python_requires = >=3.9
 zip_safe = False
 install_requires = 
 	invenio-assets>=2.0.0
 	invenio-i18n>=1.3.1
 	invenio_config_tugraz>=0.11.0
 	invenio_records_global_search>=0.0.1
+	invenio_records_marc21>=0.21.0
 
 [options.extras_require]
 tests = 
 	invenio-app>=1.3.4,<1.4.0
+	invenio-previewer>=2.2.0
 	invenio-search[opensearch2]>=2.1.0,<3.0.0
 	pytest-black-ng>=0.4.0
 	pytest-invenio>=2.1.0,<3.0.0
 	Sphinx>=4.5.0
 
 [options.entry_points]
 invenio_base.apps =
```

### Comparing `invenio-theme-tugraz-4.12.8/tests/conftest.py` & `invenio-theme-tugraz-4.12.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.12.8/tests/test_invenio_theme_tugraz.py` & `invenio-theme-tugraz-4.12.9/tests/test_invenio_theme_tugraz.py`

 * *Files identical despite different names*

