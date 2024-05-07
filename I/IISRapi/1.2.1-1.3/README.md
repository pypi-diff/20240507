# Comparing `tmp/IISRapi-1.2.1.tar.gz` & `tmp/IISRapi-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IISRapi-1.2.1.tar", last modified: Mon May  6 03:38:59 2024, max compression
+gzip compressed data, was "IISRapi-1.3.tar", last modified: Tue May  7 08:03:01 2024, max compression
```

## Comparing `IISRapi-1.2.1.tar` & `IISRapi-1.3.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 03:38:59.249205 IISRapi-1.2.1/
-drwxrwxrwx   0        0        0        0 2024-05-06 03:38:59.207369 IISRapi-1.2.1/IISRapi/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:53:31.000000 IISRapi-1.2.1/IISRapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:38:59.245627 IISRapi-1.2.1/IISRapi/model/
--rw-rw-rw-   0        0        0       26 2024-04-22 06:07:16.000000 IISRapi-1.2.1/IISRapi/model/__init__.py
--rw-rw-rw-   0        0        0      202 2024-04-22 08:37:02.000000 IISRapi-1.2.1/IISRapi/model/data.py
--rw-rw-rw-   0        0        0     6003 2024-04-24 06:16:12.000000 IISRapi-1.2.1/IISRapi/model/ner.py
--rw-rw-rw-   0        0        0     4120 2024-05-06 03:26:04.000000 IISRapi-1.2.1/IISRapi/model/pun.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:38:59.236987 IISRapi-1.2.1/IISRapi.egg-info/
--rw-rw-rw-   0        0        0      140 2024-05-06 03:38:58.000000 IISRapi-1.2.1/IISRapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-05-06 03:38:58.000000 IISRapi-1.2.1/IISRapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 03:38:58.000000 IISRapi-1.2.1/IISRapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-06 03:38:58.000000 IISRapi-1.2.1/IISRapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-06 03:38:58.000000 IISRapi-1.2.1/IISRapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      140 2024-05-06 03:38:59.247210 IISRapi-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-06 03:38:59.250333 IISRapi-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      242 2024-05-06 03:36:29.000000 IISRapi-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:03:01.174411 IISRapi-1.3/
+drwxrwxrwx   0        0        0        0 2024-05-07 08:03:01.124997 IISRapi-1.3/IISRapi/
+-rw-rw-rw-   0        0        0       23 2024-05-06 09:29:00.000000 IISRapi-1.3/IISRapi/__init__.py
+-rw-rw-rw-   0        0        0     1169 2024-05-07 07:25:10.000000 IISRapi-1.3/IISRapi/data.py
+-rw-rw-rw-   0        0        0    18021 2024-05-07 07:58:39.000000 IISRapi-1.3/IISRapi/tool.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:03:01.174411 IISRapi-1.3/IISRapi.egg-info/
+-rw-rw-rw-   0        0        0     1649 2024-05-07 08:03:00.000000 IISRapi-1.3/IISRapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-05-07 08:03:00.000000 IISRapi-1.3/IISRapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 08:03:00.000000 IISRapi-1.3/IISRapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-07 08:03:00.000000 IISRapi-1.3/IISRapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 08:03:00.000000 IISRapi-1.3/IISRapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1649 2024-05-07 08:03:01.174411 IISRapi-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-07 08:03:01.174411 IISRapi-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      492 2024-05-07 08:02:29.000000 IISRapi-1.3/setup.py
```

