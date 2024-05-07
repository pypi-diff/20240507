# Comparing `tmp/lizard-ui-5.2.tar.gz` & `tmp/lizard-ui-5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lizard-ui-5.2.tar", last modified: Thu Oct  8 12:07:23 2015, max compression
+gzip compressed data, was "dist/lizard-ui-5.3.tar", last modified: Thu Oct  8 14:24:03 2015, max compression
```

## Comparing `lizard-ui-5.2.tar` & `lizard-ui-5.3.tar`

### file list

```diff
@@ -1,1220 +1,1220 @@
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/
--rw-r--r--   0 reinout    (501) staff       (20)    28364 2015-10-08 12:07:22.000000 lizard-ui-5.2/CHANGES.rst
--rw-r--r--   0 reinout    (501) staff       (20)       45 2015-10-08 12:07:22.000000 lizard-ui-5.2/CREDITS.rst
--rw-r--r--   0 reinout    (501) staff       (20)     7651 2015-10-08 12:07:22.000000 lizard-ui-5.2/LICENSE.rst
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/
--rw-r--r--   0 reinout    (501) staff       (20)        9 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/__init__.py
--rw-r--r--   0 reinout    (501) staff       (20)      822 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/admin.py
--rw-r--r--   0 reinout    (501) staff       (20)     5212 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/configchecker.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/docs/
--rw-r--r--   0 reinout    (501) staff       (20)      673 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/docs/__init__.html
--rw-r--r--   0 reinout    (501) staff       (20)      357 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/docs/admin.html
--rw-r--r--   0 reinout    (501) staff       (20)     1974 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/docs/middleware.html
--rw-r--r--   0 reinout    (501) staff       (20)     2884 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/docs/models.html
--rw-r--r--   0 reinout    (501) staff       (20)     7008 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/docs/pycco.css
--rw-r--r--   0 reinout    (501) staff       (20)     6786 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/docs/tests.html
--rw-r--r--   0 reinout    (501) staff       (20)     9633 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/docs/testsettings.html
--rw-r--r--   0 reinout    (501) staff       (20)     8682 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/docs/urls.html
--rw-r--r--   0 reinout    (501) staff       (20)     8233 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/docs/views.html
--rw-r--r--   0 reinout    (501) staff       (20)      690 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/forms.py
--rw-r--r--   0 reinout    (501) staff       (20)     1421 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/layout.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/af/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/af/LC_MESSAGES/
--rw-r--r--   0 reinout    (501) staff       (20)     2013 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/af/LC_MESSAGES/django.mo
--rw-r--r--   0 reinout    (501) staff       (20)     4238 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/af/LC_MESSAGES/django.po
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/ar/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/ar/LC_MESSAGES/
--rw-r--r--   0 reinout    (501) staff       (20)      646 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 reinout    (501) staff       (20)     3802 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0 reinout    (501) staff       (20)      906 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/en/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/en/LC_MESSAGES/
--rw-r--r--   0 reinout    (501) staff       (20)      413 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 reinout    (501) staff       (20)     3572 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 reinout    (501) staff       (20)      378 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 reinout    (501) staff       (20)      764 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/nl/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/nl/LC_MESSAGES/
--rw-r--r--   0 reinout    (501) staff       (20)     2908 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 reinout    (501) staff       (20)     4579 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0 reinout    (501) staff       (20)      645 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/nl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 reinout    (501) staff       (20)     1005 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/nl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/vi/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/vi/LC_MESSAGES/
--rw-r--r--   0 reinout    (501) staff       (20)      538 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 reinout    (501) staff       (20)     3772 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/zh/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/zh/LC_MESSAGES/
--rw-r--r--   0 reinout    (501) staff       (20)     1912 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 reinout    (501) staff       (20)     4114 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/management/
--rw-r--r--   0 reinout    (501) staff       (20)       10 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/management/__init__.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/management/commands/
--rw-r--r--   0 reinout    (501) staff       (20)       10 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/management/commands/__init__.py
--rw-r--r--   0 reinout    (501) staff       (20)      474 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/management/commands/check_config.py
--rw-r--r--   0 reinout    (501) staff       (20)     1476 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/management/commands/i18n.py
--rw-r--r--   0 reinout    (501) staff       (20)      485 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/middleware.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/migrations/
--rw-r--r--   0 reinout    (501) staff       (20)     2882 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/migrations/0001_initial.py
--rw-r--r--   0 reinout    (501) staff       (20)     2588 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/migrations/0002_auto__chg_field_applicationscreen_description__chg_field_applicationic.py
--rw-r--r--   0 reinout    (501) staff       (20)     1949 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/migrations/0003_adding_description_field.py
--rw-r--r--   0 reinout    (501) staff       (20)     2233 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/migrations/0004_auto__add_field_applicationicon_sub_screen.py
--rw-r--r--   0 reinout    (501) staff       (20)     2637 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/migrations/0005_auto__chg_field_applicationicon_sub_screen__add_unique_applicationicon.py
--rw-r--r--   0 reinout    (501) staff       (20)     2802 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/migrations/0006_auto__add_field_applicationicon_data_set.py
--rw-r--r--   0 reinout    (501) staff       (20)     3440 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/migrations/0007_auto__add_customerlogo.py
--rw-r--r--   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/migrations/__init__.py
--rw-r--r--   0 reinout    (501) staff       (20)     5849 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/models.py
--rw-r--r--   0 reinout    (501) staff       (20)      250 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/multitenancy.py
--rw-r--r--   0 reinout    (501) staff       (20)     2966 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/settingshelper.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/
--rw-r--r--   0 reinout    (501) staff       (20)     1861 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/ie.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/buttons/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/buttons/icons/
--rwxr-xr-x   0 reinout    (501) staff       (20)      655 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/buttons/icons/cross.png
--rwxr-xr-x   0 reinout    (501) staff       (20)      455 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/buttons/icons/key.png
--rwxr-xr-x   0 reinout    (501) staff       (20)      537 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/buttons/icons/tick.png
--rw-r--r--   0 reinout    (501) staff       (20)      930 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/buttons/readme.txt
--rw-r--r--   0 reinout    (501) staff       (20)     2004 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/buttons/screen.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/fancy-type/
--rw-r--r--   0 reinout    (501) staff       (20)      340 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/fancy-type/readme.txt
--rw-r--r--   0 reinout    (501) staff       (20)     2173 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/fancy-type/screen.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/
--rw-r--r--   0 reinout    (501) staff       (20)      777 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/doc.png
--rw-r--r--   0 reinout    (501) staff       (20)      641 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/email.png
--rw-r--r--   0 reinout    (501) staff       (20)    46848 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/external.png
--rw-r--r--   0 reinout    (501) staff       (20)      691 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/feed.png
--rw-r--r--   0 reinout    (501) staff       (20)      741 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/im.png
--rw-r--r--   0 reinout    (501) staff       (20)      591 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/pdf.png
--rw-r--r--   0 reinout    (501) staff       (20)    46990 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/visited.png
--rw-r--r--   0 reinout    (501) staff       (20)      663 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/xls.png
--rw-r--r--   0 reinout    (501) staff       (20)      449 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/readme.txt
--rw-r--r--   0 reinout    (501) staff       (20)     1343 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/screen.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/rtl/
--rw-r--r--   0 reinout    (501) staff       (20)      327 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/rtl/readme.txt
--rw-r--r--   0 reinout    (501) staff       (20)     4839 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/plugins/rtl/screen.css
--rw-r--r--   0 reinout    (501) staff       (20)     1284 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/print.css
--rw-r--r--   0 reinout    (501) staff       (20)    11833 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/screen.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/src/
--rw-r--r--   0 reinout    (501) staff       (20)     1835 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/src/forms.css
--rwxr-xr-x   0 reinout    (501) staff       (20)     9486 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/src/grid.css
--rw-r--r--   0 reinout    (501) staff       (20)      195 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/src/grid.png
--rw-r--r--   0 reinout    (501) staff       (20)     2537 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/src/ie.css
--rwxr-xr-x   0 reinout    (501) staff       (20)     1826 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/src/print.css
--rwxr-xr-x   0 reinout    (501) staff       (20)     1232 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/src/reset.css
--rw-r--r--   0 reinout    (501) staff       (20)     3182 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/blueprint/src/typography.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/
--rw-r--r--   0 reinout    (501) staff       (20)      344 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/.gitignore
--rw-r--r--   0 reinout    (501) staff       (20)       34 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/.travis.yml
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/css/
--rw-r--r--   0 reinout    (501) staff       (20)    22111 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/css/bootstrap-responsive.css
--rw-r--r--   0 reinout    (501) staff       (20)    16849 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/css/bootstrap-responsive.min.css
--rw-r--r--   0 reinout    (501) staff       (20)   154037 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/css/bootstrap.css
--rw-r--r--   0 reinout    (501) staff       (20)   127579 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/js/
--rw-r--r--   0 reinout    (501) staff       (20)    61979 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/js/bootstrap.js
--rw-r--r--   0 reinout    (501) staff       (20)    28519 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 reinout    (501) staff       (20)    25120 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/CHANGELOG.md
--rw-r--r--   0 reinout    (501) staff       (20)      175 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/component.json
--rw-r--r--   0 reinout    (501) staff       (20)      297 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/composer.json
--rw-r--r--   0 reinout    (501) staff       (20)     3487 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/CONTRIBUTING.md
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/css/
--rw-r--r--   0 reinout    (501) staff       (20)    22111 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/css/bootstrap-responsive.css
--rw-r--r--   0 reinout    (501) staff       (20)   153960 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/css/bootstrap.css
--rw-r--r--   0 reinout    (501) staff       (20)    22486 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/css/docs.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/ico/
--rw-r--r--   0 reinout    (501) staff       (20)    11392 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-114-precomposed.png
--rw-r--r--   0 reinout    (501) staff       (20)    16780 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-144-precomposed.png
--rw-r--r--   0 reinout    (501) staff       (20)     4026 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-57-precomposed.png
--rw-r--r--   0 reinout    (501) staff       (20)     5681 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-72-precomposed.png
--rw-r--r--   0 reinout    (501) staff       (20)     1150 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/ico/favicon.ico
--rw-r--r--   0 reinout    (501) staff       (20)     2711 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/ico/favicon.png
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/
--rw-r--r--   0 reinout    (501) staff       (20)    30612 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-docs-readme.png
--rw-r--r--   0 reinout    (501) staff       (20)   125346 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-mdo-sfmoma-01.jpg
--rw-r--r--   0 reinout    (501) staff       (20)    81284 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-mdo-sfmoma-02.jpg
--rw-r--r--   0 reinout    (501) staff       (20)    49063 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-mdo-sfmoma-03.jpg
--rw-r--r--   0 reinout    (501) staff       (20)    11244 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-bootstrap-features.png
--rw-r--r--   0 reinout    (501) staff       (20)     6450 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-masthead-pattern.png
--rw-r--r--   0 reinout    (501) staff       (20)    10572 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-responsive-illustrations.png
--rw-r--r--   0 reinout    (501) staff       (20)    30968 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-twitter-github.png
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/
--rw-r--r--   0 reinout    (501) staff       (20)    62853 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/8020select.png
--rw-r--r--   0 reinout    (501) staff       (20)   136480 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/adoptahydrant.png
--rw-r--r--   0 reinout    (501) staff       (20)    72725 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/breakingnews.png
--rw-r--r--   0 reinout    (501) staff       (20)    39837 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/fleetio.png
--rw-r--r--   0 reinout    (501) staff       (20)    76560 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/gathercontent.png
--rw-r--r--   0 reinout    (501) staff       (20)     7258 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/jshint.png
--rw-r--r--   0 reinout    (501) staff       (20)    48259 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/kippt.png
--rw-r--r--   0 reinout    (501) staff       (20)    50225 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/soundready.png
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/
--rw-r--r--   0 reinout    (501) staff       (20)   339980 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-carousel.png
--rw-r--r--   0 reinout    (501) staff       (20)   209039 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-fluid.png
--rw-r--r--   0 reinout    (501) staff       (20)   136021 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-justified-nav.png
--rw-r--r--   0 reinout    (501) staff       (20)   117303 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-marketing-narrow.png
--rw-r--r--   0 reinout    (501) staff       (20)   134269 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-marketing.png
--rw-r--r--   0 reinout    (501) staff       (20)    22037 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-signin.png
--rw-r--r--   0 reinout    (501) staff       (20)    36099 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-starter.png
--rw-r--r--   0 reinout    (501) staff       (20)    30820 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-sticky-footer.png
--rw-r--r--   0 reinout    (501) staff       (20)    55522 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/browser-icon-chrome.png
--rw-r--r--   0 reinout    (501) staff       (20)   175994 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/browser-icon-firefox.png
--rw-r--r--   0 reinout    (501) staff       (20)   209527 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/browser-icon-safari.png
--rw-r--r--   0 reinout    (501) staff       (20)    83303 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/slide-01.jpg
--rw-r--r--   0 reinout    (501) staff       (20)   137070 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/slide-02.jpg
--rw-r--r--   0 reinout    (501) staff       (20)   137378 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/slide-03.jpg
--rw-r--r--   0 reinout    (501) staff       (20)     8777 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/glyphicons-halflings-white.png
--rw-r--r--   0 reinout    (501) staff       (20)    12799 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/glyphicons-halflings.png
--rw-r--r--   0 reinout    (501) staff       (20)       84 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/grid-baseline-20px.png
--rw-r--r--   0 reinout    (501) staff       (20)    12824 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/less-logo-large.png
--rw-r--r--   0 reinout    (501) staff       (20)     1008 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/responsive-illustrations.png
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/
--rw-r--r--   0 reinout    (501) staff       (20)     4036 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/application.js
--rw-r--r--   0 reinout    (501) staff       (20)     3483 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-affix.js
--rw-r--r--   0 reinout    (501) staff       (20)     2524 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-alert.js
--rw-r--r--   0 reinout    (501) staff       (20)     2841 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-button.js
--rw-r--r--   0 reinout    (501) staff       (20)     6057 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-carousel.js
--rw-r--r--   0 reinout    (501) staff       (20)     4735 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-collapse.js
--rw-r--r--   0 reinout    (501) staff       (20)     4203 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-dropdown.js
--rw-r--r--   0 reinout    (501) staff       (20)     6656 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-modal.js
--rw-r--r--   0 reinout    (501) staff       (20)     3115 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-popover.js
--rw-r--r--   0 reinout    (501) staff       (20)     4655 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-scrollspy.js
--rw-r--r--   0 reinout    (501) staff       (20)     3496 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-tab.js
--rw-r--r--   0 reinout    (501) staff       (20)    10138 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-tooltip.js
--rw-r--r--   0 reinout    (501) staff       (20)     1756 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-transition.js
--rw-r--r--   0 reinout    (501) staff       (20)     8320 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-typeahead.js
--rw-r--r--   0 reinout    (501) staff       (20)    61979 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap.js
--rw-r--r--   0 reinout    (501) staff       (20)    28526 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap.min.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/google-code-prettify/
--rw-r--r--   0 reinout    (501) staff       (20)      817 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/google-code-prettify/prettify.css
--rw-r--r--   0 reinout    (501) staff       (20)    13632 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/google-code-prettify/prettify.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/holder/
--rw-r--r--   0 reinout    (501) staff       (20)    11731 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/holder/holder.js
--rw-r--r--   0 reinout    (501) staff       (20)     2376 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/html5shiv.js
--rw-r--r--   0 reinout    (501) staff       (20)    92629 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/jquery.js
--rw-r--r--   0 reinout    (501) staff       (20)     3249 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/README.md
--rw-r--r--   0 reinout    (501) staff       (20)    94309 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/base-css.html
--rw-r--r--   0 reinout    (501) staff       (20)   107153 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/components.html
--rw-r--r--   0 reinout    (501) staff       (20)    27043 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/customize.html
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/
--rw-r--r--   0 reinout    (501) staff       (20)    15641 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/carousel.html
--rw-r--r--   0 reinout    (501) staff       (20)     7697 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/fluid.html
--rw-r--r--   0 reinout    (501) staff       (20)     5825 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/hero.html
--rw-r--r--   0 reinout    (501) staff       (20)     6130 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/justified-nav.html
--rw-r--r--   0 reinout    (501) staff       (20)     4712 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/marketing-narrow.html
--rw-r--r--   0 reinout    (501) staff       (20)     3634 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/signin.html
--rw-r--r--   0 reinout    (501) staff       (20)     3333 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/starter-template.html
--rw-r--r--   0 reinout    (501) staff       (20)     5798 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/sticky-footer-navbar.html
--rw-r--r--   0 reinout    (501) staff       (20)     4174 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/sticky-footer.html
--rw-r--r--   0 reinout    (501) staff       (20)    12644 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/extend.html
--rw-r--r--   0 reinout    (501) staff       (20)    17348 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/getting-started.html
--rw-r--r--   0 reinout    (501) staff       (20)     9693 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/index.html
--rw-r--r--   0 reinout    (501) staff       (20)    91135 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/javascript.html
--rw-r--r--   0 reinout    (501) staff       (20)    25153 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/scaffolding.html
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/
--rw-r--r--   0 reinout    (501) staff       (20)     6537 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/layout.mustache
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/
--rw-r--r--   0 reinout    (501) staff       (20)    94743 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/base-css.mustache
--rw-r--r--   0 reinout    (501) staff       (20)   110205 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/components.mustache
--rw-r--r--   0 reinout    (501) staff       (20)    23053 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/customize.mustache
--rw-r--r--   0 reinout    (501) staff       (20)     7993 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/extend.mustache
--rw-r--r--   0 reinout    (501) staff       (20)    13609 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/getting-started.mustache
--rw-r--r--   0 reinout    (501) staff       (20)     5269 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/index.mustache
--rw-r--r--   0 reinout    (501) staff       (20)    93014 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/javascript.mustache
--rw-r--r--   0 reinout    (501) staff       (20)    21739 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/scaffolding.mustache
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/img/
--rw-r--r--   0 reinout    (501) staff       (20)     8777 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/img/glyphicons-halflings-white.png
--rw-r--r--   0 reinout    (501) staff       (20)    12799 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/img/glyphicons-halflings.png
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/
--rw-r--r--   0 reinout    (501) staff       (20)      232 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/.jshintrc
--rw-r--r--   0 reinout    (501) staff       (20)     3483 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-affix.js
--rw-r--r--   0 reinout    (501) staff       (20)     2524 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-alert.js
--rw-r--r--   0 reinout    (501) staff       (20)     2841 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-button.js
--rw-r--r--   0 reinout    (501) staff       (20)     6057 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-carousel.js
--rw-r--r--   0 reinout    (501) staff       (20)     4735 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-collapse.js
--rw-r--r--   0 reinout    (501) staff       (20)     4203 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-dropdown.js
--rw-r--r--   0 reinout    (501) staff       (20)     6656 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-modal.js
--rw-r--r--   0 reinout    (501) staff       (20)     3115 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-popover.js
--rw-r--r--   0 reinout    (501) staff       (20)     4655 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-scrollspy.js
--rw-r--r--   0 reinout    (501) staff       (20)     3496 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-tab.js
--rw-r--r--   0 reinout    (501) staff       (20)    10138 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-tooltip.js
--rw-r--r--   0 reinout    (501) staff       (20)     1756 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-transition.js
--rw-r--r--   0 reinout    (501) staff       (20)     8320 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-typeahead.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/
--rw-r--r--   0 reinout    (501) staff       (20)     2134 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/index.html
--rw-r--r--   0 reinout    (501) staff       (20)     2146 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/phantom.js
--rw-r--r--   0 reinout    (501) staff       (20)      331 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/server.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/
--rw-r--r--   0 reinout    (501) staff       (20)      797 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-affix.js
--rw-r--r--   0 reinout    (501) staff       (20)     2099 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-alert.js
--rw-r--r--   0 reinout    (501) staff       (20)     3761 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-button.js
--rw-r--r--   0 reinout    (501) staff       (20)     6044 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-carousel.js
--rw-r--r--   0 reinout    (501) staff       (20)     2913 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-collapse.js
--rw-r--r--   0 reinout    (501) staff       (20)     6328 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-dropdown.js
--rw-r--r--   0 reinout    (501) staff       (20)     4362 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-modal.js
--rw-r--r--   0 reinout    (501) staff       (20)      714 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-phantom.js
--rw-r--r--   0 reinout    (501) staff       (20)     4553 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-popover.js
--rw-r--r--   0 reinout    (501) staff       (20)     1203 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-scrollspy.js
--rw-r--r--   0 reinout    (501) staff       (20)     2848 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-tab.js
--rw-r--r--   0 reinout    (501) staff       (20)    10849 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-tooltip.js
--rw-r--r--   0 reinout    (501) staff       (20)      374 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-transition.js
--rw-r--r--   0 reinout    (501) staff       (20)     7584 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-typeahead.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/vendor/
--rw-r--r--   0 reinout    (501) staff       (20)    92629 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/vendor/jquery.js
--rw-r--r--   0 reinout    (501) staff       (20)     4560 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/vendor/qunit.css
--rw-r--r--   0 reinout    (501) staff       (20)    38070 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/vendor/qunit.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/
--rw-r--r--   0 reinout    (501) staff       (20)      636 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/accordion.less
--rw-r--r--   0 reinout    (501) staff       (20)     1369 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/alerts.less
--rw-r--r--   0 reinout    (501) staff       (20)     1633 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/bootstrap.less
--rw-r--r--   0 reinout    (501) staff       (20)      431 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/breadcrumbs.less
--rw-r--r--   0 reinout    (501) staff       (20)     5709 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/button-groups.less
--rw-r--r--   0 reinout    (501) staff       (20)     4766 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/buttons.less
--rw-r--r--   0 reinout    (501) staff       (20)     2482 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/carousel.less
--rw-r--r--   0 reinout    (501) staff       (20)      644 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/close.less
--rw-r--r--   0 reinout    (501) staff       (20)     1282 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/code.less
--rw-r--r--   0 reinout    (501) staff       (20)      306 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/component-animations.less
--rw-r--r--   0 reinout    (501) staff       (20)     5493 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/dropdowns.less
--rw-r--r--   0 reinout    (501) staff       (20)    20690 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/font-awesome.less
--rw-r--r--   0 reinout    (501) staff       (20)    15866 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/forms.less
--rw-r--r--   0 reinout    (501) staff       (20)      429 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/grid.less
--rw-r--r--   0 reinout    (501) staff       (20)      521 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/hero-unit.less
--rw-r--r--   0 reinout    (501) staff       (20)     1884 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/labels-badges.less
--rw-r--r--   0 reinout    (501) staff       (20)      329 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/layouts.less
--rw-r--r--   0 reinout    (501) staff       (20)    18012 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/lizard-bootstrap.less
--rw-r--r--   0 reinout    (501) staff       (20)      860 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/media.less
--rw-r--r--   0 reinout    (501) staff       (20)    23042 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/mixins.less
--rw-r--r--   0 reinout    (501) staff       (20)     1978 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/modals.less
--rw-r--r--   0 reinout    (501) staff       (20)    12002 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/navbar.less
--rw-r--r--   0 reinout    (501) staff       (20)     8163 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/navs.less
--rw-r--r--   0 reinout    (501) staff       (20)      760 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/pager.less
--rw-r--r--   0 reinout    (501) staff       (20)     2678 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/pagination.less
--rw-r--r--   0 reinout    (501) staff       (20)     3077 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/popovers.less
--rw-r--r--   0 reinout    (501) staff       (20)     2858 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/progress-bars.less
--rw-r--r--   0 reinout    (501) staff       (20)     4201 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/reset.less
--rw-r--r--   0 reinout    (501) staff       (20)      565 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/responsive-1200px-min.less
--rw-r--r--   0 reinout    (501) staff       (20)     3920 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/responsive-767px-max.less
--rw-r--r--   0 reinout    (501) staff       (20)      463 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/responsive-768px-979px.less
--rw-r--r--   0 reinout    (501) staff       (20)     4328 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/responsive-navbar.less
--rw-r--r--   0 reinout    (501) staff       (20)     1602 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/responsive-utilities.less
--rw-r--r--   0 reinout    (501) staff       (20)     1069 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/responsive.less
--rw-r--r--   0 reinout    (501) staff       (20)      885 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/scaffolding.less
--rw-r--r--   0 reinout    (501) staff       (20)    10841 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/sprites.less
--rw-r--r--   0 reinout    (501) staff       (20)     6255 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/tables.less
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/
--rw-r--r--   0 reinout    (501) staff       (20)     6411 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/buttons.html
--rw-r--r--   0 reinout    (501) staff       (20)     5475 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/css-tests.css
--rw-r--r--   0 reinout    (501) staff       (20)    40138 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/css-tests.html
--rw-r--r--   0 reinout    (501) staff       (20)     2362 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/forms-responsive.html
--rw-r--r--   0 reinout    (501) staff       (20)     4079 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/forms.html
--rw-r--r--   0 reinout    (501) staff       (20)     4692 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/navbar-fixed-top.html
--rw-r--r--   0 reinout    (501) staff       (20)     4711 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/navbar-static-top.html
--rw-r--r--   0 reinout    (501) staff       (20)     4797 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/navbar.html
--rw-r--r--   0 reinout    (501) staff       (20)     1192 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/thumbnails.less
--rw-r--r--   0 reinout    (501) staff       (20)     1684 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/tooltip.less
--rw-r--r--   0 reinout    (501) staff       (20)     4857 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/type.less
--rw-r--r--   0 reinout    (501) staff       (20)      335 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/utilities.less
--rw-r--r--   0 reinout    (501) staff       (20)     9134 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/variables.less
--rw-r--r--   0 reinout    (501) staff       (20)      552 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/less/wells.less
--rw-r--r--   0 reinout    (501) staff       (20)    10172 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/LICENSE
--rw-r--r--   0 reinout    (501) staff       (20)     4561 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/Makefile
--rw-r--r--   0 reinout    (501) staff       (20)      700 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/package.json
--rw-r--r--   0 reinout    (501) staff       (20)     4599 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap/README.md
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap-tour/
--rw-r--r--   0 reinout    (501) staff       (20)     1723 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap-tour/bootstrap-tour.min.css
--rw-r--r--   0 reinout    (501) staff       (20)    14438 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/bootstrap-tour/bootstrap-tour.min.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/css/
--rw-r--r--   0 reinout    (501) staff       (20)     3181 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/css/colorpicker.css
--rw-r--r--   0 reinout    (501) staff       (20)     4073 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/css/layout.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/
--rw-r--r--   0 reinout    (501) staff       (20)       49 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/blank.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1897 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_background.png
--rw-r--r--   0 reinout    (501) staff       (20)      532 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_hex.png
--rw-r--r--   0 reinout    (501) staff       (20)      970 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_hsb_b.png
--rw-r--r--   0 reinout    (501) staff       (20)     1012 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_hsb_h.png
--rw-r--r--   0 reinout    (501) staff       (20)     1171 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_hsb_s.png
--rw-r--r--   0 reinout    (501) staff       (20)       86 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_indic.gif
--rw-r--r--   0 reinout    (501) staff       (20)    10355 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_overlay.png
--rw-r--r--   0 reinout    (501) staff       (20)      970 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_rgb_b.png
--rw-r--r--   0 reinout    (501) staff       (20)     1069 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_rgb_g.png
--rw-r--r--   0 reinout    (501) staff       (20)     1066 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_rgb_r.png
--rw-r--r--   0 reinout    (501) staff       (20)       78 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_select.gif
--rw-r--r--   0 reinout    (501) staff       (20)      984 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_submit.png
--rw-r--r--   0 reinout    (501) staff       (20)     1916 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_background.png
--rw-r--r--   0 reinout    (501) staff       (20)      562 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_hex.png
--rw-r--r--   0 reinout    (501) staff       (20)     1097 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_hsb_b.png
--rw-r--r--   0 reinout    (501) staff       (20)      970 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_hsb_h.png
--rw-r--r--   0 reinout    (501) staff       (20)     1168 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_hsb_s.png
--rw-r--r--   0 reinout    (501) staff       (20)       86 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_indic.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1008 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_rgb_b.png
--rw-r--r--   0 reinout    (501) staff       (20)     1069 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_rgb_g.png
--rw-r--r--   0 reinout    (501) staff       (20)     1018 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_rgb_r.png
--rw-r--r--   0 reinout    (501) staff       (20)      997 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_submit.png
--rw-r--r--   0 reinout    (501) staff       (20)      506 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/select.png
--rw-r--r--   0 reinout    (501) staff       (20)      518 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/select2.png
--rw-r--r--   0 reinout    (501) staff       (20)      315 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/slider.png
--rw-r--r--   0 reinout    (501) staff       (20)    19968 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/images/Thumbs.db
--rw-r--r--   0 reinout    (501) staff       (20)     8411 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/index.html
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/js/
--rw-r--r--   0 reinout    (501) staff       (20)    17164 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/js/colorpicker.js
--rw-r--r--   0 reinout    (501) staff       (20)      604 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/js/eye.js
--rw-r--r--   0 reinout    (501) staff       (20)   124995 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/js/jquery.js
--rw-r--r--   0 reinout    (501) staff       (20)     1829 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/js/layout.js
--rw-r--r--   0 reinout    (501) staff       (20)     7135 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/colorpicker/js/utils.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/datatables/
--rw-r--r--   0 reinout    (501) staff       (20)        7 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/.gitignore
--rw-r--r--   0 reinout    (501) staff       (20)     1440 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/license-bsd.txt
--rw-r--r--   0 reinout    (501) staff       (20)    17987 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/license-gpl2.txt
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/
--rw-r--r--   0 reinout    (501) staff       (20)     6148 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/.DS_Store
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/css/
--rw-r--r--   0 reinout    (501) staff       (20)     1341 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/css/demo_page.css
--rw-r--r--   0 reinout    (501) staff       (20)     9689 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/css/demo_table.css
--rw-r--r--   0 reinout    (501) staff       (20)     8930 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/css/demo_table_jui.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/images/
--rw-r--r--   0 reinout    (501) staff       (20)      612 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/images/back_disabled.jpg
--rw-r--r--   0 reinout    (501) staff       (20)      807 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/images/back_enabled.jpg
--rw-r--r--   0 reinout    (501) staff       (20)      894 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/images/favicon.ico
--rw-r--r--   0 reinout    (501) staff       (20)      635 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/images/forward_disabled.jpg
--rw-r--r--   0 reinout    (501) staff       (20)      852 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/images/forward_enabled.jpg
--rw-r--r--   0 reinout    (501) staff       (20)      263 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/images/sort_asc.png
--rw-r--r--   0 reinout    (501) staff       (20)      252 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/images/sort_asc_disabled.png
--rw-r--r--   0 reinout    (501) staff       (20)      282 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/images/sort_both.png
--rw-r--r--   0 reinout    (501) staff       (20)      260 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/images/sort_desc.png
--rw-r--r--   0 reinout    (501) staff       (20)      251 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/images/sort_desc_disabled.png
--rw-r--r--   0 reinout    (501) staff       (20)    27490 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/images/Sorting icons.psd
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/js/
--rw-r--r--   0 reinout    (501) staff       (20)   230256 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/js/jquery.dataTables.js
--rw-r--r--   0 reinout    (501) staff       (20)    70883 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/js/jquery.dataTables.min.js
--rw-r--r--   0 reinout    (501) staff       (20)    19393 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/js/jquery.dataTables.min.js.gz
--rw-r--r--   0 reinout    (501) staff       (20)    91625 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/media/js/jquery.js
--rw-r--r--   0 reinout    (501) staff       (20)      965 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/datatables/Readme.txt
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/daterangepicker/
--rw-r--r--   0 reinout    (501) staff       (20)     4128 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/daterangepicker/daterangepicker.css
--rw-r--r--   0 reinout    (501) staff       (20)    20548 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/daterangepicker/daterangepicker.js
--rw-r--r--   0 reinout    (501) staff       (20)     3948 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/daterangepicker/daterangepicker.orig.css
--rw-r--r--   0 reinout    (501) staff       (20)    19832 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/daterangepicker/daterangepicker.orig.js
--rw-r--r--   0 reinout    (501) staff       (20)     2230 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/daterangepicker/README.md
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/font-awesome/
--rw-r--r--   0 reinout    (501) staff       (20)    25255 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/font-awesome/font-awesome-ie7.min.css
--rwxr-xr-x   0 reinout    (501) staff       (20)    25395 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/font-awesome/fontawesome-webfont.eot
--rwxr-xr-x   0 reinout    (501) staff       (20)   138488 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/font-awesome/fontawesome-webfont.svg
--rwxr-xr-x   0 reinout    (501) staff       (20)    55096 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/font-awesome/fontawesome-webfont.ttf
--rwxr-xr-x   0 reinout    (501) staff       (20)    29380 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/font-awesome/fontawesome-webfont.woff
--rw-r--r--   0 reinout    (501) staff       (20)    48748 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/font-awesome/FontAwesome.otf
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/html5shiv/
--rw-r--r--   0 reinout    (501) staff       (20)     9342 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/html5shiv/html5shiv.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/jquery/
--rw-r--r--   0 reinout    (501) staff       (20)    94840 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery/jquery.min.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/
--rwxr-xr-x   0 reinout    (501) staff       (20)    19314 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/excanvas.min.js
--rw-r--r--   0 reinout    (501) staff       (20)     6110 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.colorhelpers.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    14146 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.axislabels.js
--rw-r--r--   0 reinout    (501) staff       (20)     5871 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.categories.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5191 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.crosshair.js
--rw-r--r--   0 reinout    (501) staff       (20)    12637 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.errorbars.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6772 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.fillbetween.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7351 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.image.js
--rwxr-xr-x   0 reinout    (501) staff       (20)   106306 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    14160 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.navigate.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    30114 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.pie.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1335 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.resize.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    12018 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.selection.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6968 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.stack.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2441 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.symbol.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4180 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.threshold.js
--rw-r--r--   0 reinout    (501) staff       (20)    12968 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.time.js
--rw-r--r--   0 reinout    (501) staff       (20)    12037 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.touch.js
--rw-r--r--   0 reinout    (501) staff       (20)     1069 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-flot/LICENSE.txt
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/jquery-json/
--rw-r--r--   0 reinout    (501) staff       (20)     4712 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-json/jquery.json-2.3.js
--rw-r--r--   0 reinout    (501) staff       (20)     2177 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-json/jquery.json-2.3.min.js
--rw-r--r--   0 reinout    (501) staff       (20)    17521 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-json/json2.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/jquery-mobile-events/
--rw-r--r--   0 reinout    (501) staff       (20)    15443 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-mobile-events/jquery.mobile-events.min.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/jquery-resize/
--rw-r--r--   0 reinout    (501) staff       (20)     9195 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-resize/jquery.ba-resize.js
--rw-r--r--   0 reinout    (501) staff       (20)     1098 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-resize/jquery.ba-resize.min.js
--rw-r--r--   0 reinout    (501) staff       (20)    15098 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-resize/LICENSE-GPL
--rw-r--r--   0 reinout    (501) staff       (20)     1062 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-resize/LICENSE-MIT
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/jquery-transform/
--rw-r--r--   0 reinout    (501) staff       (20)    51654 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-transform/jquery.transform-0.9.3.js
--rw-r--r--   0 reinout    (501) staff       (20)    20250 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-transform/jquery.transform-0.9.3.min.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/
--rw-r--r--   0 reinout    (501) staff       (20)      847 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/ajax-loader.gif
--rw-r--r--   0 reinout    (501) staff       (20)      110 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/file.gif
--rw-r--r--   0 reinout    (501) staff       (20)      105 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/folder-closed.gif
--rw-r--r--   0 reinout    (501) staff       (20)      106 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/folder.gif
--rw-r--r--   0 reinout    (501) staff       (20)      837 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/minus.gif
--rw-r--r--   0 reinout    (501) staff       (20)      841 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/plus.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1877 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-black-line.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1216 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-black.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1993 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-default-line.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1222 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-default.gif
--rw-r--r--   0 reinout    (501) staff       (20)      807 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-famfamfam-line.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1280 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-famfamfam.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1877 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-gray-line.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1230 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-gray.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1877 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-red-line.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1230 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-red.gif
--rw-r--r--   0 reinout    (501) staff       (20)     2866 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/jquery.treeview.async.js
--rw-r--r--   0 reinout    (501) staff       (20)     2651 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/jquery.treeview.css
--rw-r--r--   0 reinout    (501) staff       (20)     1567 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/jquery.treeview.edit.js
--rw-r--r--   0 reinout    (501) staff       (20)     8264 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/jquery.treeview.js
--rw-r--r--   0 reinout    (501) staff       (20)    13156 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jquery-treeview/jquery.treeview.sortable.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/
--rw-r--r--   0 reinout    (501) staff       (20)   365958 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/jquery-ui.js
--rw-r--r--   0 reinout    (501) staff       (20)   365673 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/jquery-ui.orig.js
--rw-r--r--   0 reinout    (501) staff       (20)      924 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/jquery.ui.datepicker-nl.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/
--rw-r--r--   0 reinout    (501) staff       (20)      180 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-r--r--   0 reinout    (501) staff       (20)      178 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-bg_flat_75_ffffff_40x100.png
--rw-r--r--   0 reinout    (501) staff       (20)      120 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 reinout    (501) staff       (20)      105 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 reinout    (501) staff       (20)      111 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 reinout    (501) staff       (20)      110 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 reinout    (501) staff       (20)      119 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 reinout    (501) staff       (20)      101 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 reinout    (501) staff       (20)     4369 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 reinout    (501) staff       (20)     4369 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 reinout    (501) staff       (20)     4369 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0 reinout    (501) staff       (20)     4369 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0 reinout    (501) staff       (20)     4369 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 reinout    (501) staff       (20)    33422 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/jquery-ui.css
--rw-r--r--   0 reinout    (501) staff       (20)    33172 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/jquery-ui.orig.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/less/
--rw-r--r--   0 reinout    (501) staff       (20)    44423 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/less/less-1.2.1.min.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/
--rw-r--r--   0 reinout    (501) staff       (20)      622 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/60degree_gray.png
--rw-r--r--   0 reinout    (501) staff       (20)     3208 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/ajax-loader.gif
--rw-r--r--   0 reinout    (501) staff       (20)      723 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/ajax-loader2.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1849 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/ajax-loader3.gif
--rw-r--r--   0 reinout    (501) staff       (20)     2545 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/ajax-loader4.gif
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/
--rw-r--r--   0 reinout    (501) staff       (20)     3718 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/3di.png
--rw-r--r--   0 reinout    (501) staff       (20)     7306 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/alkmaar.png
--rw-r--r--   0 reinout    (501) staff       (20)     2811 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/almere.png
--rw-r--r--   0 reinout    (501) staff       (20)     3948 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/appicon_eleaf.png
--rw-r--r--   0 reinout    (501) staff       (20)     3457 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/appicon_knmi.png
--rw-r--r--   0 reinout    (501) staff       (20)     3694 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/appicon_neo.png
--rw-r--r--   0 reinout    (501) staff       (20)     3665 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/appicon_pwn.png
--rw-r--r--   0 reinout    (501) staff       (20)     4927 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/appicon_satapp.png
--rw-r--r--   0 reinout    (501) staff       (20)     7269 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/boek.png
--rw-r--r--   0 reinout    (501) staff       (20)     3825 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/ciw.png
--rw-r--r--   0 reinout    (501) staff       (20)     5848 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/controlnext.png
--rw-r--r--   0 reinout    (501) staff       (20)     4001 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/dacom.png
--rw-r--r--   0 reinout    (501) staff       (20)     6430 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/deltares.png
--rw-r--r--   0 reinout    (501) staff       (20)     3425 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/dike.png
--rw-r--r--   0 reinout    (501) staff       (20)     5693 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/download.png
--rw-r--r--   0 reinout    (501) staff       (20)     4740 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/download_grijs.png
--rw-r--r--   0 reinout    (501) staff       (20)     6136 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/drought.png
--rw-r--r--   0 reinout    (501) staff       (20)     3207 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/energieverbruik.png
--rw-r--r--   0 reinout    (501) staff       (20)     4231 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/floodapp.png
--rw-r--r--   0 reinout    (501) staff       (20)     4194 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/flooding.png
--rw-r--r--   0 reinout    (501) staff       (20)     3802 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/flooding2.png
--rw-r--r--   0 reinout    (501) staff       (20)     6488 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/gisflow.png
--rw-r--r--   0 reinout    (501) staff       (20)     7098 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/grondwater.png
--rw-r--r--   0 reinout    (501) staff       (20)     5949 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/hdsr.png
--rw-r--r--   0 reinout    (501) staff       (20)     5474 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/history.png
--rw-r--r--   0 reinout    (501) staff       (20)     4478 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/kaartlagen.png
--rw-r--r--   0 reinout    (501) staff       (20)     3881 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/keringen.png
--rw-r--r--   0 reinout    (501) staff       (20)     4816 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/kpi.png
--rw-r--r--   0 reinout    (501) staff       (20)     5623 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/kustviewer.png
--rw-r--r--   0 reinout    (501) staff       (20)     6110 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/kwantiteit.png
--rw-r--r--   0 reinout    (501) staff       (20)     4110 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/lcms.png
--rw-r--r--   0 reinout    (501) staff       (20)     6125 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/leveeportal.png
--rw-r--r--   0 reinout    (501) staff       (20)     6178 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/lizard.png
--rw-r--r--   0 reinout    (501) staff       (20)     6220 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/lizard_alarm.png
--rw-r--r--   0 reinout    (501) staff       (20)     6146 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/maatregelen.png
--rw-r--r--   0 reinout    (501) staff       (20)     3200 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/meetgegevens.png
--rw-r--r--   0 reinout    (501) staff       (20)     4135 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/modelresultaten.png
--rw-r--r--   0 reinout    (501) staff       (20)     5010 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/narrowcasting.png
--rw-r--r--   0 reinout    (501) staff       (20)     3038 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/neerslag.png
--rw-r--r--   0 reinout    (501) staff       (20)     5789 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/nhi.png
--rw-r--r--   0 reinout    (501) staff       (20)     6598 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/nieuwe_kaart_van_nederland.png
--rw-r--r--   0 reinout    (501) staff       (20)     6869 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/noorderpark.png
--rw-r--r--   0 reinout    (501) staff       (20)     2688 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/oevers.png
--rw-r--r--   0 reinout    (501) staff       (20)     5547 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/oppervlaktewater.png
--rw-r--r--   0 reinout    (501) staff       (20)     5116 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/peilschaal.png
--rw-r--r--   0 reinout    (501) staff       (20)     6945 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/planning.png
--rw-r--r--   0 reinout    (501) staff       (20)     3182 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/play.png
--rw-r--r--   0 reinout    (501) staff       (20)     6512 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/projecten.png
--rw-r--r--   0 reinout    (501) staff       (20)     3360 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/RegimeApp.png
--rw-r--r--   0 reinout    (501) staff       (20)     6853 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/riolering.png
--rw-r--r--   0 reinout    (501) staff       (20)     6941 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/rws.png
--rw-r--r--   0 reinout    (501) staff       (20)     5770 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/statistiek.png
--rw-r--r--   0 reinout    (501) staff       (20)     4110 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/statusoverzicht.png
--rw-r--r--   0 reinout    (501) staff       (20)     6066 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/sticky.png
--rw-r--r--   0 reinout    (501) staff       (20)     5910 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/stowa.png
--rw-r--r--   0 reinout    (501) staff       (20)     3789 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/telecontrolnet.png
--rw-r--r--   0 reinout    (501) staff       (20)     4518 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/turtle.png
--rw-r--r--   0 reinout    (501) staff       (20)     5546 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/twitter.png
--rw-r--r--   0 reinout    (501) staff       (20)     5656 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/upload.png
--rw-r--r--   0 reinout    (501) staff       (20)     4618 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/upload_grijs.png
--rw-r--r--   0 reinout    (501) staff       (20)     6318 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/uploadserver.png
--rw-r--r--   0 reinout    (501) staff       (20)     4023 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/urk.png
--rw-r--r--   0 reinout    (501) staff       (20)     4602 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/VerlorenBerging.png
--rw-r--r--   0 reinout    (501) staff       (20)     6855 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/vss.png
--rw-r--r--   0 reinout    (501) staff       (20)     3360 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/waterbalance.png
--rw-r--r--   0 reinout    (501) staff       (20)     6465 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/waterkwaliteit.png
--rw-r--r--   0 reinout    (501) staff       (20)     6012 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/WIT.png
--rw-r--r--   0 reinout    (501) staff       (20)     4465 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/wms.png
--rw-r--r--   0 reinout    (501) staff       (20)     6696 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/workspace_metingen.png
--rw-r--r--   0 reinout    (501) staff       (20)     6680 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/workspace_neerslag.png
--rw-r--r--   0 reinout    (501) staff       (20)     6474 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/workspace_oppervlaktewater.png
--rw-r--r--   0 reinout    (501) staff       (20)     7505 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/workspace_riolering.png
--rw-r--r--   0 reinout    (501) staff       (20)     7539 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/workspace_wateropstraat.png
--rw-r--r--   0 reinout    (501) staff       (20)     6528 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/zettingen.png
--rw-r--r--   0 reinout    (501) staff       (20)     3728 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/zuiderzeeland.png
--rw-r--r--   0 reinout    (501) staff       (20)      153 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/arrow_collapse.png
--rw-r--r--   0 reinout    (501) staff       (20)      155 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/arrow_expand.png
--rw-r--r--   0 reinout    (501) staff       (20)      336 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/arrows.png
--rw-r--r--   0 reinout    (501) staff       (20)      598 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/background.png
--rw-r--r--   0 reinout    (501) staff       (20)      157 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/bar_background copy.png
--rw-r--r--   0 reinout    (501) staff       (20)     1273 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/bar_background.png
--rw-r--r--   0 reinout    (501) staff       (20)     1636 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/box-awesome.css
--rw-r--r--   0 reinout    (501) staff       (20)    28711 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/buttons.css
--rw-r--r--   0 reinout    (501) staff       (20)      142 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/carbon_fibre.png
--rw-r--r--   0 reinout    (501) staff       (20)     1996 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/close.png
--rw-r--r--   0 reinout    (501) staff       (20)     1946 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/csrf.js
--rw-r--r--   0 reinout    (501) staff       (20)   102370 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/fabric_1.png
--rw-r--r--   0 reinout    (501) staff       (20)     1406 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/favicon.ico
--rw-r--r--   0 reinout    (501) staff       (20)     2089 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/icon-chart.png
--rw-r--r--   0 reinout    (501) staff       (20)      980 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/icon-legend.png
--rw-r--r--   0 reinout    (501) staff       (20)    77720 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/leather_1.png
--rw-r--r--   0 reinout    (501) staff       (20)    17387 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/lizard_ui.js
--rw-r--r--   0 reinout    (501) staff       (20)     3749 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/logo.png
--rw-r--r--   0 reinout    (501) staff       (20)    48689 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/old_mathematics.png
--rw-r--r--   0 reinout    (501) staff       (20)    10726 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/OpenLayers.Control.NensLayerSwitcher.js
--rw-r--r--   0 reinout    (501) staff       (20)      863 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/print.css
--rw-r--r--   0 reinout    (501) staff       (20)      140 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/small_bar_background.png
--rw-r--r--   0 reinout    (501) staff       (20)      916 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/tabs.css
--rw-r--r--   0 reinout    (501) staff       (20)      133 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/lizard_ui/white_carbon.png
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/momentjs/
--rw-r--r--   0 reinout    (501) staff       (20)    36776 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/momentjs/moment.js
--rw-r--r--   0 reinout    (501) staff       (20)    11484 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/momentjs/moment.min.js
--rw-r--r--   0 reinout    (501) staff       (20)     2395 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/momentjs/nl.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/
--rwxr-xr-x   0 reinout    (501) staff       (20)     1285 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/authors.txt
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/
--rw-r--r--   0 reinout    (501) staff       (20)       42 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/blank.gif
--rw-r--r--   0 reinout    (501) staff       (20)     4067 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/cloud-popup-relative.png
--rw-r--r--   0 reinout    (501) staff       (20)     1024 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/drag-rectangle-off.png
--rw-r--r--   0 reinout    (501) staff       (20)     1041 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/drag-rectangle-on.png
--rw-r--r--   0 reinout    (501) staff       (20)      298 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/east-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)      303 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/layer-switcher-maximize.png
--rw-r--r--   0 reinout    (501) staff       (20)      367 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/layer-switcher-minimize.png
--rw-r--r--   0 reinout    (501) staff       (20)      758 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/marker-blue.png
--rw-r--r--   0 reinout    (501) staff       (20)      703 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/marker-gold.png
--rw-r--r--   0 reinout    (501) staff       (20)      753 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/marker-green.png
--rw-r--r--   0 reinout    (501) staff       (20)      601 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/marker.png
--rw-r--r--   0 reinout    (501) staff       (20)     3028 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/measuring-stick-off.png
--rw-r--r--   0 reinout    (501) staff       (20)     3725 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/measuring-stick-on.png
--rw-r--r--   0 reinout    (501) staff       (20)      298 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/north-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)     3511 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/panning-hand-off.png
--rw-r--r--   0 reinout    (501) staff       (20)     3565 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/panning-hand-on.png
--rw-r--r--   0 reinout    (501) staff       (20)      236 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/slider.png
--rw-r--r--   0 reinout    (501) staff       (20)      310 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/south-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)      299 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/west-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)      229 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/zoom-minus-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)      276 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/zoom-plus-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)      545 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/zoom-world-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)      232 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/zoombar.png
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/
--rwxr-xr-x   0 reinout    (501) staff       (20)   175037 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/deprecated.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/
--rwxr-xr-x   0 reinout    (501) staff       (20)      457 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/errorIcon.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     3480 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebug.css
--rwxr-xr-x   0 reinout    (501) staff       (20)      651 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebug.html
--rwxr-xr-x   0 reinout    (501) staff       (20)    19181 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebug.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      384 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebugx.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      524 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/infoIcon.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1561 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/license.txt
--rwxr-xr-x   0 reinout    (501) staff       (20)      545 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/readme.txt
--rwxr-xr-x   0 reinout    (501) staff       (20)      516 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/warningIcon.png
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/
--rwxr-xr-x   0 reinout    (501) staff       (20)     3633 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Animation.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/
--rwxr-xr-x   0 reinout    (501) staff       (20)    25310 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Bounds.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3740 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Class.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5071 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Date.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5398 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Element.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6425 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/LonLat.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3649 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Pixel.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2191 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Size.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    13356 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7885 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Console.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/
--rwxr-xr-x   0 reinout    (501) staff       (20)     5908 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ArgParser.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3155 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Attribution.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1217 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Button.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5044 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/CacheRead.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     8033 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/CacheWrite.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    11478 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/DragFeature.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4416 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/DragPan.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7217 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/DrawFeature.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2771 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/EditingToolbar.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5376 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Geolocate.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    20030 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/GetFeature.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    14041 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Graticule.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4399 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/KeyboardDefaults.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    17640 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/LayerSwitcher.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    11790 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Measure.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    31212 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ModifyFeature.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4960 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/MousePosition.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     9585 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Navigation.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    13519 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/NavigationHistory.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1836 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/NavToolbar.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    25888 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/OverviewMap.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3270 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Pan.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    14528 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Panel.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2578 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PanPanel.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6681 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PanZoom.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    12487 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PanZoomBar.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     8122 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Permalink.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6646 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PinchZoom.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2856 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Scale.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6670 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ScaleLine.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    20556 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/SelectFeature.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    21423 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/SLDSelect.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    21409 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Snapping.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    19587 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Split.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5219 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/TouchNavigation.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    23368 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/TransformFeature.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6984 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/UTFGrid.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    18600 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/WMSGetFeatureInfo.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    13067 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/WMTSGetFeatureInfo.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4142 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Zoom.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3811 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomBox.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      937 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomIn.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      942 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomOut.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1817 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomPanel.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1126 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomToMaxExtent.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    11237 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Events/
--rwxr-xr-x   0 reinout    (501) staff       (20)     5945 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Events/buttonclick.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    31565 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Events.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Feature/
--rwxr-xr-x   0 reinout    (501) staff       (20)    18603 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Feature/Vector.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6505 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Feature.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/
--rwxr-xr-x   0 reinout    (501) staff       (20)     9330 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Comparison.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2341 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/FeatureId.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1320 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Function.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3424 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Logical.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3523 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Spatial.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2279 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/ArcXML/
--rwxr-xr-x   0 reinout    (501) staff       (20)     1430 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/ArcXML/Features.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    40703 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/ArcXML.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    23184 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Atom.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    11931 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Context.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    16333 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CQL.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetDomain/
--rwxr-xr-x   0 reinout    (501) staff       (20)     8222 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetDomain/v2_0_2.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      992 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetDomain.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetRecords/
--rwxr-xr-x   0 reinout    (501) staff       (20)    16614 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetRecords/v2_0_2.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1000 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetRecords.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/
--rwxr-xr-x   0 reinout    (501) staff       (20)    18804 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/v1.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7390 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/v1_0_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     8704 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/v1_1_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1505 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    24949 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GeoJSON.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    14717 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GeoRSS.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/
--rwxr-xr-x   0 reinout    (501) staff       (20)    24742 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/Base.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7439 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/v2.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    18906 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/v3.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    35433 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    12944 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GPX.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    13212 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/JSON.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    55468 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/KML.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3427 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OGCExceptionReport.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    16106 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OSM.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/
--rwxr-xr-x   0 reinout    (501) staff       (20)    12883 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/v1.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2061 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/v1_0_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4249 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/v1_1_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2415 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSContext/
--rwxr-xr-x   0 reinout    (501) staff       (20)    23703 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSContext/v0_3_1.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2691 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSContext.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6971 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/QueryStringFilter.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/
--rwxr-xr-x   0 reinout    (501) staff       (20)    52979 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/v1.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1305 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/v1_0_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5438 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/v1_0_0_GeoServer.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2321 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSCapabilities/
--rwxr-xr-x   0 reinout    (501) staff       (20)     5680 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSCapabilities/v1_0_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1345 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSCapabilities.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6397 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSGetFeatureOfInterest.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    11307 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSGetObservation.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6597 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Text.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7036 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WCSGetCoverage.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7716 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFS.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/
--rwxr-xr-x   0 reinout    (501) staff       (20)     3724 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/v1.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4360 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/v1_0_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2024 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/v1_1_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1646 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6993 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSDescribeFeatureType.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/
--rwxr-xr-x   0 reinout    (501) staff       (20)    16316 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/v1.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6988 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/v1_0_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7931 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/v1_1_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      996 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    14807 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WKT.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/
--rwxr-xr-x   0 reinout    (501) staff       (20)    38512 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/v1.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3097 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/v1_0_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4538 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/v1_1_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6353 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/
--rwxr-xr-x   0 reinout    (501) staff       (20)    14702 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5037 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1845 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1677 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1_1.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2982 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1_1_WMSC.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5893 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_3.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      951 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_3_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1514 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSDescribeLayer/
--rwxr-xr-x   0 reinout    (501) staff       (20)     3757 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSDescribeLayer/v1_1.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2353 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSDescribeLayer.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     9782 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSGetFeatureInfo.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMTSCapabilities/
--rwxr-xr-x   0 reinout    (501) staff       (20)     9301 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMTSCapabilities/v1_0_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4352 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMTSCapabilities.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSCapabilities/
--rwxr-xr-x   0 reinout    (501) staff       (20)     3945 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSCapabilities/v1_0_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1306 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSCapabilities.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6276 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSDescribeProcess.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     9602 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSExecute.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS/
--rwxr-xr-x   0 reinout    (501) staff       (20)    11114 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS/v1.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1360 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS/v1_1_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1970 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XML/
--rwxr-xr-x   0 reinout    (501) staff       (20)     5696 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XML/VersionedOGC.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    31465 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XML.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3904 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/
--rwxr-xr-x   0 reinout    (501) staff       (20)    18626 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Collection.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2952 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Curve.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    14975 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/LinearRing.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    25718 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/LineString.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    10486 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/MultiLineString.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1913 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/MultiPoint.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1355 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/MultiPolygon.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     8912 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Point.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     9394 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Polygon.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    15685 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/
--rwxr-xr-x   0 reinout    (501) staff       (20)     7721 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Box.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    17540 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Click.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    16375 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Drag.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    14095 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Feature.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5076 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Hover.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3660 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Keyboard.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     9528 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/MouseWheel.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    16921 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Path.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6304 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Pinch.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    16306 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Point.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    10643 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Polygon.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    14706 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/RegularPolygon.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     9461 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6817 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Icon.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4700 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Kinetic.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/
--rwxr-xr-x   0 reinout    (501) staff       (20)      662 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ar.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4500 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/be-tarask.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      757 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/bg.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3153 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/br.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3633 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ca.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2997 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/cs-CZ.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3397 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/da-DK.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3509 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/de.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      491 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/el.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      670 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/en-CA.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3576 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/en.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3709 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/es.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      568 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/fi.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3440 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/fr.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      767 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/fur.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3262 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/gl.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3166 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/gsw.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1060 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/hr.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3161 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/hsb.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3526 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/hu.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3143 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ia.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3129 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/id.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      465 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/io.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      710 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/is.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3512 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/it.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3875 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ja.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      678 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/km.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3968 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ksh.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1267 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/lt.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3342 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nb.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1119 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nds.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3239 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nl.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      486 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nn.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3163 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/oc.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3923 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/pl.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3430 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/pt-BR.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3259 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/pt.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4515 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ru.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3203 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/sk.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3056 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/sv-SE.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      538 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/te.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3340 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/vi.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3129 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/zh-CN.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3153 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/zh-TW.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4268 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/
--rwxr-xr-x   0 reinout    (501) staff       (20)     7956 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/ArcGIS93Rest.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    18984 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/ArcGISCache.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    14638 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/ArcIMS.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    10513 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Bing.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2111 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Boxes.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    14272 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/EventPane.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    12249 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/FixedZoomLevels.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     8593 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/GeoRSS.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Google/
--rwxr-xr-x   0 reinout    (501) staff       (20)    16330 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Google/v3.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    24682 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Google.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    47032 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Grid.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7191 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/HTTPRequest.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7832 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Image.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6009 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/KaMap.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4875 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/KaMapCache.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    18252 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/MapGuide.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6713 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/MapServer.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4920 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Markers.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3922 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/OSM.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    10022 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/PointGrid.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4459 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/PointTrack.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5103 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/SphericalMercator.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     9613 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Text.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5786 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/TileCache.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7441 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/TMS.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5425 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/UTFGrid.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Vector/
--rwxr-xr-x   0 reinout    (501) staff       (20)     4709 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Vector/RootContainer.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    34709 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Vector.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     9926 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/WMS.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    18357 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/WMTS.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2948 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/WorldWind.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5776 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/XYZ.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     9399 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Zoomify.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    46776 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    93493 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Map.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Marker/
--rwxr-xr-x   0 reinout    (501) staff       (20)     2794 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Marker/Box.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6315 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Marker.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/
--rwxr-xr-x   0 reinout    (501) staff       (20)     6530 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/Anchored.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     5576 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/AnchoredBubble.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    11967 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/Framed.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     8380 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/FramedCloud.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    35284 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    10970 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Projection.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/CSW/
--rwxr-xr-x   0 reinout    (501) staff       (20)     4004 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/CSW/v2_0_2.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      871 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/CSW.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    20226 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/HTTP.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    13112 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/Script.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/SOS/
--rwxr-xr-x   0 reinout    (501) staff       (20)     4244 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/SOS/v1_0_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      956 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/SOS.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/
--rwxr-xr-x   0 reinout    (501) staff       (20)    15122 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/v1.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1481 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/v1_0_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2689 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/v1_1_0.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2834 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     8408 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/
--rwxr-xr-x   0 reinout    (501) staff       (20)    33022 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/Canvas.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    34381 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/Elements.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    34784 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/SVG.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    33790 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/VML.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    13322 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Request/
--rwxr-xr-x   0 reinout    (501) staff       (20)    17370 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Request/XMLHttpRequest.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    16643 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Request.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7377 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Rule.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2741 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/SingleFile.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2631 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Spherical.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/
--rwxr-xr-x   0 reinout    (501) staff       (20)     9419 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/BBOX.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     8958 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Cluster.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4979 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Filter.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3985 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Fixed.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6316 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Paging.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3610 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Refresh.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7481 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Save.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3157 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    14798 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Style.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2912 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Style2.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     6263 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/StyleMap.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/
--rwxr-xr-x   0 reinout    (501) staff       (20)     2260 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Line.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     4815 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Point.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     2659 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Polygon.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1020 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Raster.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1947 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Text.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1556 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/Image/
--rwxr-xr-x   0 reinout    (501) staff       (20)     8150 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/Image/IFrame.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    16449 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/Image.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     7418 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/UTFGrid.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     8951 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     8083 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tween.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    59252 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Util.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    18871 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Rico/
--rwxr-xr-x   0 reinout    (501) staff       (20)     6679 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Rico/Color.js
--rwxr-xr-x   0 reinout    (501) staff       (20)    11895 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Rico/Corner.js
--rwxr-xr-x   0 reinout    (501) staff       (20)      696 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Rico/license.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     1537 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/license.txt
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/licenses/
--rwxr-xr-x   0 reinout    (501) staff       (20)    11358 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/licenses/APACHE-2.0.txt
--rwxr-xr-x   0 reinout    (501) staff       (20)     1462 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/licenses/BSD-LICENSE.txt
--rwxr-xr-x   0 reinout    (501) staff       (20)     1023 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/licenses/MIT-LICENSE.txt
--rwxr-xr-x   0 reinout    (501) staff       (20)  2823171 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/OpenLayers.debug.js
--rwxr-xr-x   0 reinout    (501) staff       (20)   739729 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/OpenLayers.js
--rwxr-xr-x   0 reinout    (501) staff       (20)  1225156 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/OpenLayers.light.debug.js
--rwxr-xr-x   0 reinout    (501) staff       (20)   287078 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/OpenLayers.light.js
--rwxr-xr-x   0 reinout    (501) staff       (20)  1388259 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/OpenLayers.mobile.debug.js
--rwxr-xr-x   0 reinout    (501) staff       (20)   332603 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/OpenLayers.mobile.js
--rwxr-xr-x   0 reinout    (501) staff       (20)     3407 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/readme.md
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/
--rwxr-xr-x   0 reinout    (501) staff       (20)      303 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/google.css
--rwxr-xr-x   0 reinout    (501) staff       (20)      229 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/google.tidy.css
--rwxr-xr-x   0 reinout    (501) staff       (20)      212 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/ie6-style.css
--rwxr-xr-x   0 reinout    (501) staff       (20)      184 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/ie6-style.tidy.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/
--rwxr-xr-x   0 reinout    (501) staff       (20)     1614 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/add_point_off.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1464 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/add_point_on.png
--rwxr-xr-x   0 reinout    (501) staff       (20)       42 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/blank.gif
--rwxr-xr-x   0 reinout    (501) staff       (20)     1078 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/close.gif
--rwxr-xr-x   0 reinout    (501) staff       (20)     1024 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/drag-rectangle-off.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1041 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/drag-rectangle-on.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1565 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_line_off.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1396 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_line_on.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1610 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_point_off.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1458 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_point_on.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1544 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_polygon_off.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1405 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_polygon_on.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     2222 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/editing_tool_bar.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1541 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/move_feature_off.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1377 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/move_feature_on.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     6628 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/navigation_history.png
--rwxr-xr-x   0 reinout    (501) staff       (20)       79 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/overview_replacement.gif
--rwxr-xr-x   0 reinout    (501) staff       (20)      564 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan-panel-NOALPHA.png
--rwxr-xr-x   0 reinout    (501) staff       (20)      814 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan-panel.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1696 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan_off.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1566 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan_on.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     3511 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/panning-hand-off.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     3565 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/panning-hand-on.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1612 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/remove_point_off.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1461 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/remove_point_on.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1211 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/ruler.png
--rwxr-xr-x   0 reinout    (501) staff       (20)      354 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/save_features_off.png
--rwxr-xr-x   0 reinout    (501) staff       (20)      361 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/save_features_on.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1499 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_next_off.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1686 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_next_on.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1476 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_previous_off.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1592 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_previous_on.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1173 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/zoom-panel-NOALPHA.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     1285 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/zoom-panel.png
--rwxr-xr-x   0 reinout    (501) staff       (20)     9948 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/style.css
--rwxr-xr-x   0 reinout    (501) staff       (20)     1688 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/style.mobile.css
--rwxr-xr-x   0 reinout    (501) staff       (20)      970 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/style.mobile.tidy.css
--rwxr-xr-x   0 reinout    (501) staff       (20)     7547 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/style.tidy.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/
--rwxr-xr-x   0 reinout    (501) staff       (20)    69566 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/BeautifulSoup.py
--rwxr-xr-x   0 reinout    (501) staff       (20)     2337 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/closure_library_jscompiler.py
--rwxr-xr-x   0 reinout    (501) staff       (20)      861 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/closure_ws.py
--rwxr-xr-x   0 reinout    (501) staff       (20)     8324 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/exampleparser.py
--rwxr-xr-x   0 reinout    (501) staff       (20)     7006 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/jsmin.c
--rwxr-xr-x   0 reinout    (501) staff       (20)     7471 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/jsmin.py
--rwxr-xr-x   0 reinout    (501) staff       (20)     8955 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/mergejs.py
--rwxr-xr-x   0 reinout    (501) staff       (20)     2088 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/minimize.py
--rwxr-xr-x   0 reinout    (501) staff       (20)     1359 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/oldot.py
--rwxr-xr-x   0 reinout    (501) staff       (20)      643 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/README.txt
--rwxr-xr-x   0 reinout    (501) staff       (20)     1487 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/release.sh
--rwxr-xr-x   0 reinout    (501) staff       (20)     1498 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/shrinksafe.py
--rwxr-xr-x   0 reinout    (501) staff       (20)     1086 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/toposort.py
--rwxr-xr-x   0 reinout    (501) staff       (20)     2519 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/update_dev_dir.sh
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/
--rw-r--r--   0 reinout    (501) staff       (20)   180452 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/deprecated.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/
--rw-r--r--   0 reinout    (501) staff       (20)       42 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/blank.gif
--rw-r--r--   0 reinout    (501) staff       (20)     4067 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/cloud-popup-relative.png
--rw-r--r--   0 reinout    (501) staff       (20)     1024 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/drag-rectangle-off.png
--rw-r--r--   0 reinout    (501) staff       (20)     1041 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/drag-rectangle-on.png
--rw-r--r--   0 reinout    (501) staff       (20)      298 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/east-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)      303 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/layer-switcher-maximize.png
--rw-r--r--   0 reinout    (501) staff       (20)      367 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/layer-switcher-minimize.png
--rw-r--r--   0 reinout    (501) staff       (20)      758 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/marker-blue.png
--rw-r--r--   0 reinout    (501) staff       (20)      703 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/marker-gold.png
--rw-r--r--   0 reinout    (501) staff       (20)      753 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/marker-green.png
--rw-r--r--   0 reinout    (501) staff       (20)      601 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/marker.png
--rw-r--r--   0 reinout    (501) staff       (20)     3028 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/measuring-stick-off.png
--rw-r--r--   0 reinout    (501) staff       (20)     3725 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/measuring-stick-on.png
--rw-r--r--   0 reinout    (501) staff       (20)      298 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/north-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)     3511 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/panning-hand-off.png
--rw-r--r--   0 reinout    (501) staff       (20)     3565 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/panning-hand-on.png
--rw-r--r--   0 reinout    (501) staff       (20)      236 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/slider.png
--rw-r--r--   0 reinout    (501) staff       (20)      310 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/south-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)      299 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/west-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)      229 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/zoom-minus-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)      276 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/zoom-plus-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)      545 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/zoom-world-mini.png
--rw-r--r--   0 reinout    (501) staff       (20)      232 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/zoombar.png
--rw-r--r--   0 reinout    (501) staff       (20)   770256 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/OpenLayers.js
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/
--rw-r--r--   0 reinout    (501) staff       (20)      142 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/google.css
--rw-r--r--   0 reinout    (501) staff       (20)      212 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/ie6-style.css
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/
--rw-r--r--   0 reinout    (501) staff       (20)     1614 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/add_point_off.png
--rw-r--r--   0 reinout    (501) staff       (20)     1464 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/add_point_on.png
--rw-r--r--   0 reinout    (501) staff       (20)       42 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/blank.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1078 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/close.gif
--rw-r--r--   0 reinout    (501) staff       (20)     1024 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/drag-rectangle-off.png
--rw-r--r--   0 reinout    (501) staff       (20)     1041 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/drag-rectangle-on.png
--rw-r--r--   0 reinout    (501) staff       (20)     1565 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_line_off.png
--rw-r--r--   0 reinout    (501) staff       (20)     1396 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_line_on.png
--rw-r--r--   0 reinout    (501) staff       (20)     1610 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_point_off.png
--rw-r--r--   0 reinout    (501) staff       (20)     1458 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_point_on.png
--rw-r--r--   0 reinout    (501) staff       (20)     1544 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_polygon_off.png
--rw-r--r--   0 reinout    (501) staff       (20)     1405 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_polygon_on.png
--rw-r--r--   0 reinout    (501) staff       (20)     2222 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/editing_tool_bar.png
--rw-r--r--   0 reinout    (501) staff       (20)     1541 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/move_feature_off.png
--rw-r--r--   0 reinout    (501) staff       (20)     1377 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/move_feature_on.png
--rw-r--r--   0 reinout    (501) staff       (20)     6628 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/navigation_history.png
--rw-r--r--   0 reinout    (501) staff       (20)       79 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/overview_replacement.gif
--rw-r--r--   0 reinout    (501) staff       (20)      564 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan-panel-NOALPHA.png
--rw-r--r--   0 reinout    (501) staff       (20)      814 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan-panel.png
--rw-r--r--   0 reinout    (501) staff       (20)     1696 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan_off.png
--rw-r--r--   0 reinout    (501) staff       (20)     1566 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan_on.png
--rw-r--r--   0 reinout    (501) staff       (20)     3511 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/panning-hand-off.png
--rw-r--r--   0 reinout    (501) staff       (20)     3565 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/panning-hand-on.png
--rw-r--r--   0 reinout    (501) staff       (20)     1612 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/remove_point_off.png
--rw-r--r--   0 reinout    (501) staff       (20)     1461 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/remove_point_on.png
--rw-r--r--   0 reinout    (501) staff       (20)     1211 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/ruler.png
--rw-r--r--   0 reinout    (501) staff       (20)      354 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/save_features_off.png
--rw-r--r--   0 reinout    (501) staff       (20)      361 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/save_features_on.png
--rw-r--r--   0 reinout    (501) staff       (20)     1499 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_next_off.png
--rw-r--r--   0 reinout    (501) staff       (20)     1686 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_next_on.png
--rw-r--r--   0 reinout    (501) staff       (20)     1476 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_previous_off.png
--rw-r--r--   0 reinout    (501) staff       (20)     1592 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_previous_on.png
--rw-r--r--   0 reinout    (501) staff       (20)     1173 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/zoom-panel-NOALPHA.png
--rw-r--r--   0 reinout    (501) staff       (20)     1285 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/zoom-panel.png
--rw-r--r--   0 reinout    (501) staff       (20)    10791 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/style.css
--rw-r--r--   0 reinout    (501) staff       (20)     1799 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/style.mobile.css
--rw-r--r--   0 reinout    (501) staff       (20)     1263 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/README.blueprint
--rw-r--r--   0 reinout    (501) staff       (20)     1738 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/README.bootstrap
--rw-r--r--   0 reinout    (501) staff       (20)      197 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/README.colorpicker
--rw-r--r--   0 reinout    (501) staff       (20)    18093 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/README.datatables
--rw-r--r--   0 reinout    (501) staff       (20)      311 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/README.daterangepicker.txt
--rw-r--r--   0 reinout    (501) staff       (20)      285 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/README.jquery
--rw-r--r--   0 reinout    (501) staff       (20)      802 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/README.jqueryui
--rw-r--r--   0 reinout    (501) staff       (20)       56 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/README.less
--rw-r--r--   0 reinout    (501) staff       (20)      272 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/README.openlayers
--rw-r--r--   0 reinout    (501) staff       (20)      137 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/README.sprites
--rw-r--r--   0 reinout    (501) staff       (20)      436 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/README.treeview
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/static/sprites/
--rw-r--r--   0 reinout    (501) staff       (20)     3223 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/calendar-light.png
--rw-r--r--   0 reinout    (501) staff       (20)     3084 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/calendar.png
--rw-r--r--   0 reinout    (501) staff       (20)     3200 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/clock-light.png
--rw-r--r--   0 reinout    (501) staff       (20)     3090 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/compass.png
--rw-r--r--   0 reinout    (501) staff       (20)     1410 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/direction.png
--rw-r--r--   0 reinout    (501) staff       (20)     1351 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/left_arrow.png
--rw-r--r--   0 reinout    (501) staff       (20)     1403 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/link.png
--rw-r--r--   0 reinout    (501) staff       (20)     3205 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/location-light.png
--rw-r--r--   0 reinout    (501) staff       (20)     3131 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/marker-light.png
--rw-r--r--   0 reinout    (501) staff       (20)     3005 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/marker.png
--rw-r--r--   0 reinout    (501) staff       (20)     1253 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/read_it_later.png
--rwxr-xr-x   0 reinout    (501) staff       (20)    49192 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/sprite.css
--rw-r--r--   0 reinout    (501) staff       (20)   250121 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/sprites copy.png
--rw-r--r--   0 reinout    (501) staff       (20)   294540 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/sprites.png
--rw-r--r--   0 reinout    (501) staff       (20)     3051 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/star-light.png
--rw-r--r--   0 reinout    (501) staff       (20)     1361 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/star.png
--rwxr-xr-x   0 reinout    (501) staff       (20)    79454 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/test.htm
--rw-r--r--   0 reinout    (501) staff       (20)     1184 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/trashbin-light.png
--rw-r--r--   0 reinout    (501) staff       (20)      308 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/static/sprites/warning.png
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/templates/
--rw-r--r--   0 reinout    (501) staff       (20)     1383 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/404.html
--rw-r--r--   0 reinout    (501) staff       (20)     1517 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/500.html
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/
--rw-r--r--   0 reinout    (501) staff       (20)     1605 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/change_language.html
--rw-r--r--   0 reinout    (501) staff       (20)     1380 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/cmsbase.html
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/
--rw-r--r--   0 reinout    (501) staff       (20)      569 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-appscreens.html
--rw-r--r--   0 reinout    (501) staff       (20)      756 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-blocks-view.html
--rw-r--r--   0 reinout    (501) staff       (20)     4475 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-blocks.html
--rw-r--r--   0 reinout    (501) staff       (20)      923 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-breadcrumbs.html
--rw-r--r--   0 reinout    (501) staff       (20)      342 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-cms-layout.html
--rw-r--r--   0 reinout    (501) staff       (20)     2329 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-images.html
--rw-r--r--   0 reinout    (501) staff       (20)     1167 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-portaltabs.html
--rw-r--r--   0 reinout    (501) staff       (20)      425 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-printbutton.html
--rw-r--r--   0 reinout    (501) staff       (20)     1118 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-table.html
--rw-r--r--   0 reinout    (501) staff       (20)      392 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-textual.html
--rw-r--r--   0 reinout    (501) staff       (20)     1949 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_accordion1.html
--rw-r--r--   0 reinout    (501) staff       (20)     1256 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_accordion2.html
--rw-r--r--   0 reinout    (501) staff       (20)     1101 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_accordion3.html
--rw-r--r--   0 reinout    (501) staff       (20)     2080 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_collapsible.html
--rw-r--r--   0 reinout    (501) staff       (20)    95353 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_icons.html
--rw-r--r--   0 reinout    (501) staff       (20)    30965 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_jqueryui.html
--rw-r--r--   0 reinout    (501) staff       (20)     1024 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_sidebarstretch.html
--rw-r--r--   0 reinout    (501) staff       (20)     1676 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_tree.html
--rw-r--r--   0 reinout    (501) staff       (20)     1131 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_vertical.html
--rw-r--r--   0 reinout    (501) staff       (20)     2936 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/lizard-ui-introduction.html
--rw-r--r--   0 reinout    (501) staff       (20)      648 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/icon_include.html
--rw-r--r--   0 reinout    (501) staff       (20)      132 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/icons.html
--rw-r--r--   0 reinout    (501) staff       (20)      289 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/lizardbase.html
--rw-r--r--   0 reinout    (501) staff       (20)     1342 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/login.html
--rw-r--r--   0 reinout    (501) staff       (20)     1637 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/modal_login.html
--rw-r--r--   0 reinout    (501) staff       (20)    16524 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/realbase.html
--rw-r--r--   0 reinout    (501) staff       (20)     1563 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templates/lizard_ui/tree_snippet.html
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:23.000000 lizard-ui-5.2/lizard_ui/templatetags/
--rw-r--r--   0 reinout    (501) staff       (20)        9 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templatetags/__init__.py
--rw-r--r--   0 reinout    (501) staff       (20)     4444 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/templatetags/utility.py
--rw-r--r--   0 reinout    (501) staff       (20)     6646 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/tests.py
--rw-r--r--   0 reinout    (501) staff       (20)     3181 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/testsettings.py
--rw-r--r--   0 reinout    (501) staff       (20)      514 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/uisettings.py
--rw-r--r--   0 reinout    (501) staff       (20)     4902 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/urls.py
--rw-r--r--   0 reinout    (501) staff       (20)    22825 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui/views.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui.egg-info/
--rw-r--r--   0 reinout    (501) staff       (20)        1 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui.egg-info/dependency_links.txt
--rw-r--r--   0 reinout    (501) staff       (20)       20 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui.egg-info/entry_points.txt
--rw-r--r--   0 reinout    (501) staff       (20)        1 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui.egg-info/not-zip-safe
--rw-r--r--   0 reinout    (501) staff       (20)    52111 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui.egg-info/PKG-INFO
--rw-r--r--   0 reinout    (501) staff       (20)      182 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui.egg-info/requires.txt
--rw-r--r--   0 reinout    (501) staff       (20)    62695 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui.egg-info/SOURCES.txt
--rw-r--r--   0 reinout    (501) staff       (20)       10 2015-10-08 12:07:22.000000 lizard-ui-5.2/lizard_ui.egg-info/top_level.txt
--rw-r--r--   0 reinout    (501) staff       (20)      105 2015-10-08 12:07:22.000000 lizard-ui-5.2/MANIFEST.in
--rw-r--r--   0 reinout    (501) staff       (20)    52111 2015-10-08 12:07:23.000000 lizard-ui-5.2/PKG-INFO
--rw-r--r--   0 reinout    (501) staff       (20)     9752 2015-10-08 12:07:22.000000 lizard-ui-5.2/README.rst
--rw-r--r--   0 reinout    (501) staff       (20)      228 2015-10-08 12:07:23.000000 lizard-ui-5.2/setup.cfg
--rw-r--r--   0 reinout    (501) staff       (20)     1313 2015-10-08 12:07:22.000000 lizard-ui-5.2/setup.py
--rw-r--r--   0 reinout    (501) staff       (20)      501 2015-10-08 12:07:22.000000 lizard-ui-5.2/TODO.rst
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/
+-rw-r--r--   0 reinout    (501) staff       (20)    28584 2015-10-08 14:24:02.000000 lizard-ui-5.3/CHANGES.rst
+-rw-r--r--   0 reinout    (501) staff       (20)       45 2015-10-08 14:24:02.000000 lizard-ui-5.3/CREDITS.rst
+-rw-r--r--   0 reinout    (501) staff       (20)     7651 2015-10-08 14:24:02.000000 lizard-ui-5.3/LICENSE.rst
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/
+-rw-r--r--   0 reinout    (501) staff       (20)        9 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)      822 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/admin.py
+-rw-r--r--   0 reinout    (501) staff       (20)     5212 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/configchecker.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/docs/
+-rw-r--r--   0 reinout    (501) staff       (20)      673 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/docs/__init__.html
+-rw-r--r--   0 reinout    (501) staff       (20)      357 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/docs/admin.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1974 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/docs/middleware.html
+-rw-r--r--   0 reinout    (501) staff       (20)     2884 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/docs/models.html
+-rw-r--r--   0 reinout    (501) staff       (20)     7008 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/docs/pycco.css
+-rw-r--r--   0 reinout    (501) staff       (20)     6786 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/docs/tests.html
+-rw-r--r--   0 reinout    (501) staff       (20)     9633 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/docs/testsettings.html
+-rw-r--r--   0 reinout    (501) staff       (20)     8682 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/docs/urls.html
+-rw-r--r--   0 reinout    (501) staff       (20)     8233 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/docs/views.html
+-rw-r--r--   0 reinout    (501) staff       (20)      690 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/forms.py
+-rw-r--r--   0 reinout    (501) staff       (20)     1421 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/layout.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/locale/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/locale/af/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/locale/af/LC_MESSAGES/
+-rw-r--r--   0 reinout    (501) staff       (20)     2013 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/af/LC_MESSAGES/django.mo
+-rw-r--r--   0 reinout    (501) staff       (20)     4238 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/af/LC_MESSAGES/django.po
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/locale/ar/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 reinout    (501) staff       (20)      646 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 reinout    (501) staff       (20)     3802 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0 reinout    (501) staff       (20)      906 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/locale/en/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/locale/en/LC_MESSAGES/
+-rw-r--r--   0 reinout    (501) staff       (20)      413 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 reinout    (501) staff       (20)     3572 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 reinout    (501) staff       (20)      378 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 reinout    (501) staff       (20)      764 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/locale/nl/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 reinout    (501) staff       (20)     2908 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 reinout    (501) staff       (20)     4579 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0 reinout    (501) staff       (20)      645 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/nl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 reinout    (501) staff       (20)     1005 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/nl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/locale/vi/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 reinout    (501) staff       (20)      538 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 reinout    (501) staff       (20)     3772 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/locale/zh/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 reinout    (501) staff       (20)     1912 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 reinout    (501) staff       (20)     4114 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/management/
+-rw-r--r--   0 reinout    (501) staff       (20)       10 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/management/__init__.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/management/commands/
+-rw-r--r--   0 reinout    (501) staff       (20)       10 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/management/commands/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)      474 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/management/commands/check_config.py
+-rw-r--r--   0 reinout    (501) staff       (20)     1476 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/management/commands/i18n.py
+-rw-r--r--   0 reinout    (501) staff       (20)      485 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/middleware.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/migrations/
+-rw-r--r--   0 reinout    (501) staff       (20)     2882 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/migrations/0001_initial.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2588 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/migrations/0002_auto__chg_field_applicationscreen_description__chg_field_applicationic.py
+-rw-r--r--   0 reinout    (501) staff       (20)     1949 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/migrations/0003_adding_description_field.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2233 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/migrations/0004_auto__add_field_applicationicon_sub_screen.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2637 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/migrations/0005_auto__chg_field_applicationicon_sub_screen__add_unique_applicationicon.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2802 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/migrations/0006_auto__add_field_applicationicon_data_set.py
+-rw-r--r--   0 reinout    (501) staff       (20)     3440 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/migrations/0007_auto__add_customerlogo.py
+-rw-r--r--   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/migrations/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)     5849 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/models.py
+-rw-r--r--   0 reinout    (501) staff       (20)      250 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/multitenancy.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2966 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/settingshelper.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/blueprint/
+-rw-r--r--   0 reinout    (501) staff       (20)     1861 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/ie.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/buttons/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/buttons/icons/
+-rwxr-xr-x   0 reinout    (501) staff       (20)      655 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/buttons/icons/cross.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)      455 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/buttons/icons/key.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)      537 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/buttons/icons/tick.png
+-rw-r--r--   0 reinout    (501) staff       (20)      930 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/buttons/readme.txt
+-rw-r--r--   0 reinout    (501) staff       (20)     2004 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/buttons/screen.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/fancy-type/
+-rw-r--r--   0 reinout    (501) staff       (20)      340 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/fancy-type/readme.txt
+-rw-r--r--   0 reinout    (501) staff       (20)     2173 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/fancy-type/screen.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/
+-rw-r--r--   0 reinout    (501) staff       (20)      777 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/doc.png
+-rw-r--r--   0 reinout    (501) staff       (20)      641 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/email.png
+-rw-r--r--   0 reinout    (501) staff       (20)    46848 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/external.png
+-rw-r--r--   0 reinout    (501) staff       (20)      691 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/feed.png
+-rw-r--r--   0 reinout    (501) staff       (20)      741 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/im.png
+-rw-r--r--   0 reinout    (501) staff       (20)      591 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/pdf.png
+-rw-r--r--   0 reinout    (501) staff       (20)    46990 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/visited.png
+-rw-r--r--   0 reinout    (501) staff       (20)      663 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/xls.png
+-rw-r--r--   0 reinout    (501) staff       (20)      449 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/readme.txt
+-rw-r--r--   0 reinout    (501) staff       (20)     1343 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/screen.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/rtl/
+-rw-r--r--   0 reinout    (501) staff       (20)      327 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/rtl/readme.txt
+-rw-r--r--   0 reinout    (501) staff       (20)     4839 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/plugins/rtl/screen.css
+-rw-r--r--   0 reinout    (501) staff       (20)     1284 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/print.css
+-rw-r--r--   0 reinout    (501) staff       (20)    11833 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/screen.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/blueprint/src/
+-rw-r--r--   0 reinout    (501) staff       (20)     1835 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/src/forms.css
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9486 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/src/grid.css
+-rw-r--r--   0 reinout    (501) staff       (20)      195 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/src/grid.png
+-rw-r--r--   0 reinout    (501) staff       (20)     2537 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/src/ie.css
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1826 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/src/print.css
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1232 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/src/reset.css
+-rw-r--r--   0 reinout    (501) staff       (20)     3182 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/blueprint/src/typography.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/
+-rw-r--r--   0 reinout    (501) staff       (20)      344 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/.gitignore
+-rw-r--r--   0 reinout    (501) staff       (20)       34 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/.travis.yml
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/css/
+-rw-r--r--   0 reinout    (501) staff       (20)    22111 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/css/bootstrap-responsive.css
+-rw-r--r--   0 reinout    (501) staff       (20)    16849 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/css/bootstrap-responsive.min.css
+-rw-r--r--   0 reinout    (501) staff       (20)   154037 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/css/bootstrap.css
+-rw-r--r--   0 reinout    (501) staff       (20)   127579 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/js/
+-rw-r--r--   0 reinout    (501) staff       (20)    61979 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/js/bootstrap.js
+-rw-r--r--   0 reinout    (501) staff       (20)    28519 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 reinout    (501) staff       (20)    25120 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/CHANGELOG.md
+-rw-r--r--   0 reinout    (501) staff       (20)      175 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/component.json
+-rw-r--r--   0 reinout    (501) staff       (20)      297 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/composer.json
+-rw-r--r--   0 reinout    (501) staff       (20)     3487 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/CONTRIBUTING.md
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/css/
+-rw-r--r--   0 reinout    (501) staff       (20)    22111 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/css/bootstrap-responsive.css
+-rw-r--r--   0 reinout    (501) staff       (20)   153960 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/css/bootstrap.css
+-rw-r--r--   0 reinout    (501) staff       (20)    22486 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/css/docs.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/ico/
+-rw-r--r--   0 reinout    (501) staff       (20)    11392 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-114-precomposed.png
+-rw-r--r--   0 reinout    (501) staff       (20)    16780 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-144-precomposed.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4026 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-57-precomposed.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5681 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-72-precomposed.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1150 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/ico/favicon.ico
+-rw-r--r--   0 reinout    (501) staff       (20)     2711 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/ico/favicon.png
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/
+-rw-r--r--   0 reinout    (501) staff       (20)    30612 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-docs-readme.png
+-rw-r--r--   0 reinout    (501) staff       (20)   125346 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-mdo-sfmoma-01.jpg
+-rw-r--r--   0 reinout    (501) staff       (20)    81284 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-mdo-sfmoma-02.jpg
+-rw-r--r--   0 reinout    (501) staff       (20)    49063 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-mdo-sfmoma-03.jpg
+-rw-r--r--   0 reinout    (501) staff       (20)    11244 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-bootstrap-features.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6450 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-masthead-pattern.png
+-rw-r--r--   0 reinout    (501) staff       (20)    10572 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-responsive-illustrations.png
+-rw-r--r--   0 reinout    (501) staff       (20)    30968 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-twitter-github.png
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/
+-rw-r--r--   0 reinout    (501) staff       (20)    62853 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/8020select.png
+-rw-r--r--   0 reinout    (501) staff       (20)   136480 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/adoptahydrant.png
+-rw-r--r--   0 reinout    (501) staff       (20)    72725 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/breakingnews.png
+-rw-r--r--   0 reinout    (501) staff       (20)    39837 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/fleetio.png
+-rw-r--r--   0 reinout    (501) staff       (20)    76560 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/gathercontent.png
+-rw-r--r--   0 reinout    (501) staff       (20)     7258 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/jshint.png
+-rw-r--r--   0 reinout    (501) staff       (20)    48259 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/kippt.png
+-rw-r--r--   0 reinout    (501) staff       (20)    50225 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/soundready.png
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/
+-rw-r--r--   0 reinout    (501) staff       (20)   339980 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-carousel.png
+-rw-r--r--   0 reinout    (501) staff       (20)   209039 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-fluid.png
+-rw-r--r--   0 reinout    (501) staff       (20)   136021 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-justified-nav.png
+-rw-r--r--   0 reinout    (501) staff       (20)   117303 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-marketing-narrow.png
+-rw-r--r--   0 reinout    (501) staff       (20)   134269 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-marketing.png
+-rw-r--r--   0 reinout    (501) staff       (20)    22037 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-signin.png
+-rw-r--r--   0 reinout    (501) staff       (20)    36099 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-starter.png
+-rw-r--r--   0 reinout    (501) staff       (20)    30820 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-sticky-footer.png
+-rw-r--r--   0 reinout    (501) staff       (20)    55522 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/browser-icon-chrome.png
+-rw-r--r--   0 reinout    (501) staff       (20)   175994 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/browser-icon-firefox.png
+-rw-r--r--   0 reinout    (501) staff       (20)   209527 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/browser-icon-safari.png
+-rw-r--r--   0 reinout    (501) staff       (20)    83303 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/slide-01.jpg
+-rw-r--r--   0 reinout    (501) staff       (20)   137070 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/slide-02.jpg
+-rw-r--r--   0 reinout    (501) staff       (20)   137378 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/slide-03.jpg
+-rw-r--r--   0 reinout    (501) staff       (20)     8777 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/glyphicons-halflings-white.png
+-rw-r--r--   0 reinout    (501) staff       (20)    12799 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/glyphicons-halflings.png
+-rw-r--r--   0 reinout    (501) staff       (20)       84 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/grid-baseline-20px.png
+-rw-r--r--   0 reinout    (501) staff       (20)    12824 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/less-logo-large.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1008 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/responsive-illustrations.png
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/
+-rw-r--r--   0 reinout    (501) staff       (20)     4036 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/application.js
+-rw-r--r--   0 reinout    (501) staff       (20)     3483 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-affix.js
+-rw-r--r--   0 reinout    (501) staff       (20)     2524 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-alert.js
+-rw-r--r--   0 reinout    (501) staff       (20)     2841 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-button.js
+-rw-r--r--   0 reinout    (501) staff       (20)     6057 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-carousel.js
+-rw-r--r--   0 reinout    (501) staff       (20)     4735 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-collapse.js
+-rw-r--r--   0 reinout    (501) staff       (20)     4203 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-dropdown.js
+-rw-r--r--   0 reinout    (501) staff       (20)     6656 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-modal.js
+-rw-r--r--   0 reinout    (501) staff       (20)     3115 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-popover.js
+-rw-r--r--   0 reinout    (501) staff       (20)     4655 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-scrollspy.js
+-rw-r--r--   0 reinout    (501) staff       (20)     3496 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-tab.js
+-rw-r--r--   0 reinout    (501) staff       (20)    10138 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-tooltip.js
+-rw-r--r--   0 reinout    (501) staff       (20)     1756 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-transition.js
+-rw-r--r--   0 reinout    (501) staff       (20)     8320 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-typeahead.js
+-rw-r--r--   0 reinout    (501) staff       (20)    61979 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap.js
+-rw-r--r--   0 reinout    (501) staff       (20)    28526 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap.min.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/google-code-prettify/
+-rw-r--r--   0 reinout    (501) staff       (20)      817 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/google-code-prettify/prettify.css
+-rw-r--r--   0 reinout    (501) staff       (20)    13632 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/google-code-prettify/prettify.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/holder/
+-rw-r--r--   0 reinout    (501) staff       (20)    11731 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/holder/holder.js
+-rw-r--r--   0 reinout    (501) staff       (20)     2376 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/html5shiv.js
+-rw-r--r--   0 reinout    (501) staff       (20)    92629 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/jquery.js
+-rw-r--r--   0 reinout    (501) staff       (20)     3249 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/README.md
+-rw-r--r--   0 reinout    (501) staff       (20)    94309 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/base-css.html
+-rw-r--r--   0 reinout    (501) staff       (20)   107153 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/components.html
+-rw-r--r--   0 reinout    (501) staff       (20)    27043 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/customize.html
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/
+-rw-r--r--   0 reinout    (501) staff       (20)    15641 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/carousel.html
+-rw-r--r--   0 reinout    (501) staff       (20)     7697 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/fluid.html
+-rw-r--r--   0 reinout    (501) staff       (20)     5825 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/hero.html
+-rw-r--r--   0 reinout    (501) staff       (20)     6130 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/justified-nav.html
+-rw-r--r--   0 reinout    (501) staff       (20)     4712 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/marketing-narrow.html
+-rw-r--r--   0 reinout    (501) staff       (20)     3634 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/signin.html
+-rw-r--r--   0 reinout    (501) staff       (20)     3333 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/starter-template.html
+-rw-r--r--   0 reinout    (501) staff       (20)     5798 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/sticky-footer-navbar.html
+-rw-r--r--   0 reinout    (501) staff       (20)     4174 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/sticky-footer.html
+-rw-r--r--   0 reinout    (501) staff       (20)    12644 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/extend.html
+-rw-r--r--   0 reinout    (501) staff       (20)    17348 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/getting-started.html
+-rw-r--r--   0 reinout    (501) staff       (20)     9693 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/index.html
+-rw-r--r--   0 reinout    (501) staff       (20)    91135 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/javascript.html
+-rw-r--r--   0 reinout    (501) staff       (20)    25153 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/scaffolding.html
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/
+-rw-r--r--   0 reinout    (501) staff       (20)     6537 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/layout.mustache
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/
+-rw-r--r--   0 reinout    (501) staff       (20)    94743 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/base-css.mustache
+-rw-r--r--   0 reinout    (501) staff       (20)   110205 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/components.mustache
+-rw-r--r--   0 reinout    (501) staff       (20)    23053 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/customize.mustache
+-rw-r--r--   0 reinout    (501) staff       (20)     7993 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/extend.mustache
+-rw-r--r--   0 reinout    (501) staff       (20)    13609 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/getting-started.mustache
+-rw-r--r--   0 reinout    (501) staff       (20)     5269 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/index.mustache
+-rw-r--r--   0 reinout    (501) staff       (20)    93014 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/javascript.mustache
+-rw-r--r--   0 reinout    (501) staff       (20)    21739 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/scaffolding.mustache
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/img/
+-rw-r--r--   0 reinout    (501) staff       (20)     8777 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/img/glyphicons-halflings-white.png
+-rw-r--r--   0 reinout    (501) staff       (20)    12799 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/img/glyphicons-halflings.png
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/
+-rw-r--r--   0 reinout    (501) staff       (20)      232 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/.jshintrc
+-rw-r--r--   0 reinout    (501) staff       (20)     3483 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-affix.js
+-rw-r--r--   0 reinout    (501) staff       (20)     2524 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-alert.js
+-rw-r--r--   0 reinout    (501) staff       (20)     2841 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-button.js
+-rw-r--r--   0 reinout    (501) staff       (20)     6057 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-carousel.js
+-rw-r--r--   0 reinout    (501) staff       (20)     4735 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-collapse.js
+-rw-r--r--   0 reinout    (501) staff       (20)     4203 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-dropdown.js
+-rw-r--r--   0 reinout    (501) staff       (20)     6656 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-modal.js
+-rw-r--r--   0 reinout    (501) staff       (20)     3115 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-popover.js
+-rw-r--r--   0 reinout    (501) staff       (20)     4655 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-scrollspy.js
+-rw-r--r--   0 reinout    (501) staff       (20)     3496 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-tab.js
+-rw-r--r--   0 reinout    (501) staff       (20)    10138 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-tooltip.js
+-rw-r--r--   0 reinout    (501) staff       (20)     1756 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-transition.js
+-rw-r--r--   0 reinout    (501) staff       (20)     8320 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-typeahead.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/
+-rw-r--r--   0 reinout    (501) staff       (20)     2134 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/index.html
+-rw-r--r--   0 reinout    (501) staff       (20)     2146 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/phantom.js
+-rw-r--r--   0 reinout    (501) staff       (20)      331 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/server.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/
+-rw-r--r--   0 reinout    (501) staff       (20)      797 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-affix.js
+-rw-r--r--   0 reinout    (501) staff       (20)     2099 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-alert.js
+-rw-r--r--   0 reinout    (501) staff       (20)     3761 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-button.js
+-rw-r--r--   0 reinout    (501) staff       (20)     6044 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-carousel.js
+-rw-r--r--   0 reinout    (501) staff       (20)     2913 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-collapse.js
+-rw-r--r--   0 reinout    (501) staff       (20)     6328 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-dropdown.js
+-rw-r--r--   0 reinout    (501) staff       (20)     4362 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-modal.js
+-rw-r--r--   0 reinout    (501) staff       (20)      714 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-phantom.js
+-rw-r--r--   0 reinout    (501) staff       (20)     4553 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-popover.js
+-rw-r--r--   0 reinout    (501) staff       (20)     1203 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-scrollspy.js
+-rw-r--r--   0 reinout    (501) staff       (20)     2848 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-tab.js
+-rw-r--r--   0 reinout    (501) staff       (20)    10849 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-tooltip.js
+-rw-r--r--   0 reinout    (501) staff       (20)      374 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-transition.js
+-rw-r--r--   0 reinout    (501) staff       (20)     7584 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-typeahead.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/vendor/
+-rw-r--r--   0 reinout    (501) staff       (20)    92629 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/vendor/jquery.js
+-rw-r--r--   0 reinout    (501) staff       (20)     4560 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/vendor/qunit.css
+-rw-r--r--   0 reinout    (501) staff       (20)    38070 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/vendor/qunit.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/
+-rw-r--r--   0 reinout    (501) staff       (20)      636 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/accordion.less
+-rw-r--r--   0 reinout    (501) staff       (20)     1369 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/alerts.less
+-rw-r--r--   0 reinout    (501) staff       (20)     1633 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/bootstrap.less
+-rw-r--r--   0 reinout    (501) staff       (20)      431 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/breadcrumbs.less
+-rw-r--r--   0 reinout    (501) staff       (20)     5709 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/button-groups.less
+-rw-r--r--   0 reinout    (501) staff       (20)     4766 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/buttons.less
+-rw-r--r--   0 reinout    (501) staff       (20)     2482 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/carousel.less
+-rw-r--r--   0 reinout    (501) staff       (20)      644 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/close.less
+-rw-r--r--   0 reinout    (501) staff       (20)     1282 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/code.less
+-rw-r--r--   0 reinout    (501) staff       (20)      306 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/component-animations.less
+-rw-r--r--   0 reinout    (501) staff       (20)     5493 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/dropdowns.less
+-rw-r--r--   0 reinout    (501) staff       (20)    20690 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/font-awesome.less
+-rw-r--r--   0 reinout    (501) staff       (20)    15866 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/forms.less
+-rw-r--r--   0 reinout    (501) staff       (20)      429 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/grid.less
+-rw-r--r--   0 reinout    (501) staff       (20)      521 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/hero-unit.less
+-rw-r--r--   0 reinout    (501) staff       (20)     1884 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/labels-badges.less
+-rw-r--r--   0 reinout    (501) staff       (20)      329 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/layouts.less
+-rw-r--r--   0 reinout    (501) staff       (20)    18012 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/lizard-bootstrap.less
+-rw-r--r--   0 reinout    (501) staff       (20)      860 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/media.less
+-rw-r--r--   0 reinout    (501) staff       (20)    23042 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/mixins.less
+-rw-r--r--   0 reinout    (501) staff       (20)     1978 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/modals.less
+-rw-r--r--   0 reinout    (501) staff       (20)    12002 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/navbar.less
+-rw-r--r--   0 reinout    (501) staff       (20)     8163 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/navs.less
+-rw-r--r--   0 reinout    (501) staff       (20)      760 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/pager.less
+-rw-r--r--   0 reinout    (501) staff       (20)     2678 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/pagination.less
+-rw-r--r--   0 reinout    (501) staff       (20)     3077 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/popovers.less
+-rw-r--r--   0 reinout    (501) staff       (20)     2858 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/progress-bars.less
+-rw-r--r--   0 reinout    (501) staff       (20)     4201 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/reset.less
+-rw-r--r--   0 reinout    (501) staff       (20)      565 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/responsive-1200px-min.less
+-rw-r--r--   0 reinout    (501) staff       (20)     3920 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/responsive-767px-max.less
+-rw-r--r--   0 reinout    (501) staff       (20)      463 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/responsive-768px-979px.less
+-rw-r--r--   0 reinout    (501) staff       (20)     4328 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/responsive-navbar.less
+-rw-r--r--   0 reinout    (501) staff       (20)     1602 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/responsive-utilities.less
+-rw-r--r--   0 reinout    (501) staff       (20)     1069 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/responsive.less
+-rw-r--r--   0 reinout    (501) staff       (20)      885 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/scaffolding.less
+-rw-r--r--   0 reinout    (501) staff       (20)    10841 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/sprites.less
+-rw-r--r--   0 reinout    (501) staff       (20)     6255 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/tables.less
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/
+-rw-r--r--   0 reinout    (501) staff       (20)     6411 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/buttons.html
+-rw-r--r--   0 reinout    (501) staff       (20)     5475 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/css-tests.css
+-rw-r--r--   0 reinout    (501) staff       (20)    40138 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/css-tests.html
+-rw-r--r--   0 reinout    (501) staff       (20)     2362 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/forms-responsive.html
+-rw-r--r--   0 reinout    (501) staff       (20)     4079 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/forms.html
+-rw-r--r--   0 reinout    (501) staff       (20)     4692 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/navbar-fixed-top.html
+-rw-r--r--   0 reinout    (501) staff       (20)     4711 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/navbar-static-top.html
+-rw-r--r--   0 reinout    (501) staff       (20)     4797 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/navbar.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1192 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/thumbnails.less
+-rw-r--r--   0 reinout    (501) staff       (20)     1684 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/tooltip.less
+-rw-r--r--   0 reinout    (501) staff       (20)     4857 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/type.less
+-rw-r--r--   0 reinout    (501) staff       (20)      335 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/utilities.less
+-rw-r--r--   0 reinout    (501) staff       (20)     9134 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/variables.less
+-rw-r--r--   0 reinout    (501) staff       (20)      552 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/less/wells.less
+-rw-r--r--   0 reinout    (501) staff       (20)    10172 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/LICENSE
+-rw-r--r--   0 reinout    (501) staff       (20)     4561 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/Makefile
+-rw-r--r--   0 reinout    (501) staff       (20)      700 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/package.json
+-rw-r--r--   0 reinout    (501) staff       (20)     4599 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap/README.md
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/bootstrap-tour/
+-rw-r--r--   0 reinout    (501) staff       (20)     1723 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap-tour/bootstrap-tour.min.css
+-rw-r--r--   0 reinout    (501) staff       (20)    14438 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/bootstrap-tour/bootstrap-tour.min.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/css/
+-rw-r--r--   0 reinout    (501) staff       (20)     3181 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/css/colorpicker.css
+-rw-r--r--   0 reinout    (501) staff       (20)     4073 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/css/layout.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/
+-rw-r--r--   0 reinout    (501) staff       (20)       49 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/blank.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1897 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_background.png
+-rw-r--r--   0 reinout    (501) staff       (20)      532 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_hex.png
+-rw-r--r--   0 reinout    (501) staff       (20)      970 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_hsb_b.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1012 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_hsb_h.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1171 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_hsb_s.png
+-rw-r--r--   0 reinout    (501) staff       (20)       86 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_indic.gif
+-rw-r--r--   0 reinout    (501) staff       (20)    10355 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_overlay.png
+-rw-r--r--   0 reinout    (501) staff       (20)      970 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_rgb_b.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1069 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_rgb_g.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1066 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_rgb_r.png
+-rw-r--r--   0 reinout    (501) staff       (20)       78 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_select.gif
+-rw-r--r--   0 reinout    (501) staff       (20)      984 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_submit.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1916 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_background.png
+-rw-r--r--   0 reinout    (501) staff       (20)      562 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_hex.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1097 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_hsb_b.png
+-rw-r--r--   0 reinout    (501) staff       (20)      970 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_hsb_h.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1168 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_hsb_s.png
+-rw-r--r--   0 reinout    (501) staff       (20)       86 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_indic.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1008 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_rgb_b.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1069 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_rgb_g.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1018 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_rgb_r.png
+-rw-r--r--   0 reinout    (501) staff       (20)      997 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_submit.png
+-rw-r--r--   0 reinout    (501) staff       (20)      506 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/select.png
+-rw-r--r--   0 reinout    (501) staff       (20)      518 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/select2.png
+-rw-r--r--   0 reinout    (501) staff       (20)      315 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/slider.png
+-rw-r--r--   0 reinout    (501) staff       (20)    19968 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/images/Thumbs.db
+-rw-r--r--   0 reinout    (501) staff       (20)     8411 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/index.html
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/js/
+-rw-r--r--   0 reinout    (501) staff       (20)    17164 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/js/colorpicker.js
+-rw-r--r--   0 reinout    (501) staff       (20)      604 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/js/eye.js
+-rw-r--r--   0 reinout    (501) staff       (20)   124995 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/js/jquery.js
+-rw-r--r--   0 reinout    (501) staff       (20)     1829 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/js/layout.js
+-rw-r--r--   0 reinout    (501) staff       (20)     7135 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/colorpicker/js/utils.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/datatables/
+-rw-r--r--   0 reinout    (501) staff       (20)        7 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/.gitignore
+-rw-r--r--   0 reinout    (501) staff       (20)     1440 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/license-bsd.txt
+-rw-r--r--   0 reinout    (501) staff       (20)    17987 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/license-gpl2.txt
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/
+-rw-r--r--   0 reinout    (501) staff       (20)     6148 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/.DS_Store
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/css/
+-rw-r--r--   0 reinout    (501) staff       (20)     1341 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/css/demo_page.css
+-rw-r--r--   0 reinout    (501) staff       (20)     9689 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/css/demo_table.css
+-rw-r--r--   0 reinout    (501) staff       (20)     8930 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/css/demo_table_jui.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/images/
+-rw-r--r--   0 reinout    (501) staff       (20)      612 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/images/back_disabled.jpg
+-rw-r--r--   0 reinout    (501) staff       (20)      807 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/images/back_enabled.jpg
+-rw-r--r--   0 reinout    (501) staff       (20)      894 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/images/favicon.ico
+-rw-r--r--   0 reinout    (501) staff       (20)      635 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/images/forward_disabled.jpg
+-rw-r--r--   0 reinout    (501) staff       (20)      852 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/images/forward_enabled.jpg
+-rw-r--r--   0 reinout    (501) staff       (20)      263 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/images/sort_asc.png
+-rw-r--r--   0 reinout    (501) staff       (20)      252 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/images/sort_asc_disabled.png
+-rw-r--r--   0 reinout    (501) staff       (20)      282 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/images/sort_both.png
+-rw-r--r--   0 reinout    (501) staff       (20)      260 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/images/sort_desc.png
+-rw-r--r--   0 reinout    (501) staff       (20)      251 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/images/sort_desc_disabled.png
+-rw-r--r--   0 reinout    (501) staff       (20)    27490 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/images/Sorting icons.psd
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/js/
+-rw-r--r--   0 reinout    (501) staff       (20)   230256 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/js/jquery.dataTables.js
+-rw-r--r--   0 reinout    (501) staff       (20)    70883 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/js/jquery.dataTables.min.js
+-rw-r--r--   0 reinout    (501) staff       (20)    19393 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/js/jquery.dataTables.min.js.gz
+-rw-r--r--   0 reinout    (501) staff       (20)    91625 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/media/js/jquery.js
+-rw-r--r--   0 reinout    (501) staff       (20)      965 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/datatables/Readme.txt
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/daterangepicker/
+-rw-r--r--   0 reinout    (501) staff       (20)     4128 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/daterangepicker/daterangepicker.css
+-rw-r--r--   0 reinout    (501) staff       (20)    20548 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/daterangepicker/daterangepicker.js
+-rw-r--r--   0 reinout    (501) staff       (20)     3948 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/daterangepicker/daterangepicker.orig.css
+-rw-r--r--   0 reinout    (501) staff       (20)    19832 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/daterangepicker/daterangepicker.orig.js
+-rw-r--r--   0 reinout    (501) staff       (20)     2230 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/daterangepicker/README.md
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/font-awesome/
+-rw-r--r--   0 reinout    (501) staff       (20)    25255 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/font-awesome/font-awesome-ie7.min.css
+-rwxr-xr-x   0 reinout    (501) staff       (20)    25395 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/font-awesome/fontawesome-webfont.eot
+-rwxr-xr-x   0 reinout    (501) staff       (20)   138488 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/font-awesome/fontawesome-webfont.svg
+-rwxr-xr-x   0 reinout    (501) staff       (20)    55096 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/font-awesome/fontawesome-webfont.ttf
+-rwxr-xr-x   0 reinout    (501) staff       (20)    29380 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/font-awesome/fontawesome-webfont.woff
+-rw-r--r--   0 reinout    (501) staff       (20)    48748 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/font-awesome/FontAwesome.otf
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/html5shiv/
+-rw-r--r--   0 reinout    (501) staff       (20)     9342 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/html5shiv/html5shiv.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/jquery/
+-rw-r--r--   0 reinout    (501) staff       (20)    94840 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery/jquery.min.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    19314 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/excanvas.min.js
+-rw-r--r--   0 reinout    (501) staff       (20)     6110 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.colorhelpers.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    14146 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.axislabels.js
+-rw-r--r--   0 reinout    (501) staff       (20)     5871 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.categories.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5191 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.crosshair.js
+-rw-r--r--   0 reinout    (501) staff       (20)    12637 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.errorbars.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6772 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.fillbetween.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7351 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.image.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)   106306 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    14160 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.navigate.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    30114 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.pie.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1335 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.resize.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    12018 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.selection.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6968 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.stack.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2441 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.symbol.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4180 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.threshold.js
+-rw-r--r--   0 reinout    (501) staff       (20)    12968 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.time.js
+-rw-r--r--   0 reinout    (501) staff       (20)    12037 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.touch.js
+-rw-r--r--   0 reinout    (501) staff       (20)     1069 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-flot/LICENSE.txt
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/jquery-json/
+-rw-r--r--   0 reinout    (501) staff       (20)     4712 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-json/jquery.json-2.3.js
+-rw-r--r--   0 reinout    (501) staff       (20)     2177 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-json/jquery.json-2.3.min.js
+-rw-r--r--   0 reinout    (501) staff       (20)    17521 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-json/json2.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/jquery-mobile-events/
+-rw-r--r--   0 reinout    (501) staff       (20)    15443 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-mobile-events/jquery.mobile-events.min.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/jquery-resize/
+-rw-r--r--   0 reinout    (501) staff       (20)     9195 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-resize/jquery.ba-resize.js
+-rw-r--r--   0 reinout    (501) staff       (20)     1098 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-resize/jquery.ba-resize.min.js
+-rw-r--r--   0 reinout    (501) staff       (20)    15098 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-resize/LICENSE-GPL
+-rw-r--r--   0 reinout    (501) staff       (20)     1062 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-resize/LICENSE-MIT
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/jquery-transform/
+-rw-r--r--   0 reinout    (501) staff       (20)    51654 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-transform/jquery.transform-0.9.3.js
+-rw-r--r--   0 reinout    (501) staff       (20)    20250 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-transform/jquery.transform-0.9.3.min.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/
+-rw-r--r--   0 reinout    (501) staff       (20)      847 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/ajax-loader.gif
+-rw-r--r--   0 reinout    (501) staff       (20)      110 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/file.gif
+-rw-r--r--   0 reinout    (501) staff       (20)      105 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/folder-closed.gif
+-rw-r--r--   0 reinout    (501) staff       (20)      106 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/folder.gif
+-rw-r--r--   0 reinout    (501) staff       (20)      837 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/minus.gif
+-rw-r--r--   0 reinout    (501) staff       (20)      841 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/plus.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1877 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-black-line.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1216 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-black.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1993 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-default-line.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1222 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-default.gif
+-rw-r--r--   0 reinout    (501) staff       (20)      807 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-famfamfam-line.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1280 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-famfamfam.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1877 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-gray-line.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1230 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-gray.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1877 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-red-line.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1230 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-red.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     2866 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/jquery.treeview.async.js
+-rw-r--r--   0 reinout    (501) staff       (20)     2651 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/jquery.treeview.css
+-rw-r--r--   0 reinout    (501) staff       (20)     1567 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/jquery.treeview.edit.js
+-rw-r--r--   0 reinout    (501) staff       (20)     8264 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/jquery.treeview.js
+-rw-r--r--   0 reinout    (501) staff       (20)    13156 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jquery-treeview/jquery.treeview.sortable.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/
+-rw-r--r--   0 reinout    (501) staff       (20)   365958 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/jquery-ui.js
+-rw-r--r--   0 reinout    (501) staff       (20)   365673 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/jquery-ui.orig.js
+-rw-r--r--   0 reinout    (501) staff       (20)      924 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/jquery.ui.datepicker-nl.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/
+-rw-r--r--   0 reinout    (501) staff       (20)      180 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-r--r--   0 reinout    (501) staff       (20)      178 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-bg_flat_75_ffffff_40x100.png
+-rw-r--r--   0 reinout    (501) staff       (20)      120 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 reinout    (501) staff       (20)      105 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 reinout    (501) staff       (20)      111 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 reinout    (501) staff       (20)      110 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 reinout    (501) staff       (20)      119 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 reinout    (501) staff       (20)      101 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4369 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4369 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4369 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4369 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4369 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 reinout    (501) staff       (20)    33422 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/jquery-ui.css
+-rw-r--r--   0 reinout    (501) staff       (20)    33172 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/jquery-ui.orig.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/less/
+-rw-r--r--   0 reinout    (501) staff       (20)    44423 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/less/less-1.2.1.min.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/
+-rw-r--r--   0 reinout    (501) staff       (20)      622 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/60degree_gray.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3208 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/ajax-loader.gif
+-rw-r--r--   0 reinout    (501) staff       (20)      723 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/ajax-loader2.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1849 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/ajax-loader3.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     2545 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/ajax-loader4.gif
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/
+-rw-r--r--   0 reinout    (501) staff       (20)     3718 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/3di.png
+-rw-r--r--   0 reinout    (501) staff       (20)     7306 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/alkmaar.png
+-rw-r--r--   0 reinout    (501) staff       (20)     2811 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/almere.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3948 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/appicon_eleaf.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3457 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/appicon_knmi.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3694 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/appicon_neo.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3665 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/appicon_pwn.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4927 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/appicon_satapp.png
+-rw-r--r--   0 reinout    (501) staff       (20)     7269 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/boek.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3825 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/ciw.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5848 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/controlnext.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4001 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/dacom.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6430 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/deltares.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3425 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/dike.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5693 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/download.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4740 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/download_grijs.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6136 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/drought.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3207 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/energieverbruik.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4231 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/floodapp.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4194 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/flooding.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3802 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/flooding2.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6488 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/gisflow.png
+-rw-r--r--   0 reinout    (501) staff       (20)     7098 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/grondwater.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5949 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/hdsr.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5474 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/history.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4478 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/kaartlagen.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3881 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/keringen.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4816 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/kpi.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5623 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/kustviewer.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6110 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/kwantiteit.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4110 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/lcms.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6125 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/leveeportal.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6178 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/lizard.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6220 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/lizard_alarm.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6146 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/maatregelen.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3200 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/meetgegevens.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4135 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/modelresultaten.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5010 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/narrowcasting.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3038 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/neerslag.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5789 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/nhi.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6598 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/nieuwe_kaart_van_nederland.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6869 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/noorderpark.png
+-rw-r--r--   0 reinout    (501) staff       (20)     2688 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/oevers.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5547 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/oppervlaktewater.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5116 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/peilschaal.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6945 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/planning.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3182 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/play.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6512 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/projecten.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3360 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/RegimeApp.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6853 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/riolering.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6941 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/rws.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5770 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/statistiek.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4110 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/statusoverzicht.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6066 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/sticky.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5910 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/stowa.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3789 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/telecontrolnet.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4518 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/turtle.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5546 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/twitter.png
+-rw-r--r--   0 reinout    (501) staff       (20)     5656 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/upload.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4618 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/upload_grijs.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6318 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/uploadserver.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4023 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/urk.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4602 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/VerlorenBerging.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6855 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/vss.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3360 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/waterbalance.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6465 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/waterkwaliteit.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6012 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/WIT.png
+-rw-r--r--   0 reinout    (501) staff       (20)     4465 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/wms.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6696 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/workspace_metingen.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6680 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/workspace_neerslag.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6474 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/workspace_oppervlaktewater.png
+-rw-r--r--   0 reinout    (501) staff       (20)     7505 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/workspace_riolering.png
+-rw-r--r--   0 reinout    (501) staff       (20)     7539 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/workspace_wateropstraat.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6528 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/zettingen.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3728 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/zuiderzeeland.png
+-rw-r--r--   0 reinout    (501) staff       (20)      153 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/arrow_collapse.png
+-rw-r--r--   0 reinout    (501) staff       (20)      155 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/arrow_expand.png
+-rw-r--r--   0 reinout    (501) staff       (20)      336 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/arrows.png
+-rw-r--r--   0 reinout    (501) staff       (20)      598 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/background.png
+-rw-r--r--   0 reinout    (501) staff       (20)      157 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/bar_background copy.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1273 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/bar_background.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1636 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/box-awesome.css
+-rw-r--r--   0 reinout    (501) staff       (20)    28711 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/buttons.css
+-rw-r--r--   0 reinout    (501) staff       (20)      142 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/carbon_fibre.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1996 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/close.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1946 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/csrf.js
+-rw-r--r--   0 reinout    (501) staff       (20)   102370 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/fabric_1.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1406 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/favicon.ico
+-rw-r--r--   0 reinout    (501) staff       (20)     2089 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/icon-chart.png
+-rw-r--r--   0 reinout    (501) staff       (20)      980 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/icon-legend.png
+-rw-r--r--   0 reinout    (501) staff       (20)    77720 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/leather_1.png
+-rw-r--r--   0 reinout    (501) staff       (20)    17387 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/lizard_ui.js
+-rw-r--r--   0 reinout    (501) staff       (20)     3749 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/logo.png
+-rw-r--r--   0 reinout    (501) staff       (20)    48689 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/old_mathematics.png
+-rw-r--r--   0 reinout    (501) staff       (20)    10726 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/OpenLayers.Control.NensLayerSwitcher.js
+-rw-r--r--   0 reinout    (501) staff       (20)      863 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/print.css
+-rw-r--r--   0 reinout    (501) staff       (20)      140 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/small_bar_background.png
+-rw-r--r--   0 reinout    (501) staff       (20)      916 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/tabs.css
+-rw-r--r--   0 reinout    (501) staff       (20)      133 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/lizard_ui/white_carbon.png
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/momentjs/
+-rw-r--r--   0 reinout    (501) staff       (20)    36776 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/momentjs/moment.js
+-rw-r--r--   0 reinout    (501) staff       (20)    11484 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/momentjs/moment.min.js
+-rw-r--r--   0 reinout    (501) staff       (20)     2395 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/momentjs/nl.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1285 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/authors.txt
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/
+-rw-r--r--   0 reinout    (501) staff       (20)       42 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/blank.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     4067 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/cloud-popup-relative.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1024 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/drag-rectangle-off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1041 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/drag-rectangle-on.png
+-rw-r--r--   0 reinout    (501) staff       (20)      298 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/east-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)      303 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/layer-switcher-maximize.png
+-rw-r--r--   0 reinout    (501) staff       (20)      367 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/layer-switcher-minimize.png
+-rw-r--r--   0 reinout    (501) staff       (20)      758 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/marker-blue.png
+-rw-r--r--   0 reinout    (501) staff       (20)      703 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/marker-gold.png
+-rw-r--r--   0 reinout    (501) staff       (20)      753 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/marker-green.png
+-rw-r--r--   0 reinout    (501) staff       (20)      601 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/marker.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3028 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/measuring-stick-off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3725 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/measuring-stick-on.png
+-rw-r--r--   0 reinout    (501) staff       (20)      298 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/north-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3511 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/panning-hand-off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3565 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/panning-hand-on.png
+-rw-r--r--   0 reinout    (501) staff       (20)      236 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/slider.png
+-rw-r--r--   0 reinout    (501) staff       (20)      310 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/south-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)      299 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/west-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)      229 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/zoom-minus-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)      276 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/zoom-plus-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)      545 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/zoom-world-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)      232 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/zoombar.png
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/
+-rwxr-xr-x   0 reinout    (501) staff       (20)   175037 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/deprecated.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/
+-rwxr-xr-x   0 reinout    (501) staff       (20)      457 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/errorIcon.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3480 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebug.css
+-rwxr-xr-x   0 reinout    (501) staff       (20)      651 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebug.html
+-rwxr-xr-x   0 reinout    (501) staff       (20)    19181 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebug.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      384 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebugx.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      524 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/infoIcon.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1561 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/license.txt
+-rwxr-xr-x   0 reinout    (501) staff       (20)      545 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/readme.txt
+-rwxr-xr-x   0 reinout    (501) staff       (20)      516 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/warningIcon.png
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3633 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Animation.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    25310 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Bounds.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3740 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Class.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5071 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Date.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5398 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Element.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6425 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/LonLat.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3649 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Pixel.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2191 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Size.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    13356 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7885 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Console.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5908 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ArgParser.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3155 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Attribution.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1217 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Button.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5044 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/CacheRead.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8033 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/CacheWrite.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    11478 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/DragFeature.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4416 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/DragPan.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7217 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/DrawFeature.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2771 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/EditingToolbar.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5376 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Geolocate.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    20030 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/GetFeature.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    14041 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Graticule.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4399 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/KeyboardDefaults.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    17640 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/LayerSwitcher.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    11790 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Measure.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    31212 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ModifyFeature.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4960 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/MousePosition.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9585 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Navigation.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    13519 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/NavigationHistory.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1836 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/NavToolbar.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    25888 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/OverviewMap.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3270 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Pan.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    14528 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Panel.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2578 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PanPanel.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6681 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PanZoom.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    12487 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PanZoomBar.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8122 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Permalink.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6646 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PinchZoom.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2856 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Scale.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6670 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ScaleLine.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    20556 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/SelectFeature.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    21423 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/SLDSelect.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    21409 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Snapping.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    19587 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Split.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5219 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/TouchNavigation.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    23368 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/TransformFeature.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6984 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/UTFGrid.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    18600 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/WMSGetFeatureInfo.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    13067 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/WMTSGetFeatureInfo.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4142 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Zoom.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3811 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomBox.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      937 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomIn.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      942 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomOut.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1817 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomPanel.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1126 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomToMaxExtent.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    11237 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Events/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5945 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Events/buttonclick.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    31565 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Events.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Feature/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    18603 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Feature/Vector.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6505 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Feature.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9330 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Comparison.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2341 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/FeatureId.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1320 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Function.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3424 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Logical.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3523 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Spatial.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2279 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/ArcXML/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1430 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/ArcXML/Features.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    40703 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/ArcXML.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    23184 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Atom.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    11931 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Context.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    16333 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CQL.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetDomain/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8222 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetDomain/v2_0_2.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      992 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetDomain.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetRecords/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    16614 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetRecords/v2_0_2.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1000 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetRecords.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    18804 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/v1.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7390 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/v1_0_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8704 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/v1_1_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1505 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    24949 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GeoJSON.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    14717 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GeoRSS.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    24742 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/Base.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7439 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/v2.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    18906 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/v3.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    35433 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    12944 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GPX.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    13212 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/JSON.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    55468 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/KML.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3427 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OGCExceptionReport.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    16106 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OSM.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    12883 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/v1.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2061 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/v1_0_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4249 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/v1_1_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2415 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSContext/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    23703 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSContext/v0_3_1.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2691 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSContext.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6971 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/QueryStringFilter.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    52979 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/v1.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1305 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/v1_0_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5438 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/v1_0_0_GeoServer.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2321 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSCapabilities/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5680 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSCapabilities/v1_0_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1345 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSCapabilities.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6397 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSGetFeatureOfInterest.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    11307 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSGetObservation.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6597 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Text.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7036 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WCSGetCoverage.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7716 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFS.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3724 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/v1.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4360 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/v1_0_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2024 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/v1_1_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1646 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6993 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSDescribeFeatureType.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    16316 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/v1.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6988 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/v1_0_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7931 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/v1_1_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      996 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    14807 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WKT.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    38512 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/v1.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3097 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/v1_0_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4538 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/v1_1_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6353 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    14702 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5037 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1845 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1677 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1_1.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2982 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1_1_WMSC.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5893 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_3.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      951 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_3_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1514 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSDescribeLayer/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3757 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSDescribeLayer/v1_1.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2353 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSDescribeLayer.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9782 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSGetFeatureInfo.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMTSCapabilities/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9301 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMTSCapabilities/v1_0_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4352 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMTSCapabilities.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSCapabilities/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3945 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSCapabilities/v1_0_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1306 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSCapabilities.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6276 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSDescribeProcess.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9602 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSExecute.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    11114 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS/v1.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1360 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS/v1_1_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1970 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XML/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5696 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XML/VersionedOGC.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    31465 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XML.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3904 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    18626 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Collection.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2952 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Curve.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    14975 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/LinearRing.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    25718 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/LineString.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    10486 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/MultiLineString.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1913 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/MultiPoint.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1355 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/MultiPolygon.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8912 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Point.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9394 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Polygon.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    15685 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7721 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Box.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    17540 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Click.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    16375 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Drag.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    14095 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Feature.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5076 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Hover.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3660 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Keyboard.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9528 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/MouseWheel.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    16921 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Path.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6304 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Pinch.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    16306 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Point.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    10643 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Polygon.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    14706 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/RegularPolygon.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9461 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6817 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Icon.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4700 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Kinetic.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/
+-rwxr-xr-x   0 reinout    (501) staff       (20)      662 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ar.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4500 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/be-tarask.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      757 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/bg.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3153 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/br.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3633 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ca.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2997 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/cs-CZ.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3397 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/da-DK.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3509 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/de.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      491 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/el.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      670 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/en-CA.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3576 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/en.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3709 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/es.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      568 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/fi.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3440 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/fr.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      767 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/fur.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3262 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/gl.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3166 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/gsw.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1060 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/hr.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3161 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/hsb.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3526 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/hu.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3143 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ia.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3129 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/id.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      465 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/io.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      710 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/is.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3512 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/it.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3875 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ja.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      678 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/km.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3968 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ksh.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1267 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/lt.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3342 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nb.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1119 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nds.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3239 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nl.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      486 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nn.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3163 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/oc.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3923 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/pl.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3430 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/pt-BR.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3259 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/pt.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4515 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ru.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3203 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/sk.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3056 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/sv-SE.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      538 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/te.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3340 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/vi.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3129 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/zh-CN.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3153 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/zh-TW.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4268 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7956 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/ArcGIS93Rest.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    18984 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/ArcGISCache.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    14638 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/ArcIMS.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    10513 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Bing.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2111 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Boxes.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    14272 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/EventPane.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    12249 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/FixedZoomLevels.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8593 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/GeoRSS.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Google/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    16330 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Google/v3.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    24682 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Google.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    47032 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Grid.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7191 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/HTTPRequest.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7832 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Image.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6009 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/KaMap.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4875 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/KaMapCache.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    18252 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/MapGuide.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6713 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/MapServer.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4920 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Markers.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3922 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/OSM.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    10022 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/PointGrid.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4459 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/PointTrack.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5103 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/SphericalMercator.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9613 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Text.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5786 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/TileCache.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7441 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/TMS.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5425 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/UTFGrid.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Vector/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4709 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Vector/RootContainer.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    34709 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Vector.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9926 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/WMS.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    18357 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/WMTS.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2948 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/WorldWind.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5776 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/XYZ.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9399 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Zoomify.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    46776 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    93493 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Map.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Marker/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2794 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Marker/Box.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6315 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Marker.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6530 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/Anchored.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     5576 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/AnchoredBubble.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    11967 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/Framed.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8380 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/FramedCloud.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    35284 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    10970 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Projection.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/CSW/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4004 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/CSW/v2_0_2.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      871 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/CSW.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    20226 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/HTTP.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    13112 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/Script.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/SOS/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4244 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/SOS/v1_0_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      956 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/SOS.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    15122 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/v1.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1481 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/v1_0_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2689 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/v1_1_0.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2834 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8408 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    33022 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/Canvas.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    34381 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/Elements.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    34784 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/SVG.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    33790 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/VML.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    13322 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Request/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    17370 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Request/XMLHttpRequest.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    16643 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Request.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7377 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Rule.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2741 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/SingleFile.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2631 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Spherical.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9419 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/BBOX.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8958 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Cluster.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4979 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Filter.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3985 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Fixed.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6316 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Paging.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3610 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Refresh.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7481 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Save.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3157 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    14798 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Style.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2912 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Style2.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6263 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/StyleMap.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2260 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Line.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     4815 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Point.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2659 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Polygon.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1020 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Raster.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1947 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Text.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1556 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/Image/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8150 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/Image/IFrame.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    16449 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/Image.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7418 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/UTFGrid.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8951 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8083 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tween.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    59252 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Util.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    18871 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Rico/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6679 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Rico/Color.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)    11895 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Rico/Corner.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)      696 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Rico/license.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1537 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/license.txt
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/licenses/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    11358 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/licenses/APACHE-2.0.txt
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1462 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/licenses/BSD-LICENSE.txt
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1023 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/licenses/MIT-LICENSE.txt
+-rwxr-xr-x   0 reinout    (501) staff       (20)  2823171 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/OpenLayers.debug.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)   739729 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/OpenLayers.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)  1225156 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/OpenLayers.light.debug.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)   287078 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/OpenLayers.light.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)  1388259 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/OpenLayers.mobile.debug.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)   332603 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/OpenLayers.mobile.js
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3407 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/readme.md
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/
+-rwxr-xr-x   0 reinout    (501) staff       (20)      303 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/google.css
+-rwxr-xr-x   0 reinout    (501) staff       (20)      229 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/google.tidy.css
+-rwxr-xr-x   0 reinout    (501) staff       (20)      212 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/ie6-style.css
+-rwxr-xr-x   0 reinout    (501) staff       (20)      184 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/ie6-style.tidy.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1614 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/add_point_off.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1464 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/add_point_on.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)       42 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/blank.gif
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1078 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/close.gif
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1024 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/drag-rectangle-off.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1041 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/drag-rectangle-on.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1565 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_line_off.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1396 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_line_on.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1610 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_point_off.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1458 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_point_on.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1544 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_polygon_off.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1405 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_polygon_on.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2222 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/editing_tool_bar.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1541 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/move_feature_off.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1377 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/move_feature_on.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     6628 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/navigation_history.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)       79 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/overview_replacement.gif
+-rwxr-xr-x   0 reinout    (501) staff       (20)      564 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan-panel-NOALPHA.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)      814 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan-panel.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1696 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan_off.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1566 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan_on.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3511 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/panning-hand-off.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     3565 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/panning-hand-on.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1612 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/remove_point_off.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1461 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/remove_point_on.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1211 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/ruler.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)      354 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/save_features_off.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)      361 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/save_features_on.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1499 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_next_off.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1686 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_next_on.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1476 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_previous_off.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1592 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_previous_on.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1173 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/zoom-panel-NOALPHA.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1285 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/zoom-panel.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)     9948 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/style.css
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1688 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/style.mobile.css
+-rwxr-xr-x   0 reinout    (501) staff       (20)      970 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/style.mobile.tidy.css
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7547 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/style.tidy.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/
+-rwxr-xr-x   0 reinout    (501) staff       (20)    69566 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/BeautifulSoup.py
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2337 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/closure_library_jscompiler.py
+-rwxr-xr-x   0 reinout    (501) staff       (20)      861 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/closure_ws.py
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8324 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/exampleparser.py
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7006 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/jsmin.c
+-rwxr-xr-x   0 reinout    (501) staff       (20)     7471 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/jsmin.py
+-rwxr-xr-x   0 reinout    (501) staff       (20)     8955 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/mergejs.py
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2088 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/minimize.py
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1359 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/oldot.py
+-rwxr-xr-x   0 reinout    (501) staff       (20)      643 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/README.txt
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1487 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/release.sh
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1498 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/shrinksafe.py
+-rwxr-xr-x   0 reinout    (501) staff       (20)     1086 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/toposort.py
+-rwxr-xr-x   0 reinout    (501) staff       (20)     2519 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/update_dev_dir.sh
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/
+-rw-r--r--   0 reinout    (501) staff       (20)   180452 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/deprecated.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/
+-rw-r--r--   0 reinout    (501) staff       (20)       42 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/blank.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     4067 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/cloud-popup-relative.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1024 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/drag-rectangle-off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1041 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/drag-rectangle-on.png
+-rw-r--r--   0 reinout    (501) staff       (20)      298 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/east-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)      303 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/layer-switcher-maximize.png
+-rw-r--r--   0 reinout    (501) staff       (20)      367 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/layer-switcher-minimize.png
+-rw-r--r--   0 reinout    (501) staff       (20)      758 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/marker-blue.png
+-rw-r--r--   0 reinout    (501) staff       (20)      703 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/marker-gold.png
+-rw-r--r--   0 reinout    (501) staff       (20)      753 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/marker-green.png
+-rw-r--r--   0 reinout    (501) staff       (20)      601 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/marker.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3028 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/measuring-stick-off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3725 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/measuring-stick-on.png
+-rw-r--r--   0 reinout    (501) staff       (20)      298 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/north-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3511 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/panning-hand-off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3565 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/panning-hand-on.png
+-rw-r--r--   0 reinout    (501) staff       (20)      236 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/slider.png
+-rw-r--r--   0 reinout    (501) staff       (20)      310 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/south-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)      299 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/west-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)      229 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/zoom-minus-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)      276 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/zoom-plus-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)      545 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/zoom-world-mini.png
+-rw-r--r--   0 reinout    (501) staff       (20)      232 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/zoombar.png
+-rw-r--r--   0 reinout    (501) staff       (20)   770256 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/OpenLayers.js
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/
+-rw-r--r--   0 reinout    (501) staff       (20)      142 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/google.css
+-rw-r--r--   0 reinout    (501) staff       (20)      212 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/ie6-style.css
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/
+-rw-r--r--   0 reinout    (501) staff       (20)     1614 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/add_point_off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1464 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/add_point_on.png
+-rw-r--r--   0 reinout    (501) staff       (20)       42 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/blank.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1078 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/close.gif
+-rw-r--r--   0 reinout    (501) staff       (20)     1024 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/drag-rectangle-off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1041 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/drag-rectangle-on.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1565 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_line_off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1396 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_line_on.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1610 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_point_off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1458 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_point_on.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1544 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_polygon_off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1405 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_polygon_on.png
+-rw-r--r--   0 reinout    (501) staff       (20)     2222 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/editing_tool_bar.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1541 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/move_feature_off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1377 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/move_feature_on.png
+-rw-r--r--   0 reinout    (501) staff       (20)     6628 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/navigation_history.png
+-rw-r--r--   0 reinout    (501) staff       (20)       79 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/overview_replacement.gif
+-rw-r--r--   0 reinout    (501) staff       (20)      564 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan-panel-NOALPHA.png
+-rw-r--r--   0 reinout    (501) staff       (20)      814 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan-panel.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1696 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan_off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1566 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan_on.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3511 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/panning-hand-off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3565 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/panning-hand-on.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1612 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/remove_point_off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1461 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/remove_point_on.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1211 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/ruler.png
+-rw-r--r--   0 reinout    (501) staff       (20)      354 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/save_features_off.png
+-rw-r--r--   0 reinout    (501) staff       (20)      361 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/save_features_on.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1499 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_next_off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1686 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_next_on.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1476 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_previous_off.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1592 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_previous_on.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1173 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/zoom-panel-NOALPHA.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1285 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/zoom-panel.png
+-rw-r--r--   0 reinout    (501) staff       (20)    10791 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/style.css
+-rw-r--r--   0 reinout    (501) staff       (20)     1799 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/style.mobile.css
+-rw-r--r--   0 reinout    (501) staff       (20)     1263 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/README.blueprint
+-rw-r--r--   0 reinout    (501) staff       (20)     1738 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/README.bootstrap
+-rw-r--r--   0 reinout    (501) staff       (20)      197 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/README.colorpicker
+-rw-r--r--   0 reinout    (501) staff       (20)    18093 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/README.datatables
+-rw-r--r--   0 reinout    (501) staff       (20)      311 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/README.daterangepicker.txt
+-rw-r--r--   0 reinout    (501) staff       (20)      285 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/README.jquery
+-rw-r--r--   0 reinout    (501) staff       (20)      802 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/README.jqueryui
+-rw-r--r--   0 reinout    (501) staff       (20)       56 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/README.less
+-rw-r--r--   0 reinout    (501) staff       (20)      272 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/README.openlayers
+-rw-r--r--   0 reinout    (501) staff       (20)      137 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/README.sprites
+-rw-r--r--   0 reinout    (501) staff       (20)      436 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/README.treeview
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/static/sprites/
+-rw-r--r--   0 reinout    (501) staff       (20)     3223 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/calendar-light.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3084 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/calendar.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3200 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/clock-light.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3090 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/compass.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1410 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/direction.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1351 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/left_arrow.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1403 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/link.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3205 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/location-light.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3131 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/marker-light.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3005 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/marker.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1253 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/read_it_later.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)    49192 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/sprite.css
+-rw-r--r--   0 reinout    (501) staff       (20)   250121 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/sprites copy.png
+-rw-r--r--   0 reinout    (501) staff       (20)   294540 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/sprites.png
+-rw-r--r--   0 reinout    (501) staff       (20)     3051 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/star-light.png
+-rw-r--r--   0 reinout    (501) staff       (20)     1361 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/star.png
+-rwxr-xr-x   0 reinout    (501) staff       (20)    79454 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/test.htm
+-rw-r--r--   0 reinout    (501) staff       (20)     1184 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/trashbin-light.png
+-rw-r--r--   0 reinout    (501) staff       (20)      308 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/static/sprites/warning.png
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/templates/
+-rw-r--r--   0 reinout    (501) staff       (20)     1383 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/404.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1517 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/500.html
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/
+-rw-r--r--   0 reinout    (501) staff       (20)     1605 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/change_language.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1380 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/cmsbase.html
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/
+-rw-r--r--   0 reinout    (501) staff       (20)      569 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-appscreens.html
+-rw-r--r--   0 reinout    (501) staff       (20)      756 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-blocks-view.html
+-rw-r--r--   0 reinout    (501) staff       (20)     4475 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-blocks.html
+-rw-r--r--   0 reinout    (501) staff       (20)      923 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-breadcrumbs.html
+-rw-r--r--   0 reinout    (501) staff       (20)      342 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-cms-layout.html
+-rw-r--r--   0 reinout    (501) staff       (20)     2329 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-images.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1167 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-portaltabs.html
+-rw-r--r--   0 reinout    (501) staff       (20)      425 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-printbutton.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1118 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-table.html
+-rw-r--r--   0 reinout    (501) staff       (20)      392 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-textual.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1949 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_accordion1.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1256 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_accordion2.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1101 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_accordion3.html
+-rw-r--r--   0 reinout    (501) staff       (20)     2080 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_collapsible.html
+-rw-r--r--   0 reinout    (501) staff       (20)    95353 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_icons.html
+-rw-r--r--   0 reinout    (501) staff       (20)    30965 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_jqueryui.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1024 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_sidebarstretch.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1676 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_tree.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1131 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_vertical.html
+-rw-r--r--   0 reinout    (501) staff       (20)     2936 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/lizard-ui-introduction.html
+-rw-r--r--   0 reinout    (501) staff       (20)      648 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/icon_include.html
+-rw-r--r--   0 reinout    (501) staff       (20)      132 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/icons.html
+-rw-r--r--   0 reinout    (501) staff       (20)      289 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/lizardbase.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1342 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/login.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1637 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/modal_login.html
+-rw-r--r--   0 reinout    (501) staff       (20)    16524 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/realbase.html
+-rw-r--r--   0 reinout    (501) staff       (20)     1563 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templates/lizard_ui/tree_snippet.html
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui/templatetags/
+-rw-r--r--   0 reinout    (501) staff       (20)        9 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templatetags/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)     4444 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/templatetags/utility.py
+-rw-r--r--   0 reinout    (501) staff       (20)     6646 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/tests.py
+-rw-r--r--   0 reinout    (501) staff       (20)     3181 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/testsettings.py
+-rw-r--r--   0 reinout    (501) staff       (20)      514 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/uisettings.py
+-rw-r--r--   0 reinout    (501) staff       (20)     4902 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/urls.py
+-rw-r--r--   0 reinout    (501) staff       (20)    21934 2015-10-08 14:24:02.000000 lizard-ui-5.3/lizard_ui/views.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui.egg-info/
+-rw-r--r--   0 reinout    (501) staff       (20)        1 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 reinout    (501) staff       (20)       20 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui.egg-info/entry_points.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        1 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui.egg-info/not-zip-safe
+-rw-r--r--   0 reinout    (501) staff       (20)    52419 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui.egg-info/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)      182 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui.egg-info/requires.txt
+-rw-r--r--   0 reinout    (501) staff       (20)    62695 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 reinout    (501) staff       (20)       10 2015-10-08 14:24:03.000000 lizard-ui-5.3/lizard_ui.egg-info/top_level.txt
+-rw-r--r--   0 reinout    (501) staff       (20)      105 2015-10-08 14:24:02.000000 lizard-ui-5.3/MANIFEST.in
+-rw-r--r--   0 reinout    (501) staff       (20)    52419 2015-10-08 14:24:03.000000 lizard-ui-5.3/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)     9752 2015-10-08 14:24:02.000000 lizard-ui-5.3/README.rst
+-rw-r--r--   0 reinout    (501) staff       (20)      228 2015-10-08 14:24:03.000000 lizard-ui-5.3/setup.cfg
+-rw-r--r--   0 reinout    (501) staff       (20)     1313 2015-10-08 14:24:02.000000 lizard-ui-5.3/setup.py
+-rw-r--r--   0 reinout    (501) staff       (20)      501 2015-10-08 14:24:02.000000 lizard-ui-5.3/TODO.rst
```

### Comparing `lizard-ui-5.2/CHANGES.rst` & `lizard-ui-5.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 Changelog of lizard-ui
 ======================
 
 
+5.3 (2015-10-08)
+----------------
+
+- Moved language checker over to lizard-map. That way it can be enabled
+  through a ``Setting`` object.
+  [reinout]
+
+- Using correct session key for storing the language.
+  [reinout]
+
+
 5.2 (2015-10-08)
 ----------------
 
 - Started with arabic translation (only login/logout has been translated till
   now, though, as test).
   [reinout]
```

### Comparing `lizard-ui-5.2/LICENSE.rst` & `lizard-ui-5.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/admin.py` & `lizard-ui-5.3/lizard_ui/admin.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/configchecker.py` & `lizard-ui-5.3/lizard_ui/configchecker.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/docs/__init__.html` & `lizard-ui-5.3/lizard_ui/docs/__init__.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/docs/middleware.html` & `lizard-ui-5.3/lizard_ui/docs/middleware.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/docs/models.html` & `lizard-ui-5.3/lizard_ui/docs/models.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/docs/pycco.css` & `lizard-ui-5.3/lizard_ui/docs/pycco.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/docs/tests.html` & `lizard-ui-5.3/lizard_ui/docs/tests.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/docs/testsettings.html` & `lizard-ui-5.3/lizard_ui/docs/testsettings.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/docs/urls.html` & `lizard-ui-5.3/lizard_ui/docs/urls.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/docs/views.html` & `lizard-ui-5.3/lizard_ui/docs/views.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/forms.py` & `lizard-ui-5.3/lizard_ui/forms.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/layout.py` & `lizard-ui-5.3/lizard_ui/layout.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/af/LC_MESSAGES/django.mo` & `lizard-ui-5.3/lizard_ui/locale/af/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/af/LC_MESSAGES/django.po` & `lizard-ui-5.3/lizard_ui/locale/af/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/ar/LC_MESSAGES/django.mo` & `lizard-ui-5.3/lizard_ui/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/ar/LC_MESSAGES/django.po` & `lizard-ui-5.3/lizard_ui/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/ar/LC_MESSAGES/djangojs.po` & `lizard-ui-5.3/lizard_ui/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/en/LC_MESSAGES/django.po` & `lizard-ui-5.3/lizard_ui/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/en/LC_MESSAGES/djangojs.po` & `lizard-ui-5.3/lizard_ui/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/nl/LC_MESSAGES/django.mo` & `lizard-ui-5.3/lizard_ui/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/nl/LC_MESSAGES/django.po` & `lizard-ui-5.3/lizard_ui/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/nl/LC_MESSAGES/djangojs.mo` & `lizard-ui-5.3/lizard_ui/locale/nl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/nl/LC_MESSAGES/djangojs.po` & `lizard-ui-5.3/lizard_ui/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/vi/LC_MESSAGES/django.mo` & `lizard-ui-5.3/lizard_ui/locale/vi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/vi/LC_MESSAGES/django.po` & `lizard-ui-5.3/lizard_ui/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/zh/LC_MESSAGES/django.mo` & `lizard-ui-5.3/lizard_ui/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/locale/zh/LC_MESSAGES/django.po` & `lizard-ui-5.3/lizard_ui/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/management/commands/i18n.py` & `lizard-ui-5.3/lizard_ui/management/commands/i18n.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/migrations/0001_initial.py` & `lizard-ui-5.3/lizard_ui/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/migrations/0002_auto__chg_field_applicationscreen_description__chg_field_applicationic.py` & `lizard-ui-5.3/lizard_ui/migrations/0002_auto__chg_field_applicationscreen_description__chg_field_applicationic.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/migrations/0003_adding_description_field.py` & `lizard-ui-5.3/lizard_ui/migrations/0003_adding_description_field.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/migrations/0004_auto__add_field_applicationicon_sub_screen.py` & `lizard-ui-5.3/lizard_ui/migrations/0004_auto__add_field_applicationicon_sub_screen.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/migrations/0005_auto__chg_field_applicationicon_sub_screen__add_unique_applicationicon.py` & `lizard-ui-5.3/lizard_ui/migrations/0005_auto__chg_field_applicationicon_sub_screen__add_unique_applicationicon.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/migrations/0006_auto__add_field_applicationicon_data_set.py` & `lizard-ui-5.3/lizard_ui/migrations/0006_auto__add_field_applicationicon_data_set.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/migrations/0007_auto__add_customerlogo.py` & `lizard-ui-5.3/lizard_ui/migrations/0007_auto__add_customerlogo.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/models.py` & `lizard-ui-5.3/lizard_ui/models.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/settingshelper.py` & `lizard-ui-5.3/lizard_ui/settingshelper.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/ie.css` & `lizard-ui-5.3/lizard_ui/static/blueprint/ie.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/buttons/icons/cross.png` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/buttons/icons/cross.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/buttons/icons/tick.png` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/buttons/icons/tick.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/buttons/readme.txt` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/buttons/readme.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/buttons/screen.css` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/buttons/screen.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/fancy-type/screen.css` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/fancy-type/screen.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/doc.png` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/doc.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/email.png` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/email.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/external.png` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/external.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/feed.png` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/feed.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/im.png` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/im.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/pdf.png` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/pdf.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/visited.png` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/visited.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/icons/xls.png` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/icons/xls.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/link-icons/screen.css` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/link-icons/screen.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/plugins/rtl/screen.css` & `lizard-ui-5.3/lizard_ui/static/blueprint/plugins/rtl/screen.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/print.css` & `lizard-ui-5.3/lizard_ui/static/blueprint/print.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/screen.css` & `lizard-ui-5.3/lizard_ui/static/blueprint/screen.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/src/forms.css` & `lizard-ui-5.3/lizard_ui/static/blueprint/src/forms.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/src/grid.css` & `lizard-ui-5.3/lizard_ui/static/blueprint/src/grid.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/src/ie.css` & `lizard-ui-5.3/lizard_ui/static/blueprint/src/ie.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/src/print.css` & `lizard-ui-5.3/lizard_ui/static/blueprint/src/print.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/src/reset.css` & `lizard-ui-5.3/lizard_ui/static/blueprint/src/reset.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/blueprint/src/typography.css` & `lizard-ui-5.3/lizard_ui/static/blueprint/src/typography.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/css/bootstrap-responsive.css` & `lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/css/bootstrap-responsive.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/css/bootstrap-responsive.min.css` & `lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/css/bootstrap-responsive.min.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/css/bootstrap.css` & `lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/css/bootstrap.min.css` & `lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/js/bootstrap.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/bootstrap/js/bootstrap.min.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/CHANGELOG.md` & `lizard-ui-5.3/lizard_ui/static/bootstrap/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/CONTRIBUTING.md` & `lizard-ui-5.3/lizard_ui/static/bootstrap/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/css/bootstrap-responsive.css` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/css/bootstrap-responsive.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/css/bootstrap.css` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/css/docs.css` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/css/docs.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-114-precomposed.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-114-precomposed.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-144-precomposed.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-144-precomposed.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-57-precomposed.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-57-precomposed.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-72-precomposed.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/ico/apple-touch-icon-72-precomposed.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/ico/favicon.ico` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/ico/favicon.ico`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/ico/favicon.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/ico/favicon.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-docs-readme.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-docs-readme.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-mdo-sfmoma-01.jpg` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-mdo-sfmoma-01.jpg`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-mdo-sfmoma-02.jpg` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-mdo-sfmoma-02.jpg`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-mdo-sfmoma-03.jpg` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bootstrap-mdo-sfmoma-03.jpg`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-bootstrap-features.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-bootstrap-features.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-masthead-pattern.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-masthead-pattern.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-responsive-illustrations.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-responsive-illustrations.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-twitter-github.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/bs-docs-twitter-github.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/8020select.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/8020select.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/adoptahydrant.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/adoptahydrant.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/breakingnews.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/breakingnews.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/fleetio.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/fleetio.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/gathercontent.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/gathercontent.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/jshint.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/jshint.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/kippt.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/kippt.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/example-sites/soundready.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/example-sites/soundready.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-carousel.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-carousel.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-fluid.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-fluid.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-justified-nav.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-justified-nav.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-marketing-narrow.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-marketing-narrow.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-marketing.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-marketing.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-signin.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-signin.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-starter.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-starter.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-sticky-footer.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/bootstrap-example-sticky-footer.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/browser-icon-chrome.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/browser-icon-chrome.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/browser-icon-firefox.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/browser-icon-firefox.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/browser-icon-safari.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/browser-icon-safari.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/slide-01.jpg` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/slide-01.jpg`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/slide-02.jpg` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/slide-02.jpg`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/examples/slide-03.jpg` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/examples/slide-03.jpg`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/glyphicons-halflings-white.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/glyphicons-halflings.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/less-logo-large.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/less-logo-large.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/img/responsive-illustrations.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/img/responsive-illustrations.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/application.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/application.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-affix.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-affix.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-alert.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-alert.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-button.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-button.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-carousel.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-carousel.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-collapse.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-collapse.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-dropdown.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-dropdown.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-modal.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-modal.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-popover.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-popover.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-scrollspy.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-scrollspy.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-tab.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-tab.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-tooltip.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-tooltip.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-transition.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-transition.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-typeahead.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap-typeahead.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/bootstrap.min.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/google-code-prettify/prettify.css` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/google-code-prettify/prettify.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/google-code-prettify/prettify.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/google-code-prettify/prettify.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/holder/holder.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/holder/holder.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/html5shiv.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/html5shiv.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/jquery.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/jquery.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/assets/js/README.md` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/assets/js/README.md`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/base-css.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/base-css.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/components.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/components.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/customize.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/customize.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/carousel.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/carousel.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/fluid.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/fluid.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/hero.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/hero.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/justified-nav.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/justified-nav.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/marketing-narrow.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/marketing-narrow.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/signin.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/signin.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/starter-template.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/starter-template.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/sticky-footer-navbar.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/sticky-footer-navbar.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/examples/sticky-footer.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/examples/sticky-footer.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/extend.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/extend.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/getting-started.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/getting-started.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/index.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/index.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/javascript.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/javascript.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/scaffolding.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/scaffolding.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/layout.mustache` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/layout.mustache`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/base-css.mustache` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/base-css.mustache`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/components.mustache` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/components.mustache`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/customize.mustache` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/customize.mustache`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/extend.mustache` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/extend.mustache`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/getting-started.mustache` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/getting-started.mustache`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/index.mustache` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/index.mustache`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/javascript.mustache` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/javascript.mustache`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/docs/templates/pages/scaffolding.mustache` & `lizard-ui-5.3/lizard_ui/static/bootstrap/docs/templates/pages/scaffolding.mustache`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/img/glyphicons-halflings-white.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/img/glyphicons-halflings.png` & `lizard-ui-5.3/lizard_ui/static/bootstrap/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-affix.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-affix.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-alert.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-alert.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-button.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-button.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-carousel.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-carousel.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-collapse.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-collapse.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-dropdown.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-dropdown.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-modal.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-modal.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-popover.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-popover.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-scrollspy.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-scrollspy.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-tab.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-tab.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-tooltip.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-tooltip.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-transition.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-transition.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/bootstrap-typeahead.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/bootstrap-typeahead.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/index.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/index.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/phantom.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/phantom.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-affix.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-affix.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-alert.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-alert.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-button.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-button.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-carousel.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-carousel.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-collapse.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-collapse.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-dropdown.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-dropdown.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-modal.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-modal.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-phantom.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-phantom.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-popover.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-popover.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-scrollspy.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-scrollspy.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-tab.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-tab.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-tooltip.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-tooltip.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-typeahead.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/unit/bootstrap-typeahead.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/vendor/jquery.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/vendor/jquery.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/vendor/qunit.css` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/vendor/qunit.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/js/tests/vendor/qunit.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap/js/tests/vendor/qunit.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/accordion.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/accordion.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/alerts.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/alerts.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/bootstrap.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/bootstrap.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/button-groups.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/button-groups.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/buttons.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/buttons.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/carousel.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/carousel.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/close.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/close.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/code.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/code.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/dropdowns.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/dropdowns.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/font-awesome.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/font-awesome.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/forms.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/forms.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/hero-unit.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/hero-unit.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/labels-badges.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/labels-badges.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/lizard-bootstrap.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/lizard-bootstrap.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/media.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/media.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/mixins.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/mixins.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/modals.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/modals.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/navbar.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/navbar.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/navs.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/navs.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/pager.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/pager.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/pagination.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/pagination.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/popovers.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/popovers.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/progress-bars.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/progress-bars.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/reset.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/reset.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/responsive-1200px-min.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/responsive-1200px-min.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/responsive-767px-max.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/responsive-767px-max.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/responsive-navbar.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/responsive-navbar.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/responsive-utilities.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/responsive-utilities.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/responsive.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/responsive.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/scaffolding.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/scaffolding.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/sprites.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/sprites.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/tables.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/tables.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/buttons.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/buttons.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/css-tests.css` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/css-tests.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/css-tests.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/css-tests.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/forms-responsive.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/forms-responsive.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/forms.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/forms.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/navbar-fixed-top.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/navbar-fixed-top.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/navbar-static-top.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/navbar-static-top.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/tests/navbar.html` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/tests/navbar.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/thumbnails.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/thumbnails.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/tooltip.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/tooltip.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/type.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/type.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/variables.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/variables.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/less/wells.less` & `lizard-ui-5.3/lizard_ui/static/bootstrap/less/wells.less`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/LICENSE` & `lizard-ui-5.3/lizard_ui/static/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/Makefile` & `lizard-ui-5.3/lizard_ui/static/bootstrap/Makefile`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/package.json` & `lizard-ui-5.3/lizard_ui/static/bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap/README.md` & `lizard-ui-5.3/lizard_ui/static/bootstrap/README.md`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap-tour/bootstrap-tour.min.css` & `lizard-ui-5.3/lizard_ui/static/bootstrap-tour/bootstrap-tour.min.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/bootstrap-tour/bootstrap-tour.min.js` & `lizard-ui-5.3/lizard_ui/static/bootstrap-tour/bootstrap-tour.min.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/css/colorpicker.css` & `lizard-ui-5.3/lizard_ui/static/colorpicker/css/colorpicker.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/css/layout.css` & `lizard-ui-5.3/lizard_ui/static/colorpicker/css/layout.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_background.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_background.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_hex.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_hex.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_hsb_b.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_hsb_b.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_hsb_h.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_hsb_h.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_hsb_s.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_hsb_s.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_overlay.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_overlay.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_rgb_b.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_rgb_b.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_rgb_g.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_rgb_g.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_rgb_r.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_rgb_r.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/colorpicker_submit.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/colorpicker_submit.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_background.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_background.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_hex.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_hex.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_hsb_b.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_hsb_b.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_hsb_h.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_hsb_h.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_hsb_s.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_hsb_s.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_rgb_b.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_rgb_b.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_rgb_g.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_rgb_g.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_rgb_r.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_rgb_r.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/custom_submit.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/custom_submit.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/select2.png` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/select2.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/images/Thumbs.db` & `lizard-ui-5.3/lizard_ui/static/colorpicker/images/Thumbs.db`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/index.html` & `lizard-ui-5.3/lizard_ui/static/colorpicker/index.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/js/colorpicker.js` & `lizard-ui-5.3/lizard_ui/static/colorpicker/js/colorpicker.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/js/eye.js` & `lizard-ui-5.3/lizard_ui/static/colorpicker/js/eye.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/js/jquery.js` & `lizard-ui-5.3/lizard_ui/static/colorpicker/js/jquery.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/js/layout.js` & `lizard-ui-5.3/lizard_ui/static/colorpicker/js/layout.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/colorpicker/js/utils.js` & `lizard-ui-5.3/lizard_ui/static/colorpicker/js/utils.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/license-bsd.txt` & `lizard-ui-5.3/lizard_ui/static/datatables/license-bsd.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/license-gpl2.txt` & `lizard-ui-5.3/lizard_ui/static/datatables/license-gpl2.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/.DS_Store` & `lizard-ui-5.3/lizard_ui/static/datatables/media/.DS_Store`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/css/demo_page.css` & `lizard-ui-5.3/lizard_ui/static/datatables/media/css/demo_page.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/css/demo_table.css` & `lizard-ui-5.3/lizard_ui/static/datatables/media/css/demo_table.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/css/demo_table_jui.css` & `lizard-ui-5.3/lizard_ui/static/datatables/media/css/demo_table_jui.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/images/back_disabled.jpg` & `lizard-ui-5.3/lizard_ui/static/datatables/media/images/back_disabled.jpg`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/images/back_enabled.jpg` & `lizard-ui-5.3/lizard_ui/static/datatables/media/images/back_enabled.jpg`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/images/favicon.ico` & `lizard-ui-5.3/lizard_ui/static/datatables/media/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/images/forward_disabled.jpg` & `lizard-ui-5.3/lizard_ui/static/datatables/media/images/forward_disabled.jpg`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/images/forward_enabled.jpg` & `lizard-ui-5.3/lizard_ui/static/datatables/media/images/forward_enabled.jpg`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/images/Sorting icons.psd` & `lizard-ui-5.3/lizard_ui/static/datatables/media/images/Sorting icons.psd`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/js/jquery.dataTables.js` & `lizard-ui-5.3/lizard_ui/static/datatables/media/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/js/jquery.dataTables.min.js` & `lizard-ui-5.3/lizard_ui/static/datatables/media/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/js/jquery.dataTables.min.js.gz` & `lizard-ui-5.3/lizard_ui/static/datatables/media/js/jquery.dataTables.min.js.gz`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/media/js/jquery.js` & `lizard-ui-5.3/lizard_ui/static/datatables/media/js/jquery.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/datatables/Readme.txt` & `lizard-ui-5.3/lizard_ui/static/datatables/Readme.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/daterangepicker/daterangepicker.css` & `lizard-ui-5.3/lizard_ui/static/daterangepicker/daterangepicker.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/daterangepicker/daterangepicker.js` & `lizard-ui-5.3/lizard_ui/static/daterangepicker/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/daterangepicker/daterangepicker.orig.css` & `lizard-ui-5.3/lizard_ui/static/daterangepicker/daterangepicker.orig.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/daterangepicker/daterangepicker.orig.js` & `lizard-ui-5.3/lizard_ui/static/daterangepicker/daterangepicker.orig.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/daterangepicker/README.md` & `lizard-ui-5.3/lizard_ui/static/daterangepicker/README.md`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/font-awesome/font-awesome-ie7.min.css` & `lizard-ui-5.3/lizard_ui/static/font-awesome/font-awesome-ie7.min.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/font-awesome/fontawesome-webfont.eot` & `lizard-ui-5.3/lizard_ui/static/font-awesome/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/font-awesome/fontawesome-webfont.svg` & `lizard-ui-5.3/lizard_ui/static/font-awesome/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/font-awesome/fontawesome-webfont.ttf` & `lizard-ui-5.3/lizard_ui/static/font-awesome/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/font-awesome/fontawesome-webfont.woff` & `lizard-ui-5.3/lizard_ui/static/font-awesome/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/font-awesome/FontAwesome.otf` & `lizard-ui-5.3/lizard_ui/static/font-awesome/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/html5shiv/html5shiv.js` & `lizard-ui-5.3/lizard_ui/static/html5shiv/html5shiv.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery/jquery.min.js` & `lizard-ui-5.3/lizard_ui/static/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/excanvas.min.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/excanvas.min.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.colorhelpers.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.colorhelpers.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.axislabels.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.axislabels.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.categories.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.categories.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.crosshair.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.crosshair.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.errorbars.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.errorbars.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.fillbetween.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.fillbetween.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.image.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.image.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.navigate.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.navigate.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.pie.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.pie.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.resize.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.resize.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.selection.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.selection.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.stack.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.stack.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.symbol.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.symbol.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.threshold.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.threshold.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.time.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.time.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/jquery.flot.touch.js` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/jquery.flot.touch.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-flot/LICENSE.txt` & `lizard-ui-5.3/lizard_ui/static/jquery-flot/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-json/jquery.json-2.3.js` & `lizard-ui-5.3/lizard_ui/static/jquery-json/jquery.json-2.3.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-json/jquery.json-2.3.min.js` & `lizard-ui-5.3/lizard_ui/static/jquery-json/jquery.json-2.3.min.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-json/json2.js` & `lizard-ui-5.3/lizard_ui/static/jquery-json/json2.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-mobile-events/jquery.mobile-events.min.js` & `lizard-ui-5.3/lizard_ui/static/jquery-mobile-events/jquery.mobile-events.min.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-resize/jquery.ba-resize.js` & `lizard-ui-5.3/lizard_ui/static/jquery-resize/jquery.ba-resize.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-resize/jquery.ba-resize.min.js` & `lizard-ui-5.3/lizard_ui/static/jquery-resize/jquery.ba-resize.min.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-resize/LICENSE-GPL` & `lizard-ui-5.3/lizard_ui/static/jquery-resize/LICENSE-GPL`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-resize/LICENSE-MIT` & `lizard-ui-5.3/lizard_ui/static/jquery-resize/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-transform/jquery.transform-0.9.3.js` & `lizard-ui-5.3/lizard_ui/static/jquery-transform/jquery.transform-0.9.3.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-transform/jquery.transform-0.9.3.min.js` & `lizard-ui-5.3/lizard_ui/static/jquery-transform/jquery.transform-0.9.3.min.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/ajax-loader.gif` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/minus.gif` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/minus.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/plus.gif` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/plus.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-black-line.gif` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-black-line.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-black.gif` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-black.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-default-line.gif` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-default-line.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-default.gif` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-default.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-famfamfam.gif` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-famfamfam.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-gray-line.gif` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-gray-line.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-gray.gif` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-gray.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-red-line.gif` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-red-line.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/images/treeview-red.gif` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/images/treeview-red.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/jquery.treeview.async.js` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/jquery.treeview.async.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/jquery.treeview.css` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/jquery.treeview.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/jquery.treeview.edit.js` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/jquery.treeview.edit.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/jquery.treeview.js` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/jquery.treeview.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jquery-treeview/jquery.treeview.sortable.js` & `lizard-ui-5.3/lizard_ui/static/jquery-treeview/jquery.treeview.sortable.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jqueryui/jquery-ui.js` & `lizard-ui-5.3/lizard_ui/static/jqueryui/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jqueryui/jquery-ui.orig.js` & `lizard-ui-5.3/lizard_ui/static/jqueryui/jquery-ui.orig.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jqueryui/jquery.ui.datepicker-nl.js` & `lizard-ui-5.3/lizard_ui/static/jqueryui/jquery.ui.datepicker-nl.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-icons_222222_256x240.png` & `lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-icons_2e83ff_256x240.png` & `lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-icons_454545_256x240.png` & `lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-icons_888888_256x240.png` & `lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/images/ui-icons_cd0a0a_256x240.png` & `lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/jquery-ui.css` & `lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/jqueryui/smoothness/jquery-ui.orig.css` & `lizard-ui-5.3/lizard_ui/static/jqueryui/smoothness/jquery-ui.orig.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/less/less-1.2.1.min.js` & `lizard-ui-5.3/lizard_ui/static/less/less-1.2.1.min.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/60degree_gray.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/60degree_gray.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/ajax-loader.gif` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/ajax-loader2.gif` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/ajax-loader2.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/ajax-loader3.gif` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/ajax-loader3.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/ajax-loader4.gif` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/ajax-loader4.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/3di.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/3di.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/alkmaar.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/alkmaar.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/almere.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/almere.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/appicon_eleaf.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/appicon_eleaf.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/appicon_knmi.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/appicon_knmi.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/appicon_neo.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/appicon_neo.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/appicon_pwn.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/appicon_pwn.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/appicon_satapp.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/appicon_satapp.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/boek.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/boek.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/ciw.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/ciw.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/controlnext.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/controlnext.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/dacom.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/dacom.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/deltares.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/deltares.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/dike.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/dike.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/download.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/download.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/download_grijs.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/download_grijs.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/drought.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/drought.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/energieverbruik.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/energieverbruik.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/floodapp.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/floodapp.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/flooding.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/flooding.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/flooding2.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/flooding2.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/gisflow.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/gisflow.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/grondwater.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/grondwater.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/hdsr.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/hdsr.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/history.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/history.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/kaartlagen.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/kaartlagen.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/keringen.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/keringen.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/kpi.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/kpi.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/kustviewer.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/kustviewer.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/kwantiteit.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/kwantiteit.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/lcms.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/lcms.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/leveeportal.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/leveeportal.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/lizard.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/lizard.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/lizard_alarm.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/lizard_alarm.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/maatregelen.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/maatregelen.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/meetgegevens.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/meetgegevens.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/modelresultaten.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/modelresultaten.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/narrowcasting.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/narrowcasting.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/neerslag.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/neerslag.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/nhi.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/nhi.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/nieuwe_kaart_van_nederland.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/nieuwe_kaart_van_nederland.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/noorderpark.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/noorderpark.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/oevers.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/oevers.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/oppervlaktewater.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/oppervlaktewater.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/peilschaal.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/peilschaal.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/planning.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/planning.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/play.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/play.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/projecten.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/projecten.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/RegimeApp.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/RegimeApp.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/riolering.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/riolering.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/rws.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/rws.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/statistiek.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/statistiek.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/statusoverzicht.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/statusoverzicht.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/sticky.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/sticky.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/stowa.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/stowa.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/telecontrolnet.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/telecontrolnet.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/turtle.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/turtle.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/twitter.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/twitter.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/upload.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/upload.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/upload_grijs.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/upload_grijs.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/uploadserver.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/uploadserver.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/urk.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/urk.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/VerlorenBerging.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/VerlorenBerging.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/vss.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/vss.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/waterbalance.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/waterbalance.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/waterkwaliteit.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/waterkwaliteit.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/WIT.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/WIT.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/wms.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/wms.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/workspace_metingen.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/workspace_metingen.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/workspace_neerslag.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/workspace_neerslag.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/workspace_oppervlaktewater.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/workspace_oppervlaktewater.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/workspace_riolering.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/workspace_riolering.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/workspace_wateropstraat.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/workspace_wateropstraat.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/zettingen.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/zettingen.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/app_icons/zuiderzeeland.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/app_icons/zuiderzeeland.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/background.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/background.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/bar_background.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/bar_background.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/box-awesome.css` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/box-awesome.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/buttons.css` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/buttons.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/close.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/close.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/csrf.js` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/csrf.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/fabric_1.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/fabric_1.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/favicon.ico` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/icon-chart.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/icon-chart.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/icon-legend.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/icon-legend.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/leather_1.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/leather_1.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/lizard_ui.js` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/lizard_ui.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/logo.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/logo.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/old_mathematics.png` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/old_mathematics.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/OpenLayers.Control.NensLayerSwitcher.js` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/OpenLayers.Control.NensLayerSwitcher.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/print.css` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/print.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/lizard_ui/tabs.css` & `lizard-ui-5.3/lizard_ui/static/lizard_ui/tabs.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/momentjs/moment.js` & `lizard-ui-5.3/lizard_ui/static/momentjs/moment.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/momentjs/moment.min.js` & `lizard-ui-5.3/lizard_ui/static/momentjs/moment.min.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/momentjs/nl.js` & `lizard-ui-5.3/lizard_ui/static/momentjs/nl.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/authors.txt` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/authors.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/cloud-popup-relative.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/cloud-popup-relative.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/drag-rectangle-off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/drag-rectangle-off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/drag-rectangle-on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/drag-rectangle-on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/marker-blue.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/marker-blue.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/marker-gold.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/marker-gold.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/marker-green.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/marker-green.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/marker.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/marker.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/measuring-stick-off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/measuring-stick-off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/measuring-stick-on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/measuring-stick-on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/panning-hand-off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/panning-hand-off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/panning-hand-on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/panning-hand-on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/img/zoom-world-mini.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/img/zoom-world-mini.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/deprecated.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/deprecated.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebug.css` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebug.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebug.html` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebug.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebug.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/firebug.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/infoIcon.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/infoIcon.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/license.txt` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/license.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/readme.txt` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/readme.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/warningIcon.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Firebug/warningIcon.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Animation.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Animation.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Bounds.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Bounds.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Class.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Class.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Date.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Date.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Element.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Element.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/LonLat.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/LonLat.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Pixel.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Pixel.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Size.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes/Size.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/BaseTypes.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Console.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Console.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ArgParser.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ArgParser.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Attribution.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Attribution.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Button.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Button.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/CacheRead.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/CacheRead.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/CacheWrite.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/CacheWrite.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/DragFeature.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/DragFeature.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/DragPan.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/DragPan.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/DrawFeature.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/DrawFeature.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/EditingToolbar.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/EditingToolbar.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Geolocate.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Geolocate.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/GetFeature.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/GetFeature.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Graticule.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Graticule.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/KeyboardDefaults.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/KeyboardDefaults.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/LayerSwitcher.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/LayerSwitcher.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Measure.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Measure.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ModifyFeature.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ModifyFeature.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/MousePosition.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/MousePosition.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Navigation.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Navigation.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/NavigationHistory.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/NavigationHistory.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/NavToolbar.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/NavToolbar.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/OverviewMap.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/OverviewMap.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Pan.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Pan.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Panel.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Panel.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PanPanel.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PanPanel.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PanZoom.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PanZoom.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PanZoomBar.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PanZoomBar.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Permalink.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Permalink.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PinchZoom.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/PinchZoom.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Scale.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Scale.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ScaleLine.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ScaleLine.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/SelectFeature.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/SelectFeature.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/SLDSelect.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/SLDSelect.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Snapping.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Snapping.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Split.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Split.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/TouchNavigation.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/TouchNavigation.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/TransformFeature.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/TransformFeature.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/UTFGrid.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/UTFGrid.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/WMSGetFeatureInfo.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/WMSGetFeatureInfo.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/WMTSGetFeatureInfo.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/WMTSGetFeatureInfo.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Zoom.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/Zoom.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomBox.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomBox.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomIn.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomIn.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomOut.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomOut.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomPanel.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomPanel.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomToMaxExtent.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control/ZoomToMaxExtent.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Control.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Events/buttonclick.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Events/buttonclick.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Events.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Events.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Feature/Vector.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Feature/Vector.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Feature.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Feature.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Comparison.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Comparison.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/FeatureId.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/FeatureId.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Function.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Function.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Logical.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Logical.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Spatial.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter/Spatial.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Filter.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/ArcXML/Features.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/ArcXML/Features.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/ArcXML.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/ArcXML.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Atom.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Atom.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Context.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Context.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CQL.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CQL.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetDomain/v2_0_2.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetDomain/v2_0_2.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetDomain.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetDomain.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetRecords/v2_0_2.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetRecords/v2_0_2.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetRecords.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/CSWGetRecords.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/v1.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/v1.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/v1_0_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/v1_0_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/v1_1_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter/v1_1_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Filter.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GeoJSON.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GeoJSON.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GeoRSS.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GeoRSS.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/Base.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/Base.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/v2.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/v2.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/v3.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML/v3.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GML.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GPX.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/GPX.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/JSON.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/JSON.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/KML.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/KML.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OGCExceptionReport.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OGCExceptionReport.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OSM.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OSM.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/v1.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/v1.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/v1_0_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/v1_0_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/v1_1_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon/v1_1_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSCommon.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSContext/v0_3_1.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSContext/v0_3_1.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSContext.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/OWSContext.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/QueryStringFilter.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/QueryStringFilter.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/v1.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/v1.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/v1_0_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/v1_0_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/v1_0_0_GeoServer.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD/v1_0_0_GeoServer.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SLD.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSCapabilities/v1_0_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSCapabilities/v1_0_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSCapabilities.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSCapabilities.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSGetFeatureOfInterest.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSGetFeatureOfInterest.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSGetObservation.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/SOSGetObservation.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Text.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/Text.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WCSGetCoverage.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WCSGetCoverage.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFS.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFS.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/v1.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/v1.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/v1_0_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/v1_0_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/v1_1_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities/v1_1_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSCapabilities.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSDescribeFeatureType.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFSDescribeFeatureType.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/v1.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/v1.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/v1_0_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/v1_0_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/v1_1_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST/v1_1_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WFST.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WKT.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WKT.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/v1.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/v1.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/v1_0_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/v1_0_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/v1_1_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC/v1_1_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMC.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1_1.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1_1.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1_1_WMSC.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_1_1_WMSC.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_3.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_3.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_3_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities/v1_3_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSCapabilities.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSDescribeLayer/v1_1.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSDescribeLayer/v1_1.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSDescribeLayer.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSDescribeLayer.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSGetFeatureInfo.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMSGetFeatureInfo.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMTSCapabilities/v1_0_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMTSCapabilities/v1_0_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMTSCapabilities.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WMTSCapabilities.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSCapabilities/v1_0_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSCapabilities/v1_0_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSCapabilities.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSCapabilities.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSDescribeProcess.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSDescribeProcess.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSExecute.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/WPSExecute.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS/v1.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS/v1.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS/v1_1_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS/v1_1_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XLS.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XML/VersionedOGC.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XML/VersionedOGC.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XML.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format/XML.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Format.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Collection.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Collection.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Curve.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Curve.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/LinearRing.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/LinearRing.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/LineString.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/LineString.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/MultiLineString.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/MultiLineString.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/MultiPoint.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/MultiPoint.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/MultiPolygon.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/MultiPolygon.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Point.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Point.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Polygon.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry/Polygon.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Geometry.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Box.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Box.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Click.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Click.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Drag.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Drag.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Feature.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Feature.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Hover.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Hover.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Keyboard.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Keyboard.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/MouseWheel.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/MouseWheel.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Path.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Path.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Pinch.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Pinch.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Point.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Point.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Polygon.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/Polygon.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/RegularPolygon.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler/RegularPolygon.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Handler.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Icon.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Icon.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Kinetic.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Kinetic.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ar.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ar.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/be-tarask.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/be-tarask.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/bg.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/bg.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/br.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/br.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ca.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ca.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/cs-CZ.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/cs-CZ.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/da-DK.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/da-DK.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/de.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/de.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/en-CA.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/en-CA.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/en.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/en.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/es.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/es.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/fi.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/fi.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/fr.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/fr.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/fur.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/fur.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/gl.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/gl.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/gsw.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/gsw.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/hr.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/hr.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/hsb.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/hsb.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/hu.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/hu.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ia.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ia.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/id.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/id.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/is.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/is.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/it.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/it.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ja.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ja.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/km.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/km.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ksh.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ksh.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/lt.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/lt.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nb.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nb.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nds.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nds.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nl.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/nl.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/oc.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/oc.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/pl.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/pl.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/pt-BR.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/pt-BR.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/pt.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/pt.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ru.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/ru.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/sk.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/sk.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/sv-SE.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/sv-SE.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/te.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/te.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/vi.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/vi.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/zh-CN.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/zh-CN.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/zh-TW.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang/zh-TW.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Lang.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/ArcGIS93Rest.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/ArcGIS93Rest.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/ArcGISCache.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/ArcGISCache.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/ArcIMS.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/ArcIMS.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Bing.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Bing.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Boxes.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Boxes.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/EventPane.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/EventPane.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/FixedZoomLevels.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/FixedZoomLevels.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/GeoRSS.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/GeoRSS.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Google/v3.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Google/v3.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Google.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Google.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Grid.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Grid.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/HTTPRequest.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/HTTPRequest.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Image.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Image.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/KaMap.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/KaMap.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/KaMapCache.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/KaMapCache.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/MapGuide.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/MapGuide.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/MapServer.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/MapServer.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Markers.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Markers.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/OSM.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/OSM.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/PointGrid.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/PointGrid.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/PointTrack.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/PointTrack.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/SphericalMercator.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/SphericalMercator.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Text.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Text.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/TileCache.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/TileCache.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/TMS.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/TMS.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/UTFGrid.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/UTFGrid.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Vector/RootContainer.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Vector/RootContainer.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Vector.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Vector.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/WMS.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/WMS.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/WMTS.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/WMTS.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/WorldWind.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/WorldWind.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/XYZ.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/XYZ.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Zoomify.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer/Zoomify.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Layer.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Map.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Map.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Marker/Box.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Marker/Box.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Marker.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Marker.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/Anchored.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/Anchored.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/AnchoredBubble.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/AnchoredBubble.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/Framed.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/Framed.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/FramedCloud.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup/FramedCloud.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Popup.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Projection.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Projection.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/CSW/v2_0_2.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/CSW/v2_0_2.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/CSW.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/CSW.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/HTTP.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/HTTP.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/Script.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/Script.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/SOS/v1_0_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/SOS/v1_0_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/SOS.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/SOS.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/v1.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/v1.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/v1_0_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/v1_0_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/v1_1_0.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS/v1_1_0.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol/WFS.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Protocol.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/Canvas.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/Canvas.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/Elements.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/Elements.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/SVG.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/SVG.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/VML.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer/VML.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Renderer.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Request/XMLHttpRequest.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Request/XMLHttpRequest.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Request.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Request.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Rule.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Rule.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/SingleFile.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/SingleFile.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Spherical.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Spherical.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/BBOX.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/BBOX.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Cluster.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Cluster.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Filter.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Filter.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Fixed.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Fixed.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Paging.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Paging.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Refresh.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Refresh.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Save.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy/Save.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Strategy.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Style.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Style.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Style2.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Style2.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/StyleMap.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/StyleMap.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Line.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Line.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Point.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Point.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Polygon.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Polygon.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Raster.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Raster.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Text.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer/Text.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Symbolizer.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/Image/IFrame.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/Image/IFrame.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/Image.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/Image.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/UTFGrid.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile/UTFGrid.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tile.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tween.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Tween.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Util.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers/Util.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/OpenLayers.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Rico/Color.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Rico/Color.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Rico/Corner.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Rico/Corner.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/lib/Rico/license.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/lib/Rico/license.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/license.txt` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/license.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/licenses/APACHE-2.0.txt` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/licenses/APACHE-2.0.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/licenses/BSD-LICENSE.txt` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/licenses/BSD-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/licenses/MIT-LICENSE.txt` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/licenses/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/OpenLayers.debug.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/OpenLayers.debug.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/OpenLayers.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/OpenLayers.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/OpenLayers.light.debug.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/OpenLayers.light.debug.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/OpenLayers.light.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/OpenLayers.light.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/OpenLayers.mobile.debug.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/OpenLayers.mobile.debug.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/OpenLayers.mobile.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/OpenLayers.mobile.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/readme.md` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/readme.md`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/add_point_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/add_point_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/add_point_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/add_point_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/close.gif` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/close.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/drag-rectangle-off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/drag-rectangle-off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/drag-rectangle-on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/drag-rectangle-on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_line_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_line_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_line_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_line_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_point_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_point_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_point_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_point_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_polygon_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_polygon_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_polygon_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/draw_polygon_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/editing_tool_bar.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/editing_tool_bar.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/move_feature_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/move_feature_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/move_feature_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/move_feature_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/navigation_history.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/navigation_history.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan-panel-NOALPHA.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan-panel-NOALPHA.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan-panel.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan-panel.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/pan_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/panning-hand-off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/panning-hand-off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/panning-hand-on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/panning-hand-on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/remove_point_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/remove_point_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/remove_point_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/remove_point_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/ruler.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/ruler.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_next_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_next_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_next_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_next_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_previous_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_previous_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_previous_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/view_previous_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/zoom-panel-NOALPHA.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/zoom-panel-NOALPHA.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/img/zoom-panel.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/img/zoom-panel.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/style.css` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/style.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/style.mobile.css` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/style.mobile.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/style.mobile.tidy.css` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/style.mobile.tidy.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/theme/default/style.tidy.css` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/theme/default/style.tidy.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/BeautifulSoup.py` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/BeautifulSoup.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/closure_library_jscompiler.py` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/closure_library_jscompiler.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/closure_ws.py` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/closure_ws.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/exampleparser.py` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/exampleparser.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/jsmin.c` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/jsmin.c`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/jsmin.py` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/jsmin.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/mergejs.py` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/mergejs.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/minimize.py` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/minimize.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/oldot.py` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/oldot.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/README.txt` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/README.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/release.sh` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/release.sh`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/shrinksafe.py` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/shrinksafe.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/toposort.py` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/toposort.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.12-r7/tools/update_dev_dir.sh` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.12-r7/tools/update_dev_dir.sh`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/deprecated.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/deprecated.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/cloud-popup-relative.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/cloud-popup-relative.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/drag-rectangle-off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/drag-rectangle-off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/drag-rectangle-on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/drag-rectangle-on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/marker-blue.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/marker-blue.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/marker-gold.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/marker-gold.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/marker-green.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/marker-green.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/marker.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/marker.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/measuring-stick-off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/measuring-stick-off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/measuring-stick-on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/measuring-stick-on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/panning-hand-off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/panning-hand-off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/panning-hand-on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/panning-hand-on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/img/zoom-world-mini.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/img/zoom-world-mini.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/OpenLayers.js` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/OpenLayers.js`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/add_point_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/add_point_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/add_point_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/add_point_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/close.gif` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/close.gif`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/drag-rectangle-off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/drag-rectangle-off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/drag-rectangle-on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/drag-rectangle-on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_line_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_line_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_line_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_line_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_point_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_point_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_point_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_point_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_polygon_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_polygon_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_polygon_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/draw_polygon_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/editing_tool_bar.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/editing_tool_bar.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/move_feature_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/move_feature_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/move_feature_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/move_feature_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/navigation_history.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/navigation_history.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan-panel-NOALPHA.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan-panel-NOALPHA.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan-panel.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan-panel.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/pan_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/panning-hand-off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/panning-hand-off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/panning-hand-on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/panning-hand-on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/remove_point_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/remove_point_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/remove_point_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/remove_point_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/ruler.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/ruler.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_next_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_next_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_next_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_next_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_previous_off.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_previous_off.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_previous_on.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/view_previous_on.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/zoom-panel-NOALPHA.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/zoom-panel-NOALPHA.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/img/zoom-panel.png` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/img/zoom-panel.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/style.css` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/style.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/openlayers/1.13.1/theme/default/style.mobile.css` & `lizard-ui-5.3/lizard_ui/static/openlayers/1.13.1/theme/default/style.mobile.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/README.blueprint` & `lizard-ui-5.3/lizard_ui/static/README.blueprint`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/README.bootstrap` & `lizard-ui-5.3/lizard_ui/static/README.bootstrap`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/README.datatables` & `lizard-ui-5.3/lizard_ui/static/README.datatables`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/README.jqueryui` & `lizard-ui-5.3/lizard_ui/static/README.jqueryui`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/calendar-light.png` & `lizard-ui-5.3/lizard_ui/static/sprites/calendar-light.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/calendar.png` & `lizard-ui-5.3/lizard_ui/static/sprites/calendar.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/clock-light.png` & `lizard-ui-5.3/lizard_ui/static/sprites/clock-light.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/compass.png` & `lizard-ui-5.3/lizard_ui/static/sprites/compass.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/direction.png` & `lizard-ui-5.3/lizard_ui/static/sprites/direction.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/left_arrow.png` & `lizard-ui-5.3/lizard_ui/static/sprites/left_arrow.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/link.png` & `lizard-ui-5.3/lizard_ui/static/sprites/link.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/location-light.png` & `lizard-ui-5.3/lizard_ui/static/sprites/location-light.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/marker-light.png` & `lizard-ui-5.3/lizard_ui/static/sprites/marker-light.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/marker.png` & `lizard-ui-5.3/lizard_ui/static/sprites/marker.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/read_it_later.png` & `lizard-ui-5.3/lizard_ui/static/sprites/read_it_later.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/sprite.css` & `lizard-ui-5.3/lizard_ui/static/sprites/sprite.css`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/sprites copy.png` & `lizard-ui-5.3/lizard_ui/static/sprites/sprites copy.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/sprites.png` & `lizard-ui-5.3/lizard_ui/static/sprites/sprites.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/star-light.png` & `lizard-ui-5.3/lizard_ui/static/sprites/star-light.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/star.png` & `lizard-ui-5.3/lizard_ui/static/sprites/star.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/test.htm` & `lizard-ui-5.3/lizard_ui/static/sprites/test.htm`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/static/sprites/trashbin-light.png` & `lizard-ui-5.3/lizard_ui/static/sprites/trashbin-light.png`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/404.html` & `lizard-ui-5.3/lizard_ui/templates/404.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/500.html` & `lizard-ui-5.3/lizard_ui/templates/500.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/change_language.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/change_language.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/cmsbase.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/cmsbase.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-appscreens.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-appscreens.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-blocks-view.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-blocks-view.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-blocks.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-blocks.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-breadcrumbs.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-images.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-images.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-portaltabs.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-portaltabs.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example-table.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example-table.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_accordion1.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_accordion1.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_accordion2.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_accordion2.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_accordion3.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_accordion3.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_collapsible.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_collapsible.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_icons.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_icons.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_jqueryui.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_jqueryui.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_sidebarstretch.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_sidebarstretch.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_tree.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_tree.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/example_vertical.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/example_vertical.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/examples/lizard-ui-introduction.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/examples/lizard-ui-introduction.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/icon_include.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/icon_include.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/login.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/login.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/modal_login.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/modal_login.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/realbase.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/realbase.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templates/lizard_ui/tree_snippet.html` & `lizard-ui-5.3/lizard_ui/templates/lizard_ui/tree_snippet.html`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/templatetags/utility.py` & `lizard-ui-5.3/lizard_ui/templatetags/utility.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/tests.py` & `lizard-ui-5.3/lizard_ui/tests.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/testsettings.py` & `lizard-ui-5.3/lizard_ui/testsettings.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/uisettings.py` & `lizard-ui-5.3/lizard_ui/uisettings.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/urls.py` & `lizard-ui-5.3/lizard_ui/urls.py`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/lizard_ui/views.py` & `lizard-ui-5.3/lizard_ui/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 from django.shortcuts import get_object_or_404
 from django.shortcuts import render
 
 from django.template import Context, loader
 
 from django.utils.translation import check_for_language
-from django.utils.translation import get_language
 from django.utils.translation import ugettext as _
 
 from django.views.generic.base import TemplateView, View
 from django.views.generic.edit import FormView
 
 from lizard_ui.forms import LoginForm, ChangeLanguageForm
 from lizard_ui.layout import Action
@@ -163,15 +162,16 @@
             if request.is_ajax():
                 response = HttpResponse(json.dumps({'success': True}),
                                         mimetype='application/json')
             else:
                 response = HttpResponseRedirect(next)
             if lang_code and check_for_language(lang_code):
                 if hasattr(request, 'session'):
-                    request.session[settings.LANGUAGE_COOKIE_NAME] = lang_code
+                    request.session['django_language'] = lang_code
+                    # django_language is hardcoded, on 1.6 it isn't importable.
                 else:
                     response.set_cookie(settings.LANGUAGE_COOKIE_NAME, lang_code)
             return response
 
         if request.is_ajax():
             errors = ' '.join(form.non_field_errors())
             for fieldname, errorlist in form.errors.items():
@@ -297,34 +297,17 @@
         ``UI_SITE_ACTIONS`` are on the left, a login link (if
         ``UI_SHOW_LOGIN`` is True) on the right.
 
         """
         actions = copy(uisettings.SITE_ACTIONS)
 
         if uisettings.SHOW_LANGUAGE_PICKER:
-            languages = settings.LANGUAGES
-            if len(languages) > 1:
-                language_code = get_language()  # current language code
-                language_name = _('Language')  # sort of default
-                try:
-                    language_name = dict(settings.LANGUAGES)[language_code.lower()]
-                except KeyError:
-                    for code, name in languages:
-                        if language_code.lower().startswith(code):
-                            language_name = name
-                            break
-                query_string = urllib.urlencode(
-                    {'next': self.request.path_info})
-                lang_action = Action(icon='icon-flag')
-                lang_action.url = '%s?%s' % (
-                    reverse('lizard_ui.change_language'), query_string)
-                lang_action.name = language_name
-                lang_action.description = _('Pick a language')
-                lang_action.klass = 'ui-change-language-link'
-                actions.append(lang_action)
+            # Deprecated. It is now a admin-configurable setting
+            # (``show_language_picker``) in lizard-map
+            pass
 
         if uisettings.SHOW_LOGIN:
             query_string = urllib.urlencode({'next': self.request.path_info})
             if self.request.user.is_authenticated():
                 # Name of the user. TODO: link to profile page.
                 # The action is just text-with-an-icon right now.
                 action = Action(icon='icon-user')
```

### Comparing `lizard-ui-5.2/lizard_ui.egg-info/PKG-INFO` & `lizard-ui-5.3/lizard_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: lizard-ui
-Version: 5.2
+Version: 5.3
 Summary: Basic user interface for lizard websites
 Home-page: http://www.nelen-schuurmans.nl/lizard/
 Author: Reinout van Rees
 Author-email: reinout.vanrees@nelen-schuurmans.nl
 License: LGPL
 Description: lizard-ui
         =========
@@ -321,14 +321,25 @@
         - TODO started this library
         
         
         Changelog of lizard-ui
         ======================
         
         
+        5.3 (2015-10-08)
+        ----------------
+        
+        - Moved language checker over to lizard-map. That way it can be enabled
+          through a ``Setting`` object.
+          [reinout]
+        
+        - Using correct session key for storing the language.
+          [reinout]
+        
+        
         5.2 (2015-10-08)
         ----------------
         
         - Started with arabic translation (only login/logout has been translated till
           now, though, as test).
           [reinout]
```

### Comparing `lizard-ui-5.2/lizard_ui.egg-info/SOURCES.txt` & `lizard-ui-5.3/lizard_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/PKG-INFO` & `lizard-ui-5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: lizard-ui
-Version: 5.2
+Version: 5.3
 Summary: Basic user interface for lizard websites
 Home-page: http://www.nelen-schuurmans.nl/lizard/
 Author: Reinout van Rees
 Author-email: reinout.vanrees@nelen-schuurmans.nl
 License: LGPL
 Description: lizard-ui
         =========
@@ -321,14 +321,25 @@
         - TODO started this library
         
         
         Changelog of lizard-ui
         ======================
         
         
+        5.3 (2015-10-08)
+        ----------------
+        
+        - Moved language checker over to lizard-map. That way it can be enabled
+          through a ``Setting`` object.
+          [reinout]
+        
+        - Using correct session key for storing the language.
+          [reinout]
+        
+        
         5.2 (2015-10-08)
         ----------------
         
         - Started with arabic translation (only login/logout has been translated till
           now, though, as test).
           [reinout]
```

### Comparing `lizard-ui-5.2/README.rst` & `lizard-ui-5.3/README.rst`

 * *Files identical despite different names*

### Comparing `lizard-ui-5.2/setup.py` & `lizard-ui-5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '5.2'
+version = '5.3'
 
 long_description = '\n\n'.join([
     open('README.rst').read(),
     open('TODO.rst').read(),
     open('CREDITS.rst').read(),
     open('CHANGES.rst').read(),
     ])
```

