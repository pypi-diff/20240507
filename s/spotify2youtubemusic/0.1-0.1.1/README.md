# Comparing `tmp/spotify2youtubemusic-0.1.tar.gz` & `tmp/spotify2youtubemusic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify2youtubemusic-0.1.tar", last modified: Tue May  7 06:10:58 2024, max compression
+gzip compressed data, was "spotify2youtubemusic-0.1.1.tar", last modified: Tue May  7 06:30:04 2024, max compression
```

## Comparing `spotify2youtubemusic-0.1.tar` & `spotify2youtubemusic-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 06:10:58.745457 spotify2youtubemusic-0.1/
--rw-rw-rw-   0        0        0       90 2024-05-07 06:10:58.739428 spotify2youtubemusic-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-07 06:10:58.745457 spotify2youtubemusic-0.1/setup.cfg
--rw-rw-rw-   0        0        0      474 2024-05-07 06:10:32.000000 spotify2youtubemusic-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:10:58.739428 spotify2youtubemusic-0.1/spotify2youtubemusic/
--rw-rw-rw-   0        0        0      331 2024-05-07 05:55:09.000000 spotify2youtubemusic-0.1/spotify2youtubemusic/download.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:10:58.739428 spotify2youtubemusic-0.1/spotify2youtubemusic.egg-info/
--rw-rw-rw-   0        0        0       90 2024-05-07 06:10:58.000000 spotify2youtubemusic-0.1/spotify2youtubemusic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-05-07 06:10:58.000000 spotify2youtubemusic-0.1/spotify2youtubemusic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 06:10:58.000000 spotify2youtubemusic-0.1/spotify2youtubemusic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-07 06:10:58.000000 spotify2youtubemusic-0.1/spotify2youtubemusic.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2024-05-07 06:10:58.000000 spotify2youtubemusic-0.1/spotify2youtubemusic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-07 06:10:58.000000 spotify2youtubemusic-0.1/spotify2youtubemusic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 06:30:04.933369 spotify2youtubemusic-0.1.1/
+-rw-rw-rw-   0        0        0       92 2024-05-07 06:30:04.926814 spotify2youtubemusic-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-07 06:30:04.933920 spotify2youtubemusic-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      547 2024-05-07 06:29:48.000000 spotify2youtubemusic-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:30:04.926814 spotify2youtubemusic-0.1.1/spotify2youtubemusic/
+-rw-rw-rw-   0        0        0      380 2024-05-07 06:29:44.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic/download.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:30:04.926814 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/
+-rw-rw-rw-   0        0        0       92 2024-05-07 06:30:04.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-05-07 06:30:04.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 06:30:04.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-07 06:30:04.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2024-05-07 06:30:04.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-07 06:30:04.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/top_level.txt
```

