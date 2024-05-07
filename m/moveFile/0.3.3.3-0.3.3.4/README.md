# Comparing `tmp/moveFile-0.3.3.3.tar.gz` & `tmp/moveFile-0.3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveFile-0.3.3.3.tar", last modified: Thu Jan 11 07:14:52 2024, max compression
+gzip compressed data, was "moveFile-0.3.3.4.tar", last modified: Tue May  7 08:42:27 2024, max compression
```

## Comparing `moveFile-0.3.3.3.tar` & `moveFile-0.3.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-01-11 07:14:52.812431 moveFile-0.3.3.3/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 moveFile-0.3.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 moveFile-0.3.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0      411 2024-01-11 07:14:52.812431 moveFile-0.3.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 moveFile-0.3.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-01-11 07:14:52.772430 moveFile-0.3.3.3/moveFile/
-drwxrwxrwx   0        0        0        0 2024-01-11 07:14:52.807429 moveFile-0.3.3.3/moveFile/Ui/
--rw-rw-rw-   0        0        0        0 2023-02-22 02:56:19.000000 moveFile-0.3.3.3/moveFile/Ui/__init__.py
--rw-rw-rw-   0        0        0    71168 2023-04-28 06:15:40.000000 moveFile-0.3.3.3/moveFile/Ui/moveFileUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-22 08:31:58.000000 moveFile-0.3.3.3/moveFile/__init__.py
--rw-rw-rw-   0        0        0    35840 2023-04-28 06:14:13.000000 moveFile-0.3.3.3/moveFile/find_file_return_path_m1.pyd
--rw-rw-rw-   0        0        0   233984 2024-01-11 07:11:59.000000 moveFile-0.3.3.3/moveFile/moveFile.pyd
--rw-rw-rw-   0        0        0    68608 2023-04-28 06:14:21.000000 moveFile-0.3.3.3/moveFile/moveFileUi.pyd
--rw-rw-rw-   0        0        0    69632 2023-04-28 06:14:45.000000 moveFile-0.3.3.3/moveFile/optionDb.pyd
-drwxrwxrwx   0        0        0        0 2024-01-11 07:14:52.795432 moveFile-0.3.3.3/moveFile.egg-info/
--rw-rw-rw-   0        0        0      411 2024-01-11 07:14:52.000000 moveFile-0.3.3.3/moveFile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2024-01-11 07:14:52.000000 moveFile-0.3.3.3/moveFile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-11 07:14:52.000000 moveFile-0.3.3.3/moveFile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-01-11 07:14:52.000000 moveFile-0.3.3.3/moveFile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      135 2024-01-11 07:14:52.815433 moveFile-0.3.3.3/setup.cfg
--rw-rw-rw-   0        0        0      979 2024-01-11 07:14:30.000000 moveFile-0.3.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:42:27.239325 moveFile-0.3.3.4/
+-rw-rw-rw-   0        0        0        0 2024-05-07 08:41:22.000000 moveFile-0.3.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 moveFile-0.3.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      411 2024-05-07 08:42:27.239325 moveFile-0.3.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 moveFile-0.3.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 08:42:27.211319 moveFile-0.3.3.4/moveFile/
+drwxrwxrwx   0        0        0        0 2024-05-07 08:42:27.235338 moveFile-0.3.3.4/moveFile/Ui/
+-rw-rw-rw-   0        0        0        0 2023-02-22 02:56:19.000000 moveFile-0.3.3.4/moveFile/Ui/__init__.py
+-rw-rw-rw-   0        0        0    71168 2023-04-28 06:15:40.000000 moveFile-0.3.3.4/moveFile/Ui/moveFileUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-22 08:31:58.000000 moveFile-0.3.3.4/moveFile/__init__.py
+-rw-rw-rw-   0        0        0    35840 2023-04-28 06:14:13.000000 moveFile-0.3.3.4/moveFile/find_file_return_path_m1.pyd
+-rw-rw-rw-   0        0        0   235520 2024-05-07 08:29:27.000000 moveFile-0.3.3.4/moveFile/moveFile.pyd
+-rw-rw-rw-   0        0        0    68608 2023-04-28 06:14:21.000000 moveFile-0.3.3.4/moveFile/moveFileUi.pyd
+-rw-rw-rw-   0        0        0    69632 2023-04-28 06:14:45.000000 moveFile-0.3.3.4/moveFile/optionDb.pyd
+drwxrwxrwx   0        0        0        0 2024-05-07 08:42:27.226324 moveFile-0.3.3.4/moveFile.egg-info/
+-rw-rw-rw-   0        0        0      411 2024-05-07 08:42:27.000000 moveFile-0.3.3.4/moveFile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2024-05-07 08:42:27.000000 moveFile-0.3.3.4/moveFile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 08:42:27.000000 moveFile-0.3.3.4/moveFile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 08:42:27.000000 moveFile-0.3.3.4/moveFile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2024-05-07 08:42:27.241322 moveFile-0.3.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      979 2024-05-07 08:31:31.000000 moveFile-0.3.3.4/setup.py
```

### Comparing `moveFile-0.3.3.3/setup.py` & `moveFile-0.3.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
 PATCH = 3
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.3"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.4"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "moveFile",
 	version = VERSION,
```

