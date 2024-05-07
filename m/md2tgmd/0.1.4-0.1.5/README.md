# Comparing `tmp/md2tgmd-0.1.4.tar.gz` & `tmp/md2tgmd-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2tgmd-0.1.4.tar", last modified: Tue May  7 07:30:50 2024, max compression
+gzip compressed data, was "md2tgmd-0.1.5.tar", last modified: Tue May  7 08:39:09 2024, max compression
```

## Comparing `md2tgmd-0.1.4.tar` & `md2tgmd-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:30:50.308371 md2tgmd-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-07 07:30:41.000000 md2tgmd-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-07 07:30:50.308371 md2tgmd-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-07 07:30:41.000000 md2tgmd-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:30:50.308371 md2tgmd-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 07:30:41.000000 md2tgmd-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:30:50.308371 md2tgmd-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:30:50.308371 md2tgmd-0.1.4/src/md2tgmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-07 07:30:50.000000 md2tgmd-0.1.4/src/md2tgmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 07:30:50.000000 md2tgmd-0.1.4/src/md2tgmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:30:50.000000 md2tgmd-0.1.4/src/md2tgmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 07:30:50.000000 md2tgmd-0.1.4/src/md2tgmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-07 07:30:41.000000 md2tgmd-0.1.4/src/md2tgmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:39:09.497786 md2tgmd-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-07 08:39:00.000000 md2tgmd-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-07 08:39:09.497786 md2tgmd-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-07 08:39:00.000000 md2tgmd-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:39:09.497786 md2tgmd-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 08:39:00.000000 md2tgmd-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:39:09.493786 md2tgmd-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:39:09.497786 md2tgmd-0.1.5/src/md2tgmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-07 08:39:09.000000 md2tgmd-0.1.5/src/md2tgmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 08:39:09.000000 md2tgmd-0.1.5/src/md2tgmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:39:09.000000 md2tgmd-0.1.5/src/md2tgmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 08:39:09.000000 md2tgmd-0.1.5/src/md2tgmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-07 08:39:00.000000 md2tgmd-0.1.5/src/md2tgmd.py
```

### Comparing `md2tgmd-0.1.4/LICENSE` & `md2tgmd-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `md2tgmd-0.1.4/PKG-INFO` & `md2tgmd-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2tgmd
-Version: 0.1.4
+Version: 0.1.5
 Summary: md2tgmd is a Markdown to Telegram-specific-markdown converter.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # md2tgmd
 
 md2tgmd is a Markdown to [Telegram-specific-markdown](https://core.telegram.org/bots/api#formatting-options) converter.
```

### Comparing `md2tgmd-0.1.4/README.md` & `md2tgmd-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `md2tgmd-0.1.4/src/md2tgmd.egg-info/PKG-INFO` & `md2tgmd-0.1.5/src/md2tgmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2tgmd
-Version: 0.1.4
+Version: 0.1.5
 Summary: md2tgmd is a Markdown to Telegram-specific-markdown converter.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # md2tgmd
 
 md2tgmd is a Markdown to [Telegram-specific-markdown](https://core.telegram.org/bots/api#formatting-options) converter.
```

