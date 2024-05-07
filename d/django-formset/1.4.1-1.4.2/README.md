# Comparing `tmp/django_formset-1.4.1.tar.gz` & `tmp/django_formset-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_formset-1.4.1.tar", last modified: Sat May  4 22:05:05 2024, max compression
+gzip compressed data, was "django_formset-1.4.2.tar", last modified: Tue May  7 12:43:58 2024, max compression
```

## Comparing `django_formset-1.4.1.tar` & `django_formset-1.4.2.tar`

### file list

```diff
@@ -1,470 +1,470 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.294127 django_formset-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-04 22:04:34.000000 django_formset-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-04 22:04:34.000000 django_formset-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-04 22:05:05.294127 django_formset-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-05-04 22:04:34.000000 django_formset-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.294127 django_formset-1.4.1/django_formset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-04 22:05:05.000000 django_formset-1.4.1/django_formset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-05-04 22:05:05.000000 django_formset-1.4.1/django_formset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 22:05:05.000000 django_formset-1.4.1/django_formset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 22:05:04.000000 django_formset-1.4.1/django_formset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 22:05:05.000000 django_formset-1.4.1/django_formset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 22:05:05.000000 django_formset-1.4.1/django_formset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.234125 django_formset-1.4.1/formset/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)    23321 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/fieldset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.234125 django_formset-1.4.1/formset/locale/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/af/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/af/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.234125 django_formset-1.4.1/formset/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.234125 django_formset-1.4.1/formset/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/bg/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/bg/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.234125 django_formset-1.4.1/formset/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/ca/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/ca/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.234125 django_formset-1.4.1/formset/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/cs/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/cs/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/da/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/da/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/el/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/el/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/eo/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/et/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/et/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/eu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/eu/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/eu_ES/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/eu_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/eu_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/fa/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/fa/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/fi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/fi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12714 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/he/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/he/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/he_IL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/he_IL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/he_IL/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/he_IL/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/hr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/hr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/hu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/hu/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/hy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/hy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/hy/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/hy/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/it/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/it/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/ja/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/ja/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/ko_KR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/lt/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/lt/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/lv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/lv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/mn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/mn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/mn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/mn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/nb/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/nl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/nl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/pl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/pt_PT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/ro/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/ro/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/sk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/sk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/sl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/sl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/sl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/sr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/sr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/sr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/sr_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/sr_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/sr_Latn_BA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/sr_Latn_BA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/sv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/sv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/tr_TR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/tr_TR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.254126 django_formset-1.4.1/formset/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12914 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/uk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.254126 django_formset-1.4.1/formset/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/zh_CN/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.254126 django_formset-1.4.1/formset/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.254126 django_formset-1.4.1/formset/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/ranges.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.254126 django_formset-1.4.1/formset/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/bulma.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/foundation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/tailwind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/uikit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.254126 django_formset-1.4.1/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/richtext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7894 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/richtext/controls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/richtext/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/richtext/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/richtext/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.226125 django_formset-1.4.1/formset/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.226125 django_formset-1.4.1/formset/static/formset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.258126 django_formset-1.4.1/formset/static/formset/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-04 22:05:00.000000 django_formset-1.4.1/formset/static/formset/css/bootstrap5-extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-04 22:05:00.000000 django_formset-1.4.1/formset/static/formset/css/bootstrap5-extra.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-04 22:05:00.000000 django_formset-1.4.1/formset/static/formset/css/collections.css
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-04 22:05:00.000000 django_formset-1.4.1/formset/static/formset/css/collections.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-05-04 22:05:01.000000 django_formset-1.4.1/formset/static/formset/css/tailwind.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.258126 django_formset-1.4.1/formset/static/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-zip.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.266126 django_formset-1.4.1/formset/static/formset/js/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/Calendar-SME4CT3M.js
--rw-r--r--   0 runner    (1001) docker     (127)    44541 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/CountrySelectize-6YQ6A6VY.js
--rw-r--r--   0 runner    (1001) docker     (127)    17740 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/DateTime-4XMVQT2P.js
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/DjangoSelectize-JMSV2QXX.js
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/DjangoSlug-SHZN726V.js
--rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/DualSelector-233VL6HH.js
--rw-r--r--   0 runner    (1001) docker     (127)   270393 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/PhoneNumber-KCJABOET.js
--rw-r--r--   0 runner    (1001) docker     (127)   313209 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/RichtextArea-QY2VVCDL.js
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/SortableSelect-27BKOQAW.js
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-65OJRBX6.js
--rw-r--r--   0 runner    (1001) docker     (127)    58061 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-CRVLB3K3.js
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-FDUUONAQ.js
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-NIKVGHIO.js
--rw-r--r--   0 runner    (1001) docker     (127)    44439 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-NOGHTXP6.js
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-P2VM2T3G.js
--rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-QHDAXJJP.js
--rw-r--r--   0 runner    (1001) docker     (127)    15239 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-RLE6ONWJ.js
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-SERXULES.js
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-W5RPWA2M.js
--rw-r--r--   0 runner    (1001) docker     (127)    68979 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-XQYS6DVW.js
--rw-r--r--   0 runner    (1001) docker     (127)    63654 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/django-formset.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.266126 django_formset-1.4.1/formset/static/formset/tiptap-extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/tiptap-extensions/footnote.js
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/tiptap-extensions/procurator.js
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/tiptap-extensions/simple_image.js
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/tiptap-extensions/simple_link.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.230125 django_formset-1.4.1/formset/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.226125 django_formset-1.4.1/formset/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.266126 django_formset-1.4.1/formset/templates/admin/formset/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/admin/formset/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.266126 django_formset-1.4.1/formset/templates/calendar/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/calendar/hours.html
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/calendar/months.html
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/calendar/range.html
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/calendar/weeks.html
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/calendar/years.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.266126 django_formset-1.4.1/formset/templates/formset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.266126 django_formset-1.4.1/formset/templates/formset/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.270126 django_formset-1.4.1/formset/templates/formset/bootstrap/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/form.html
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.270126 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/richtextarea.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.270126 django_formset-1.4.1/formset/templates/formset/bulma/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.270126 django_formset-1.4.1/formset/templates/formset/bulma/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.270126 django_formset-1.4.1/formset/templates/formset/bulma/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/widgets/select.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.274126 django_formset-1.4.1/formset/templates/formset/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.274126 django_formset-1.4.1/formset/templates/formset/default/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/move_all_left.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/move_all_right.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/move_selected_left.html
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/move_selected_right.html
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/redo_selected.html
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/undo_selected.html
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/detached_field.html
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/field_errors.html
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/form_dialog.html
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.278126 django_formset-1.4.1/formset/templates/formset/default/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/button.html
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/calendar.html
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/country_selectize.html
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/datetime.html
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/richtextarea.html
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/selectize.html
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/form_attrs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.278126 django_formset-1.4.1/formset/templates/formset/foundation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.278126 django_formset-1.4.1/formset/templates/formset/foundation/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.278126 django_formset-1.4.1/formset/templates/formset/foundation/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/widgets/inlined_input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.286127 django_formset-1.4.1/formset/templates/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/activator.svg
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/add-fill.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/align-center.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/align-justify.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/align-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/align-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/arrow-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/arrow-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/blockquote.svg
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/bold.svg
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/bulletlist.svg
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/calendar-today.svg
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/chevron-double-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/chevron-double-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/clearformat.svg
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/codeblock.svg
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/decreasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/delete-back.svg
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/double-chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/double-chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/footnote.svg
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/hardbreak.svg
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading.svg
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading3.svg
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading4.svg
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading5.svg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading6.svg
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/horizontalrule.svg
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/increasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/indentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/italic.svg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/letters.svg
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/link.svg
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/orderedlist.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/outdentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/placeholder.svg
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/questionmark.svg
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/redo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/reset.svg
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/send.svg
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/separator.svg
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/strike.svg
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/subscript.svg
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/superscript.svg
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/textcolor.svg
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/trash.svg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/underline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/undo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/unlink.svg
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/non_field_errors.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/align.html
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/color.html
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/control.html
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/dialog_control.html
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/form_dialog.html
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/separator.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/tailwind/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/tailwind/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/form.html
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/radio.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/uikit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/uikit/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/uikit/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.294127 django_formset-1.4.1/formset/templates/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/bulletlist.html
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/doc.html
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/footnote.html
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/footnote_ref.html
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/footnotes_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/horizontalrule.html
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/listitem.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.294127 django_formset-1.4.1/formset/templates/richtext/marks/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/bold.html
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/code.html
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/italic.html
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/procurator.html
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/simple_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/textcolor.html
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/underline.html
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/orderedlist.html
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/paragraph.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.294127 django_formset-1.4.1/formset/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templatetags/formsetify.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templatetags/phonenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templatetags/richtext.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12184 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 22:05:05.294127 django_formset-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-04 22:04:34.000000 django_formset-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.422795 django_formset-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 12:43:26.000000 django_formset-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 12:43:26.000000 django_formset-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-07 12:43:58.418795 django_formset-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-05-07 12:43:26.000000 django_formset-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.418795 django_formset-1.4.2/django_formset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-07 12:43:58.000000 django_formset-1.4.2/django_formset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-05-07 12:43:58.000000 django_formset-1.4.2/django_formset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:43:58.000000 django_formset-1.4.2/django_formset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:43:58.000000 django_formset-1.4.2/django_formset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 12:43:58.000000 django_formset-1.4.2/django_formset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 12:43:58.000000 django_formset-1.4.2/django_formset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.370796 django_formset-1.4.2/formset/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23321 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/fieldset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.350796 django_formset-1.4.2/formset/locale/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.370796 django_formset-1.4.2/formset/locale/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/af/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/af/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.350796 django_formset-1.4.2/formset/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.370796 django_formset-1.4.2/formset/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.350796 django_formset-1.4.2/formset/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.370796 django_formset-1.4.2/formset/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/bg/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/bg/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.350796 django_formset-1.4.2/formset/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/ca/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/ca/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.350796 django_formset-1.4.2/formset/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/cs/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/cs/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/da/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/da/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/de/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/el/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/el/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/eo/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/et/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/et/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/eu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/eu/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/eu_ES/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/eu_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/fa/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/fa/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/fi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/fi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12714 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/he/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/he/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/he_IL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/he_IL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/he_IL/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/he_IL/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/hr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/hr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/hu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/hu/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/hy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/hy/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/hy/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/it/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/it/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/ja/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/ja/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/ko_KR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/lt/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/lt/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/lv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/lv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/mn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/mn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/mn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/nb/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/nl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/nl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/pl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/pl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/pt_PT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/ro/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/ro/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/sk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/sk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/sl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/sl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/sr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/sr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/sr_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/sr_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/sr_Latn_BA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/sr_Latn_BA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/sv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/sv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/tr_TR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/tr_TR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12914 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/uk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/zh_CN/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.390796 django_formset-1.4.2/formset/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/ranges.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.390796 django_formset-1.4.2/formset/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/bulma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/tailwind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/uikit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.390796 django_formset-1.4.2/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/richtext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7894 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/richtext/controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/richtext/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/richtext/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/richtext/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/static/formset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.390796 django_formset-1.4.2/formset/static/formset/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-07 12:43:53.000000 django_formset-1.4.2/formset/static/formset/css/bootstrap5-extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-07 12:43:53.000000 django_formset-1.4.2/formset/static/formset/css/bootstrap5-extra.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-07 12:43:53.000000 django_formset-1.4.2/formset/static/formset/css/collections.css
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-07 12:43:53.000000 django_formset-1.4.2/formset/static/formset/css/collections.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-05-07 12:43:54.000000 django_formset-1.4.2/formset/static/formset/css/tailwind.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.394796 django_formset-1.4.2/formset/static/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-zip.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/static/formset/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/Calendar-5KXZG25G.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44541 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/CountrySelectize-RPAYKZSN.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17740 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/DateTime-WW4TXK6Y.js
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/DjangoSelectize-XUOHPSUG.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/DjangoSlug-SHZN726V.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/DualSelector-G47GXWWH.js
+-rw-r--r--   0 runner    (1001) docker     (127)   270393 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/PhoneNumber-RCXY4VXK.js
+-rw-r--r--   0 runner    (1001) docker     (127)   313209 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/RichtextArea-34WSI64S.js
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/SortableSelect-6YQLVCNF.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-65OJRBX6.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58061 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-6IBLXZPA.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68979 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-B7PX5YAU.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-FDUUONAQ.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44439 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-NOGHTXP6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-P2VM2T3G.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15239 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-RLE6ONWJ.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-SERXULES.js
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-W5RPWA2M.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-WKRSL2PQ.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-XO2BBJ6P.js
+-rw-r--r--   0 runner    (1001) docker     (127)    63688 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/django-formset.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/static/formset/tiptap-extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/tiptap-extensions/footnote.js
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/tiptap-extensions/procurator.js
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/tiptap-extensions/simple_image.js
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/tiptap-extensions/simple_link.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.366796 django_formset-1.4.2/formset/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/templates/admin/formset/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/admin/formset/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/templates/calendar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/calendar/hours.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/calendar/months.html
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/calendar/range.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/calendar/weeks.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/calendar/years.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/templates/formset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/templates/formset/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/templates/formset/bootstrap/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/richtextarea.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.402796 django_formset-1.4.2/formset/templates/formset/bulma/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.402796 django_formset-1.4.2/formset/templates/formset/bulma/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.402796 django_formset-1.4.2/formset/templates/formset/bulma/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/widgets/select.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.402796 django_formset-1.4.2/formset/templates/formset/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.402796 django_formset-1.4.2/formset/templates/formset/default/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/move_all_left.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/move_all_right.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/move_selected_left.html
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/move_selected_right.html
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/redo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/undo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/detached_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/field_errors.html
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/form_dialog.html
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.406796 django_formset-1.4.2/formset/templates/formset/default/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/country_selectize.html
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/datetime.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/richtextarea.html
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/selectize.html
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/form_attrs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.406796 django_formset-1.4.2/formset/templates/formset/foundation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.406796 django_formset-1.4.2/formset/templates/formset/foundation/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.406796 django_formset-1.4.2/formset/templates/formset/foundation/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/widgets/inlined_input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/activator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/add-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/align-center.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/align-justify.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/align-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/align-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/arrow-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/arrow-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/blockquote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/bold.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/bulletlist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/calendar-today.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/chevron-double-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/chevron-double-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/clearformat.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/codeblock.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/decreasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/delete-back.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/double-chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/double-chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/footnote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/hardbreak.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/horizontalrule.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/increasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/indentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/italic.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/letters.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/link.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/orderedlist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/outdentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/placeholder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/questionmark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/reset.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/send.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/separator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/strike.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/subscript.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/superscript.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/textcolor.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/underline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/unlink.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/non_field_errors.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/align.html
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/color.html
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/control.html
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/dialog_control.html
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/form_dialog.html
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/separator.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/tailwind/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/tailwind/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/radio.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/uikit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/uikit/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/uikit/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.418795 django_formset-1.4.2/formset/templates/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/bulletlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/doc.html
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/footnote.html
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/footnote_ref.html
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/footnotes_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/horizontalrule.html
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/listitem.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.418795 django_formset-1.4.2/formset/templates/richtext/marks/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/bold.html
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/code.html
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/italic.html
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/procurator.html
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/simple_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/textcolor.html
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/underline.html
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/orderedlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.418795 django_formset-1.4.2/formset/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templatetags/formsetify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templatetags/phonenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templatetags/richtext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12184 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21405 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 12:43:58.422795 django_formset-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-07 12:43:26.000000 django_formset-1.4.2/setup.py
```

### Comparing `django_formset-1.4.1/LICENSE` & `django_formset-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/PKG-INFO` & `django_formset-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.4.1
+Version: 1.4.2
 Summary: The missing widgets and form manipulation library for Django
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django_formset-1.4.1/README.md` & `django_formset-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/django_formset.egg-info/PKG-INFO` & `django_formset-1.4.2/django_formset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.4.1
+Version: 1.4.2
 Summary: The missing widgets and form manipulation library for Django
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django_formset-1.4.1/django_formset.egg-info/SOURCES.txt` & `django_formset-1.4.2/django_formset.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -136,34 +136,34 @@
 formset/static/formset/icons/file-font.svg
 formset/static/formset/icons/file-missing.svg
 formset/static/formset/icons/file-pdf.svg
 formset/static/formset/icons/file-picture.svg
 formset/static/formset/icons/file-unknown.svg
 formset/static/formset/icons/file-video.svg
 formset/static/formset/icons/file-zip.svg
-formset/static/formset/js/Calendar-SME4CT3M.js
-formset/static/formset/js/CountrySelectize-6YQ6A6VY.js
-formset/static/formset/js/DateTime-4XMVQT2P.js
-formset/static/formset/js/DjangoSelectize-JMSV2QXX.js
+formset/static/formset/js/Calendar-5KXZG25G.js
+formset/static/formset/js/CountrySelectize-RPAYKZSN.js
+formset/static/formset/js/DateTime-WW4TXK6Y.js
+formset/static/formset/js/DjangoSelectize-XUOHPSUG.js
 formset/static/formset/js/DjangoSlug-SHZN726V.js
-formset/static/formset/js/DualSelector-233VL6HH.js
-formset/static/formset/js/PhoneNumber-KCJABOET.js
-formset/static/formset/js/RichtextArea-QY2VVCDL.js
-formset/static/formset/js/SortableSelect-27BKOQAW.js
+formset/static/formset/js/DualSelector-G47GXWWH.js
+formset/static/formset/js/PhoneNumber-RCXY4VXK.js
+formset/static/formset/js/RichtextArea-34WSI64S.js
+formset/static/formset/js/SortableSelect-6YQLVCNF.js
 formset/static/formset/js/chunk-65OJRBX6.js
-formset/static/formset/js/chunk-CRVLB3K3.js
+formset/static/formset/js/chunk-6IBLXZPA.js
+formset/static/formset/js/chunk-B7PX5YAU.js
 formset/static/formset/js/chunk-FDUUONAQ.js
-formset/static/formset/js/chunk-NIKVGHIO.js
 formset/static/formset/js/chunk-NOGHTXP6.js
 formset/static/formset/js/chunk-P2VM2T3G.js
-formset/static/formset/js/chunk-QHDAXJJP.js
 formset/static/formset/js/chunk-RLE6ONWJ.js
 formset/static/formset/js/chunk-SERXULES.js
 formset/static/formset/js/chunk-W5RPWA2M.js
-formset/static/formset/js/chunk-XQYS6DVW.js
+formset/static/formset/js/chunk-WKRSL2PQ.js
+formset/static/formset/js/chunk-XO2BBJ6P.js
 formset/static/formset/js/django-formset.js
 formset/static/formset/tiptap-extensions/footnote.js
 formset/static/formset/tiptap-extensions/procurator.js
 formset/static/formset/tiptap-extensions/simple_image.js
 formset/static/formset/tiptap-extensions/simple_link.js
 formset/templates/admin/formset/change_form.html
 formset/templates/calendar/hours.html
```

### Comparing `django_formset-1.4.1/formset/boundfield.py` & `django_formset-1.4.2/formset/boundfield.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/calendar.py` & `django_formset-1.4.2/formset/calendar.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/collection.py` & `django_formset-1.4.2/formset/collection.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/dialog.py` & `django_formset-1.4.2/formset/dialog.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/fields.py` & `django_formset-1.4.2/formset/fields.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/fieldset.py` & `django_formset-1.4.2/formset/fieldset.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/af/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/af/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/af/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/af/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/ar/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/ar/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/bg/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/bg/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/bg/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/bg/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/ca/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/ca/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/ca/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/ca/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/cs/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/cs/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/cs/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/da/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/da/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/da/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/da/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/de/LC_MESSAGES/django.po` & `django_formset-1.4.2/formset/locale/de/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -41,119 +41,119 @@
 msgid "Input value must be a multiple of {step_value}."
 msgstr ""
 "Bitte sicherstellen, dass der Wert aus einem Vielfachen von {step_value} "
 "besteht."
 
 #: boundfield.py:206
 msgid "Please enter a valid mobile number."
-msgstr ""
+msgstr "Bitte geben Sie eine gültige Mobilfunknummer ein."
 
 #: boundfield.py:208
 msgid "Please enter a valid phone number."
-msgstr ""
+msgstr "Bitte geben Sie eine gültige Telefonnummer ein."
 
 #: boundfield.py:217
 msgid "File upload still in progress."
 msgstr "Datei wird noch immer hochgeladen."
 
 #: boundfield.py:218
 msgid "File upload failed."
 msgstr "Datei-Upload ist fehlgeschlagen."
 
 #: collection.py:327
 #, python-brace-format
 msgid "Please correct the duplicate data for {0}."
-msgstr ""
+msgstr "Bitte korrigieren Sie die Duplikate für {0}."
 
 #: collection.py:329
 msgid "and"
-msgstr ""
+msgstr "und"
 
 #: collection.py:330
 #, python-brace-format
 msgid "Please correct the duplicate data for {0}, which must be unique."
-msgstr ""
+msgstr "Bitte korrigieren Sie die Duplikate für {0}, sie müssen eindeutig sein."
 
 #: collection.py:343
 #, python-brace-format
 msgid "Not enough entries in “{collection_name}”, please add another."
-msgstr ""
+msgstr "Nicht genügend Einträge in “{collection_name}”, bitte fügen Sie etwas ein."
 
 #: collection.py:347
 #, python-brace-format
 msgid "Too many entries in “{collection_name}”, please remove one."
-msgstr ""
+msgstr "Zu viele Einträge in “{collection_name}”, bitte entfernen Sie einen."
 
 #: ranges.py:85
 msgid "Enter two valid values."
-msgstr ""
+msgstr "Zwei gültige Werte eingeben."
 
 #: ranges.py:86
 msgid "The start of the range must not exceed the end of the range."
-msgstr ""
+msgstr "Der Anfang des Bereichs darf das Ende des Bereichs nicht überschreiten."
 
 #: ranges.py:122
 msgid "Enter two valid dates."
-msgstr ""
+msgstr "Zwei gültige Daten eingeben."
 
 #: ranges.py:123
 msgid "The start date must be before the end date."
-msgstr ""
+msgstr "Das Anfangsdatum muss vor dem Enddatum liegen."
 
 #: richtext/controls.py:39
 #: templates/formset/default/buttons/richtext_heading.html:4
 #: templates/formset/default/buttons/richtext_heading.html:7
 #: templates/formset/default/buttons/richtext_heading.html:8
 msgid "Heading"
 msgstr "Überschrift"
 
 #: richtext/controls.py:57
 #: templates/formset/default/buttons/richtext_align.html:4
 #: templates/formset/default/buttons/richtext_align.html:8
 #: templates/formset/default/buttons/richtext_align.html:10
 msgid "Text Align"
-msgstr ""
+msgstr "Textausrichtung"
 
 #: richtext/controls.py:96
 #: templates/formset/default/buttons/richtext_color.html:2
 #: templates/formset/default/buttons/richtext_color.html:3
 msgid "Text Color"
-msgstr ""
+msgstr "Textfarbe"
 
 #: richtext/controls.py:129
 msgid "Indent First Line"
-msgstr ""
+msgstr "Erste Zeile einrücken"
 
 #: richtext/controls.py:133
 msgid "Outdent First Line"
-msgstr ""
+msgstr "Erste Zeile ausrücken"
 
 #: richtext/controls.py:143
 msgid "Increase Margin"
-msgstr ""
+msgstr "Abstand vergrößern"
 
 #: richtext/controls.py:147
 msgid "Decrease Margin"
-msgstr ""
+msgstr "Abstand verkleinern"
 
 #: richtext/controls.py:155
 msgid "Bold"
 msgstr "Fett"
 
 #: richtext/controls.py:160
 msgid "Blockquote"
-msgstr ""
+msgstr "Blockzitat"
 
 #: richtext/controls.py:165
 msgid "Code Block"
-msgstr ""
+msgstr "Codeblock"
 
 #: richtext/controls.py:170
 msgid "Hard Break"
-msgstr ""
+msgstr "Zeilenumbruch"
 
 #: richtext/controls.py:175
 msgid "Italic"
 msgstr "Kursiv"
 
 #: richtext/controls.py:180
 msgid "Underline"
@@ -173,67 +173,67 @@
 
 #: richtext/controls.py:200
 msgid "Clear Format"
 msgstr "Format zurücksetzen"
 
 #: richtext/controls.py:205
 msgid "Subscript"
-msgstr ""
+msgstr "Hochgestellt"
 
 #: richtext/controls.py:210
 msgid "Superscript"
-msgstr ""
+msgstr "Tiefgestellt"
 
 #: richtext/controls.py:215
 msgid "Undo"
 msgstr "Rückgängig machen"
 
 #: richtext/controls.py:220
 msgid "Redo"
 msgstr "Nochmals machen"
 
 #: richtext/controls.py:225 richtext/dialogs.py:31
 msgid "Link"
-msgstr ""
+msgstr "Link"
 
 #: richtext/controls.py:231 richtext/dialogs.py:42
 msgid "Image"
 msgstr "Bild"
 
 #: richtext/controls.py:237
 msgid "Placeholder"
-msgstr ""
+msgstr "Platzhalter"
 
 #: richtext/controls.py:242
 msgid "Separator"
 msgstr "Trennzeichen"
 
 #: richtext/dialogs.py:22
 msgid "Edit Link"
 msgstr "Link ändern"
 
 #: richtext/dialogs.py:27
 msgid "Text"
-msgstr ""
+msgstr "Text"
 
 #: richtext/dialogs.py:37
 msgid "Edit Image"
 msgstr "Bild ändern"
 
 #: richtext/dialogs.py:48
 msgid "Edit Placeholder"
-msgstr ""
+msgstr "Platzhalter bearbeiten"
 
 #: richtext/dialogs.py:54
 msgid "Variable Name"
-msgstr ""
+msgstr "Variablenname"
 
 #: richtext/dialogs.py:58
 msgid "Sample Text"
-msgstr ""
+msgstr "Beispieltext"
 
 #: templates/calendar/hours.html:3
 msgid "Previous day"
 msgstr "Vorhergehender Tag"
 
 #: templates/calendar/hours.html:6 templates/calendar/months.html:9
 #: templates/calendar/weeks.html:6
```

### Comparing `django_formset-1.4.1/formset/locale/de/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/de/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/el/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/el/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/el/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/el/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/eo/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/eo/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/eo/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/es/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/es/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/et/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/et/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/et/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/et/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/eu/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/eu/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/eu/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/eu/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/eu_ES/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/eu_ES/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/fa/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/fa/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/fa/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/fa/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/fi/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/fi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/fi/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/fi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/fr/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/fr/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/he/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/he/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/he/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/he/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/he_IL/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/he_IL/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/he_IL/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/he_IL/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/hr/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/hr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/hr/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/hr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/hu/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/hu/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/hu/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/hu/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/hy/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/hy/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/hy/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/hy/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/it/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/it/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/ja/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/ja/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/ja/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/ja/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/ko_KR/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/ko_KR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/lt/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/lt/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/lt/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/lt/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/lv/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/lv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/lv/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/lv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/mn/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/mn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/mn/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/mn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/nb/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/nb/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/nb/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/nl/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/nl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/nl/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/pl/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/pl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/pl/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/pt_BR/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/pt_PT/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/ro/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/ro/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/ro/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/ro/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/ru/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/ru/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/sk/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/sk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/sk/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/sk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/sl/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/sl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/sl/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/sl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/sr/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/sr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/sr/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/sr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/sv/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/sv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/sv/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/sv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/tr_TR/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/uk/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/uk/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/zh_CN/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/zh_CN/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.2/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po` & `django_formset-1.4.2/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/ranges.py` & `django_formset-1.4.2/formset/ranges.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,77 +6,77 @@
 
 class DateRangeCalendar(DateCalendar):
     template_name = 'formset/default/widgets/calendar.html'
 
     def __init__(self, attrs=None, calendar_renderer=None):
         default_attrs = {
             'type': 'regex',
-            'pattern': r'^\d{4}-\d{2}-\d{2};\d{4}-\d{2}-\d{2}$',
+            'pattern': r'\d{4}-\d{2}-\d{2};\d{4}-\d{2}-\d{2}',
             'is': 'django-daterangecalendar',
         }
         if attrs:
             default_attrs.update(**attrs)
         super().__init__(attrs=default_attrs, calendar_renderer=calendar_renderer)
 
 
 class DateRangePicker(DatePicker):
     def __init__(self, attrs=None, calendar_renderer=None):
         default_attrs = {
             'type': 'regex',
-            'pattern': r'^\d{4}-\d{2}-\d{2};\d{4}-\d{2}-\d{2}$',
+            'pattern': r'\d{4}-\d{2}-\d{2};\d{4}-\d{2}-\d{2}',
             'is': 'django-daterangepicker',
         }
         if attrs:
             default_attrs.update(**attrs)
         super().__init__(attrs=default_attrs, calendar_renderer=calendar_renderer)
 
 
 class DateRangeTextbox(DateTextbox):
     def __init__(self, attrs=None):
         default_attrs = {
             'type': 'regex',
-            'pattern': r'^\d{4}-\d{2}-\d{2};\d{4}-\d{2}-\d{2}$',
+            'pattern': r'\d{4}-\d{2}-\d{2};\d{4}-\d{2}-\d{2}',
             'is': 'django-daterangefield',
         }
         if attrs:
             default_attrs.update(**attrs)
         super().__init__(attrs=default_attrs)
 
 
 class DateTimeRangeCalendar(DateTimeCalendar):
     template_name = 'formset/default/widgets/calendar.html'
 
     def __init__(self, attrs=None, calendar_renderer=None):
         default_attrs = {
             'type': 'regex',
-            'pattern': r'^\d{4}-\d{2}-\d{2}T\d{2}:\d{2};\d{4}-\d{2}-\d{2}T\d{2}:\d{2}$',
+            'pattern': r'\d{4}-\d{2}-\d{2}T\d{2}:\d{2};\d{4}-\d{2}-\d{2}T\d{2}:\d{2}',
             'is': 'django-datetimerangecalendar',
         }
         if attrs:
             default_attrs.update(**attrs)
         super().__init__(attrs=default_attrs, calendar_renderer=calendar_renderer)
 
 
 class DateTimeRangePicker(DateTimePicker):
     def __init__(self, attrs=None, calendar_renderer=None):
         default_attrs = {
             'type': 'regex',
-            'pattern': r'^\d{4}-\d{2}-\d{2}T\d{2}:\d{2};\d{4}-\d{2}-\d{2}T\d{2}:\d{2}$',
+            'pattern': r'\d{4}-\d{2}-\d{2}T\d{2}:\d{2};\d{4}-\d{2}-\d{2}T\d{2}:\d{2}',
             'is': 'django-datetimerangepicker',
         }
         if attrs:
             default_attrs.update(**attrs)
         super().__init__(attrs=default_attrs, calendar_renderer=calendar_renderer)
 
 
 class DateTimeRangeTextbox(DateTimeTextbox):
     def __init__(self, attrs=None):
         default_attrs = {
             'type': 'regex',
-            'pattern': r'^\d{4}-\d{2}-\d{2}T\d{2}:\d{2};\d{4}-\d{2}-\d{2}T\d{2}:\d{2}$',
+            'pattern': r'\d{4}-\d{2}-\d{2}T\d{2}:\d{2};\d{4}-\d{2}-\d{2}T\d{2}:\d{2}',
             'is': 'django-datetimerangefield',
         }
         if attrs:
             default_attrs.update(**attrs)
         super().__init__(attrs=default_attrs)
```

### Comparing `django_formset-1.4.1/formset/renderers/__init__.py` & `django_formset-1.4.2/formset/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/renderers/bootstrap.py` & `django_formset-1.4.2/formset/renderers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/renderers/bulma.py` & `django_formset-1.4.2/formset/renderers/bulma.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/renderers/default.py` & `django_formset-1.4.2/formset/renderers/default.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/renderers/foundation.py` & `django_formset-1.4.2/formset/renderers/foundation.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/renderers/tailwind.py` & `django_formset-1.4.2/formset/renderers/tailwind.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/renderers/uikit.py` & `django_formset-1.4.2/formset/renderers/uikit.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/richtext/controls.py` & `django_formset-1.4.2/formset/richtext/controls.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/richtext/dialogs.py` & `django_formset-1.4.2/formset/richtext/dialogs.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/richtext/widgets.py` & `django_formset-1.4.2/formset/richtext/widgets.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/css/bootstrap5-extra.css` & `django_formset-1.4.2/formset/static/formset/css/bootstrap5-extra.css`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/css/bootstrap5-extra.css.map` & `django_formset-1.4.2/formset/static/formset/css/bootstrap5-extra.css.map`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/css/collections.css` & `django_formset-1.4.2/formset/static/formset/css/collections.css`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/css/tailwind.css` & `django_formset-1.4.2/formset/static/formset/css/tailwind.css`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/icons/file-audio.svg` & `django_formset-1.4.2/formset/static/formset/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/icons/file-empty.svg` & `django_formset-1.4.2/formset/static/formset/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/icons/file-font.svg` & `django_formset-1.4.2/formset/static/formset/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/icons/file-missing.svg` & `django_formset-1.4.2/formset/static/formset/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/icons/file-pdf.svg` & `django_formset-1.4.2/formset/static/formset/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/icons/file-picture.svg` & `django_formset-1.4.2/formset/static/formset/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/icons/file-unknown.svg` & `django_formset-1.4.2/formset/static/formset/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/icons/file-video.svg` & `django_formset-1.4.2/formset/static/formset/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/icons/file-zip.svg` & `django_formset-1.4.2/formset/static/formset/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/CountrySelectize-6YQ6A6VY.js` & `django_formset-1.4.2/formset/static/formset/js/CountrySelectize-RPAYKZSN.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     a as c
-} from "./chunk-CRVLB3K3.js";
+} from "./chunk-6IBLXZPA.js";
 import "./chunk-SERXULES.js";
 import "./chunk-W5RPWA2M.js";
 import {
     a as r
 } from "./chunk-FDUUONAQ.js";
 import "./chunk-65OJRBX6.js";
 import {
```

### Comparing `django_formset-1.4.1/formset/static/formset/js/DateTime-4XMVQT2P.js` & `django_formset-1.4.2/formset/static/formset/js/DateTime-WW4TXK6Y.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     a as v
-} from "./chunk-QHDAXJJP.js";
+} from "./chunk-WKRSL2PQ.js";
 import {
     b as m
 } from "./chunk-W5RPWA2M.js";
 import {
     a as x,
     c as f,
     d as g,
```

### Comparing `django_formset-1.4.1/formset/static/formset/js/DjangoSlug-SHZN726V.js` & `django_formset-1.4.2/formset/static/formset/js/DjangoSlug-SHZN726V.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/DualSelector-233VL6HH.js` & `django_formset-1.4.2/formset/static/formset/js/DualSelector-G47GXWWH.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as d
 } from "./chunk-SERXULES.js";
 import "./chunk-W5RPWA2M.js";
 import {
     a as p
-} from "./chunk-NIKVGHIO.js";
+} from "./chunk-XO2BBJ6P.js";
 import "./chunk-NOGHTXP6.js";
 import {
     a as v
 } from "./chunk-FDUUONAQ.js";
 import {
     a as r
 } from "./chunk-65OJRBX6.js";
```

### Comparing `django_formset-1.4.1/formset/static/formset/js/PhoneNumber-KCJABOET.js` & `django_formset-1.4.2/formset/static/formset/js/PhoneNumber-RCXY4VXK.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/RichtextArea-QY2VVCDL.js` & `django_formset-1.4.2/formset/static/formset/js/RichtextArea-34WSI64S.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     a as fa,
     b as ha,
     c as pa,
     f as Vi
-} from "./chunk-XQYS6DVW.js";
+} from "./chunk-B7PX5YAU.js";
 import {
     a as ma
 } from "./chunk-FDUUONAQ.js";
 import {
     e as ji
 } from "./chunk-RLE6ONWJ.js";
 import {
```

### Comparing `django_formset-1.4.1/formset/static/formset/js/chunk-65OJRBX6.js` & `django_formset-1.4.2/formset/static/formset/js/chunk-65OJRBX6.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/chunk-CRVLB3K3.js` & `django_formset-1.4.2/formset/static/formset/js/chunk-6IBLXZPA.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/chunk-FDUUONAQ.js` & `django_formset-1.4.2/formset/static/formset/js/chunk-FDUUONAQ.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/chunk-NIKVGHIO.js` & `django_formset-1.4.2/formset/static/formset/js/chunk-XO2BBJ6P.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/chunk-NOGHTXP6.js` & `django_formset-1.4.2/formset/static/formset/js/chunk-NOGHTXP6.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/chunk-P2VM2T3G.js` & `django_formset-1.4.2/formset/static/formset/js/chunk-P2VM2T3G.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/chunk-QHDAXJJP.js` & `django_formset-1.4.2/formset/static/formset/js/chunk-WKRSL2PQ.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/chunk-RLE6ONWJ.js` & `django_formset-1.4.2/formset/static/formset/js/chunk-RLE6ONWJ.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/chunk-SERXULES.js` & `django_formset-1.4.2/formset/static/formset/js/chunk-SERXULES.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/chunk-W5RPWA2M.js` & `django_formset-1.4.2/formset/static/formset/js/chunk-W5RPWA2M.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/chunk-XQYS6DVW.js` & `django_formset-1.4.2/formset/static/formset/js/chunk-B7PX5YAU.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/static/formset/js/django-formset.js` & `django_formset-1.4.2/formset/static/formset/js/django-formset.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
 import {
     a as er,
     b as tr,
     c as rr,
     d as M,
     e as ot,
     f as lt
-} from "./chunk-XQYS6DVW.js";
+} from "./chunk-B7PX5YAU.js";
 import {
     a as it
 } from "./chunk-FDUUONAQ.js";
 import {
     a as st
 } from "./chunk-65OJRBX6.js";
 import {
@@ -1096,15 +1096,15 @@
             let e = this.fieldElements[0];
             if (e.value && e.type === "text") {
                 if (e.minLength > 0 && e.value.length < e.minLength) return e.setCustomValidity(this.errorMessages.get("tooShort") ?? "");
                 if (e.maxLength > 0 && e.value.length > e.maxLength) return e.setCustomValidity(this.errorMessages.get("tooLong") ?? "")
             }
         }
         setValidationError() {
-            let e;
+            let e = null;
             for (e of this.fieldElements)
                 if (!e.validity.valid) break;
             for (let [t, r] of this.errorMessages)
                 if (e && e.validity[t]) return this.errorPlaceholder && (this.errorPlaceholder.innerHTML = r, e.setCustomValidity(r)), !1;
             return e instanceof HTMLInputElement && e.type === "file" ? this.validateFileInput(e, !0) : !0
         }
         reportCustomError(e) {
@@ -1176,15 +1176,15 @@
                 this.formset.submit(e).then(i => i instanceof Response && i.status === 200 ? t(i) : r(i))
             })
         }
         reset() {
             return e => (this.formset.resetToInitial(), Promise.resolve(e))
         }
         reload(e) {
-            return t => (e ? location.reload() : location.replace(window.location.pathname), Promise.resolve(t))
+            return t => (e ? location.reload() : location.replace(window.location.pathname), new Promise(r => window.setTimeout(() => r(t), 3e3)))
         }
         proceed(e) {
             return async t => {
                 if (typeof e == "string" && e.length > 0) location.href = e;
                 else if (t instanceof Response && t.status === 200) {
                     let r = await t.clone().json();
                     r.success_url ? location.href = r.success_url : console.warn("Neither a success-, nor a proceed-URL are given.")
@@ -2025,65 +2025,65 @@
 
     function r(o, u, d, c = void 0) {
         customElements.get(u) instanceof Function ? o() : (window.customElements.define(u, d, c), window.customElements.whenDefined(u).then(() => o()))
     }
 
     function i(o) {
         o.querySelector('select[is="django-selectize"]') && t.push(new Promise((d, c) => {
-            import("./DjangoSelectize-JMSV2QXX.js").then(({
+            import("./DjangoSelectize-XUOHPSUG.js").then(({
                 DjangoSelectizeElement: l
             }) => {
                 r(d, "django-selectize", l, {
                     extends: "select"
                 })
             }).catch(l => c(l))
         })), o.querySelector('select[is="django-country-selectize"]') && t.push(new Promise((d, c) => {
-            import("./CountrySelectize-6YQ6A6VY.js").then(({
+            import("./CountrySelectize-RPAYKZSN.js").then(({
                 CountrySelectizeElement: l
             }) => {
                 r(d, "django-country-selectize", l, {
                     extends: "select"
                 })
             }).catch(l => c(l))
         })), o.querySelector("django-sortable-select") ? t.push(new Promise((d, c) => {
-            import("./SortableSelect-27BKOQAW.js").then(({
+            import("./SortableSelect-6YQLVCNF.js").then(({
                 SortableSelectElement: l
             }) => {
-                customElements.get("django-sortable-select") instanceof Function ? d() : window.customElements.define("django-sortable-select", l), import("./DualSelector-233VL6HH.js").then(({
+                customElements.get("django-sortable-select") instanceof Function ? d() : window.customElements.define("django-sortable-select", l), import("./DualSelector-G47GXWWH.js").then(({
                     DualSelectorElement: k
                 }) => {
                     customElements.get("django-dual-selector") instanceof Function ? d() : (window.customElements.define("django-dual-selector", k, {
                         extends: "select"
                     }), Promise.all([window.customElements.whenDefined("django-sortable-select"), window.customElements.whenDefined("django-dual-selector")]).then(() => d()))
                 }).catch(k => c(k))
             }).catch(l => c(l))
         })) : o.querySelector('select[is="django-dual-selector"]') && t.push(new Promise((d, c) => {
-            import("./DualSelector-233VL6HH.js").then(({
+            import("./DualSelector-G47GXWWH.js").then(({
                 DualSelectorElement: l
             }) => {
                 r(d, "django-dual-selector", l, {
                     extends: "select"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-phone-number"]') && t.push(new Promise((d, c) => {
-            import("./PhoneNumber-KCJABOET.js").then(({
+            import("./PhoneNumber-RCXY4VXK.js").then(({
                 PhoneNumberElement: l
             }) => {
                 r(d, "django-phone-number", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelectorAll('textarea[is="django-richtext"]').forEach(d => {
             t.push(new Promise((c, l) => {
                 let k = () => {
                     d.isInitialized ? c() : d.addEventListener("connected", () => c(), {
                         once: !0
                     })
                 };
-                import("./RichtextArea-QY2VVCDL.js").then(({
+                import("./RichtextArea-34WSI64S.js").then(({
                     RichTextAreaElement: G
                 }) => {
                     customElements.get("django-richtext") instanceof Function ? k() : (window.customElements.define("django-richtext", G, {
                         extends: "textarea"
                     }), window.customElements.whenDefined("django-richtext").then(k))
                 }).catch(G => l(G))
             }))
@@ -2092,103 +2092,103 @@
                 DjangoSlugElement: l
             }) => {
                 r(d, "django-slug", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-4XMVQT2P.js").then(({
+            import("./DateTime-WW4TXK6Y.js").then(({
                 DateFieldElement: l
             }) => {
                 r(d, "django-datefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-SME4CT3M.js").then(({
+            import("./Calendar-5KXZG25G.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-datecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-4XMVQT2P.js").then(({
+            import("./DateTime-WW4TXK6Y.js").then(({
                 DatePickerElement: l
             }) => {
                 r(d, "django-datepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-4XMVQT2P.js").then(({
+            import("./DateTime-WW4TXK6Y.js").then(({
                 DateTimeFieldElement: l
             }) => {
                 r(d, "django-datetimefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-SME4CT3M.js").then(({
+            import("./Calendar-5KXZG25G.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-datetimecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-4XMVQT2P.js").then(({
+            import("./DateTime-WW4TXK6Y.js").then(({
                 DateTimePickerElement: l
             }) => {
                 r(d, "django-datetimepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-daterangefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-4XMVQT2P.js").then(({
+            import("./DateTime-WW4TXK6Y.js").then(({
                 DateRangeFieldElement: l
             }) => {
                 r(d, "django-daterangefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-daterangecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-SME4CT3M.js").then(({
+            import("./Calendar-5KXZG25G.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-daterangecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-daterangepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-4XMVQT2P.js").then(({
+            import("./DateTime-WW4TXK6Y.js").then(({
                 DateRangePickerElement: l
             }) => {
                 r(d, "django-daterangepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimerangefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-4XMVQT2P.js").then(({
+            import("./DateTime-WW4TXK6Y.js").then(({
                 DateTimeRangeFieldElement: l
             }) => {
                 r(d, "django-datetimerangefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimerangecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-SME4CT3M.js").then(({
+            import("./Calendar-5KXZG25G.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-datetimerangecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimerangepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-4XMVQT2P.js").then(({
+            import("./DateTime-WW4TXK6Y.js").then(({
                 DateTimeRangePickerElement: l
             }) => {
                 r(d, "django-datetimerangepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         }))
```

### Comparing `django_formset-1.4.1/formset/static/formset/tiptap-extensions/footnote.js` & `django_formset-1.4.2/formset/static/formset/tiptap-extensions/footnote.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/calendar/hours.html` & `django_formset-1.4.2/formset/templates/calendar/hours.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/calendar/months.html` & `django_formset-1.4.2/formset/templates/calendar/months.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/calendar/weeks.html` & `django_formset-1.4.2/formset/templates/calendar/weeks.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/calendar/years.html` & `django_formset-1.4.2/formset/templates/calendar/years.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/dual_selector.html` & `django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/file.html` & `django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/bulma/widgets/dual_selector.html` & `django_formset-1.4.2/formset/templates/formset/bulma/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/bulma/widgets/file.html` & `django_formset-1.4.2/formset/templates/formset/bulma/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/default/collection.html` & `django_formset-1.4.2/formset/templates/formset/default/collection.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/default/fieldset.html` & `django_formset-1.4.2/formset/templates/formset/default/fieldset.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/default/form_dialog.html` & `django_formset-1.4.2/formset/templates/formset/default/form_dialog.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/default/widgets/dual_selector.html` & `django_formset-1.4.2/formset/templates/formset/default/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/default/widgets/file.html` & `django_formset-1.4.2/formset/templates/formset/default/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/default/widgets/selectize.html` & `django_formset-1.4.2/formset/templates/formset/default/widgets/selectize.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/foundation/widgets/dual_selector.html` & `django_formset-1.4.2/formset/templates/formset/foundation/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/foundation/widgets/file.html` & `django_formset-1.4.2/formset/templates/formset/foundation/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/icons/blockquote.svg` & `django_formset-1.4.2/formset/templates/formset/icons/blockquote.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/icons/calendar-today.svg` & `django_formset-1.4.2/formset/templates/formset/icons/calendar-today.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/icons/footnote.svg` & `django_formset-1.4.2/formset/templates/formset/icons/footnote.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/icons/letters.svg` & `django_formset-1.4.2/formset/templates/formset/icons/letters.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/icons/placeholder.svg` & `django_formset-1.4.2/formset/templates/formset/icons/placeholder.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/icons/questionmark.svg` & `django_formset-1.4.2/formset/templates/formset/icons/questionmark.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/icons/strike.svg` & `django_formset-1.4.2/formset/templates/formset/icons/strike.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/icons/subscript.svg` & `django_formset-1.4.2/formset/templates/formset/icons/subscript.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/icons/unlink.svg` & `django_formset-1.4.2/formset/templates/formset/icons/unlink.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/richtext/align.html` & `django_formset-1.4.2/formset/templates/formset/richtext/align.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/richtext/color.html` & `django_formset-1.4.2/formset/templates/formset/richtext/color.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/richtext/heading.html` & `django_formset-1.4.2/formset/templates/formset/richtext/heading.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/tailwind/widgets/dual_selector.html` & `django_formset-1.4.2/formset/templates/formset/tailwind/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/tailwind/widgets/file.html` & `django_formset-1.4.2/formset/templates/formset/tailwind/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templates/formset/uikit/widgets/file.html` & `django_formset-1.4.2/formset/templates/formset/uikit/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templatetags/formsetify.py` & `django_formset-1.4.2/formset/templatetags/formsetify.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templatetags/phonenumber.py` & `django_formset-1.4.2/formset/templatetags/phonenumber.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/templatetags/richtext.py` & `django_formset-1.4.2/formset/templatetags/richtext.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/upload.py` & `django_formset-1.4.2/formset/upload.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/utils.py` & `django_formset-1.4.2/formset/utils.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/views.py` & `django_formset-1.4.2/formset/views.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.1/formset/widgets.py` & `django_formset-1.4.2/formset/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,24 +331,24 @@
 
 
 class PhoneNumberInput(TextInput):
     def __init__(self, attrs=None):
         super().__init__(attrs)
         self.attrs.update({
             'is': 'django-phone-number',
-            'pattern': r'^\+\d{3,16}$',  # E.164 format
+            'pattern': r'\+\d{3,16}',  # E.164 format
         })
 
 
 class SlugInput(TextInput):
     def __init__(self, populate_from, attrs=None):
         super().__init__(attrs)
         self.attrs.update({
             'is': 'django-slug',
-            'pattern': '^[-a-zA-Z0-9_]+$',
+            'pattern': r'[\-a-zA-Z0-9_]+',
             'populate-from': populate_from,
         })
 
 
 class UploadedFileInput(FileInput):
     """
     Widget to be used as a replacement for fields of type :class:`django.forms.fields.FileField`
```

### Comparing `django_formset-1.4.1/setup.py` & `django_formset-1.4.2/setup.py`

 * *Files identical despite different names*

