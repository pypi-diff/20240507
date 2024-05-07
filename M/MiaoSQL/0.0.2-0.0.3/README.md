# Comparing `tmp/MiaoSQL-0.0.2.tar.gz` & `tmp/MiaoSQL-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MiaoSQL-0.0.2.tar", last modified: Mon Mar 18 14:58:51 2024, max compression
+gzip compressed data, was "MiaoSQL-0.0.3.tar", last modified: Tue May  7 04:53:46 2024, max compression
```

## Comparing `MiaoSQL-0.0.2.tar` & `MiaoSQL-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 14:58:51.300310 MiaoSQL-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-03-18 14:58:51.296038 MiaoSQL-0.0.2/MiaoSQL/
--rw-rw-rw-   0        0        0        0 2024-03-18 14:02:58.000000 MiaoSQL-0.0.2/MiaoSQL/__init__.py
--rw-rw-rw-   0        0        0     4283 2024-03-18 14:40:42.000000 MiaoSQL-0.0.2/MiaoSQL/miaosql.py
-drwxrwxrwx   0        0        0        0 2024-03-18 14:58:51.299301 MiaoSQL-0.0.2/MiaoSQL.egg-info/
--rw-rw-rw-   0        0        0      300 2024-03-18 14:58:51.000000 MiaoSQL-0.0.2/MiaoSQL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2024-03-18 14:58:51.000000 MiaoSQL-0.0.2/MiaoSQL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 14:58:51.000000 MiaoSQL-0.0.2/MiaoSQL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-18 14:58:51.000000 MiaoSQL-0.0.2/MiaoSQL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      300 2024-03-18 14:58:51.300310 MiaoSQL-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-18 14:58:51.300310 MiaoSQL-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      437 2024-03-18 14:58:49.000000 MiaoSQL-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 04:53:46.721742 MiaoSQL-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-05-07 04:53:46.717229 MiaoSQL-0.0.3/MiaoSQL/
+-rw-rw-rw-   0        0        0        0 2024-03-18 14:02:58.000000 MiaoSQL-0.0.3/MiaoSQL/__init__.py
+-rw-rw-rw-   0        0        0     9460 2024-05-07 04:49:25.000000 MiaoSQL-0.0.3/MiaoSQL/miaosql.py
+drwxrwxrwx   0        0        0        0 2024-05-07 04:53:46.720228 MiaoSQL-0.0.3/MiaoSQL.egg-info/
+-rw-rw-rw-   0        0        0      300 2024-05-07 04:53:46.000000 MiaoSQL-0.0.3/MiaoSQL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2024-05-07 04:53:46.000000 MiaoSQL-0.0.3/MiaoSQL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 04:53:46.000000 MiaoSQL-0.0.3/MiaoSQL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 04:53:46.000000 MiaoSQL-0.0.3/MiaoSQL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      300 2024-05-07 04:53:46.721742 MiaoSQL-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-07 04:53:46.721742 MiaoSQL-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      420 2024-05-07 04:53:40.000000 MiaoSQL-0.0.3/setup.py
```

