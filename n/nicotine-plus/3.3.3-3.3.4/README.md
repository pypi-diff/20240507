# Comparing `tmp/nicotine_plus-3.3.3.tar.gz` & `tmp/nicotine_plus-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicotine_plus-3.3.3.tar", last modified: Sun May  5 18:39:12 2024, max compression
+gzip compressed data, was "nicotine_plus-3.3.4.tar", last modified: Mon May  6 22:22:10 2024, max compression
```

## Comparing `nicotine_plus-3.3.3.tar` & `nicotine_plus-3.3.4.tar`

### file list

```diff
@@ -1,708 +1,708 @@
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.480173 nicotine_plus-3.3.3/
--rw-r--r--   0 default   (1000) default   (1000)     3734 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/AUTHORS.md
--rw-r--r--   0 default   (1000) default   (1000)    35147 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/COPYING
--rw-r--r--   0 default   (1000) default   (1000)      545 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/MANIFEST.in
--rw-r--r--   0 default   (1000) default   (1000)   202130 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/NEWS.md
--rw-r--r--   0 default   (1000) default   (1000)     1276 2024-05-05 18:39:12.480173 nicotine_plus-3.3.3/PKG-INFO
--rw-r--r--   0 default   (1000) default   (1000)     3043 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/README.md
--rw-r--r--   0 default   (1000) default   (1000)     2781 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/TRANSLATORS.md
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.265177 nicotine_plus-3.3.3/data/
--rw-r--r--   0 default   (1000) default   (1000)     1523 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/data/nicotine.1
--rw-r--r--   0 default   (1000) default   (1000)     5129 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/data/org.nicotine_plus.Nicotine.appdata.xml.in
--rw-r--r--   0 default   (1000) default   (1000)      424 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/data/org.nicotine_plus.Nicotine.desktop.in
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.265177 nicotine_plus-3.3.3/data/scripts/
--rw-r--r--   0 default   (1000) default   (1000)     5030 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/data/scripts/update_ip_country_data.py
--rw-r--r--   0 default   (1000) default   (1000)     1838 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/data/scripts/update_translation_template.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.267176 nicotine_plus-3.3.3/doc/
--rw-r--r--   0 default   (1000) default   (1000)     2377 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/doc/DEPENDENCIES.md
--rw-r--r--   0 default   (1000) default   (1000)    13491 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/doc/DEVELOPING.md
--rw-r--r--   0 default   (1000) default   (1000)     6999 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/doc/DOWNLOADS.md
--rw-r--r--   0 default   (1000) default   (1000)     3106 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/doc/PACKAGING.md
--rw-r--r--   0 default   (1000) default   (1000)    80371 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/doc/SLSKPROTOCOL.md
--rw-r--r--   0 default   (1000) default   (1000)     5104 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/doc/TESTING.md
--rw-r--r--   0 default   (1000) default   (1000)     4757 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/doc/TRANSLATIONS.md
--rwxr-xr-x   0 default   (1000) default   (1000)     1269 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/nicotine
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.479173 nicotine_plus-3.3.3/nicotine_plus.egg-info/
--rw-r--r--   0 default   (1000) default   (1000)     1276 2024-05-05 18:39:11.000000 nicotine_plus-3.3.3/nicotine_plus.egg-info/PKG-INFO
--rw-r--r--   0 default   (1000) default   (1000)    28692 2024-05-05 18:39:12.000000 nicotine_plus-3.3.3/nicotine_plus.egg-info/SOURCES.txt
--rw-r--r--   0 default   (1000) default   (1000)        1 2024-05-05 18:39:11.000000 nicotine_plus-3.3.3/nicotine_plus.egg-info/dependency_links.txt
--rw-r--r--   0 default   (1000) default   (1000)       67 2024-05-05 18:39:11.000000 nicotine_plus-3.3.3/nicotine_plus.egg-info/requires.txt
--rw-r--r--   0 default   (1000) default   (1000)       11 2024-05-05 18:39:11.000000 nicotine_plus-3.3.3/nicotine_plus.egg-info/top_level.txt
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.295176 nicotine_plus-3.3.3/po/
--rw-r--r--   0 default   (1000) default   (1000)       65 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/LINGUAS
--rw-r--r--   0 default   (1000) default   (1000)   138793 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/ar.po
--rw-r--r--   0 default   (1000) default   (1000)   211752 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/ca.po
--rw-r--r--   0 default   (1000) default   (1000)   239736 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/cs.po
--rw-r--r--   0 default   (1000) default   (1000)   238187 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/da.po
--rw-r--r--   0 default   (1000) default   (1000)   246309 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/de.po
--rw-r--r--   0 default   (1000) default   (1000)   228944 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/eo.po
--rw-r--r--   0 default   (1000) default   (1000)   236357 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/es_CL.po
--rw-r--r--   0 default   (1000) default   (1000)   235213 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/es_ES.po
--rw-r--r--   0 default   (1000) default   (1000)   194522 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/et.po
--rw-r--r--   0 default   (1000) default   (1000)   248049 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/eu.po
--rw-r--r--   0 default   (1000) default   (1000)   249549 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/fi.po
--rw-r--r--   0 default   (1000) default   (1000)   239542 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/fr.po
--rw-r--r--   0 default   (1000) default   (1000)   264914 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/hu.po
--rw-r--r--   0 default   (1000) default   (1000)   235367 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/it.po
--rw-r--r--   0 default   (1000) default   (1000)   246272 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/lt.po
--rw-r--r--   0 default   (1000) default   (1000)   210152 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/lv.po
--rw-r--r--   0 default   (1000) default   (1000)   229665 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/nb_NO.po
--rw-r--r--   0 default   (1000) default   (1000)   138000 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/nicotine.pot
--rw-r--r--   0 default   (1000) default   (1000)   262715 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/nl.po
--rw-r--r--   0 default   (1000) default   (1000)   271139 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/pl.po
--rw-r--r--   0 default   (1000) default   (1000)   239311 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/pt_BR.po
--rw-r--r--   0 default   (1000) default   (1000)   182641 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/pt_PT.po
--rw-r--r--   0 default   (1000) default   (1000)   200906 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/ro.po
--rw-r--r--   0 default   (1000) default   (1000)   254214 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/ru.po
--rw-r--r--   0 default   (1000) default   (1000)   254027 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/sk.po
--rw-r--r--   0 default   (1000) default   (1000)   143517 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/sq.po
--rw-r--r--   0 default   (1000) default   (1000)   239340 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/sv.po
--rw-r--r--   0 default   (1000) default   (1000)   231510 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/tr.po
--rw-r--r--   0 default   (1000) default   (1000)   253243 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/uk.po
--rw-r--r--   0 default   (1000) default   (1000)   198546 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/po/zh_CN.po
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.304176 nicotine_plus-3.3.3/pynicotine/
--rw-r--r--   0 default   (1000) default   (1000)     7129 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)      801 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/__main__.py
--rw-r--r--   0 default   (1000) default   (1000)     8642 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/buddies.py
--rw-r--r--   0 default   (1000) default   (1000)    21348 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/chatrooms.py
--rw-r--r--   0 default   (1000) default   (1000)     5222 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/cli.py
--rw-r--r--   0 default   (1000) default   (1000)    29012 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/config.py
--rw-r--r--   0 default   (1000) default   (1000)    12478 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/core.py
--rw-r--r--   0 default   (1000) default   (1000)    52454 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/downloads.py
--rw-r--r--   0 default   (1000) default   (1000)     9156 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/events.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.305176 nicotine_plus-3.3.3/pynicotine/external/
--rw-r--r--   0 default   (1000) default   (1000)    21663 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/external/README.md
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/external/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.307176 nicotine_plus-3.3.3/pynicotine/external/data/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/external/data/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)   747340 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/external/data/country_codes.py
--rw-r--r--   0 default   (1000) default   (1000)  2696565 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/external/data/ip_ranges.py
--rw-r--r--   0 default   (1000) default   (1000)    71390 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/external/tinytag.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.314176 nicotine_plus-3.3.3/pynicotine/gtkgui/
--rw-r--r--   0 default   (1000) default   (1000)     5735 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)    38383 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/application.py
--rw-r--r--   0 default   (1000) default   (1000)    16598 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/buddies.py
--rw-r--r--   0 default   (1000) default   (1000)    34847 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/chatrooms.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.315176 nicotine_plus-3.3.3/pynicotine/gtkgui/css/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/css/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)     2240 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/css/style.css
--rw-r--r--   0 default   (1000) default   (1000)      648 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/css/style_gtk3.css
--rw-r--r--   0 default   (1000) default   (1000)      899 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/css/style_gtk4.css
--rw-r--r--   0 default   (1000) default   (1000)      783 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/css/style_gtk4_darwin.css
--rw-r--r--   0 default   (1000) default   (1000)      406 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/css/style_libadwaita.css
--rw-r--r--   0 default   (1000) default   (1000)      554 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/css/style_libadwaita_csd.css
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.318176 nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)    13990 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/about.py
--rw-r--r--   0 default   (1000) default   (1000)    10335 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/fastconfigure.py
--rw-r--r--   0 default   (1000) default   (1000)     5268 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/fileproperties.py
--rw-r--r--   0 default   (1000) default   (1000)    16955 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/pluginsettings.py
--rw-r--r--   0 default   (1000) default   (1000)   128074 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/preferences.py
--rw-r--r--   0 default   (1000) default   (1000)     1298 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/shortcuts.py
--rw-r--r--   0 default   (1000) default   (1000)     4578 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/statistics.py
--rw-r--r--   0 default   (1000) default   (1000)     7066 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/wishlist.py
--rw-r--r--   0 default   (1000) default   (1000)     8444 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/downloads.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.319176 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.319176 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.239177 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/128x128/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.320176 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/128x128/apps/
--rw-r--r--   0 default   (1000) default   (1000)      824 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/128x128/apps/org.nicotine_plus.Nicotine.svg
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.239177 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/16x16/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.320176 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/16x16/apps/
--rw-r--r--   0 default   (1000) default   (1000)     1053 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/16x16/apps/org.nicotine_plus.Nicotine.svg
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.240177 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/24x24/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.321176 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/24x24/apps/
--rw-r--r--   0 default   (1000) default   (1000)      772 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/24x24/apps/org.nicotine_plus.Nicotine.svg
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.240177 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/256x256/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.321176 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/256x256/apps/
--rw-r--r--   0 default   (1000) default   (1000)      862 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/256x256/apps/org.nicotine_plus.Nicotine.svg
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.240177 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/32x32/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.322176 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/32x32/apps/
--rw-r--r--   0 default   (1000) default   (1000)      799 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/32x32/apps/org.nicotine_plus.Nicotine.svg
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.241177 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/48x48/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.322176 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/48x48/apps/
--rw-r--r--   0 default   (1000) default   (1000)      868 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/48x48/apps/org.nicotine_plus.Nicotine.svg
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.241177 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/64x64/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.322176 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/64x64/apps/
--rw-r--r--   0 default   (1000) default   (1000)      871 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/64x64/apps/org.nicotine_plus.Nicotine.svg
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.323176 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.325176 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/apps/
--rw-r--r--   0 default   (1000) default   (1000)     1048 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-away.svg
--rw-r--r--   0 default   (1000) default   (1000)      881 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-connect.svg
--rw-r--r--   0 default   (1000) default   (1000)     1091 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-disconnect.svg
--rw-r--r--   0 default   (1000) default   (1000)      999 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-msg.svg
--rw-r--r--   0 default   (1000) default   (1000)      824 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine.svg
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.412174 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)     1285 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ad.svg
--rw-r--r--   0 default   (1000) default   (1000)      947 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ae.svg
--rw-r--r--   0 default   (1000) default   (1000)     1231 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-af.svg
--rw-r--r--   0 default   (1000) default   (1000)     1610 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ag.svg
--rw-r--r--   0 default   (1000) default   (1000)     2222 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ai.svg
--rw-r--r--   0 default   (1000) default   (1000)     1727 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-al.svg
--rw-r--r--   0 default   (1000) default   (1000)      908 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-am.svg
--rw-r--r--   0 default   (1000) default   (1000)     1392 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ao.svg
--rw-r--r--   0 default   (1000) default   (1000)      701 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ar.svg
--rw-r--r--   0 default   (1000) default   (1000)     1493 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-as.svg
--rw-r--r--   0 default   (1000) default   (1000)      565 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-at.svg
--rw-r--r--   0 default   (1000) default   (1000)     1775 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-au.svg
--rw-r--r--   0 default   (1000) default   (1000)     1023 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-aw.svg
--rw-r--r--   0 default   (1000) default   (1000)      940 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ax.svg
--rw-r--r--   0 default   (1000) default   (1000)     1033 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-az.svg
--rw-r--r--   0 default   (1000) default   (1000)     1070 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ba.svg
--rw-r--r--   0 default   (1000) default   (1000)     1904 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bb.svg
--rw-r--r--   0 default   (1000) default   (1000)      722 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bd.svg
--rw-r--r--   0 default   (1000) default   (1000)      910 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-be.svg
--rw-r--r--   0 default   (1000) default   (1000)      837 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bf.svg
--rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bg.svg
--rw-r--r--   0 default   (1000) default   (1000)      630 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bh.svg
--rw-r--r--   0 default   (1000) default   (1000)     1722 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bi.svg
--rw-r--r--   0 default   (1000) default   (1000)      907 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bj.svg
--rw-r--r--   0 default   (1000) default   (1000)     1700 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bl.svg
--rw-r--r--   0 default   (1000) default   (1000)     2151 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bm.svg
--rw-r--r--   0 default   (1000) default   (1000)      839 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bn.svg
--rw-r--r--   0 default   (1000) default   (1000)      908 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bo.svg
--rw-r--r--   0 default   (1000) default   (1000)     1314 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-br.svg
--rw-r--r--   0 default   (1000) default   (1000)      925 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bs.svg
--rw-r--r--   0 default   (1000) default   (1000)      712 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bt.svg
--rw-r--r--   0 default   (1000) default   (1000)      782 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bv.svg
--rw-r--r--   0 default   (1000) default   (1000)      762 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bw.svg
--rw-r--r--   0 default   (1000) default   (1000)     1116 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-by.svg
--rw-r--r--   0 default   (1000) default   (1000)     1631 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bz.svg
--rw-r--r--   0 default   (1000) default   (1000)      904 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ca.svg
--rw-r--r--   0 default   (1000) default   (1000)     1237 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cc.svg
--rw-r--r--   0 default   (1000) default   (1000)     1012 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cd.svg
--rw-r--r--   0 default   (1000) default   (1000)     1422 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cf.svg
--rw-r--r--   0 default   (1000) default   (1000)     1060 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cg.svg
--rw-r--r--   0 default   (1000) default   (1000)      790 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ch.svg
--rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ci.svg
--rw-r--r--   0 default   (1000) default   (1000)     1697 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ck.svg
--rw-r--r--   0 default   (1000) default   (1000)      874 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cl.svg
--rw-r--r--   0 default   (1000) default   (1000)     1241 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cm.svg
--rw-r--r--   0 default   (1000) default   (1000)     1323 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cn.svg
--rw-r--r--   0 default   (1000) default   (1000)      908 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-co.svg
--rw-r--r--   0 default   (1000) default   (1000)      762 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cr.svg
--rw-r--r--   0 default   (1000) default   (1000)      972 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cu.svg
--rw-r--r--   0 default   (1000) default   (1000)     1611 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cv.svg
--rw-r--r--   0 default   (1000) default   (1000)      933 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cw.svg
--rw-r--r--   0 default   (1000) default   (1000)     1844 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cx.svg
--rw-r--r--   0 default   (1000) default   (1000)     1623 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cy.svg
--rw-r--r--   0 default   (1000) default   (1000)      754 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cz.svg
--rw-r--r--   0 default   (1000) default   (1000)      908 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-de.svg
--rw-r--r--   0 default   (1000) default   (1000)     1042 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dj.svg
--rw-r--r--   0 default   (1000) default   (1000)      569 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dk.svg
--rw-r--r--   0 default   (1000) default   (1000)     1988 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dm.svg
--rw-r--r--   0 default   (1000) default   (1000)     1170 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-do.svg
--rw-r--r--   0 default   (1000) default   (1000)     1086 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dz.svg
--rw-r--r--   0 default   (1000) default   (1000)     1430 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ec.svg
--rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ee.svg
--rw-r--r--   0 default   (1000) default   (1000)     1788 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-eg.svg
--rw-r--r--   0 default   (1000) default   (1000)     1364 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-er.svg
--rw-r--r--   0 default   (1000) default   (1000)     1235 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-es.svg
--rw-r--r--   0 default   (1000) default   (1000)     1535 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-et.svg
--rw-r--r--   0 default   (1000) default   (1000)     1632 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-eu.svg
--rw-r--r--   0 default   (1000) default   (1000)      529 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fi.svg
--rw-r--r--   0 default   (1000) default   (1000)     2134 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fj.svg
--rw-r--r--   0 default   (1000) default   (1000)     4020 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fk.svg
--rw-r--r--   0 default   (1000) default   (1000)      967 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fm.svg
--rw-r--r--   0 default   (1000) default   (1000)      742 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fo.svg
--rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fr.svg
--rw-r--r--   0 default   (1000) default   (1000)      908 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ga.svg
--rw-r--r--   0 default   (1000) default   (1000)     1330 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gb.svg
--rw-r--r--   0 default   (1000) default   (1000)     1854 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gd.svg
--rw-r--r--   0 default   (1000) default   (1000)      855 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ge.svg
--rw-r--r--   0 default   (1000) default   (1000)     1004 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gf.svg
--rw-r--r--   0 default   (1000) default   (1000)      791 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gg.svg
--rw-r--r--   0 default   (1000) default   (1000)     1201 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gh.svg
--rw-r--r--   0 default   (1000) default   (1000)     1614 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gi.svg
--rw-r--r--   0 default   (1000) default   (1000)     1095 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gl.svg
--rw-r--r--   0 default   (1000) default   (1000)      947 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gm.svg
--rw-r--r--   0 default   (1000) default   (1000)      910 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gn.svg
--rw-r--r--   0 default   (1000) default   (1000)    10261 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gp.svg
--rw-r--r--   0 default   (1000) default   (1000)     1281 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gq.svg
--rw-r--r--   0 default   (1000) default   (1000)      614 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gr.svg
--rw-r--r--   0 default   (1000) default   (1000)     4785 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gs.svg
--rw-r--r--   0 default   (1000) default   (1000)      849 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gt.svg
--rw-r--r--   0 default   (1000) default   (1000)     2731 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gu.svg
--rw-r--r--   0 default   (1000) default   (1000)     1192 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gw.svg
--rw-r--r--   0 default   (1000) default   (1000)     1433 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gy.svg
--rw-r--r--   0 default   (1000) default   (1000)     1531 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hk.svg
--rw-r--r--   0 default   (1000) default   (1000)     1798 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hm.svg
--rw-r--r--   0 default   (1000) default   (1000)     1086 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hn.svg
--rw-r--r--   0 default   (1000) default   (1000)     1450 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hr.svg
--rw-r--r--   0 default   (1000) default   (1000)     1874 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ht.svg
--rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hu.svg
--rw-r--r--   0 default   (1000) default   (1000)      552 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-id.svg
--rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ie.svg
--rw-r--r--   0 default   (1000) default   (1000)      742 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-il.svg
--rw-r--r--   0 default   (1000) default   (1000)     1619 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-im.svg
--rw-r--r--   0 default   (1000) default   (1000)      996 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-in.svg
--rw-r--r--   0 default   (1000) default   (1000)     5301 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-io.svg
--rw-r--r--   0 default   (1000) default   (1000)     1433 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-iq.svg
--rw-r--r--   0 default   (1000) default   (1000)     3449 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ir.svg
--rw-r--r--   0 default   (1000) default   (1000)      782 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-is.svg
--rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-it.svg
--rw-r--r--   0 default   (1000) default   (1000)     1306 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-je.svg
--rw-r--r--   0 default   (1000) default   (1000)     1137 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-jm.svg
--rw-r--r--   0 default   (1000) default   (1000)     1091 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-jo.svg
--rw-r--r--   0 default   (1000) default   (1000)      525 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-jp.svg
--rw-r--r--   0 default   (1000) default   (1000)     1604 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ke.svg
--rw-r--r--   0 default   (1000) default   (1000)     1098 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kg.svg
--rw-r--r--   0 default   (1000) default   (1000)      994 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kh.svg
--rw-r--r--   0 default   (1000) default   (1000)     3464 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ki.svg
--rw-r--r--   0 default   (1000) default   (1000)     1339 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-km.svg
--rw-r--r--   0 default   (1000) default   (1000)     1434 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kn.svg
--rw-r--r--   0 default   (1000) default   (1000)      944 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kp.svg
--rw-r--r--   0 default   (1000) default   (1000)     2304 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kr.svg
--rw-r--r--   0 default   (1000) default   (1000)      951 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kw.svg
--rw-r--r--   0 default   (1000) default   (1000)     1892 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ky.svg
--rw-r--r--   0 default   (1000) default   (1000)     2699 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kz.svg
--rw-r--r--   0 default   (1000) default   (1000)      774 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-la.svg
--rw-r--r--   0 default   (1000) default   (1000)     1334 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lb.svg
--rw-r--r--   0 default   (1000) default   (1000)      959 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lc.svg
--rw-r--r--   0 default   (1000) default   (1000)      710 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-li.svg
--rw-r--r--   0 default   (1000) default   (1000)     2836 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lk.svg
--rw-r--r--   0 default   (1000) default   (1000)     1269 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lr.svg
--rw-r--r--   0 default   (1000) default   (1000)     1240 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ls.svg
--rw-r--r--   0 default   (1000) default   (1000)      908 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lt.svg
--rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lu.svg
--rw-r--r--   0 default   (1000) default   (1000)      564 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lv.svg
--rw-r--r--   0 default   (1000) default   (1000)     1033 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ly.svg
--rw-r--r--   0 default   (1000) default   (1000)      769 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ma.svg
--rw-r--r--   0 default   (1000) default   (1000)      552 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mc.svg
--rw-r--r--   0 default   (1000) default   (1000)     1462 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-md.svg
--rw-r--r--   0 default   (1000) default   (1000)     2943 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-me.svg
--rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mf.svg
--rw-r--r--   0 default   (1000) default   (1000)      749 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mg.svg
--rw-r--r--   0 default   (1000) default   (1000)     1002 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mh.svg
--rw-r--r--   0 default   (1000) default   (1000)     1303 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mk.svg
--rw-r--r--   0 default   (1000) default   (1000)      910 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ml.svg
--rw-r--r--   0 default   (1000) default   (1000)     1038 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mm.svg
--rw-r--r--   0 default   (1000) default   (1000)     1058 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mn.svg
--rw-r--r--   0 default   (1000) default   (1000)     1369 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mo.svg
--rw-r--r--   0 default   (1000) default   (1000)     1103 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mp.svg
--rw-r--r--   0 default   (1000) default   (1000)     4357 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mq.svg
--rw-r--r--   0 default   (1000) default   (1000)      866 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mr.svg
--rw-r--r--   0 default   (1000) default   (1000)     2017 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ms.svg
--rw-r--r--   0 default   (1000) default   (1000)      849 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mt.svg
--rw-r--r--   0 default   (1000) default   (1000)     1105 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mu.svg
--rw-r--r--   0 default   (1000) default   (1000)      823 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mv.svg
--rw-r--r--   0 default   (1000) default   (1000)      959 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mw.svg
--rw-r--r--   0 default   (1000) default   (1000)     1047 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mx.svg
--rw-r--r--   0 default   (1000) default   (1000)     1197 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-my.svg
--rw-r--r--   0 default   (1000) default   (1000)     1430 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mz.svg
--rw-r--r--   0 default   (1000) default   (1000)     3248 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-na.svg
--rw-r--r--   0 default   (1000) default   (1000)     1609 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nc.svg
--rw-r--r--   0 default   (1000) default   (1000)      957 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ne.svg
--rw-r--r--   0 default   (1000) default   (1000)     1077 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nf.svg
--rw-r--r--   0 default   (1000) default   (1000)      567 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ng.svg
--rw-r--r--   0 default   (1000) default   (1000)      734 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ni.svg
--rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nl.svg
--rw-r--r--   0 default   (1000) default   (1000)      782 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-no.svg
--rw-r--r--   0 default   (1000) default   (1000)     1499 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-np.svg
--rw-r--r--   0 default   (1000) default   (1000)      938 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nr.svg
--rw-r--r--   0 default   (1000) default   (1000)     1920 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nu.svg
--rw-r--r--   0 default   (1000) default   (1000)     1615 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nz.svg
--rw-r--r--   0 default   (1000) default   (1000)      900 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-om.svg
--rw-r--r--   0 default   (1000) default   (1000)     1016 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pa.svg
--rw-r--r--   0 default   (1000) default   (1000)      567 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pe.svg
--rw-r--r--   0 default   (1000) default   (1000)     1794 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pf.svg
--rw-r--r--   0 default   (1000) default   (1000)     1669 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pg.svg
--rw-r--r--   0 default   (1000) default   (1000)     1429 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ph.svg
--rw-r--r--   0 default   (1000) default   (1000)     1368 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pk.svg
--rw-r--r--   0 default   (1000) default   (1000)      552 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pl.svg
--rw-r--r--   0 default   (1000) default   (1000)     3087 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pm.svg
--rw-r--r--   0 default   (1000) default   (1000)     2235 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pn.svg
--rw-r--r--   0 default   (1000) default   (1000)      890 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pr.svg
--rw-r--r--   0 default   (1000) default   (1000)      952 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ps.svg
--rw-r--r--   0 default   (1000) default   (1000)     1358 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pt.svg
--rw-r--r--   0 default   (1000) default   (1000)      722 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pw.svg
--rw-r--r--   0 default   (1000) default   (1000)      924 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-py.svg
--rw-r--r--   0 default   (1000) default   (1000)      630 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-qa.svg
--rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-re.svg
--rw-r--r--   0 default   (1000) default   (1000)      910 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ro.svg
--rw-r--r--   0 default   (1000) default   (1000)     1563 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-rs.svg
--rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ru.svg
--rw-r--r--   0 default   (1000) default   (1000)     1237 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-rw.svg
--rw-r--r--   0 default   (1000) default   (1000)     2711 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sa.svg
--rw-r--r--   0 default   (1000) default   (1000)     2349 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sb.svg
--rw-r--r--   0 default   (1000) default   (1000)     1349 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sc.svg
--rw-r--r--   0 default   (1000) default   (1000)      952 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sd.svg
--rw-r--r--   0 default   (1000) default   (1000)      727 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-se.svg
--rw-r--r--   0 default   (1000) default   (1000)      785 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sg.svg
--rw-r--r--   0 default   (1000) default   (1000)     2379 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sh.svg
--rw-r--r--   0 default   (1000) default   (1000)      833 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-si.svg
--rw-r--r--   0 default   (1000) default   (1000)      782 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sj.svg
--rw-r--r--   0 default   (1000) default   (1000)     2502 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sk.svg
--rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sl.svg
--rw-r--r--   0 default   (1000) default   (1000)      847 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sm.svg
--rw-r--r--   0 default   (1000) default   (1000)     1038 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sn.svg
--rw-r--r--   0 default   (1000) default   (1000)      644 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-so.svg
--rw-r--r--   0 default   (1000) default   (1000)     1050 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sr.svg
--rw-r--r--   0 default   (1000) default   (1000)     1483 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ss.svg
--rw-r--r--   0 default   (1000) default   (1000)     1304 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-st.svg
--rw-r--r--   0 default   (1000) default   (1000)      836 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sv.svg
--rw-r--r--   0 default   (1000) default   (1000)     1881 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sx.svg
--rw-r--r--   0 default   (1000) default   (1000)     1128 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sy.svg
--rw-r--r--   0 default   (1000) default   (1000)     1511 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sz.svg
--rw-r--r--   0 default   (1000) default   (1000)     2128 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tc.svg
--rw-r--r--   0 default   (1000) default   (1000)      910 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-td.svg
--rw-r--r--   0 default   (1000) default   (1000)     1329 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tf.svg
--rw-r--r--   0 default   (1000) default   (1000)     1067 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tg.svg
--rw-r--r--   0 default   (1000) default   (1000)      762 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-th.svg
--rw-r--r--   0 default   (1000) default   (1000)     1092 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tj.svg
--rw-r--r--   0 default   (1000) default   (1000)     1081 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tk.svg
--rw-r--r--   0 default   (1000) default   (1000)     1081 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tl.svg
--rw-r--r--   0 default   (1000) default   (1000)     2403 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tm.svg
--rw-r--r--   0 default   (1000) default   (1000)      761 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tn.svg
--rw-r--r--   0 default   (1000) default   (1000)      972 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-to.svg
--rw-r--r--   0 default   (1000) default   (1000)      786 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tr.svg
--rw-r--r--   0 default   (1000) default   (1000)      929 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tt.svg
--rw-r--r--   0 default   (1000) default   (1000)     2173 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tv.svg
--rw-r--r--   0 default   (1000) default   (1000)      893 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tw.svg
--rw-r--r--   0 default   (1000) default   (1000)     1200 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tz.svg
--rw-r--r--   0 default   (1000) default   (1000)      710 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ua.svg
--rw-r--r--   0 default   (1000) default   (1000)     1794 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ug.svg
--rw-r--r--   0 default   (1000) default   (1000)     1478 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-um.svg
--rw-r--r--   0 default   (1000) default   (1000)     1478 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-us.svg
--rw-r--r--   0 default   (1000) default   (1000)     1520 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-uy.svg
--rw-r--r--   0 default   (1000) default   (1000)      987 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-uz.svg
--rw-r--r--   0 default   (1000) default   (1000)     2009 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-va.svg
--rw-r--r--   0 default   (1000) default   (1000)     1178 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vc.svg
--rw-r--r--   0 default   (1000) default   (1000)     1117 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ve.svg
--rw-r--r--   0 default   (1000) default   (1000)     2341 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vg.svg
--rw-r--r--   0 default   (1000) default   (1000)     5594 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vi.svg
--rw-r--r--   0 default   (1000) default   (1000)      802 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vn.svg
--rw-r--r--   0 default   (1000) default   (1000)     1382 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vu.svg
--rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-wf.svg
--rw-r--r--   0 default   (1000) default   (1000)     1060 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ws.svg
--rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ye.svg
--rw-r--r--   0 default   (1000) default   (1000)     4143 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-yt.svg
--rw-r--r--   0 default   (1000) default   (1000)     1408 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-za.svg
--rw-r--r--   0 default   (1000) default   (1000)     1795 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-zm.svg
--rw-r--r--   0 default   (1000) default   (1000)     1382 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-zw.svg
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.415174 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/status/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/status/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)      127 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/status/nplus-status-available-symbolic.svg
--rw-r--r--   0 default   (1000) default   (1000)      264 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/status/nplus-status-away-symbolic.svg
--rw-r--r--   0 default   (1000) default   (1000)      229 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/status/nplus-status-offline-symbolic.svg
--rw-r--r--   0 default   (1000) default   (1000)      303 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/status/nplus-tab-changed-symbolic.svg
--rw-r--r--   0 default   (1000) default   (1000)      111 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/status/nplus-tab-highlight-symbolic.svg
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.242177 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/symbolic/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.415174 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/symbolic/apps/
--rw-r--r--   0 default   (1000) default   (1000)      471 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/symbolic/apps/org.nicotine_plus.Nicotine-symbolic.svg
--rw-r--r--   0 default   (1000) default   (1000)    19520 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/interests.py
--rw-r--r--   0 default   (1000) default   (1000)    44036 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/mainwindow.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.419174 nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)     4290 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/chatcommandhelp.py
--rw-r--r--   0 default   (1000) default   (1000)     8428 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/chathistory.py
--rw-r--r--   0 default   (1000) default   (1000)     1148 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/downloadspeeds.py
--rw-r--r--   0 default   (1000) default   (1000)    10376 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/roomlist.py
--rw-r--r--   0 default   (1000) default   (1000)     3405 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/roomwall.py
--rw-r--r--   0 default   (1000) default   (1000)     1145 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/searchfilterhelp.py
--rw-r--r--   0 default   (1000) default   (1000)     3869 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/transferspeeds.py
--rw-r--r--   0 default   (1000) default   (1000)     1140 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/uploadspeeds.py
--rw-r--r--   0 default   (1000) default   (1000)    19501 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/privatechat.py
--rw-r--r--   0 default   (1000) default   (1000)    66579 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/search.py
--rw-r--r--   0 default   (1000) default   (1000)    42533 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/transfers.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.423174 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)     2205 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/buddies.ui
--rw-r--r--   0 default   (1000) default   (1000)    12957 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/chatrooms.ui
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.425174 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)    10107 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/about.ui
--rw-r--r--   0 default   (1000) default   (1000)    27088 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/fastconfigure.ui
--rw-r--r--   0 default   (1000) default   (1000)    11763 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/fileproperties.ui
--rw-r--r--   0 default   (1000) default   (1000)     2687 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/preferences.ui
--rw-r--r--   0 default   (1000) default   (1000)    14958 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/shortcuts.ui
--rw-r--r--   0 default   (1000) default   (1000)    12229 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/statistics.ui
--rw-r--r--   0 default   (1000) default   (1000)     7574 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/wishlist.ui
--rw-r--r--   0 default   (1000) default   (1000)     9000 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/downloads.ui
--rw-r--r--   0 default   (1000) default   (1000)     9800 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/interests.ui
--rw-r--r--   0 default   (1000) default   (1000)    91518 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/mainwindow.ui
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.427174 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)     1585 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/chathistory.ui
--rw-r--r--   0 default   (1000) default   (1000)     3865 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/downloadspeeds.ui
--rw-r--r--   0 default   (1000) default   (1000)     4562 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/roomlist.ui
--rw-r--r--   0 default   (1000) default   (1000)     2123 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/roomwall.ui
--rw-r--r--   0 default   (1000) default   (1000)    21077 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/searchfilterhelp.ui
--rw-r--r--   0 default   (1000) default   (1000)     3857 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/uploadspeeds.ui
--rw-r--r--   0 default   (1000) default   (1000)     4258 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/privatechat.ui
--rw-r--r--   0 default   (1000) default   (1000)    19243 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/search.ui
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.430174 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)    18563 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/ban.ui
--rw-r--r--   0 default   (1000) default   (1000)    48075 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/chats.ui
--rw-r--r--   0 default   (1000) default   (1000)    28503 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/downloads.ui
--rw-r--r--   0 default   (1000) default   (1000)    15345 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/ignore.ui
--rw-r--r--   0 default   (1000) default   (1000)    12528 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/log.ui
--rw-r--r--   0 default   (1000) default   (1000)    16388 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/network.ui
--rw-r--r--   0 default   (1000) default   (1000)     7466 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/nowplaying.ui
--rw-r--r--   0 default   (1000) default   (1000)    15448 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/plugin.ui
--rw-r--r--   0 default   (1000) default   (1000)    29269 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/search.ui
--rw-r--r--   0 default   (1000) default   (1000)    10474 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/shares.ui
--rw-r--r--   0 default   (1000) default   (1000)    16898 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/uploads.ui
--rw-r--r--   0 default   (1000) default   (1000)     7955 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/urlhandlers.ui
--rw-r--r--   0 default   (1000) default   (1000)     4163 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/userinfo.ui
--rw-r--r--   0 default   (1000) default   (1000)    91850 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/userinterface.ui
--rw-r--r--   0 default   (1000) default   (1000)    10457 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/uploads.ui
--rw-r--r--   0 default   (1000) default   (1000)    15231 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/userbrowse.ui
--rw-r--r--   0 default   (1000) default   (1000)    40552 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/ui/userinfo.ui
--rw-r--r--   0 default   (1000) default   (1000)     8099 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/uploads.py
--rw-r--r--   0 default   (1000) default   (1000)    53390 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/userbrowse.py
--rw-r--r--   0 default   (1000) default   (1000)    25533 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/userinfo.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.437174 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)     3756 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/accelerator.py
--rw-r--r--   0 default   (1000) default   (1000)     1391 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/clipboard.py
--rw-r--r--   0 default   (1000) default   (1000)    22735 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/dialogs.py
--rw-r--r--   0 default   (1000) default   (1000)    13452 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/filechooser.py
--rw-r--r--   0 default   (1000) default   (1000)    28505 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/iconnotebook.py
--rw-r--r--   0 default   (1000) default   (1000)     3539 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/infobar.py
--rw-r--r--   0 default   (1000) default   (1000)     2924 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/popover.py
--rw-r--r--   0 default   (1000) default   (1000)    19042 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/popupmenu.py
--rw-r--r--   0 default   (1000) default   (1000)    31842 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/textentry.py
--rw-r--r--   0 default   (1000) default   (1000)    16824 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/textview.py
--rw-r--r--   0 default   (1000) default   (1000)    19601 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/theme.py
--rw-r--r--   0 default   (1000) default   (1000)    37425 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/trayicon.py
--rw-r--r--   0 default   (1000) default   (1000)    33332 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/treeview.py
--rw-r--r--   0 default   (1000) default   (1000)     3496 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/ui.py
--rw-r--r--   0 default   (1000) default   (1000)     2313 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/window.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.437174 nicotine_plus-3.3.3/pynicotine/headless/
--rw-r--r--   0 default   (1000) default   (1000)      903 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/headless/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)     4080 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/headless/application.py
--rw-r--r--   0 default   (1000) default   (1000)     2713 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/i18n.py
--rw-r--r--   0 default   (1000) default   (1000)     4258 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/interests.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.438174 nicotine_plus-3.3.3/pynicotine/locale/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:11.000000 nicotine_plus-3.3.3/pynicotine/locale/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.438174 nicotine_plus-3.3.3/pynicotine/locale/ca/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.438174 nicotine_plus-3.3.3/pynicotine/locale/ca/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/ca/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/ca/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.439174 nicotine_plus-3.3.3/pynicotine/locale/de/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.439174 nicotine_plus-3.3.3/pynicotine/locale/de/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/de/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/de/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.439174 nicotine_plus-3.3.3/pynicotine/locale/es_CL/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.439174 nicotine_plus-3.3.3/pynicotine/locale/es_CL/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/es_CL/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/es_CL/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.440174 nicotine_plus-3.3.3/pynicotine/locale/es_ES/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.440174 nicotine_plus-3.3.3/pynicotine/locale/es_ES/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/es_ES/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/es_ES/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.441174 nicotine_plus-3.3.3/pynicotine/locale/et/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.441174 nicotine_plus-3.3.3/pynicotine/locale/et/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/et/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/et/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.441174 nicotine_plus-3.3.3/pynicotine/locale/fr/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.442174 nicotine_plus-3.3.3/pynicotine/locale/fr/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/fr/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/fr/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.442174 nicotine_plus-3.3.3/pynicotine/locale/hu/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.442174 nicotine_plus-3.3.3/pynicotine/locale/hu/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/hu/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/hu/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.443174 nicotine_plus-3.3.3/pynicotine/locale/it/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.443174 nicotine_plus-3.3.3/pynicotine/locale/it/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/it/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/it/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.443174 nicotine_plus-3.3.3/pynicotine/locale/lv/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.444174 nicotine_plus-3.3.3/pynicotine/locale/lv/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/lv/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/lv/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.444174 nicotine_plus-3.3.3/pynicotine/locale/nl/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.444174 nicotine_plus-3.3.3/pynicotine/locale/nl/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/nl/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/nl/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.445174 nicotine_plus-3.3.3/pynicotine/locale/pl/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.445174 nicotine_plus-3.3.3/pynicotine/locale/pl/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/pl/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/pl/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.445174 nicotine_plus-3.3.3/pynicotine/locale/pt_BR/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.446174 nicotine_plus-3.3.3/pynicotine/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/pt_BR/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/pt_BR/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.446174 nicotine_plus-3.3.3/pynicotine/locale/pt_PT/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.446174 nicotine_plus-3.3.3/pynicotine/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/pt_PT/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/pt_PT/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.447174 nicotine_plus-3.3.3/pynicotine/locale/ru/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.447174 nicotine_plus-3.3.3/pynicotine/locale/ru/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/ru/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/ru/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.448174 nicotine_plus-3.3.3/pynicotine/locale/tr/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.448174 nicotine_plus-3.3.3/pynicotine/locale/tr/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/tr/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:10.000000 nicotine_plus-3.3.3/pynicotine/locale/tr/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.449174 nicotine_plus-3.3.3/pynicotine/locale/uk/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.449174 nicotine_plus-3.3.3/pynicotine/locale/uk/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:11.000000 nicotine_plus-3.3.3/pynicotine/locale/uk/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:11.000000 nicotine_plus-3.3.3/pynicotine/locale/uk/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.449174 nicotine_plus-3.3.3/pynicotine/locale/zh_CN/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.450173 nicotine_plus-3.3.3/pynicotine/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:11.000000 nicotine_plus-3.3.3/pynicotine/locale/zh_CN/LC_MESSAGES/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:39:11.000000 nicotine_plus-3.3.3/pynicotine/locale/zh_CN/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)    11904 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/logfacility.py
--rw-r--r--   0 default   (1000) default   (1000)    20761 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/networkfilter.py
--rw-r--r--   0 default   (1000) default   (1000)     3132 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/notifications.py
--rw-r--r--   0 default   (1000) default   (1000)    10986 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/nowplaying.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.451174 nicotine_plus-3.3.3/pynicotine/plugins/
--rw-r--r--   0 default   (1000) default   (1000)     1984 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/README.md
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.452174 nicotine_plus-3.3.3/pynicotine/plugins/anti_shout/
--rw-r--r--   0 default   (1000) default   (1000)      167 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/anti_shout/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)     2539 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/anti_shout/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.454173 nicotine_plus-3.3.3/pynicotine/plugins/auto_user_browse/
--rw-r--r--   0 default   (1000) default   (1000)      166 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/auto_user_browse/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)     2056 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/auto_user_browse/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.455173 nicotine_plus-3.3.3/pynicotine/plugins/core_commands/
--rw-r--r--   0 default   (1000) default   (1000)       81 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/core_commands/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)    22036 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/core_commands/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.456174 nicotine_plus-3.3.3/pynicotine/plugins/examplars/
--rw-r--r--   0 default   (1000) default   (1000)      156 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/examplars/README.md
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/examplars/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.457173 nicotine_plus-3.3.3/pynicotine/plugins/examplars/commands/
--rw-r--r--   0 default   (1000) default   (1000)      173 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/examplars/commands/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)     1440 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/examplars/commands/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.457173 nicotine_plus-3.3.3/pynicotine/plugins/examplars/memory_debugger/
--rw-r--r--   0 default   (1000) default   (1000)      218 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/examplars/memory_debugger/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)     2658 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/examplars/memory_debugger/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.458173 nicotine_plus-3.3.3/pynicotine/plugins/examplars/port_checker/
--rw-r--r--   0 default   (1000) default   (1000)      297 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/examplars/port_checker/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)     3571 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/examplars/port_checker/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.459173 nicotine_plus-3.3.3/pynicotine/plugins/examplars/preferences/
--rw-r--r--   0 default   (1000) default   (1000)     1742 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/examplars/preferences/choices.py
--rw-r--r--   0 default   (1000) default   (1000)     1579 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/examplars/preferences/filechooser.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.459173 nicotine_plus-3.3.3/pynicotine/plugins/examplars/testreplier/
--rw-r--r--   0 default   (1000) default   (1000)      199 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/examplars/testreplier/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)     1606 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/examplars/testreplier/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.460173 nicotine_plus-3.3.3/pynicotine/plugins/leech_detector/
--rw-r--r--   0 default   (1000) default   (1000)      284 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/leech_detector/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)     7186 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/leech_detector/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.461173 nicotine_plus-3.3.3/pynicotine/plugins/multipaste/
--rw-r--r--   0 default   (1000) default   (1000)      281 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/multipaste/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)     2623 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/multipaste/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.461173 nicotine_plus-3.3.3/pynicotine/plugins/now_playing_search/
--rw-r--r--   0 default   (1000) default   (1000)      514 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/now_playing_search/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)     1574 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/now_playing_search/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.462173 nicotine_plus-3.3.3/pynicotine/plugins/now_playing_sender/
--rw-r--r--   0 default   (1000) default   (1000)      390 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/now_playing_sender/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)     5072 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/now_playing_sender/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.462173 nicotine_plus-3.3.3/pynicotine/plugins/plugin_debugger/
--rw-r--r--   0 default   (1000) default   (1000)      181 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/plugin_debugger/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)     5930 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/plugin_debugger/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.463173 nicotine_plus-3.3.3/pynicotine/plugins/spamfilter/
--rw-r--r--   0 default   (1000) default   (1000)      559 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/spamfilter/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)     3159 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/spamfilter/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.463173 nicotine_plus-3.3.3/pynicotine/plugins/youtube_info/
--rw-r--r--   0 default   (1000) default   (1000)      376 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/youtube_info/PLUGININFO
--rw-r--r--   0 default   (1000) default   (1000)     6728 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/plugins/youtube_info/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)    37898 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/pluginsystem.py
--rw-r--r--   0 default   (1000) default   (1000)    24109 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/portmapper.py
--rw-r--r--   0 default   (1000) default   (1000)    11586 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/privatechat.py
--rw-r--r--   0 default   (1000) default   (1000)    26152 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/search.py
--rw-r--r--   0 default   (1000) default   (1000)    42929 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/shares.py
--rw-r--r--   0 default   (1000) default   (1000)   114474 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/slskmessages.py
--rw-r--r--   0 default   (1000) default   (1000)   103679 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/slskproto.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.464173 nicotine_plus-3.3.3/pynicotine/tests/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.464173 nicotine_plus-3.3.3/pynicotine/tests/integration/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/integration/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)     3857 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/integration/test_startup.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.465173 nicotine_plus-3.3.3/pynicotine/tests/unit/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/__init__.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.466173 nicotine_plus-3.3.3/pynicotine/tests/unit/config/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/config/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)       70 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/config/config
--rw-r--r--   0 default   (1000) default   (1000)     2878 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/config/test_config.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.466173 nicotine_plus-3.3.3/pynicotine/tests/unit/networkfilter/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/networkfilter/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)     2785 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/networkfilter/test_country.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.468173 nicotine_plus-3.3.3/pynicotine/tests/unit/protocol/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/protocol/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)    10065 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/protocol/test_slskmessages.py
--rw-r--r--   0 default   (1000) default   (1000)     4789 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/protocol/test_slskproto.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.469173 nicotine_plus-3.3.3/pynicotine/tests/unit/search/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/search/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)     6661 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/search/test_search.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.469173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.470173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.471173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/.def/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/.def/nothing2
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/.def_file
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/.hidden_file2
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.471173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/.uvw/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/.uvw/nothing2
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/.uvw_file
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.257177 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/buddies/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.471173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/buddies/folder/
--rw-r--r--   0 default   (1000) default   (1000)       10 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/buddies/folder/somefile.txt
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/dummy_file2
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.257177 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder3/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.472173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder3/.poof2/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder3/.poof2/nothing2
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.472173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder3/test2/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder3/test2/nothing2
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.472173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder4/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder4/nothing2
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.473173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/something2/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedbuddyfiles/something2/nothing2
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.474173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.474173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/.abc/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/.abc/nothing
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/.abc_file
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/.hidden_file
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.475173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/.xyz/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/.xyz/nothing
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/.xyz_file
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/dummy_file
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.475173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/folder1/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/folder1/nothing
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.259177 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/folder2/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.475173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/folder2/.poof/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/folder2/.poof/nothing
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.475173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/folder2/test/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/folder2/test/nothing
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.476173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/something/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedfiles/something/nothing
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.476173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedinvalidfiles/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedinvalidfiles/file.txt
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.476173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedtrustedfiles/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedtrustedfiles/.hidden_file3
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.477173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedtrustedfiles/.hidden_folder/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedtrustedfiles/.hidden_folder/nothing
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedtrustedfiles/dummy_file3
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.261177 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.477173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/.hidden/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/.hidden/nothing
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.261177 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/folder2/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.261177 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/folder2/folder3/
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.477173 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/folder2/folder3/folder4/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/folder2/folder3/folder4/nothing
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)    10457 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/shares/test_shares.py
--rw-r--r--   0 default   (1000) default   (1000)     1486 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/test_i18n.py
--rw-r--r--   0 default   (1000) default   (1000)     1599 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/test_version.py
-drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-05 18:39:12.479173 nicotine_plus-3.3.3/pynicotine/tests/unit/transfers/
--rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/transfers/__init__.py
--rw-r--r--   0 default   (1000) default   (1000)     1621 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/transfers/downloads.json
--rw-r--r--   0 default   (1000) default   (1000)    15004 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/transfers/test_downloads.py
--rw-r--r--   0 default   (1000) default   (1000)    11059 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/transfers/test_get_upload_candidate.py
--rw-r--r--   0 default   (1000) default   (1000)     4151 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/transfers/test_uploads.py
--rw-r--r--   0 default   (1000) default   (1000)      426 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/tests/unit/transfers/uploads.json
--rw-r--r--   0 default   (1000) default   (1000)    17935 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/transfers.py
--rw-r--r--   0 default   (1000) default   (1000)    43643 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/uploads.py
--rw-r--r--   0 default   (1000) default   (1000)    13546 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/userbrowse.py
--rw-r--r--   0 default   (1000) default   (1000)     6671 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/userinfo.py
--rw-r--r--   0 default   (1000) default   (1000)    13673 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/users.py
--rw-r--r--   0 default   (1000) default   (1000)    28654 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pynicotine/utils.py
--rw-r--r--   0 default   (1000) default   (1000)       81 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/pyproject.toml
--rw-r--r--   0 default   (1000) default   (1000)     2919 2024-05-05 18:39:12.482173 nicotine_plus-3.3.3/setup.cfg
--rw-r--r--   0 default   (1000) default   (1000)     4825 2024-05-05 18:38:34.000000 nicotine_plus-3.3.3/setup.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.024782 nicotine_plus-3.3.4/
+-rw-r--r--   0 default   (1000) default   (1000)     3734 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/AUTHORS.md
+-rw-r--r--   0 default   (1000) default   (1000)    35147 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/COPYING
+-rw-r--r--   0 default   (1000) default   (1000)      545 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/MANIFEST.in
+-rw-r--r--   0 default   (1000) default   (1000)   202794 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/NEWS.md
+-rw-r--r--   0 default   (1000) default   (1000)     1276 2024-05-06 22:22:10.024782 nicotine_plus-3.3.4/PKG-INFO
+-rw-r--r--   0 default   (1000) default   (1000)     3043 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/README.md
+-rw-r--r--   0 default   (1000) default   (1000)     2781 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/TRANSLATORS.md
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.849783 nicotine_plus-3.3.4/data/
+-rw-r--r--   0 default   (1000) default   (1000)     1523 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/data/nicotine.1
+-rw-r--r--   0 default   (1000) default   (1000)     5178 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/data/org.nicotine_plus.Nicotine.appdata.xml.in
+-rw-r--r--   0 default   (1000) default   (1000)      424 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/data/org.nicotine_plus.Nicotine.desktop.in
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.849783 nicotine_plus-3.3.4/data/scripts/
+-rw-r--r--   0 default   (1000) default   (1000)     5030 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/data/scripts/update_ip_country_data.py
+-rw-r--r--   0 default   (1000) default   (1000)     1838 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/data/scripts/update_translation_template.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.851783 nicotine_plus-3.3.4/doc/
+-rw-r--r--   0 default   (1000) default   (1000)     2377 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/doc/DEPENDENCIES.md
+-rw-r--r--   0 default   (1000) default   (1000)    13491 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/doc/DEVELOPING.md
+-rw-r--r--   0 default   (1000) default   (1000)     6999 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/doc/DOWNLOADS.md
+-rw-r--r--   0 default   (1000) default   (1000)     3106 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/doc/PACKAGING.md
+-rw-r--r--   0 default   (1000) default   (1000)    80371 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/doc/SLSKPROTOCOL.md
+-rw-r--r--   0 default   (1000) default   (1000)     5104 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/doc/TESTING.md
+-rw-r--r--   0 default   (1000) default   (1000)     4757 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/doc/TRANSLATIONS.md
+-rwxr-xr-x   0 default   (1000) default   (1000)     1269 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/nicotine
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.022782 nicotine_plus-3.3.4/nicotine_plus.egg-info/
+-rw-r--r--   0 default   (1000) default   (1000)     1276 2024-05-06 22:22:09.000000 nicotine_plus-3.3.4/nicotine_plus.egg-info/PKG-INFO
+-rw-r--r--   0 default   (1000) default   (1000)    28692 2024-05-06 22:22:09.000000 nicotine_plus-3.3.4/nicotine_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 default   (1000) default   (1000)        1 2024-05-06 22:22:09.000000 nicotine_plus-3.3.4/nicotine_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 default   (1000) default   (1000)       67 2024-05-06 22:22:09.000000 nicotine_plus-3.3.4/nicotine_plus.egg-info/requires.txt
+-rw-r--r--   0 default   (1000) default   (1000)       11 2024-05-06 22:22:09.000000 nicotine_plus-3.3.4/nicotine_plus.egg-info/top_level.txt
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.867783 nicotine_plus-3.3.4/po/
+-rw-r--r--   0 default   (1000) default   (1000)       65 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/LINGUAS
+-rw-r--r--   0 default   (1000) default   (1000)   138793 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/ar.po
+-rw-r--r--   0 default   (1000) default   (1000)   211752 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/ca.po
+-rw-r--r--   0 default   (1000) default   (1000)   239736 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/cs.po
+-rw-r--r--   0 default   (1000) default   (1000)   238187 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/da.po
+-rw-r--r--   0 default   (1000) default   (1000)   246309 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/de.po
+-rw-r--r--   0 default   (1000) default   (1000)   228944 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/eo.po
+-rw-r--r--   0 default   (1000) default   (1000)   236357 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/es_CL.po
+-rw-r--r--   0 default   (1000) default   (1000)   235213 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/es_ES.po
+-rw-r--r--   0 default   (1000) default   (1000)   194522 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/et.po
+-rw-r--r--   0 default   (1000) default   (1000)   248049 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/eu.po
+-rw-r--r--   0 default   (1000) default   (1000)   249549 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/fi.po
+-rw-r--r--   0 default   (1000) default   (1000)   239542 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/fr.po
+-rw-r--r--   0 default   (1000) default   (1000)   264914 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/hu.po
+-rw-r--r--   0 default   (1000) default   (1000)   235367 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/it.po
+-rw-r--r--   0 default   (1000) default   (1000)   246272 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/lt.po
+-rw-r--r--   0 default   (1000) default   (1000)   210152 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/lv.po
+-rw-r--r--   0 default   (1000) default   (1000)   229665 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/nb_NO.po
+-rw-r--r--   0 default   (1000) default   (1000)   138000 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/nicotine.pot
+-rw-r--r--   0 default   (1000) default   (1000)   262715 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/nl.po
+-rw-r--r--   0 default   (1000) default   (1000)   271139 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/pl.po
+-rw-r--r--   0 default   (1000) default   (1000)   239311 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/pt_BR.po
+-rw-r--r--   0 default   (1000) default   (1000)   182641 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/pt_PT.po
+-rw-r--r--   0 default   (1000) default   (1000)   200906 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/ro.po
+-rw-r--r--   0 default   (1000) default   (1000)   254214 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/ru.po
+-rw-r--r--   0 default   (1000) default   (1000)   254027 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/sk.po
+-rw-r--r--   0 default   (1000) default   (1000)   143517 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/sq.po
+-rw-r--r--   0 default   (1000) default   (1000)   239340 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/sv.po
+-rw-r--r--   0 default   (1000) default   (1000)   231510 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/tr.po
+-rw-r--r--   0 default   (1000) default   (1000)   253243 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/uk.po
+-rw-r--r--   0 default   (1000) default   (1000)   198546 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/po/zh_CN.po
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.875783 nicotine_plus-3.3.4/pynicotine/
+-rw-r--r--   0 default   (1000) default   (1000)     7129 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)      801 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/__main__.py
+-rw-r--r--   0 default   (1000) default   (1000)     8642 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/buddies.py
+-rw-r--r--   0 default   (1000) default   (1000)    21348 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/chatrooms.py
+-rw-r--r--   0 default   (1000) default   (1000)     5222 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/cli.py
+-rw-r--r--   0 default   (1000) default   (1000)    29012 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/config.py
+-rw-r--r--   0 default   (1000) default   (1000)    12478 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/core.py
+-rw-r--r--   0 default   (1000) default   (1000)    52454 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/downloads.py
+-rw-r--r--   0 default   (1000) default   (1000)     9156 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/events.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.875783 nicotine_plus-3.3.4/pynicotine/external/
+-rw-r--r--   0 default   (1000) default   (1000)    21663 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/external/README.md
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/external/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.877783 nicotine_plus-3.3.4/pynicotine/external/data/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/external/data/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)   747340 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/external/data/country_codes.py
+-rw-r--r--   0 default   (1000) default   (1000)  2696565 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/external/data/ip_ranges.py
+-rw-r--r--   0 default   (1000) default   (1000)    71390 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/external/tinytag.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.886783 nicotine_plus-3.3.4/pynicotine/gtkgui/
+-rw-r--r--   0 default   (1000) default   (1000)     5735 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)    38383 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/application.py
+-rw-r--r--   0 default   (1000) default   (1000)    16598 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/buddies.py
+-rw-r--r--   0 default   (1000) default   (1000)    34847 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/chatrooms.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.887782 nicotine_plus-3.3.4/pynicotine/gtkgui/css/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/css/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)     2240 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/css/style.css
+-rw-r--r--   0 default   (1000) default   (1000)      648 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/css/style_gtk3.css
+-rw-r--r--   0 default   (1000) default   (1000)      899 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/css/style_gtk4.css
+-rw-r--r--   0 default   (1000) default   (1000)      783 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/css/style_gtk4_darwin.css
+-rw-r--r--   0 default   (1000) default   (1000)      406 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/css/style_libadwaita.css
+-rw-r--r--   0 default   (1000) default   (1000)      554 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/css/style_libadwaita_csd.css
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.890782 nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)    13990 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/about.py
+-rw-r--r--   0 default   (1000) default   (1000)    10335 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/fastconfigure.py
+-rw-r--r--   0 default   (1000) default   (1000)     5268 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/fileproperties.py
+-rw-r--r--   0 default   (1000) default   (1000)    16955 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/pluginsettings.py
+-rw-r--r--   0 default   (1000) default   (1000)   128248 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/preferences.py
+-rw-r--r--   0 default   (1000) default   (1000)     1298 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/shortcuts.py
+-rw-r--r--   0 default   (1000) default   (1000)     4578 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/statistics.py
+-rw-r--r--   0 default   (1000) default   (1000)     7066 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/wishlist.py
+-rw-r--r--   0 default   (1000) default   (1000)     8444 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/downloads.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.890782 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.890782 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.827783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/128x128/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.890782 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/128x128/apps/
+-rw-r--r--   0 default   (1000) default   (1000)      824 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/128x128/apps/org.nicotine_plus.Nicotine.svg
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.827783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/16x16/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.891783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/16x16/apps/
+-rw-r--r--   0 default   (1000) default   (1000)     1053 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/16x16/apps/org.nicotine_plus.Nicotine.svg
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.827783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/24x24/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.891783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/24x24/apps/
+-rw-r--r--   0 default   (1000) default   (1000)      772 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/24x24/apps/org.nicotine_plus.Nicotine.svg
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.827783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/256x256/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.891783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/256x256/apps/
+-rw-r--r--   0 default   (1000) default   (1000)      862 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/256x256/apps/org.nicotine_plus.Nicotine.svg
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.828783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/32x32/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.891783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/32x32/apps/
+-rw-r--r--   0 default   (1000) default   (1000)      799 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/32x32/apps/org.nicotine_plus.Nicotine.svg
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.828783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/48x48/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.891783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/48x48/apps/
+-rw-r--r--   0 default   (1000) default   (1000)      868 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/48x48/apps/org.nicotine_plus.Nicotine.svg
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.828783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/64x64/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.892783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/64x64/apps/
+-rw-r--r--   0 default   (1000) default   (1000)      871 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/64x64/apps/org.nicotine_plus.Nicotine.svg
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.892783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.893782 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/apps/
+-rw-r--r--   0 default   (1000) default   (1000)     1048 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-away.svg
+-rw-r--r--   0 default   (1000) default   (1000)      881 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-connect.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1091 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-disconnect.svg
+-rw-r--r--   0 default   (1000) default   (1000)      999 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-msg.svg
+-rw-r--r--   0 default   (1000) default   (1000)      824 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine.svg
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.963782 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)     1285 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ad.svg
+-rw-r--r--   0 default   (1000) default   (1000)      947 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ae.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1231 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-af.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1610 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ag.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2222 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ai.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1727 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-al.svg
+-rw-r--r--   0 default   (1000) default   (1000)      908 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-am.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1392 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ao.svg
+-rw-r--r--   0 default   (1000) default   (1000)      701 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ar.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1493 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-as.svg
+-rw-r--r--   0 default   (1000) default   (1000)      565 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-at.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1775 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-au.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1023 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-aw.svg
+-rw-r--r--   0 default   (1000) default   (1000)      940 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ax.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1033 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-az.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1070 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ba.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1904 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bb.svg
+-rw-r--r--   0 default   (1000) default   (1000)      722 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bd.svg
+-rw-r--r--   0 default   (1000) default   (1000)      910 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-be.svg
+-rw-r--r--   0 default   (1000) default   (1000)      837 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bf.svg
+-rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bg.svg
+-rw-r--r--   0 default   (1000) default   (1000)      630 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bh.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1722 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bi.svg
+-rw-r--r--   0 default   (1000) default   (1000)      907 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bj.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1700 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bl.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2151 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bm.svg
+-rw-r--r--   0 default   (1000) default   (1000)      839 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bn.svg
+-rw-r--r--   0 default   (1000) default   (1000)      908 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bo.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1314 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-br.svg
+-rw-r--r--   0 default   (1000) default   (1000)      925 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bs.svg
+-rw-r--r--   0 default   (1000) default   (1000)      712 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bt.svg
+-rw-r--r--   0 default   (1000) default   (1000)      782 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bv.svg
+-rw-r--r--   0 default   (1000) default   (1000)      762 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bw.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1116 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-by.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1631 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bz.svg
+-rw-r--r--   0 default   (1000) default   (1000)      904 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ca.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1237 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cc.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1012 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cd.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1422 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cf.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1060 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cg.svg
+-rw-r--r--   0 default   (1000) default   (1000)      790 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ch.svg
+-rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ci.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1697 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ck.svg
+-rw-r--r--   0 default   (1000) default   (1000)      874 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cl.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1241 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cm.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1323 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cn.svg
+-rw-r--r--   0 default   (1000) default   (1000)      908 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-co.svg
+-rw-r--r--   0 default   (1000) default   (1000)      762 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cr.svg
+-rw-r--r--   0 default   (1000) default   (1000)      972 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cu.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1611 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cv.svg
+-rw-r--r--   0 default   (1000) default   (1000)      933 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cw.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1844 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cx.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1623 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cy.svg
+-rw-r--r--   0 default   (1000) default   (1000)      754 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cz.svg
+-rw-r--r--   0 default   (1000) default   (1000)      908 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-de.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1042 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dj.svg
+-rw-r--r--   0 default   (1000) default   (1000)      569 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dk.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1988 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dm.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1170 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-do.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1086 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dz.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1430 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ec.svg
+-rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ee.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1788 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-eg.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1364 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-er.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1235 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-es.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1535 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-et.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1632 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-eu.svg
+-rw-r--r--   0 default   (1000) default   (1000)      529 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fi.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2134 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fj.svg
+-rw-r--r--   0 default   (1000) default   (1000)     4020 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fk.svg
+-rw-r--r--   0 default   (1000) default   (1000)      967 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fm.svg
+-rw-r--r--   0 default   (1000) default   (1000)      742 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fo.svg
+-rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fr.svg
+-rw-r--r--   0 default   (1000) default   (1000)      908 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ga.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1330 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gb.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1854 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gd.svg
+-rw-r--r--   0 default   (1000) default   (1000)      855 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ge.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1004 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gf.svg
+-rw-r--r--   0 default   (1000) default   (1000)      791 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gg.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1201 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gh.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1614 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gi.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1095 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gl.svg
+-rw-r--r--   0 default   (1000) default   (1000)      947 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gm.svg
+-rw-r--r--   0 default   (1000) default   (1000)      910 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gn.svg
+-rw-r--r--   0 default   (1000) default   (1000)    10261 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gp.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1281 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gq.svg
+-rw-r--r--   0 default   (1000) default   (1000)      614 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gr.svg
+-rw-r--r--   0 default   (1000) default   (1000)     4785 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gs.svg
+-rw-r--r--   0 default   (1000) default   (1000)      849 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gt.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2731 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gu.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1192 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gw.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1433 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gy.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1531 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hk.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1798 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hm.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1086 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hn.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1450 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hr.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1874 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ht.svg
+-rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hu.svg
+-rw-r--r--   0 default   (1000) default   (1000)      552 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-id.svg
+-rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ie.svg
+-rw-r--r--   0 default   (1000) default   (1000)      742 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-il.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1619 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-im.svg
+-rw-r--r--   0 default   (1000) default   (1000)      996 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-in.svg
+-rw-r--r--   0 default   (1000) default   (1000)     5301 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-io.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1433 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-iq.svg
+-rw-r--r--   0 default   (1000) default   (1000)     3449 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ir.svg
+-rw-r--r--   0 default   (1000) default   (1000)      782 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-is.svg
+-rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-it.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1306 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-je.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1137 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-jm.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1091 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-jo.svg
+-rw-r--r--   0 default   (1000) default   (1000)      525 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-jp.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1604 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ke.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1098 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kg.svg
+-rw-r--r--   0 default   (1000) default   (1000)      994 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kh.svg
+-rw-r--r--   0 default   (1000) default   (1000)     3464 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ki.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1339 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-km.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1434 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kn.svg
+-rw-r--r--   0 default   (1000) default   (1000)      944 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kp.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2304 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kr.svg
+-rw-r--r--   0 default   (1000) default   (1000)      951 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kw.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1892 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ky.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2699 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kz.svg
+-rw-r--r--   0 default   (1000) default   (1000)      774 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-la.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1334 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lb.svg
+-rw-r--r--   0 default   (1000) default   (1000)      959 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lc.svg
+-rw-r--r--   0 default   (1000) default   (1000)      710 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-li.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2836 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lk.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1269 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lr.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1240 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ls.svg
+-rw-r--r--   0 default   (1000) default   (1000)      908 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lt.svg
+-rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lu.svg
+-rw-r--r--   0 default   (1000) default   (1000)      564 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lv.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1033 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ly.svg
+-rw-r--r--   0 default   (1000) default   (1000)      769 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ma.svg
+-rw-r--r--   0 default   (1000) default   (1000)      552 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mc.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1462 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-md.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2943 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-me.svg
+-rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mf.svg
+-rw-r--r--   0 default   (1000) default   (1000)      749 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mg.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1002 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mh.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1303 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mk.svg
+-rw-r--r--   0 default   (1000) default   (1000)      910 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ml.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1038 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mm.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1058 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mn.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1369 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mo.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1103 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mp.svg
+-rw-r--r--   0 default   (1000) default   (1000)     4357 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mq.svg
+-rw-r--r--   0 default   (1000) default   (1000)      866 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mr.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2017 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ms.svg
+-rw-r--r--   0 default   (1000) default   (1000)      849 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mt.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1105 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mu.svg
+-rw-r--r--   0 default   (1000) default   (1000)      823 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mv.svg
+-rw-r--r--   0 default   (1000) default   (1000)      959 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mw.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1047 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mx.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1197 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-my.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1430 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mz.svg
+-rw-r--r--   0 default   (1000) default   (1000)     3248 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-na.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1609 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nc.svg
+-rw-r--r--   0 default   (1000) default   (1000)      957 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ne.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1077 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nf.svg
+-rw-r--r--   0 default   (1000) default   (1000)      567 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ng.svg
+-rw-r--r--   0 default   (1000) default   (1000)      734 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ni.svg
+-rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nl.svg
+-rw-r--r--   0 default   (1000) default   (1000)      782 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-no.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1499 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-np.svg
+-rw-r--r--   0 default   (1000) default   (1000)      938 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nr.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1920 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nu.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1615 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nz.svg
+-rw-r--r--   0 default   (1000) default   (1000)      900 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-om.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1016 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pa.svg
+-rw-r--r--   0 default   (1000) default   (1000)      567 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pe.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1794 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pf.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1669 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pg.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1429 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ph.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1368 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pk.svg
+-rw-r--r--   0 default   (1000) default   (1000)      552 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pl.svg
+-rw-r--r--   0 default   (1000) default   (1000)     3087 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pm.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2235 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pn.svg
+-rw-r--r--   0 default   (1000) default   (1000)      890 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pr.svg
+-rw-r--r--   0 default   (1000) default   (1000)      952 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ps.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1358 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pt.svg
+-rw-r--r--   0 default   (1000) default   (1000)      722 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pw.svg
+-rw-r--r--   0 default   (1000) default   (1000)      924 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-py.svg
+-rw-r--r--   0 default   (1000) default   (1000)      630 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-qa.svg
+-rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-re.svg
+-rw-r--r--   0 default   (1000) default   (1000)      910 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ro.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1563 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-rs.svg
+-rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ru.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1237 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-rw.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2711 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sa.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2349 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sb.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1349 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sc.svg
+-rw-r--r--   0 default   (1000) default   (1000)      952 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sd.svg
+-rw-r--r--   0 default   (1000) default   (1000)      727 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-se.svg
+-rw-r--r--   0 default   (1000) default   (1000)      785 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sg.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2379 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sh.svg
+-rw-r--r--   0 default   (1000) default   (1000)      833 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-si.svg
+-rw-r--r--   0 default   (1000) default   (1000)      782 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sj.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2502 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sk.svg
+-rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sl.svg
+-rw-r--r--   0 default   (1000) default   (1000)      847 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sm.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1038 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sn.svg
+-rw-r--r--   0 default   (1000) default   (1000)      644 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-so.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1050 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sr.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1483 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ss.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1304 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-st.svg
+-rw-r--r--   0 default   (1000) default   (1000)      836 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sv.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1881 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sx.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1128 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sy.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1511 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sz.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2128 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tc.svg
+-rw-r--r--   0 default   (1000) default   (1000)      910 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-td.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1329 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tf.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1067 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tg.svg
+-rw-r--r--   0 default   (1000) default   (1000)      762 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-th.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1092 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tj.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1081 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tk.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1081 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tl.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2403 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tm.svg
+-rw-r--r--   0 default   (1000) default   (1000)      761 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tn.svg
+-rw-r--r--   0 default   (1000) default   (1000)      972 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-to.svg
+-rw-r--r--   0 default   (1000) default   (1000)      786 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tr.svg
+-rw-r--r--   0 default   (1000) default   (1000)      929 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tt.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2173 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tv.svg
+-rw-r--r--   0 default   (1000) default   (1000)      893 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tw.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1200 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tz.svg
+-rw-r--r--   0 default   (1000) default   (1000)      710 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ua.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1794 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ug.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1478 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-um.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1478 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-us.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1520 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-uy.svg
+-rw-r--r--   0 default   (1000) default   (1000)      987 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-uz.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2009 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-va.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1178 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vc.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1117 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ve.svg
+-rw-r--r--   0 default   (1000) default   (1000)     2341 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vg.svg
+-rw-r--r--   0 default   (1000) default   (1000)     5594 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vi.svg
+-rw-r--r--   0 default   (1000) default   (1000)      802 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vn.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1382 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vu.svg
+-rw-r--r--   0 default   (1000) default   (1000)      752 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-wf.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1060 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ws.svg
+-rw-r--r--   0 default   (1000) default   (1000)      750 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ye.svg
+-rw-r--r--   0 default   (1000) default   (1000)     4143 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-yt.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1408 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-za.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1795 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-zm.svg
+-rw-r--r--   0 default   (1000) default   (1000)     1382 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-zw.svg
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.965782 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/status/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/status/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)      127 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/status/nplus-status-available-symbolic.svg
+-rw-r--r--   0 default   (1000) default   (1000)      264 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/status/nplus-status-away-symbolic.svg
+-rw-r--r--   0 default   (1000) default   (1000)      229 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/status/nplus-status-offline-symbolic.svg
+-rw-r--r--   0 default   (1000) default   (1000)      303 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/status/nplus-tab-changed-symbolic.svg
+-rw-r--r--   0 default   (1000) default   (1000)      111 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/status/nplus-tab-highlight-symbolic.svg
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.829783 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/symbolic/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.965782 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/symbolic/apps/
+-rw-r--r--   0 default   (1000) default   (1000)      471 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/symbolic/apps/org.nicotine_plus.Nicotine-symbolic.svg
+-rw-r--r--   0 default   (1000) default   (1000)    19520 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/interests.py
+-rw-r--r--   0 default   (1000) default   (1000)    44036 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/mainwindow.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.968782 nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)     4290 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/chatcommandhelp.py
+-rw-r--r--   0 default   (1000) default   (1000)     8428 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/chathistory.py
+-rw-r--r--   0 default   (1000) default   (1000)     1148 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/downloadspeeds.py
+-rw-r--r--   0 default   (1000) default   (1000)    10376 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/roomlist.py
+-rw-r--r--   0 default   (1000) default   (1000)     3405 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/roomwall.py
+-rw-r--r--   0 default   (1000) default   (1000)     1145 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/searchfilterhelp.py
+-rw-r--r--   0 default   (1000) default   (1000)     3869 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/transferspeeds.py
+-rw-r--r--   0 default   (1000) default   (1000)     1140 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/uploadspeeds.py
+-rw-r--r--   0 default   (1000) default   (1000)    19501 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/privatechat.py
+-rw-r--r--   0 default   (1000) default   (1000)    66579 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/search.py
+-rw-r--r--   0 default   (1000) default   (1000)    42533 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/transfers.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.971782 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)     2205 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/buddies.ui
+-rw-r--r--   0 default   (1000) default   (1000)    12957 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/chatrooms.ui
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.974782 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)    10107 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/about.ui
+-rw-r--r--   0 default   (1000) default   (1000)    27088 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/fastconfigure.ui
+-rw-r--r--   0 default   (1000) default   (1000)    11763 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/fileproperties.ui
+-rw-r--r--   0 default   (1000) default   (1000)     2687 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/preferences.ui
+-rw-r--r--   0 default   (1000) default   (1000)    14958 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/shortcuts.ui
+-rw-r--r--   0 default   (1000) default   (1000)    12229 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/statistics.ui
+-rw-r--r--   0 default   (1000) default   (1000)     7574 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/wishlist.ui
+-rw-r--r--   0 default   (1000) default   (1000)     9000 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/downloads.ui
+-rw-r--r--   0 default   (1000) default   (1000)     9800 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/interests.ui
+-rw-r--r--   0 default   (1000) default   (1000)    91518 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/mainwindow.ui
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.976782 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)     1585 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/chathistory.ui
+-rw-r--r--   0 default   (1000) default   (1000)     3865 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/downloadspeeds.ui
+-rw-r--r--   0 default   (1000) default   (1000)     4562 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/roomlist.ui
+-rw-r--r--   0 default   (1000) default   (1000)     2123 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/roomwall.ui
+-rw-r--r--   0 default   (1000) default   (1000)    21077 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/searchfilterhelp.ui
+-rw-r--r--   0 default   (1000) default   (1000)     3857 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/uploadspeeds.ui
+-rw-r--r--   0 default   (1000) default   (1000)     4258 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/privatechat.ui
+-rw-r--r--   0 default   (1000) default   (1000)    19243 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/search.ui
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.981782 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)    18563 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/ban.ui
+-rw-r--r--   0 default   (1000) default   (1000)    48075 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/chats.ui
+-rw-r--r--   0 default   (1000) default   (1000)    28503 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/downloads.ui
+-rw-r--r--   0 default   (1000) default   (1000)    15345 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/ignore.ui
+-rw-r--r--   0 default   (1000) default   (1000)    12528 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/log.ui
+-rw-r--r--   0 default   (1000) default   (1000)    16388 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/network.ui
+-rw-r--r--   0 default   (1000) default   (1000)     7466 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/nowplaying.ui
+-rw-r--r--   0 default   (1000) default   (1000)    15448 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/plugin.ui
+-rw-r--r--   0 default   (1000) default   (1000)    29269 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/search.ui
+-rw-r--r--   0 default   (1000) default   (1000)    10474 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/shares.ui
+-rw-r--r--   0 default   (1000) default   (1000)    16898 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/uploads.ui
+-rw-r--r--   0 default   (1000) default   (1000)     7955 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/urlhandlers.ui
+-rw-r--r--   0 default   (1000) default   (1000)     4163 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/userinfo.ui
+-rw-r--r--   0 default   (1000) default   (1000)    91850 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/userinterface.ui
+-rw-r--r--   0 default   (1000) default   (1000)    10457 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/uploads.ui
+-rw-r--r--   0 default   (1000) default   (1000)    15231 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/userbrowse.ui
+-rw-r--r--   0 default   (1000) default   (1000)    40552 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/ui/userinfo.ui
+-rw-r--r--   0 default   (1000) default   (1000)     8099 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/uploads.py
+-rw-r--r--   0 default   (1000) default   (1000)    53390 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/userbrowse.py
+-rw-r--r--   0 default   (1000) default   (1000)    25533 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/userinfo.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.986782 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)     3756 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/accelerator.py
+-rw-r--r--   0 default   (1000) default   (1000)     1391 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/clipboard.py
+-rw-r--r--   0 default   (1000) default   (1000)    22947 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/dialogs.py
+-rw-r--r--   0 default   (1000) default   (1000)    13452 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/filechooser.py
+-rw-r--r--   0 default   (1000) default   (1000)    28505 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/iconnotebook.py
+-rw-r--r--   0 default   (1000) default   (1000)     3539 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/infobar.py
+-rw-r--r--   0 default   (1000) default   (1000)     2924 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/popover.py
+-rw-r--r--   0 default   (1000) default   (1000)    19042 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/popupmenu.py
+-rw-r--r--   0 default   (1000) default   (1000)    31842 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/textentry.py
+-rw-r--r--   0 default   (1000) default   (1000)    16824 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/textview.py
+-rw-r--r--   0 default   (1000) default   (1000)    19601 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/theme.py
+-rw-r--r--   0 default   (1000) default   (1000)    37425 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/trayicon.py
+-rw-r--r--   0 default   (1000) default   (1000)    33332 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/treeview.py
+-rw-r--r--   0 default   (1000) default   (1000)     3496 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/ui.py
+-rw-r--r--   0 default   (1000) default   (1000)     2431 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/window.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.986782 nicotine_plus-3.3.4/pynicotine/headless/
+-rw-r--r--   0 default   (1000) default   (1000)      903 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/headless/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)     4080 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/headless/application.py
+-rw-r--r--   0 default   (1000) default   (1000)     2713 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/i18n.py
+-rw-r--r--   0 default   (1000) default   (1000)     4258 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/interests.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.986782 nicotine_plus-3.3.4/pynicotine/locale/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.987782 nicotine_plus-3.3.4/pynicotine/locale/ca/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.987782 nicotine_plus-3.3.4/pynicotine/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/ca/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/ca/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.987782 nicotine_plus-3.3.4/pynicotine/locale/de/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.988782 nicotine_plus-3.3.4/pynicotine/locale/de/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/de/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/de/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.988782 nicotine_plus-3.3.4/pynicotine/locale/es_CL/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.988782 nicotine_plus-3.3.4/pynicotine/locale/es_CL/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/es_CL/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/es_CL/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.988782 nicotine_plus-3.3.4/pynicotine/locale/es_ES/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.989782 nicotine_plus-3.3.4/pynicotine/locale/es_ES/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/es_ES/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/es_ES/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.989782 nicotine_plus-3.3.4/pynicotine/locale/et/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.989782 nicotine_plus-3.3.4/pynicotine/locale/et/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/et/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/et/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.989782 nicotine_plus-3.3.4/pynicotine/locale/fr/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.990782 nicotine_plus-3.3.4/pynicotine/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/fr/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/fr/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.990782 nicotine_plus-3.3.4/pynicotine/locale/hu/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.990782 nicotine_plus-3.3.4/pynicotine/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/hu/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/hu/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.990782 nicotine_plus-3.3.4/pynicotine/locale/it/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.991782 nicotine_plus-3.3.4/pynicotine/locale/it/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/it/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/it/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.991782 nicotine_plus-3.3.4/pynicotine/locale/lv/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.991782 nicotine_plus-3.3.4/pynicotine/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/lv/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/lv/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.991782 nicotine_plus-3.3.4/pynicotine/locale/nl/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.992782 nicotine_plus-3.3.4/pynicotine/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/nl/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/nl/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.992782 nicotine_plus-3.3.4/pynicotine/locale/pl/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.992782 nicotine_plus-3.3.4/pynicotine/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/pl/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/pl/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.992782 nicotine_plus-3.3.4/pynicotine/locale/pt_BR/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.993782 nicotine_plus-3.3.4/pynicotine/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/pt_BR/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/pt_BR/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.993782 nicotine_plus-3.3.4/pynicotine/locale/pt_PT/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.993782 nicotine_plus-3.3.4/pynicotine/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/pt_PT/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/pt_PT/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.993782 nicotine_plus-3.3.4/pynicotine/locale/ru/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.994782 nicotine_plus-3.3.4/pynicotine/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/ru/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/ru/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.994782 nicotine_plus-3.3.4/pynicotine/locale/tr/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.994782 nicotine_plus-3.3.4/pynicotine/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/tr/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/tr/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.994782 nicotine_plus-3.3.4/pynicotine/locale/uk/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.995782 nicotine_plus-3.3.4/pynicotine/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/uk/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/uk/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.995782 nicotine_plus-3.3.4/pynicotine/locale/zh_CN/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.995782 nicotine_plus-3.3.4/pynicotine/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/zh_CN/LC_MESSAGES/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:22:08.000000 nicotine_plus-3.3.4/pynicotine/locale/zh_CN/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)    11904 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/logfacility.py
+-rw-r--r--   0 default   (1000) default   (1000)    20761 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/networkfilter.py
+-rw-r--r--   0 default   (1000) default   (1000)     3132 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/notifications.py
+-rw-r--r--   0 default   (1000) default   (1000)    10986 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/nowplaying.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.996782 nicotine_plus-3.3.4/pynicotine/plugins/
+-rw-r--r--   0 default   (1000) default   (1000)     1984 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/README.md
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.996782 nicotine_plus-3.3.4/pynicotine/plugins/anti_shout/
+-rw-r--r--   0 default   (1000) default   (1000)      167 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/anti_shout/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)     2539 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/anti_shout/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.997782 nicotine_plus-3.3.4/pynicotine/plugins/auto_user_browse/
+-rw-r--r--   0 default   (1000) default   (1000)      166 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/auto_user_browse/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)     2056 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/auto_user_browse/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.997782 nicotine_plus-3.3.4/pynicotine/plugins/core_commands/
+-rw-r--r--   0 default   (1000) default   (1000)       81 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/core_commands/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)    22036 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/core_commands/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.998782 nicotine_plus-3.3.4/pynicotine/plugins/examplars/
+-rw-r--r--   0 default   (1000) default   (1000)      156 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/examplars/README.md
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/examplars/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.999782 nicotine_plus-3.3.4/pynicotine/plugins/examplars/commands/
+-rw-r--r--   0 default   (1000) default   (1000)      173 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/examplars/commands/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)     1440 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/examplars/commands/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.000782 nicotine_plus-3.3.4/pynicotine/plugins/examplars/memory_debugger/
+-rw-r--r--   0 default   (1000) default   (1000)      218 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/examplars/memory_debugger/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)     2658 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/examplars/memory_debugger/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.000782 nicotine_plus-3.3.4/pynicotine/plugins/examplars/port_checker/
+-rw-r--r--   0 default   (1000) default   (1000)      297 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/examplars/port_checker/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)     3571 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/examplars/port_checker/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.001782 nicotine_plus-3.3.4/pynicotine/plugins/examplars/preferences/
+-rw-r--r--   0 default   (1000) default   (1000)     1742 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/examplars/preferences/choices.py
+-rw-r--r--   0 default   (1000) default   (1000)     1579 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/examplars/preferences/filechooser.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.002782 nicotine_plus-3.3.4/pynicotine/plugins/examplars/testreplier/
+-rw-r--r--   0 default   (1000) default   (1000)      199 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/examplars/testreplier/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)     1606 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/examplars/testreplier/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.002782 nicotine_plus-3.3.4/pynicotine/plugins/leech_detector/
+-rw-r--r--   0 default   (1000) default   (1000)      284 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/leech_detector/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)     7186 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/leech_detector/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.003782 nicotine_plus-3.3.4/pynicotine/plugins/multipaste/
+-rw-r--r--   0 default   (1000) default   (1000)      281 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/multipaste/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)     2623 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/multipaste/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.004782 nicotine_plus-3.3.4/pynicotine/plugins/now_playing_search/
+-rw-r--r--   0 default   (1000) default   (1000)      514 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/now_playing_search/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)     1574 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/now_playing_search/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.004782 nicotine_plus-3.3.4/pynicotine/plugins/now_playing_sender/
+-rw-r--r--   0 default   (1000) default   (1000)      390 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/now_playing_sender/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)     5072 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/now_playing_sender/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.005782 nicotine_plus-3.3.4/pynicotine/plugins/plugin_debugger/
+-rw-r--r--   0 default   (1000) default   (1000)      181 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/plugin_debugger/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)     5930 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/plugin_debugger/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.006782 nicotine_plus-3.3.4/pynicotine/plugins/spamfilter/
+-rw-r--r--   0 default   (1000) default   (1000)      559 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/spamfilter/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)     3159 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/spamfilter/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.006782 nicotine_plus-3.3.4/pynicotine/plugins/youtube_info/
+-rw-r--r--   0 default   (1000) default   (1000)      376 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/youtube_info/PLUGININFO
+-rw-r--r--   0 default   (1000) default   (1000)     6728 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/plugins/youtube_info/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)    37898 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/pluginsystem.py
+-rw-r--r--   0 default   (1000) default   (1000)    24109 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/portmapper.py
+-rw-r--r--   0 default   (1000) default   (1000)    11586 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/privatechat.py
+-rw-r--r--   0 default   (1000) default   (1000)    26152 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/search.py
+-rw-r--r--   0 default   (1000) default   (1000)    42929 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/shares.py
+-rw-r--r--   0 default   (1000) default   (1000)   114474 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/slskmessages.py
+-rw-r--r--   0 default   (1000) default   (1000)   103679 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/slskproto.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.007782 nicotine_plus-3.3.4/pynicotine/tests/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.007782 nicotine_plus-3.3.4/pynicotine/tests/integration/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/integration/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)     3857 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/integration/test_startup.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.008782 nicotine_plus-3.3.4/pynicotine/tests/unit/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/__init__.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.009782 nicotine_plus-3.3.4/pynicotine/tests/unit/config/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/config/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)       70 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/config/config
+-rw-r--r--   0 default   (1000) default   (1000)     2878 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/config/test_config.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.010782 nicotine_plus-3.3.4/pynicotine/tests/unit/networkfilter/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/networkfilter/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)     2785 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/networkfilter/test_country.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.011782 nicotine_plus-3.3.4/pynicotine/tests/unit/protocol/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/protocol/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)    10065 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/protocol/test_slskmessages.py
+-rw-r--r--   0 default   (1000) default   (1000)     4789 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/protocol/test_slskproto.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.011782 nicotine_plus-3.3.4/pynicotine/tests/unit/search/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/search/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)     6661 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/search/test_search.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.012782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.013782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.013782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/.def/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/.def/nothing2
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/.def_file
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/.hidden_file2
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.014782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/.uvw/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/.uvw/nothing2
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/.uvw_file
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.838783 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/buddies/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.014782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/buddies/folder/
+-rw-r--r--   0 default   (1000) default   (1000)       10 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/buddies/folder/somefile.txt
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/dummy_file2
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.839783 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder3/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.014782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder3/.poof2/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder3/.poof2/nothing2
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.015782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder3/test2/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder3/test2/nothing2
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.015782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder4/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/folder4/nothing2
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.015782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/something2/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedbuddyfiles/something2/nothing2
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.016782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.017782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/.abc/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/.abc/nothing
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/.abc_file
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/.hidden_file
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.017782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/.xyz/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/.xyz/nothing
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/.xyz_file
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/dummy_file
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.017782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/folder1/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/folder1/nothing
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.840783 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/folder2/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.018782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/folder2/.poof/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/folder2/.poof/nothing
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.018782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/folder2/test/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/folder2/test/nothing
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.018782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/something/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedfiles/something/nothing
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.019782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedinvalidfiles/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedinvalidfiles/file.txt
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.019782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedtrustedfiles/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedtrustedfiles/.hidden_file3
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.020782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedtrustedfiles/.hidden_folder/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedtrustedfiles/.hidden_folder/nothing
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedtrustedfiles/dummy_file3
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.842783 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.020782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/.hidden/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/.hidden/nothing
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.842783 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/folder2/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:09.842783 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/folder2/folder3/
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.020782 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/folder2/folder3/folder4/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/.sharedtrustedfiles/folder/folder2/folder3/folder4/nothing
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)    10457 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/shares/test_shares.py
+-rw-r--r--   0 default   (1000) default   (1000)     1486 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/test_i18n.py
+-rw-r--r--   0 default   (1000) default   (1000)     1599 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/test_version.py
+drwxr-xr-x   0 default   (1000) default   (1000)        0 2024-05-06 22:22:10.022782 nicotine_plus-3.3.4/pynicotine/tests/unit/transfers/
+-rw-r--r--   0 default   (1000) default   (1000)        0 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/transfers/__init__.py
+-rw-r--r--   0 default   (1000) default   (1000)     1621 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/transfers/downloads.json
+-rw-r--r--   0 default   (1000) default   (1000)    15004 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/transfers/test_downloads.py
+-rw-r--r--   0 default   (1000) default   (1000)    11059 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/transfers/test_get_upload_candidate.py
+-rw-r--r--   0 default   (1000) default   (1000)     4151 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/transfers/test_uploads.py
+-rw-r--r--   0 default   (1000) default   (1000)      426 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/tests/unit/transfers/uploads.json
+-rw-r--r--   0 default   (1000) default   (1000)    17935 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/transfers.py
+-rw-r--r--   0 default   (1000) default   (1000)    43643 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/uploads.py
+-rw-r--r--   0 default   (1000) default   (1000)    13546 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/userbrowse.py
+-rw-r--r--   0 default   (1000) default   (1000)     6671 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/userinfo.py
+-rw-r--r--   0 default   (1000) default   (1000)    13673 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/users.py
+-rw-r--r--   0 default   (1000) default   (1000)    28654 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pynicotine/utils.py
+-rw-r--r--   0 default   (1000) default   (1000)       81 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/pyproject.toml
+-rw-r--r--   0 default   (1000) default   (1000)     2919 2024-05-06 22:22:10.025782 nicotine_plus-3.3.4/setup.cfg
+-rw-r--r--   0 default   (1000) default   (1000)     4825 2024-05-06 22:21:28.000000 nicotine_plus-3.3.4/setup.py
```

### Comparing `nicotine_plus-3.3.3/AUTHORS.md` & `nicotine_plus-3.3.4/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/COPYING` & `nicotine_plus-3.3.4/COPYING`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/MANIFEST.in` & `nicotine_plus-3.3.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/NEWS.md` & `nicotine_plus-3.3.4/NEWS.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 # Release Notes
 
 The current stable version of Nicotine+ is available at [DOWNLOADS.md](doc/DOWNLOADS.md).
 
 You can run the latest unstable build of Nicotine+ to test recent changes and bug fixes, see [TESTING.md](doc/TESTING.md).
 
 
+## Version 3.3.4 (May 6, 2024)
+
+### Corrections
+
+ * Fixed "Format codes" link not opening in the preferred browser
+ * Windows: Fixed regression in scrolling performance
+
+### Issues closed on GitHub
+
+ * Scrolling performance suddenly abysmal (again) ([#3000](https://github.com/nicotine-plus/nicotine-plus/issues/3000))
+ * Can't access "Format Codes" link in settings through left mouse click on 3.3.3 ([#3001](https://github.com/nicotine-plus/nicotine-plus/issues/3001))
+ * Sometimes, Nicotine+ (3.3.3) window doesn't open on top when other windows already opened full screen on the desktop. ([#3002](https://github.com/nicotine-plus/nicotine-plus/issues/3002))
+
+
 ## Version 3.3.3 (May 5, 2024)
 
 ### Changes
 
  * Performance improvements when searching for common files
  * Improved search result matching for non-Latin languages
  * Minor accessibility improvements
```

### Comparing `nicotine_plus-3.3.3/PKG-INFO` & `nicotine_plus-3.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicotine-plus
-Version: 3.3.3
+Version: 3.3.4
 Summary: Graphical client for the Soulseek peer-to-peer network
 Home-page: https://nicotine-plus.org
 Author: Nicotine+ Team
 Author-email: nicotine-team@lists.launchpad.net
 License: GPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
```

### Comparing `nicotine_plus-3.3.3/README.md` & `nicotine_plus-3.3.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Check out the [screenshots](data/screenshots/SCREENSHOTS.md) and [source code](https://github.com/nicotine-plus/nicotine-plus).
 <br clear="right">
 
 
 ## Download
 
-The current stable version of Nicotine+ is 3.3.3, released on May 5, 2024. See the [release notes](NEWS.md).
+The current stable version of Nicotine+ is 3.3.4, released on May 6, 2024. See the [release notes](NEWS.md).
 
 Downloads are available for:
 
  * [GNU/Linux, *BSD and Solaris](doc/DOWNLOADS.md#gnulinux-bsd-solaris)
  * [Windows](doc/DOWNLOADS.md#windows)
  * [macOS](doc/DOWNLOADS.md#macos)
```

### Comparing `nicotine_plus-3.3.3/TRANSLATORS.md` & `nicotine_plus-3.3.4/TRANSLATORS.md`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/data/nicotine.1` & `nicotine_plus-3.3.4/data/nicotine.1`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/data/org.nicotine_plus.Nicotine.appdata.xml.in` & `nicotine_plus-3.3.4/data/org.nicotine_plus.Nicotine.appdata.xml.in`

 * *Files 2% similar despite different names*

#### Comparing `nicotine_plus-3.3.3/data/org.nicotine_plus.Nicotine.appdata.xml.in` & `nicotine_plus-3.3.4/data/org.nicotine_plus.Nicotine.appdata.xml.in`

```diff
@@ -75,17 +75,18 @@
     <name>Nicotine+ Team</name>
   </developer>
   <content_rating type="oars-1.1">
     <content_attribute id="social-chat">intense</content_attribute>
     <content_attribute id="social-info">mild</content_attribute>
   </content_rating>
   <releases>
-    <release version="3.3.3" date="2024-05-05">
+    <release version="3.3.4" date="2024-05-06">
       <url>https://nicotine-plus.org/NEWS</url>
     </release>
+    <release version="3.3.3" date="2024-05-05"/>
     <release version="3.3.2" date="2024-02-25"/>
     <release version="3.3.1" date="2024-02-24"/>
     <release version="3.3.0" date="2024-02-01"/>
     <release version="3.2.9" date="2023-03-05"/>
     <release version="3.2.8" date="2023-01-06"/>
     <release version="3.2.7" date="2022-12-01"/>
     <release version="3.2.6" date="2022-10-21"/>
```

### Comparing `nicotine_plus-3.3.3/data/scripts/update_ip_country_data.py` & `nicotine_plus-3.3.4/data/scripts/update_ip_country_data.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/data/scripts/update_translation_template.py` & `nicotine_plus-3.3.4/data/scripts/update_translation_template.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/doc/DEPENDENCIES.md` & `nicotine_plus-3.3.4/doc/DEPENDENCIES.md`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/doc/DEVELOPING.md` & `nicotine_plus-3.3.4/doc/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/doc/DOWNLOADS.md` & `nicotine_plus-3.3.4/doc/DOWNLOADS.md`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/doc/PACKAGING.md` & `nicotine_plus-3.3.4/doc/PACKAGING.md`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/doc/SLSKPROTOCOL.md` & `nicotine_plus-3.3.4/doc/SLSKPROTOCOL.md`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/doc/TESTING.md` & `nicotine_plus-3.3.4/doc/TESTING.md`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/doc/TRANSLATIONS.md` & `nicotine_plus-3.3.4/doc/TRANSLATIONS.md`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/nicotine` & `nicotine_plus-3.3.4/nicotine`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/nicotine_plus.egg-info/PKG-INFO` & `nicotine_plus-3.3.4/nicotine_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicotine-plus
-Version: 3.3.3
+Version: 3.3.4
 Summary: Graphical client for the Soulseek peer-to-peer network
 Home-page: https://nicotine-plus.org
 Author: Nicotine+ Team
 Author-email: nicotine-team@lists.launchpad.net
 License: GPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
```

### Comparing `nicotine_plus-3.3.3/nicotine_plus.egg-info/SOURCES.txt` & `nicotine_plus-3.3.4/nicotine_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/ar.po` & `nicotine_plus-3.3.4/po/ar.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/ca.po` & `nicotine_plus-3.3.4/po/ca.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/cs.po` & `nicotine_plus-3.3.4/po/cs.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/da.po` & `nicotine_plus-3.3.4/po/da.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/de.po` & `nicotine_plus-3.3.4/po/de.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/eo.po` & `nicotine_plus-3.3.4/po/eo.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/es_CL.po` & `nicotine_plus-3.3.4/po/es_CL.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/es_ES.po` & `nicotine_plus-3.3.4/po/es_ES.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/et.po` & `nicotine_plus-3.3.4/po/et.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/eu.po` & `nicotine_plus-3.3.4/po/eu.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/fi.po` & `nicotine_plus-3.3.4/po/fi.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/fr.po` & `nicotine_plus-3.3.4/po/fr.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/hu.po` & `nicotine_plus-3.3.4/po/hu.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/it.po` & `nicotine_plus-3.3.4/po/it.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/lt.po` & `nicotine_plus-3.3.4/po/lt.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/lv.po` & `nicotine_plus-3.3.4/po/lv.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/nb_NO.po` & `nicotine_plus-3.3.4/po/nb_NO.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/nicotine.pot` & `nicotine_plus-3.3.4/po/nicotine.pot`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/nl.po` & `nicotine_plus-3.3.4/po/nl.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/pl.po` & `nicotine_plus-3.3.4/po/pl.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/pt_BR.po` & `nicotine_plus-3.3.4/po/pt_BR.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/pt_PT.po` & `nicotine_plus-3.3.4/po/pt_PT.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/ro.po` & `nicotine_plus-3.3.4/po/ro.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/ru.po` & `nicotine_plus-3.3.4/po/ru.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/sk.po` & `nicotine_plus-3.3.4/po/sk.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/sq.po` & `nicotine_plus-3.3.4/po/sq.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/sv.po` & `nicotine_plus-3.3.4/po/sv.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/tr.po` & `nicotine_plus-3.3.4/po/tr.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/uk.po` & `nicotine_plus-3.3.4/po/uk.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/po/zh_CN.po` & `nicotine_plus-3.3.4/po/zh_CN.po`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/__init__.py` & `nicotine_plus-3.3.4/pynicotine/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __application_name__ = "Nicotine+"
 __application_id__ = "org.nicotine_plus.Nicotine"
-__version__ = "3.3.3"
+__version__ = "3.3.4"
 __author__ = "Nicotine+ Team"
 __copyright__ = """© 2004–2024 Nicotine+ Contributors
 © 2003–2004 Nicotine Contributors
 © 2001–2003 PySoulSeek Contributors"""
 __website_url__ = "https://nicotine-plus.org"
 __privileges_url__ = "https://www.slsknet.org/qtlogin.php?username=%s"
 __port_checker_url__ = "https://www.slsknet.org/porttest.php?port=%s"
```

### Comparing `nicotine_plus-3.3.3/pynicotine/__main__.py` & `nicotine_plus-3.3.4/pynicotine/__main__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/buddies.py` & `nicotine_plus-3.3.4/pynicotine/buddies.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/chatrooms.py` & `nicotine_plus-3.3.4/pynicotine/chatrooms.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/cli.py` & `nicotine_plus-3.3.4/pynicotine/cli.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/config.py` & `nicotine_plus-3.3.4/pynicotine/config.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/core.py` & `nicotine_plus-3.3.4/pynicotine/core.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/downloads.py` & `nicotine_plus-3.3.4/pynicotine/downloads.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/events.py` & `nicotine_plus-3.3.4/pynicotine/events.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/external/README.md` & `nicotine_plus-3.3.4/pynicotine/external/README.md`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/external/data/country_codes.py` & `nicotine_plus-3.3.4/pynicotine/external/data/country_codes.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/external/data/ip_ranges.py` & `nicotine_plus-3.3.4/pynicotine/external/data/ip_ranges.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/external/tinytag.py` & `nicotine_plus-3.3.4/pynicotine/external/tinytag.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/__init__.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/application.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/application.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/buddies.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/buddies.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/chatrooms.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/chatrooms.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/css/style.css` & `nicotine_plus-3.3.4/pynicotine/gtkgui/css/style.css`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/css/style_gtk3.css` & `nicotine_plus-3.3.4/pynicotine/gtkgui/css/style_gtk3.css`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/css/style_gtk4.css` & `nicotine_plus-3.3.4/pynicotine/gtkgui/css/style_gtk4.css`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/css/style_gtk4_darwin.css` & `nicotine_plus-3.3.4/pynicotine/gtkgui/css/style_gtk4_darwin.css`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/css/style_libadwaita_csd.css` & `nicotine_plus-3.3.4/pynicotine/gtkgui/css/style_libadwaita_csd.css`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/about.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/about.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/fastconfigure.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/fastconfigure.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/fileproperties.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/fileproperties.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/pluginsettings.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/pluginsettings.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/preferences.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1272,14 +1272,15 @@
         self.completion_required = False
 
         format_codes_url = "https://docs.python.org/3/library/datetime.html#format-codes"
         format_codes_label = _("Format codes")
 
         self.format_codes_label.set_markup(
             f"<a href='{format_codes_url}' title='{format_codes_url}'>{format_codes_label}</a>")
+        self.format_codes_label.connect("activate-link", lambda x, url: open_uri(url))
 
         self.tts_command_combobox = ComboBox(
             container=self.tts_command_label.get_parent(), label=self.tts_command_label, has_entry=True,
             items=(
                 ("flite -t $", None),
                 ("echo $ | festival --tts", None)
             )
@@ -2121,14 +2122,15 @@
         self.application = application
 
         format_codes_url = "https://docs.python.org/3/library/datetime.html#format-codes"
         format_codes_label = _("Format codes")
 
         self.format_codes_label.set_markup(
             f"<a href='{format_codes_url}' title='{format_codes_url}'>{format_codes_label}</a>")
+        self.format_codes_label.connect("activate-link", lambda x, url: open_uri(url))
 
         self.private_chat_log_folder_button = FileChooserButton(
             self.private_chat_log_folder_label.get_parent(), window=application.preferences,
             label=self.private_chat_log_folder_label, end_button=self.private_chat_log_folder_default_button,
             chooser_type="folder"
         )
         self.chatroom_log_folder_button = FileChooserButton(
```

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/shortcuts.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/shortcuts.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/statistics.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/statistics.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/dialogs/wishlist.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/dialogs/wishlist.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/downloads.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/downloads.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/128x128/apps/org.nicotine_plus.Nicotine.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/128x128/apps/org.nicotine_plus.Nicotine.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/16x16/apps/org.nicotine_plus.Nicotine.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/16x16/apps/org.nicotine_plus.Nicotine.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/24x24/apps/org.nicotine_plus.Nicotine.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/24x24/apps/org.nicotine_plus.Nicotine.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/256x256/apps/org.nicotine_plus.Nicotine.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/256x256/apps/org.nicotine_plus.Nicotine.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/32x32/apps/org.nicotine_plus.Nicotine.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/32x32/apps/org.nicotine_plus.Nicotine.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/48x48/apps/org.nicotine_plus.Nicotine.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/48x48/apps/org.nicotine_plus.Nicotine.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/64x64/apps/org.nicotine_plus.Nicotine.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/64x64/apps/org.nicotine_plus.Nicotine.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-away.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-away.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-connect.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-connect.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-disconnect.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-disconnect.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-msg.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine-msg.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/apps/org.nicotine_plus.Nicotine.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ad.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ad.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ae.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ae.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-af.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-af.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ag.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ag.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ai.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ai.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-al.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-al.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-am.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-am.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ao.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ao.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ar.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ar.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-as.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-as.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-at.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-at.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-au.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-au.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-aw.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-aw.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ax.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ax.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-az.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-az.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ba.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ba.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bb.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bb.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bd.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bd.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-be.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-be.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bf.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bf.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bg.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bg.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bh.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bh.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bi.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bi.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bj.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bj.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bl.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bl.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bm.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bm.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bn.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bn.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bo.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bo.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-br.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-br.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bs.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bs.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bt.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bt.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bv.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bv.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bw.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bw.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-by.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-by.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bz.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-bz.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ca.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ca.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cc.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cc.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cd.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cd.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cf.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cf.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cg.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cg.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ch.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ch.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ci.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ci.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ck.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ck.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cl.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cl.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cm.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cm.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cn.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cn.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-co.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-co.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cr.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cr.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cu.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cu.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cv.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cv.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cw.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cw.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cx.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cx.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cy.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cy.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cz.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-cz.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-de.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-de.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dj.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dj.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dk.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dk.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dm.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dm.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-do.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-do.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dz.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-dz.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ec.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ec.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ee.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ee.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-eg.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-eg.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-er.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-er.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-es.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-es.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-et.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-et.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-eu.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-eu.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fi.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fi.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fj.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fj.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fk.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fk.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fm.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fm.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fo.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fo.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fr.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-fr.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ga.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ga.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gb.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gb.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gd.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gd.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ge.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ge.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gf.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gf.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gg.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gg.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gh.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gh.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gi.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gi.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gl.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gl.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gm.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gm.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gn.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gn.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gp.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gp.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gq.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gq.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gr.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gr.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gs.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gs.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gt.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gt.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gu.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gu.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gw.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gw.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gy.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-gy.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hk.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hk.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hm.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hm.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hn.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hn.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hr.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hr.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ht.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ht.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hu.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-hu.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-id.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-id.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ie.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ie.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-il.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-il.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-im.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-im.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-in.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-in.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-io.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-io.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-iq.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-iq.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ir.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ir.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-is.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-is.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-it.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-it.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-je.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-je.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-jm.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-jm.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-jo.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-jo.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-jp.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-jp.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ke.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ke.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kg.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kg.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kh.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kh.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ki.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ki.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-km.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-km.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kn.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kn.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kp.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kp.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kr.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kr.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kw.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kw.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ky.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ky.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kz.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-kz.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-la.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-la.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lb.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lb.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lc.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lc.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-li.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-li.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lk.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lk.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lr.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lr.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ls.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ls.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lt.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lt.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lu.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lu.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lv.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-lv.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ly.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ly.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ma.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ma.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mc.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mc.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-md.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-md.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-me.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-me.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mf.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mf.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mg.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mg.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mh.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mh.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mk.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mk.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ml.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ml.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mm.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mm.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mn.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mn.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mo.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mo.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mp.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mp.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mq.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mq.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mr.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mr.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ms.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ms.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mt.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mt.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mu.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mu.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mv.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mv.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mw.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mw.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mx.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mx.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-my.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-my.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mz.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-mz.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-na.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-na.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nc.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nc.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ne.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ne.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nf.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nf.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ng.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ng.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ni.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ni.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nl.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nl.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-no.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-no.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-np.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-np.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nr.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nr.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nu.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nu.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nz.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-nz.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-om.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-om.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pa.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pa.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pe.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pe.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pf.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pf.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pg.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pg.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ph.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ph.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pk.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pk.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pl.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pl.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pm.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pm.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pn.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pn.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pr.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pr.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ps.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ps.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pt.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pt.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pw.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-pw.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-py.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-py.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-qa.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-qa.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-re.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-re.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ro.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ro.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-rs.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-rs.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ru.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ru.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-rw.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-rw.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sa.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sa.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sb.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sb.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sc.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sc.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sd.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sd.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-se.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-se.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sg.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sg.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sh.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sh.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-si.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-si.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sj.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sj.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sk.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sk.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sl.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sl.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sm.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sm.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sn.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sn.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-so.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-so.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sr.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sr.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ss.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ss.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-st.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-st.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sv.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sv.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sx.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sx.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sy.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sy.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sz.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-sz.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tc.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tc.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-td.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-td.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tf.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tf.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tg.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tg.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-th.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-th.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tj.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tj.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tk.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tk.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tl.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tl.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tm.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tm.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tn.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tn.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-to.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-to.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tr.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tr.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tt.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tt.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tv.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tv.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tw.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tw.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tz.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-tz.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ua.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ua.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ug.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ug.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-um.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-um.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-us.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-us.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-uy.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-uy.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-uz.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-uz.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-va.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-va.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vc.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vc.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ve.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ve.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vg.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vg.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vi.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vi.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vn.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vn.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vu.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-vu.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-wf.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-wf.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ws.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ws.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ye.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-ye.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-yt.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-yt.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-za.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-za.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-zm.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-zm.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-zw.svg` & `nicotine_plus-3.3.4/pynicotine/gtkgui/icons/hicolor/scalable/intl/nplus-flag-zw.svg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/interests.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/interests.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/mainwindow.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/chatcommandhelp.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/chatcommandhelp.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/chathistory.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/chathistory.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/downloadspeeds.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/downloadspeeds.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/roomlist.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/roomlist.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/roomwall.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/roomwall.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/searchfilterhelp.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/searchfilterhelp.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/transferspeeds.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/transferspeeds.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/popovers/uploadspeeds.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/popovers/uploadspeeds.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/privatechat.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/privatechat.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/search.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/search.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/transfers.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/transfers.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/buddies.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/buddies.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/chatrooms.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/chatrooms.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/about.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/about.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/fastconfigure.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/fastconfigure.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/fileproperties.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/fileproperties.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/preferences.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/preferences.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/shortcuts.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/shortcuts.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/statistics.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/statistics.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/dialogs/wishlist.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/dialogs/wishlist.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/downloads.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/downloads.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/interests.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/interests.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/mainwindow.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/chathistory.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/chathistory.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/downloadspeeds.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/downloadspeeds.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/roomlist.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/roomlist.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/roomwall.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/roomwall.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/searchfilterhelp.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/searchfilterhelp.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/popovers/uploadspeeds.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/popovers/uploadspeeds.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/privatechat.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/privatechat.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/search.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/search.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/ban.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/ban.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/chats.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/chats.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/downloads.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/downloads.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/ignore.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/ignore.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/log.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/log.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/network.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/network.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/nowplaying.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/nowplaying.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/plugin.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/plugin.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/search.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/search.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/shares.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/shares.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/uploads.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/uploads.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/urlhandlers.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/urlhandlers.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/userinfo.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/userinfo.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/settings/userinterface.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/settings/userinterface.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/uploads.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/uploads.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/userbrowse.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/userbrowse.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/ui/userinfo.ui` & `nicotine_plus-3.3.4/pynicotine/gtkgui/ui/userinfo.ui`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/uploads.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/uploads.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/userbrowse.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/userbrowse.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/userinfo.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/userinfo.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/accelerator.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/accelerator.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/clipboard.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/clipboard.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/dialogs.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/dialogs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# COPYRIGHT (C) 2020-2023 Nicotine+ Contributors
+# COPYRIGHT (C) 2020-2024 Nicotine+ Contributors
 #
 # GNU GENERAL PUBLIC LICENSE
 #    Version 3, 29 June 2007
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -13,14 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
+import sys
 
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import Gtk
 
 from pynicotine.config import config
 from pynicotine.gtkgui.application import GTK_API_VERSION
@@ -169,14 +170,20 @@
         Window.active_dialogs.remove(self)
 
         if self.close_callback is not None:
             self.close_callback(self)
 
         # Hide the dialog
         self.widget.set_visible(False)
+
+        # "Soft-delete" the dialog. This is necessary to prevent the dialog from
+        # appearing in window peek on Windows
+        if sys.platform == "win32":
+            self.widget.unrealize()
+
         return True
 
     def _set_dialog_properties(self):
 
         if GTK_API_VERSION >= 4:
             self.widget.connect("close-request", self._on_close_request)
         else:
```

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/filechooser.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/filechooser.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/iconnotebook.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/iconnotebook.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/infobar.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/infobar.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/popover.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/popover.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/popupmenu.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/popupmenu.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/textentry.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/textentry.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/textview.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/textview.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/theme.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/theme.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/trayicon.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/trayicon.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/treeview.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/treeview.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/ui.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/ui.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/gtkgui/widgets/window.py` & `nicotine_plus-3.3.4/pynicotine/gtkgui/widgets/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# COPYRIGHT (C) 2022-2023 Nicotine+ Contributors
+# COPYRIGHT (C) 2022-2024 Nicotine+ Contributors
 #
 # GNU GENERAL PUBLIC LICENSE
 #    Version 3, 29 June 2007
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -74,14 +74,20 @@
         if self.activation_token is not None:
             # Set XDG activation token if provided by tray icon
             self.widget.set_startup_id(self.activation_token)
 
         self.widget.present()
 
     def hide(self):
+
+        if GTK_API_VERSION >= 4:
+            self.widget.minimize()
+        else:
+            self.widget.iconify()
+
         self.widget.set_visible(False)
 
     def close(self, *_args):
         self.widget.close()
 
     def destroy(self):
         self.widget.destroy()
```

### Comparing `nicotine_plus-3.3.3/pynicotine/headless/__init__.py` & `nicotine_plus-3.3.4/pynicotine/headless/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/headless/application.py` & `nicotine_plus-3.3.4/pynicotine/headless/application.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/i18n.py` & `nicotine_plus-3.3.4/pynicotine/i18n.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/interests.py` & `nicotine_plus-3.3.4/pynicotine/interests.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/logfacility.py` & `nicotine_plus-3.3.4/pynicotine/logfacility.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/networkfilter.py` & `nicotine_plus-3.3.4/pynicotine/networkfilter.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/notifications.py` & `nicotine_plus-3.3.4/pynicotine/notifications.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/nowplaying.py` & `nicotine_plus-3.3.4/pynicotine/nowplaying.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/README.md` & `nicotine_plus-3.3.4/pynicotine/plugins/README.md`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/anti_shout/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/anti_shout/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/auto_user_browse/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/auto_user_browse/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/core_commands/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/core_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/examplars/commands/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/examplars/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/examplars/memory_debugger/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/examplars/memory_debugger/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/examplars/port_checker/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/examplars/port_checker/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/examplars/preferences/choices.py` & `nicotine_plus-3.3.4/pynicotine/plugins/examplars/preferences/choices.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/examplars/preferences/filechooser.py` & `nicotine_plus-3.3.4/pynicotine/plugins/examplars/preferences/filechooser.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/examplars/testreplier/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/examplars/testreplier/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/leech_detector/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/leech_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/multipaste/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/multipaste/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/now_playing_search/PLUGININFO` & `nicotine_plus-3.3.4/pynicotine/plugins/now_playing_search/PLUGININFO`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/now_playing_search/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/now_playing_search/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/now_playing_sender/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/now_playing_sender/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/plugin_debugger/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/plugin_debugger/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/spamfilter/PLUGININFO` & `nicotine_plus-3.3.4/pynicotine/plugins/spamfilter/PLUGININFO`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/spamfilter/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/spamfilter/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/plugins/youtube_info/__init__.py` & `nicotine_plus-3.3.4/pynicotine/plugins/youtube_info/__init__.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/pluginsystem.py` & `nicotine_plus-3.3.4/pynicotine/pluginsystem.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/portmapper.py` & `nicotine_plus-3.3.4/pynicotine/portmapper.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/privatechat.py` & `nicotine_plus-3.3.4/pynicotine/privatechat.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/search.py` & `nicotine_plus-3.3.4/pynicotine/search.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/shares.py` & `nicotine_plus-3.3.4/pynicotine/shares.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/slskmessages.py` & `nicotine_plus-3.3.4/pynicotine/slskmessages.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/slskproto.py` & `nicotine_plus-3.3.4/pynicotine/slskproto.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/tests/integration/test_startup.py` & `nicotine_plus-3.3.4/pynicotine/tests/integration/test_startup.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/tests/unit/config/test_config.py` & `nicotine_plus-3.3.4/pynicotine/tests/unit/config/test_config.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/tests/unit/networkfilter/test_country.py` & `nicotine_plus-3.3.4/pynicotine/tests/unit/networkfilter/test_country.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/tests/unit/protocol/test_slskmessages.py` & `nicotine_plus-3.3.4/pynicotine/tests/unit/protocol/test_slskmessages.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/tests/unit/protocol/test_slskproto.py` & `nicotine_plus-3.3.4/pynicotine/tests/unit/protocol/test_slskproto.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/tests/unit/search/test_search.py` & `nicotine_plus-3.3.4/pynicotine/tests/unit/search/test_search.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/tests/unit/shares/test_shares.py` & `nicotine_plus-3.3.4/pynicotine/tests/unit/shares/test_shares.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/tests/unit/test_i18n.py` & `nicotine_plus-3.3.4/pynicotine/tests/unit/test_i18n.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/tests/unit/test_version.py` & `nicotine_plus-3.3.4/pynicotine/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/tests/unit/transfers/downloads.json` & `nicotine_plus-3.3.4/pynicotine/tests/unit/transfers/downloads.json`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/tests/unit/transfers/test_downloads.py` & `nicotine_plus-3.3.4/pynicotine/tests/unit/transfers/test_downloads.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/tests/unit/transfers/test_get_upload_candidate.py` & `nicotine_plus-3.3.4/pynicotine/tests/unit/transfers/test_get_upload_candidate.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/tests/unit/transfers/test_uploads.py` & `nicotine_plus-3.3.4/pynicotine/tests/unit/transfers/test_uploads.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/transfers.py` & `nicotine_plus-3.3.4/pynicotine/transfers.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/uploads.py` & `nicotine_plus-3.3.4/pynicotine/uploads.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/userbrowse.py` & `nicotine_plus-3.3.4/pynicotine/userbrowse.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/userinfo.py` & `nicotine_plus-3.3.4/pynicotine/userinfo.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/users.py` & `nicotine_plus-3.3.4/pynicotine/users.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/pynicotine/utils.py` & `nicotine_plus-3.3.4/pynicotine/utils.py`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/setup.cfg` & `nicotine_plus-3.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `nicotine_plus-3.3.3/setup.py` & `nicotine_plus-3.3.4/setup.py`

 * *Files identical despite different names*

