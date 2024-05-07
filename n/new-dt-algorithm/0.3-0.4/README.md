# Comparing `tmp/new_dt_algorithm-0.3.tar.gz` & `tmp/new_dt_algorithm-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_dt_algorithm-0.3.tar", last modified: Tue May  7 08:39:00 2024, max compression
+gzip compressed data, was "new_dt_algorithm-0.4.tar", last modified: Tue May  7 11:31:54 2024, max compression
```

## Comparing `new_dt_algorithm-0.3.tar` & `new_dt_algorithm-0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 08:39:00.200179 new_dt_algorithm-0.3/
--rw-rw-rw-   0        0        0      214 2024-05-07 08:39:00.200179 new_dt_algorithm-0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-07 08:29:10.000000 new_dt_algorithm-0.3/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 08:39:00.200179 new_dt_algorithm-0.3/new_dt_algorithm.egg-info/
--rw-rw-rw-   0        0        0      214 2024-05-07 08:39:00.000000 new_dt_algorithm-0.3/new_dt_algorithm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-07 08:39:00.000000 new_dt_algorithm-0.3/new_dt_algorithm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 08:39:00.000000 new_dt_algorithm-0.3/new_dt_algorithm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-07 08:39:00.000000 new_dt_algorithm-0.3/new_dt_algorithm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    29098 2024-05-07 07:54:39.000000 new_dt_algorithm-0.3/new_dt_algorithm.pyc
--rw-rw-rw-   0        0        0       42 2024-05-07 08:39:00.200179 new_dt_algorithm-0.3/setup.cfg
--rw-rw-rw-   0        0        0      444 2024-05-07 08:38:54.000000 new_dt_algorithm-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:31:54.644910 new_dt_algorithm-0.4/
+-rw-rw-rw-   0        0        0      214 2024-05-07 11:31:54.644910 new_dt_algorithm-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:26:56.000000 new_dt_algorithm-0.4/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:31:54.644910 new_dt_algorithm-0.4/new_dt_algorithm.egg-info/
+-rw-rw-rw-   0        0        0      214 2024-05-07 11:31:54.000000 new_dt_algorithm-0.4/new_dt_algorithm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-05-07 11:31:54.000000 new_dt_algorithm-0.4/new_dt_algorithm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 11:31:54.000000 new_dt_algorithm-0.4/new_dt_algorithm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-07 11:31:54.000000 new_dt_algorithm-0.4/new_dt_algorithm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    21625 2024-05-07 09:22:37.000000 new_dt_algorithm-0.4/new_dt_algorithm.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 11:31:54.644910 new_dt_algorithm-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      443 2024-05-07 11:31:37.000000 new_dt_algorithm-0.4/setup.py
```

