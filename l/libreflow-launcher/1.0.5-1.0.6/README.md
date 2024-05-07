# Comparing `tmp/libreflow_launcher-1.0.5.tar.gz` & `tmp/libreflow_launcher-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_launcher-1.0.5.tar", last modified: Mon Apr 29 17:21:13 2024, max compression
+gzip compressed data, was "libreflow_launcher-1.0.6.tar", last modified: Tue May  7 05:52:33 2024, max compression
```

## Comparing `libreflow_launcher-1.0.5.tar` & `libreflow_launcher-1.0.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 17:21:13.724658 libreflow_launcher-1.0.5/
--rw-rw-rw-   0 root         (0) root         (0)     1403 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2192 2024-04-29 17:21:13.724658 libreflow_launcher-1.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      839 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-04-29 17:21:13.725658 libreflow_launcher-1.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1691 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 17:21:13.708658 libreflow_launcher-1.0.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 17:21:13.713658 libreflow_launcher-1.0.5/src/libreflow_launcher/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-29 17:21:13.725658 libreflow_launcher-1.0.5/src/libreflow_launcher/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    18628 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 17:21:13.714658 libreflow_launcher-1.0.5/src/libreflow_launcher/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 17:21:13.715658 libreflow_launcher-1.0.5/src/libreflow_launcher/data/servers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/data/servers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/gui.py
--rw-rw-rw-   0 root         (0) root         (0)     6139 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/model.py
--rw-rw-rw-   0 root         (0) root         (0)     7983 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 17:21:13.715658 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 17:21:13.718658 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   503824 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf
--rw-rw-rw-   0 root         (0) root         (0)   445528 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf
--rw-rw-rw-   0 root         (0) root         (0)   579296 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf
--rw-rw-rw-   0 root         (0) root         (0)   528976 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/fonts/OpenSans.ttf
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/fonts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 17:21:13.718658 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 17:21:13.723658 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5628 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/arrow-down.png
--rw-rw-rw-   0 root         (0) root         (0)     5667 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/arrow-right.png
--rw-rw-rw-   0 root         (0) root         (0)     1177 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png
--rw-rw-rw-   0 root         (0) root         (0)     9732 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/close.png
--rw-rw-rw-   0 root         (0) root         (0)     9850 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/gitlab.svg
--rw-rw-rw-   0 root         (0) root         (0)     1719 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/kitsu.svg
--rw-rw-rw-   0 root         (0) root         (0)     8760 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/log-out.png
--rw-rw-rw-   0 root         (0) root         (0)     6277 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/log-out_hover.png
--rw-rw-rw-   0 root         (0) root         (0)     6277 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/log-out_normal.png
--rw-rw-rw-   0 root         (0) root         (0)     7267 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/open.png
--rw-rw-rw-   0 root         (0) root         (0)    10491 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/pypi.svg
--rw-rw-rw-   0 root         (0) root         (0)    17905 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/server.png
--rw-rw-rw-   0 root         (0) root         (0)    13119 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/settings.png
--rw-rw-rw-   0 root         (0) root         (0)    19182 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/settings_outline.png
--rw-rw-rw-   0 root         (0) root         (0)     5851 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/start.png
--rw-rw-rw-   0 root         (0) root         (0)     7946 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/trash.png
--rw-rw-rw-   0 root         (0) root         (0)     8358 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/trash_hover.png
--rw-rw-rw-   0 root         (0) root         (0)     7996 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/trash_normal.png
--rw-rw-rw-   0 root         (0) root         (0)    11968 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/user.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 17:21:13.723658 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/styles/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/styles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 17:21:13.724658 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/styles/default/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/styles/default/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5049 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/ui/styles/default/default_style.css
--rw-rw-rw-   0 root         (0) root         (0)    56780 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/src/libreflow_launcher/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 17:21:13.724658 libreflow_launcher-1.0.5/src/libreflow_launcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2192 2024-04-29 17:21:13.000000 libreflow_launcher-1.0.5/src/libreflow_launcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2191 2024-04-29 17:21:13.000000 libreflow_launcher-1.0.5/src/libreflow_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 17:21:13.000000 libreflow_launcher-1.0.5/src/libreflow_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-29 17:21:13.000000 libreflow_launcher-1.0.5/src/libreflow_launcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-29 17:21:13.000000 libreflow_launcher-1.0.5/src/libreflow_launcher.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-04-29 17:21:05.000000 libreflow_launcher-1.0.5/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.347470 libreflow_launcher-1.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2284 2024-05-07 05:52:33.347470 libreflow_launcher-1.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      839 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-07 05:52:33.347470 libreflow_launcher-1.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1691 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.333470 libreflow_launcher-1.0.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.337470 libreflow_launcher-1.0.6/src/libreflow_launcher/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-07 05:52:33.348470 libreflow_launcher-1.0.6/src/libreflow_launcher/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    18949 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.338470 libreflow_launcher-1.0.6/src/libreflow_launcher/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.338470 libreflow_launcher-1.0.6/src/libreflow_launcher/data/servers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/data/servers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     6139 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     7983 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.339470 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.341470 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   503824 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   445528 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   579296 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   528976 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/OpenSans.ttf
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.341470 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.346470 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5628 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/arrow-down.png
+-rw-rw-rw-   0 root         (0) root         (0)     5667 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/arrow-right.png
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png
+-rw-rw-rw-   0 root         (0) root         (0)     9732 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/close.png
+-rw-rw-rw-   0 root         (0) root         (0)     9850 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/gitlab.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/kitsu.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8760 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/log-out.png
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/log-out_hover.png
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/log-out_normal.png
+-rw-rw-rw-   0 root         (0) root         (0)     7267 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/open.png
+-rw-rw-rw-   0 root         (0) root         (0)    10491 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/pypi.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17905 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/server.png
+-rw-rw-rw-   0 root         (0) root         (0)    13119 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/settings.png
+-rw-rw-rw-   0 root         (0) root         (0)    19182 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/settings_outline.png
+-rw-rw-rw-   0 root         (0) root         (0)     5851 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/start.png
+-rw-rw-rw-   0 root         (0) root         (0)     7946 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/trash.png
+-rw-rw-rw-   0 root         (0) root         (0)     8358 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/trash_hover.png
+-rw-rw-rw-   0 root         (0) root         (0)     7996 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/trash_normal.png
+-rw-rw-rw-   0 root         (0) root         (0)    11968 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/user.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.346470 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/styles/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/styles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.346470 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/styles/default/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/styles/default/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5049 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/styles/default/default_style.css
+-rw-rw-rw-   0 root         (0) root         (0)    56780 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.347470 libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2284 2024-05-07 05:52:33.000000 libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2191 2024-05-07 05:52:33.000000 libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 05:52:33.000000 libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-07 05:52:33.000000 libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-07 05:52:33.000000 libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/versioneer.py
```

### Comparing `libreflow_launcher-1.0.5/CHANGELOG.md` & `libreflow_launcher-1.0.6/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.6] - 2024-05-07
+
+### Added
+
+* Shell script to start a Libreflow instance on Linux.
+
 ## [1.0.5] - 2024-04-29
 
 ### Fixed
 
 * Site name is now correctly defined on libreflow starting script (`bat` or `sh` file)
 * Install dir is now correctly used for installing libreflow instance
```

### Comparing `libreflow_launcher-1.0.5/PKG-INFO` & `libreflow_launcher-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow_launcher
-Version: 1.0.5
+Version: 1.0.6
 Summary: Launcher for instances of Libreflow asset-manager
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow_launcher
 Author: Valentin Braem
 Author-email: valentin.braem@les-fees-speciales.coop
 License: LGPLv3+
 Keywords: kabaret kitsu gazu animation pipeline libreflow launcher lfs overseer asset-manager
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.6] - 2024-05-07
+
+### Added
+
+* Shell script to start a Libreflow instance on Linux.
+
 ## [1.0.5] - 2024-04-29
 
 ### Fixed
 
 * Site name is now correctly defined on libreflow starting script (`bat` or `sh` file)
 * Install dir is now correctly used for installing libreflow instance
```

### Comparing `libreflow_launcher-1.0.5/README.md` & `libreflow_launcher-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/setup.py` & `libreflow_launcher-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/controller.py` & `libreflow_launcher-1.0.6/src/libreflow_launcher/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -386,16 +386,14 @@
             update = True
 
             # Format Kabaret Flow Extensions argument
             extensions = []
             for extension in data_resolve['extensions']:
                 if 'extension' in extension['categories']:
                     extensions.append(f'libreflow.extensions.{extension["name"]}:install_extensions')
-            
-            extensions = f'set KABARET_FLOW_EXT_INSTALLERS={";".join(extensions)}'
 
             # Format launch command with arguments
             cmd = [
                 self.poetry_path,
                 "run",
                 "python",
                 "-m",
@@ -414,29 +412,36 @@
                 site_name,
                 "--password",
                 data_resolve['redis_password'],
                 "--search-index-uri",
                 data_resolve["mongo_url"],
             ]
         
-        if platform.system() == "Windows":
-            exec_path = f"{env_folder}/libreflow.bat"
-            if update:
-                with open(exec_path, 'w+') as f:
-                    cmd.append('\npause')
+        exec_path = f"{env_folder}/libreflow"
+        exec_path += ".bat" if platform.system() == "Windows" else ".sh"
+
+        if update:
+            if platform.system() == "Windows":
+                extensions = f'set KABARET_FLOW_EXT_INSTALLERS={";".join(extensions)}'
+            else:
+                extensions = f'export KABARET_FLOW_EXT_INSTALLERS="{";".join(extensions)}"'
+
+            with open(exec_path, 'w+') as f:
+                cmd.append('\npause')
+                if platform.system() == "Windows":
                     f.write('@echo off\n\n')
-                    f.write(extensions)
-                    f.write('\n\n')
-                    f.write(' '.join(cmd))
+                f.write(extensions)
+                f.write('\n\n')
+                f.write(' '.join(cmd))
 
+        if platform.system() == "Windows":
             subprocess.Popen(exec_path, creationflags=subprocess.CREATE_NEW_CONSOLE)
-        
         elif platform.system() == "Linux":
-            # TODO
-            pass
+            subprocess.Popen(('chmod', '+x', exec_path)) 
+            subprocess.Popen(('gnome-terminal', '--', exec_path))
         
         os.chdir(store_base_path)
 
 
     def fetch_settings(self):
         return self._settings.fetch_settings()
```

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/gui.py` & `libreflow_launcher-1.0.6/src/libreflow_launcher/gui.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/model.py` & `libreflow_launcher-1.0.6/src/libreflow_launcher/model.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/resources.py` & `libreflow_launcher-1.0.6/src/libreflow_launcher/resources.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/fonts/OpenSans.ttf` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/OpenSans.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/arrow-down.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/arrow-down.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/arrow-right.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/arrow-right.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/close.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/close.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/gitlab.svg` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/gitlab.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/kitsu.svg` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/kitsu.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/log-out.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/log-out.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/log-out_hover.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/log-out_hover.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/log-out_normal.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/log-out_normal.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/open.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/open.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/pypi.svg` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/pypi.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/server.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/server.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/settings.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/settings.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/settings_outline.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/settings_outline.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/start.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/start.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/trash.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/trash.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/trash_hover.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/trash_hover.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/trash_normal.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/trash_normal.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/icons/gui/user.png` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/user.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/ui/styles/default/default_style.css` & `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/styles/default/default_style.css`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher/view.py` & `libreflow_launcher-1.0.6/src/libreflow_launcher/view.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher.egg-info/PKG-INFO` & `libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow_launcher
-Version: 1.0.5
+Version: 1.0.6
 Summary: Launcher for instances of Libreflow asset-manager
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow_launcher
 Author: Valentin Braem
 Author-email: valentin.braem@les-fees-speciales.coop
 License: LGPLv3+
 Keywords: kabaret kitsu gazu animation pipeline libreflow launcher lfs overseer asset-manager
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.6] - 2024-05-07
+
+### Added
+
+* Shell script to start a Libreflow instance on Linux.
+
 ## [1.0.5] - 2024-04-29
 
 ### Fixed
 
 * Site name is now correctly defined on libreflow starting script (`bat` or `sh` file)
 * Install dir is now correctly used for installing libreflow instance
```

### Comparing `libreflow_launcher-1.0.5/src/libreflow_launcher.egg-info/SOURCES.txt` & `libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.5/versioneer.py` & `libreflow_launcher-1.0.6/versioneer.py`

 * *Files identical despite different names*

