# Comparing `tmp/pyje-0.0.1.tar.gz` & `tmp/pyje-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyje-0.0.1.tar", last modified: Sun May  5 05:07:03 2024, max compression
+gzip compressed data, was "pyje-0.0.2.tar", last modified: Tue May  7 04:36:49 2024, max compression
```

## Comparing `pyje-0.0.1.tar` & `pyje-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 05:07:03.647990 pyje-0.0.1/
--rw-rw-rw-   0        0        0      400 2024-05-05 05:07:03.644979 pyje-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-05 04:40:58.000000 pyje-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 05:07:03.431320 pyje-0.0.1/pyje/
--rw-rw-rw-   0        0        0       23 2024-05-05 05:01:52.000000 pyje-0.0.1/pyje/__init__.py
--rw-rw-rw-   0        0        0      544 2024-05-05 04:24:18.000000 pyje-0.0.1/pyje/main.py
-drwxrwxrwx   0        0        0        0 2024-05-05 05:07:03.613233 pyje-0.0.1/pyje.egg-info/
--rw-rw-rw-   0        0        0      400 2024-05-05 05:07:03.000000 pyje-0.0.1/pyje.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2024-05-05 05:07:03.000000 pyje-0.0.1/pyje.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 05:07:03.000000 pyje-0.0.1/pyje.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-05 05:07:03.000000 pyje-0.0.1/pyje.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 05:07:03.648978 pyje-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      647 2024-05-05 05:06:39.000000 pyje-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 04:36:49.535431 pyje-0.0.2/
+-rw-rw-rw-   0        0        0      425 2024-05-07 04:36:49.531430 pyje-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-05 04:40:58.000000 pyje-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 04:36:49.031399 pyje-0.0.2/pyje/
+-rw-rw-rw-   0        0        0       48 2024-05-07 04:36:19.000000 pyje-0.0.2/pyje/__init__.py
+-rw-rw-rw-   0        0        0     4256 2024-05-07 04:33:27.000000 pyje-0.0.2/pyje/main.py
+drwxrwxrwx   0        0        0        0 2024-05-07 04:36:49.502368 pyje-0.0.2/pyje.egg-info/
+-rw-rw-rw-   0        0        0      425 2024-05-07 04:36:48.000000 pyje-0.0.2/pyje.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2024-05-07 04:36:48.000000 pyje-0.0.2/pyje.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 04:36:48.000000 pyje-0.0.2/pyje.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 04:36:48.000000 pyje-0.0.2/pyje.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-07 04:36:48.000000 pyje-0.0.2/pyje.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 04:36:49.535431 pyje-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      683 2024-05-07 04:35:49.000000 pyje-0.0.2/setup.py
```

